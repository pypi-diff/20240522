# Comparing `tmp/python_http_request-0.0.2.tar.gz` & `tmp/python_http_request-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_http_request-0.0.2.tar", max compression
+gzip compressed data, was "python_http_request-0.0.3.tar", max compression
```

## Comparing `python_http_request-0.0.2.tar` & `python_http_request-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     4690 2024-05-18 16:18:51.151968 python_http_request-0.0.2/http_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.2/http_request/py.typed
--rw-r--r--   0        0        0     1234 2024-05-18 16:19:30.790986 python_http_request-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.2/readme.md
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 python_http_request-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     6131 2024-05-22 10:04:28.702122 python_http_request-0.0.3/http_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.3/http_request/py.typed
+-rw-r--r--   0        0        0     1234 2024-05-22 10:04:33.794981 python_http_request-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.3/readme.md
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 python_http_request-0.0.3/PKG-INFO
```

### Comparing `python_http_request-0.0.2/LICENSE` & `python_http_request-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_http_request-0.0.2/pyproject.toml` & `python_http_request-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-http_request"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python http response utils."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 keywords = ["http", "request"]
```

### Comparing `python_http_request-0.0.2/PKG-INFO` & `python_http_request-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-http_request
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python http response utils.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request
 License: MIT
 Keywords: http,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

