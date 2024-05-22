# Comparing `tmp/synnax_freighter-0.7.1.tar.gz` & `tmp/synnax_freighter-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnax_freighter-0.7.1.tar", max compression
+gzip compressed data, was "synnax_freighter-0.7.2.tar", max compression
```

## Comparing `synnax_freighter-0.7.1.tar` & `synnax_freighter-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1233 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/__init__.py
--rw-r--r--   0        0        0     2101 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/alamos.py
--rw-r--r--   0        0        0     1521 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/context.py
--rw-r--r--   0        0        0     2652 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/encoder.py
--rw-r--r--   0        0        0     4650 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/exceptions.py
--rw-r--r--   0        0        0     4130 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/http.py
--rw-r--r--   0        0        0     6923 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/stream.py
--rw-r--r--   0        0        0     8026 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/sync.py
--rw-r--r--   0        0        0     4649 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/transport.py
--rw-r--r--   0        0        0     2048 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/unary.py
--rw-r--r--   0        0        0     2143 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/url.py
--rw-r--r--   0        0        0      694 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/util/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/util/asyncio.py
--rw-r--r--   0        0        0      969 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/util/threading.py
--rw-r--r--   0        0        0     6349 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/websocket.py
--rw-r--r--   0        0        0      847 2024-05-21 21:42:51.541265 synnax_freighter-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 synnax_freighter-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1233 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/__init__.py
+-rw-r--r--   0        0        0     2101 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/alamos.py
+-rw-r--r--   0        0        0     1521 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/context.py
+-rw-r--r--   0        0        0     2652 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/encoder.py
+-rw-r--r--   0        0        0     4650 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/exceptions.py
+-rw-r--r--   0        0        0     4130 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/http.py
+-rw-r--r--   0        0        0     6923 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/stream.py
+-rw-r--r--   0        0        0     8026 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/sync.py
+-rw-r--r--   0        0        0     4649 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/transport.py
+-rw-r--r--   0        0        0     2048 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/unary.py
+-rw-r--r--   0        0        0     2143 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/url.py
+-rw-r--r--   0        0        0      694 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/util/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/util/asyncio.py
+-rw-r--r--   0        0        0      969 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/util/threading.py
+-rw-r--r--   0        0        0     6349 2024-05-21 22:43:53.970249 synnax_freighter-0.7.2/freighter/websocket.py
+-rw-r--r--   0        0        0      847 2024-05-21 22:44:04.354259 synnax_freighter-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 synnax_freighter-0.7.2/PKG-INFO
```

### Comparing `synnax_freighter-0.7.1/freighter/__init__.py` & `synnax_freighter-0.7.2/freighter/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/alamos.py` & `synnax_freighter-0.7.2/freighter/alamos.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/context.py` & `synnax_freighter-0.7.2/freighter/context.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/encoder.py` & `synnax_freighter-0.7.2/freighter/encoder.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/exceptions.py` & `synnax_freighter-0.7.2/freighter/exceptions.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/http.py` & `synnax_freighter-0.7.2/freighter/http.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/stream.py` & `synnax_freighter-0.7.2/freighter/stream.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/sync.py` & `synnax_freighter-0.7.2/freighter/sync.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/transport.py` & `synnax_freighter-0.7.2/freighter/transport.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/unary.py` & `synnax_freighter-0.7.2/freighter/unary.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/url.py` & `synnax_freighter-0.7.2/freighter/url.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/util/__init__.py` & `synnax_freighter-0.7.2/freighter/util/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/util/asyncio.py` & `synnax_freighter-0.7.2/freighter/util/asyncio.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/util/threading.py` & `synnax_freighter-0.7.2/freighter/util/threading.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/freighter/websocket.py` & `synnax_freighter-0.7.2/freighter/websocket.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.7.1/pyproject.toml` & `synnax_freighter-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synnax-freighter"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["emiliano bonilla <emilbon99@gmail.com>"]
 packages = [
     { include = "freighter/**/*.py" }
 ]
 
 [tool.mypy]
@@ -17,15 +17,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 websockets = "^11.0.3"
 msgpack = "^1.0.4"
 urllib3 = "^2.0.3"
 janus = "^1.0.0"
 pydantic = "^1.10.0"
-alamos = "^0.3.42"
+alamos = "^0.3.43"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
 mypy = "^1.3.0"
 pytest-cov = "^4.1.0"
```

### Comparing `synnax_freighter-0.7.1/PKG-INFO` & `synnax_freighter-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: synnax-freighter
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: emiliano bonilla
 Author-email: emilbon99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: alamos (>=0.3.42,<0.4.0)
+Requires-Dist: alamos (>=0.3.43,<0.4.0)
 Requires-Dist: janus (>=1.0.0,<2.0.0)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
```

