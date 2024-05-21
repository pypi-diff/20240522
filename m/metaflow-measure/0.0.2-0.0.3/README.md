# Comparing `tmp/metaflow_measure-0.0.2.tar.gz` & `tmp/metaflow_measure-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow_measure-0.0.2.tar", last modified: Mon May 13 05:01:10 2024, max compression
+gzip compressed data, was "metaflow_measure-0.0.3.tar", last modified: Tue May 21 22:35:16 2024, max compression
```

## Comparing `metaflow_measure-0.0.2.tar` & `metaflow_measure-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.799363 metaflow_measure-0.0.2/
--rw-r--r--   0 ville      (501) staff       (20)    11349 2024-05-13 04:45:16.000000 metaflow_measure-0.0.2/LICENSE
--rw-r--r--   0 ville      (501) staff       (20)      246 2024-05-13 05:01:10.799173 metaflow_measure-0.0.2/PKG-INFO
--rw-r--r--   0 ville      (501) staff       (20)     4432 2024-05-13 04:53:13.000000 metaflow_measure-0.0.2/README.md
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.790549 metaflow_measure-0.0.2/metaflow_extensions/
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.790607 metaflow_measure-0.0.2/metaflow_extensions/measure/
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.793085 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.793985 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/
--rw-r--r--   0 ville      (501) staff       (20)     4551 2024-05-13 02:20:59.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/__init__.py
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.796521 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/
--rw-r--r--   0 ville      (501) staff       (20)      277 2024-05-13 02:10:29.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/__init__.py
--rw-r--r--   0 ville      (501) staff       (20)    51225 2024-05-13 02:11:21.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/base.py
--rw-r--r--   0 ville      (501) staff       (20)     4468 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/container.py
--rw-r--r--   0 ville      (501) staff       (20)     2850 2024-05-13 02:06:55.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/context.py
--rw-r--r--   0 ville      (501) staff       (20)     1543 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/context_async.py
--rw-r--r--   0 ville      (501) staff       (20)     1253 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/route.py
--rw-r--r--   0 ville      (501) staff       (20)        0 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/py.typed
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.798256 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/
--rw-r--r--   0 ville      (501) staff       (20)      233 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/__init__.py
--rw-r--r--   0 ville      (501) staff       (20)     5001 2024-05-13 02:14:38.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/cli.py
--rw-r--r--   0 ville      (501) staff       (20)     3284 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/compat.py
--rw-r--r--   0 ville      (501) staff       (20)     3904 2024-05-13 02:14:52.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/config.py
--rw-r--r--   0 ville      (501) staff       (20)      782 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/deprecation.py
--rw-r--r--   0 ville      (501) staff       (20)     1327 2024-05-13 02:15:14.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/format.py
--rw-r--r--   0 ville      (501) staff       (20)    10272 2024-05-13 02:15:04.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/hostname.py
--rw-r--r--   0 ville      (501) staff       (20)       27 2024-05-11 01:59:47.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/version.py
--rw-r--r--   0 ville      (501) staff       (20)     2977 2024-05-13 03:16:20.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog_decorator.py
--rw-r--r--   0 ville      (501) staff       (20)    10878 2024-05-13 02:52:32.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/dogstatsd_manager.py
--rw-r--r--   0 ville      (501) staff       (20)     1256 2024-05-13 02:51:51.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/measure.py
--rw-r--r--   0 ville      (501) staff       (20)      117 2024-05-13 01:59:54.000000 metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/mfextinit_org.py
-drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-13 05:01:10.798953 metaflow_measure-0.0.2/metaflow_measure.egg-info/
--rw-r--r--   0 ville      (501) staff       (20)      246 2024-05-13 05:01:10.000000 metaflow_measure-0.0.2/metaflow_measure.egg-info/PKG-INFO
--rw-r--r--   0 ville      (501) staff       (20)     1377 2024-05-13 05:01:10.000000 metaflow_measure-0.0.2/metaflow_measure.egg-info/SOURCES.txt
--rw-r--r--   0 ville      (501) staff       (20)        1 2024-05-13 05:01:10.000000 metaflow_measure-0.0.2/metaflow_measure.egg-info/dependency_links.txt
--rw-r--r--   0 ville      (501) staff       (20)       20 2024-05-13 05:01:10.000000 metaflow_measure-0.0.2/metaflow_measure.egg-info/top_level.txt
--rw-r--r--   0 ville      (501) staff       (20)       38 2024-05-13 05:01:10.799407 metaflow_measure-0.0.2/setup.cfg
--rw-r--r--   0 ville      (501) staff       (20)      446 2024-05-13 05:00:59.000000 metaflow_measure-0.0.2/setup.py
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.536733 metaflow_measure-0.0.3/
+-rw-r--r--   0 ville      (501) staff       (20)    11349 2024-05-13 04:45:16.000000 metaflow_measure-0.0.3/LICENSE
+-rw-r--r--   0 ville      (501) staff       (20)      246 2024-05-21 22:35:16.536524 metaflow_measure-0.0.3/PKG-INFO
+-rw-r--r--   0 ville      (501) staff       (20)     4700 2024-05-13 06:08:05.000000 metaflow_measure-0.0.3/README.md
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.526665 metaflow_measure-0.0.3/metaflow_extensions/
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.526713 metaflow_measure-0.0.3/metaflow_extensions/measure/
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.529147 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.530180 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/
+-rw-r--r--   0 ville      (501) staff       (20)     4551 2024-05-13 02:20:59.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/__init__.py
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.534379 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/
+-rw-r--r--   0 ville      (501) staff       (20)      277 2024-05-13 02:10:29.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/__init__.py
+-rw-r--r--   0 ville      (501) staff       (20)    51225 2024-05-13 02:11:21.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/base.py
+-rw-r--r--   0 ville      (501) staff       (20)     4468 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/container.py
+-rw-r--r--   0 ville      (501) staff       (20)     2850 2024-05-13 02:06:55.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/context.py
+-rw-r--r--   0 ville      (501) staff       (20)     1543 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/context_async.py
+-rw-r--r--   0 ville      (501) staff       (20)     1253 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/route.py
+-rw-r--r--   0 ville      (501) staff       (20)        0 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/py.typed
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.535598 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/
+-rw-r--r--   0 ville      (501) staff       (20)      233 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/__init__.py
+-rw-r--r--   0 ville      (501) staff       (20)     5001 2024-05-13 02:14:38.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/cli.py
+-rw-r--r--   0 ville      (501) staff       (20)     3284 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/compat.py
+-rw-r--r--   0 ville      (501) staff       (20)     3904 2024-05-13 02:14:52.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/config.py
+-rw-r--r--   0 ville      (501) staff       (20)      782 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/deprecation.py
+-rw-r--r--   0 ville      (501) staff       (20)     1327 2024-05-13 02:15:14.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/format.py
+-rw-r--r--   0 ville      (501) staff       (20)    10272 2024-05-13 02:15:04.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/hostname.py
+-rw-r--r--   0 ville      (501) staff       (20)       27 2024-05-11 01:59:47.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/version.py
+-rw-r--r--   0 ville      (501) staff       (20)     2977 2024-05-13 03:16:20.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog_decorator.py
+-rw-r--r--   0 ville      (501) staff       (20)    10930 2024-05-21 22:34:25.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/dogstatsd_manager.py
+-rw-r--r--   0 ville      (501) staff       (20)     1256 2024-05-13 02:51:51.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/measure.py
+-rw-r--r--   0 ville      (501) staff       (20)      117 2024-05-13 01:59:54.000000 metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/mfextinit_org.py
+drwxr-xr-x   0 ville      (501) staff       (20)        0 2024-05-21 22:35:16.536322 metaflow_measure-0.0.3/metaflow_measure.egg-info/
+-rw-r--r--   0 ville      (501) staff       (20)      246 2024-05-21 22:35:16.000000 metaflow_measure-0.0.3/metaflow_measure.egg-info/PKG-INFO
+-rw-r--r--   0 ville      (501) staff       (20)     1377 2024-05-21 22:35:16.000000 metaflow_measure-0.0.3/metaflow_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 ville      (501) staff       (20)        1 2024-05-21 22:35:16.000000 metaflow_measure-0.0.3/metaflow_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 ville      (501) staff       (20)       20 2024-05-21 22:35:16.000000 metaflow_measure-0.0.3/metaflow_measure.egg-info/top_level.txt
+-rw-r--r--   0 ville      (501) staff       (20)       38 2024-05-21 22:35:16.536772 metaflow_measure-0.0.3/setup.cfg
+-rw-r--r--   0 ville      (501) staff       (20)      446 2024-05-21 22:34:48.000000 metaflow_measure-0.0.3/setup.py
```

### Comparing `metaflow_measure-0.0.2/LICENSE` & `metaflow_measure-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/README.md` & `metaflow_measure-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,24 @@
  - Works at scale: Uses aggregators like `dogstatsd` to
    avoid overloading backend APIs.
 
  - No extra dependencies: `@datadog` installs the
    `dogstatsd` on the fly, so it works in any execution
    environment.
 
