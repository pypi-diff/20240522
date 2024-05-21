# Comparing `tmp/beam_client-0.2.8.tar.gz` & `tmp/beam_client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_client-0.2.8.tar", max compression
+gzip compressed data, was "beam_client-0.2.9.tar", max compression
```

## Comparing `beam_client-0.2.8.tar` & `beam_client-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      736 2024-05-04 16:00:40.506451 beam_client-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      597 2024-05-04 15:06:39.674647 beam_client-0.2.8/src/beam/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 02:07:20.445321 beam_client-0.2.8/src/beam/cli/__init__.py
--rw-r--r--   0        0        0      438 2024-05-04 15:06:41.089453 beam_client-0.2.8/src/beam/cli/logs.py
--rw-r--r--   0        0        0      467 2024-05-04 16:00:49.048428 beam_client-0.2.8/src/beam/cli/main.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 beam_client-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      736 2024-05-06 13:22:10.066473 beam_client-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      630 2024-05-06 13:22:11.789896 beam_client-0.2.9/src/beam/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 02:07:20.445321 beam_client-0.2.9/src/beam/cli/__init__.py
+-rw-r--r--   0        0        0      428 2024-05-06 13:22:13.619918 beam_client-0.2.9/src/beam/cli/main.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 beam_client-0.2.9/PKG-INFO
```

### Comparing `beam_client-0.2.8/pyproject.toml` & `beam_client-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beam-client"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beam/**/*.py", from = "src" },
     { include = "beam", from = "src" },
 ]
```

### Comparing `beam_client-0.2.8/src/beam/__init__.py` & `beam_client-0.2.9/src/beam/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from beta9 import env
 from beta9.abstractions.container import Container
 from beta9.abstractions.endpoint import Endpoint as endpoint
 from beta9.abstractions.function import Function as function
 from beta9.abstractions.image import Image
 from beta9.abstractions.map import Map
 from beta9.abstractions.queue import SimpleQueue as Queue
 from beta9.abstractions.taskqueue import TaskQueue as task_queue
 from beta9.abstractions.volume import Volume
 
-__version__ = "0.2.0"
+__version__ = "0.2.9"
 __all__ = [
     "__version__",
     "Map",
     "Image",
     "Queue",
     "Volume",
     "task_queue",
     "function",
     "endpoint",
     "Container",
+    "env",
 ]
```

