# Comparing `tmp/pingdat-1.4.1.tar.gz` & `tmp/pingdat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingdat-1.4.1.tar", max compression
+gzip compressed data, was "pingdat-1.5.0.tar", max compression
```

## Comparing `pingdat-1.4.1.tar` & `pingdat-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-11-22 15:47:14.201761 pingdat-1.4.1/LICENSE
--rw-r--r--   0        0        0     1958 2023-11-22 15:47:14.201761 pingdat-1.4.1/README.md
--rw-r--r--   0        0        0     1148 2023-11-22 15:47:14.201761 pingdat-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5332 2023-11-22 15:47:14.201761 pingdat-1.4.1/src/pingdat/__init__.py
--rw-r--r--   0        0        0     2234 2023-11-22 15:47:14.201761 pingdat-1.4.1/src/pingdat/__main__.py
--rw-r--r--   0        0        0     1605 2023-11-22 15:47:14.201761 pingdat-1.4.1/src/pingdat/config.py
--rw-r--r--   0        0        0     1656 2023-11-22 15:47:14.201761 pingdat-1.4.1/src/pingdat/version.py
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 pingdat-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-22 04:45:37.873469 pingdat-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1958 2024-05-22 04:45:37.873469 pingdat-1.5.0/README.md
+-rw-r--r--   0        0        0     1172 2024-05-22 04:45:37.873469 pingdat-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6163 2024-05-22 04:45:37.877469 pingdat-1.5.0/src/pingdat/__init__.py
+-rw-r--r--   0        0        0     2333 2024-05-22 04:45:37.877469 pingdat-1.5.0/src/pingdat/__main__.py
+-rw-r--r--   0        0        0     1605 2024-05-22 04:45:37.877469 pingdat-1.5.0/src/pingdat/config.py
+-rw-r--r--   0        0        0     1656 2024-05-22 04:45:37.877469 pingdat-1.5.0/src/pingdat/version.py
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 pingdat-1.5.0/PKG-INFO
```

### Comparing `pingdat-1.4.1/LICENSE` & `pingdat-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingdat-1.4.1/README.md` & `pingdat-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pingdat-1.4.1/src/pingdat/__init__.py` & `pingdat-1.5.0/src/pingdat/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Module interface to pingdat."""
 
 import logging
 import threading
 from datetime import datetime, timedelta
 
-from ping3 import ping
+import ping3
+from ping3.errors import PingError, Timeout
 from prometheus_client import Counter, Gauge, Histogram
 
 logger = logging.getLogger(__name__)
 
+ping3.EXCEPTIONS = True
+
 METRICS_LABELS = ["name", "address"]
 
 TOTAL_REQUESTS_METRICS = Counter(
     "ping_requests",
     "Total ping requests sent",
     labelnames=METRICS_LABELS,
 )
@@ -61,134 +64,155 @@
         self.timeouts = PING_TIMEOUT_METRICS.labels(**kwargs)
 
         self.response_time = RESPONSE_TIME_METRICS.labels(**kwargs)
         self.observations = RESPONSE_OBSERVATIONS.labels(**kwargs)
 
 
 class PingTarget:
-    __thread_count__ = 0
-
     def __init__(
         self,
         name,
         address,
-        interval,
         ttl=64,
         count=3,
-        timeout=None,
+        timeout=3,
         payload_size=56,
     ):
-        PingTarget.__thread_count__ += 1
-
         self.name = name
         self.address = address
-        self.timeout = timeout or interval / 2
+        self.timeout = timeout
         self.payload_size = payload_size
         self.ttl = ttl
         self.count = count
 
-        self.interval = timedelta(seconds=interval)
+        self.metrics = PingMetrics(name=name, address=address)
+        self.logger = logger.getChild("PingTarget")
 
-        self.thread_ctl = threading.Event()
-        self.loop_thread = threading.Thread(name=self.id, target=self.ping_loop)
-        self.loop_last_exec = None
+    def __call__(self):
+        """Ping the target and update metrics."""
+        self.logger.info("PING -- %s @ %s", self.name, self.address)
 
-        self.metrics = PingMetrics(name=name, address=address)
+        # track the response times so we can average them later
+        response_times = []
 
-        self.logger = logger.getChild("PingTarget")
+        for seq in range(0, self.count):
+            try:
+                delay = self.one_ping_only(seq)
+
+                self.logger.debug("ping :: %s [%d] => %d sec", self.name, seq, delay)
+
+                response_times.append(delay)
 
-    def __call__(self, seq=0):
+            except Timeout:
+                self.logger.warning("ping timeout: %s", self.name)
+                self.metrics.timeouts.inc()
+
+                # add the timeout value to the response_times list
+                response_times.append(self.timeout)
+
+            except PingError as err:
+                self.logger.error("ping error: %s => %s", self.name, err)
+                self.metrics.errors.inc()
+
+            except OSError as err:
+                self.logger.error("network error: %s => %s", self.name, err)
+                self.metrics.errors.inc()
+
+        # calculate the average response time
+        if len(response_times) > 0:
+            avg = sum(response_times) / len(response_times)
+            self.metrics.response_time.set(avg)
+
+        # use a sentinel value to indicate no response
+        else:
+            self.metrics.response_time.set(-1)
+
+    def one_ping_only(self, seq=0):
         """Ping the configured target with a given sequence number."""
 
-        self.logger.debug("ping :: %s @ %s [seq:%d]", self.name, self.address, seq)
+        self.logger.debug("ping :: %s @ %s [%d]", self.name, self.address, seq)
 
-        return ping(
+        self.metrics.requests.inc()
+
+        delay = ping3.ping(
             self.address,
             timeout=self.timeout,
             ttl=self.ttl,
             size=self.payload_size,
             seq=seq,
         )
 
+        if delay is None:
+            raise PingError("ping failed")
+
+        self.metrics.responses.inc()
+        self.metrics.observations.observe(delay)
+
+        return delay
+
+
+class PingLoop:
+
+    __thread_count__ = 0
+
+    def __init__(self, target: PingTarget, interval: int):
+        PingLoop.__thread_count__ += 1
+
+        self.target = target
+        self.interval = timedelta(seconds=interval)
+
+        self.thread_ctl = threading.Event()
+        self.loop_thread = threading.Thread(name=self.id, target=self.ping_loop)
+        self.loop_last_exec = None
+
+        self.logger = logger.getChild("PingLoop")
+
     @property
     def id(self) -> str:
-        return f"{self.address}-{PingTarget.__thread_count__}"
+        return f"{self.target.address}-{PingLoop.__thread_count__}"
 
     def start(self) -> None:
         """Start the main thread loop."""
 
         self.logger.debug("Starting ping thread")
 
         self.thread_ctl.clear()
         self.loop_thread.start()
 
     def stop(self) -> None:
         """Signal the thread to stop and wait for it to exit."""
 
-        self.logger.debug("Stopping ping thread")
+        timeout = self.interval.total_seconds() * 2
+        self.logger.debug("Stopping ping thread [%s sec]", timeout)
 
         self.thread_ctl.set()
-        self.loop_thread.join(self.timeout)
+        self.loop_thread.join(timeout)
 
         if self.loop_thread.is_alive():
             self.logger.warning("Thread failed to complete")
 
     def ping_loop(self):
         """Manage the lifecycle of the thread loop."""
 
-        self.logger.debug("BEGIN -- %s :: ping_loop @ %s", self.address, self.interval)
+        self.logger.debug("BEGIN :: ping_loop @ %s sec", self.interval)
 
         while not self.thread_ctl.is_set():
             self.loop_last_exec = datetime.now()
 
-            self.run_ping_test()
+            self.target()
 
             # figure out when to run the next step
             next_loop_time = self.loop_last_exec + self.interval
             next_loop_sleep = (next_loop_time - datetime.now()).total_seconds()
 
             # watch for overflows (pings that take longer than the thread interval)
             if next_loop_sleep <= 0:
                 self.logger.warning("ping time exceeded loop interval; overflow")
                 next_loop_sleep = 0
 
-            self.logger.debug(
-                "%s :: ping loop complete; next_step: %f",
-                self.address,
-                next_loop_sleep,
-            )
+            self.logger.debug("ping complete; next_step: %f", next_loop_sleep)
 
             # break if we are signaled to stop
             if self.thread_ctl.wait(next_loop_sleep):
                 self.logger.debug("received exit signal; ping_loop exiting")
 
-        self.logger.debug("END -- %s :: ping_loop", self.address)
-
-    def run_ping_test(self):
-        """Ping the target and update metrics."""
-        self.logger.info("PING -- %s @ %s", self.name, self.address)
-
-        response_times = []
-
-        for seq in range(0, self.count):
-            self.metrics.requests.inc()
-
-            resp = self(seq)
-
-            if resp is None:
-                self.metrics.timeouts.inc()
-                response_times.append(self.timeout)
-
-            elif resp is False:
-                self.metrics.errors.inc()
-
-            else:
-                self.metrics.responses.inc()
-                self.metrics.observations.observe(resp)
-                response_times.append(resp)
-
-        if len(response_times) > 0:
-            avg = sum(response_times) / len(response_times)
-            self.metrics.response_time.set(avg)
-
-        else:
-            self.metrics.response_time.set(-1)
+        self.logger.debug("END :: ping_loop")
```

### Comparing `pingdat-1.4.1/src/pingdat/__main__.py` & `pingdat-1.5.0/src/pingdat/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import signal
 
 import click
 from prometheus_client import start_http_server
 
-from . import PingTarget, version
+from . import PingLoop, PingTarget, version
 from .config import AppConfig, MetricsConfig
 
 logger = logging.getLogger(__name__)
 
 
 class MainApp:
     """Context used during main execution."""
@@ -20,55 +20,59 @@
 
         self.config = config
 
         self._initialize_targets(config)
         self._initialize_metrics(config.metrics)
 
     def _initialize_targets(self, config: AppConfig):
-        self.targets = []
+        self.threads = []
 
         for target_config in config.targets:
             self.logger.info(
                 "Initializing ping target: %s [%s]",
                 target_config.name,
                 target_config.address,
             )
 
             target = PingTarget(
                 name=target_config.name,
                 address=target_config.address,
-                interval=target_config.interval or config.interval,
                 timeout=target_config.timeout or config.timeout,
                 count=target_config.count or config.count,
             )
 
-            self.targets.append(target)
+            thread = PingLoop(
+                target=target,
+                interval=target_config.interval or config.interval,
+            )
+
+            self.threads.append(thread)
 
     def _initialize_metrics(self, config: MetricsConfig):
         self.logger.info(
             "Starting metrics server -- %s:%s",
             config.address,
             config.port,
         )
 
         start_http_server(config.port, addr=config.address)
 
     def __call__(self):
         self.logger.debug("Starting main app")
 
-        for obs in self.targets:
-            obs.start()
+        for thread in self.threads:
+            thread.start()
 
         try:
             signal.pause()
         except KeyboardInterrupt:
             self.logger.debug("canceled by user")
 
-        for obs in self.targets:
-            obs.stop()
+        for thread in self.threads:
+            thread.stop()
 
 
 @click.command()
 @click.option(
     "--config",
     "-f",
     default="pingdat.yaml",
```

### Comparing `pingdat-1.4.1/src/pingdat/config.py` & `pingdat-1.5.0/src/pingdat/config.py`

 * *Files identical despite different names*

### Comparing `pingdat-1.4.1/src/pingdat/version.py` & `pingdat-1.5.0/src/pingdat/version.py`

 * *Files identical despite different names*

### Comparing `pingdat-1.4.1/PKG-INFO` & `pingdat-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pingdat
-Version: 1.4.1
+Version: 1.5.0
 Summary: A simple ping exporter for Prometheus metrics.
 License: MIT
 Author: jheddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: ping3 (>=4.0.4,<5.0.0)
-Requires-Dist: prometheus-client (>=0.19.0,<0.20.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: ping3 (>=4.0.8,<5.0.0)
+Requires-Dist: prometheus-client (>=0.20.0,<0.21.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pingdat #
 
 [![PyPI](https://img.shields.io/pypi/v/pingdat.svg)](https://pypi.org/project/pingdat)
 [![LICENSE](https://img.shields.io/github/license/jheddings/pingdat)](LICENSE)
 [![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)
```