+## Installation
+
+In your development environment, install
+```
+pip install metaflow-measure
+```
+Note that you don't need to make the package available in
+container images you use to execute tasks remotely. Metaflow
+packages the extension automatically for remote execution.
+
 ## API
 
 The `measure` module exposes [`statsd`-style measurement
 functions](https://docs.datadoghq.com/metrics/custom_metrics/dogstatsd_metrics_submission/):
 `gauge`, `increment`, and `decrement`.
 
 Optionally, all `measure` functions take a keyword argument
@@ -42,18 +52,18 @@
 
 ```python
 from metaflow.plugins import measure
 
 # record a gauge metric
 measure.gauge('mymetric', value)
 
-# record a gauge metric
+# increment a metric
 measure.increment('mymetric', value)
 
-# record a gauge metric
+# decrement a metric
 measure.decrement('mymetric', value)
 ```
 
 ### Distributions
 
 In addition, `measure` provides `distribution` which allows
 you to measure distributions of values (e.g. p50, p95 etc) relying
```

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/__init__.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/base.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/base.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/container.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/container.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/context.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/context.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/context_async.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/context_async.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/dogstatsd/route.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/dogstatsd/route.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/cli.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/compat.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/compat.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/config.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/config.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/deprecation.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/format.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/format.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog/util/hostname.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog/util/hostname.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/datadog_decorator.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/datadog_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/dogstatsd_manager.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/dogstatsd_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from . import datadog as dd
 from .measure import MeasurementBackend, register_backend
 
 BASE = "https://outerbounds-metaflow-public.s3.us-west-2.amazonaws.com/"
 BINARIES = {
     ("Darwin", "arm64"): "dogstatsd-darwin-arm64",
     ("Linux", "x86_64"): "dogstatsd-linux-amd64",
+    ("Linux", "aarch64"): "dogstatsd-linux-aarch64"
 }
 
 # wait for this many seconds when another process
 # is launching the daemon
 WAIT_TO_DOWNLOAD = 7
 WAIT_TO_START = 3
```

### Comparing `metaflow_measure-0.0.2/metaflow_extensions/measure/plugins/measure.py` & `metaflow_measure-0.0.3/metaflow_extensions/measure/plugins/measure.py`

 * *Files identical despite different names*

### Comparing `metaflow_measure-0.0.2/metaflow_measure.egg-info/SOURCES.txt` & `metaflow_measure-0.0.3/metaflow_measure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

