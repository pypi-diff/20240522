# Comparing `tmp/kubectl_ng-0.9.1.tar.gz` & `tmp/kubectl_ng-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubectl_ng-0.9.1.tar", max compression
+gzip compressed data, was "kubectl_ng-0.9.2.tar", max compression
```

## Comparing `kubectl_ng-0.9.1.tar` & `kubectl_ng-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       80 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/README.md
--rw-r--r--   0        0        0      185 2023-10-17 16:16:46.328086 kubectl_ng-0.9.1/kubectl_ng/__init__.py
--rw-r--r--   0        0        0     4592 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_api_resources.py
--rw-r--r--   0        0        0     1374 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_create.py
--rw-r--r--   0        0        0     1711 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_delete.py
--rw-r--r--   0        0        0      769 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_formatters.py
--rw-r--r--   0        0        0     4285 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_get.py
--rw-r--r--   0        0        0     1981 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_version.py
--rw-r--r--   0        0        0     5464 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/_wait.py
--rw-r--r--   0        0        0      858 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/cli.py
--rw-r--r--   0        0        0      435 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/tests/resources/simple/nginx_pod_service.yaml
--rw-r--r--   0        0        0      802 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/tests/test_create_delete.py
--rw-r--r--   0        0        0     1029 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/tests/test_formatters.py
--rw-r--r--   0        0        0      818 2023-10-17 16:16:30.347718 kubectl_ng-0.9.1/kubectl_ng/tests/test_version.py
--rw-r--r--   0        0        0      623 2023-10-17 16:16:46.328086 kubectl_ng-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 kubectl_ng-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/README.md
+-rw-r--r--   0        0        0      185 2023-10-17 21:03:03.885248 kubectl_ng-0.9.2/kubectl_ng/__init__.py
+-rw-r--r--   0        0        0     4592 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_api_resources.py
+-rw-r--r--   0        0        0     1374 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_create.py
+-rw-r--r--   0        0        0     1711 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_delete.py
+-rw-r--r--   0        0        0      769 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_formatters.py
+-rw-r--r--   0        0        0     4285 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_get.py
+-rw-r--r--   0        0        0     1981 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_version.py
+-rw-r--r--   0        0        0     5464 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/_wait.py
+-rw-r--r--   0        0        0      858 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/cli.py
+-rw-r--r--   0        0        0      435 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/tests/resources/simple/nginx_pod_service.yaml
+-rw-r--r--   0        0        0      802 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/tests/test_create_delete.py
+-rw-r--r--   0        0        0     1029 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/tests/test_formatters.py
+-rw-r--r--   0        0        0      818 2023-10-17 21:02:40.577077 kubectl_ng-0.9.2/kubectl_ng/tests/test_version.py
+-rw-r--r--   0        0        0      623 2023-10-17 21:03:03.885248 kubectl_ng-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 kubectl_ng-0.9.2/PKG-INFO
```

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_api_resources.py` & `kubectl_ng-0.9.2/kubectl_ng/_api_resources.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_create.py` & `kubectl_ng-0.9.2/kubectl_ng/_create.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_delete.py` & `kubectl_ng-0.9.2/kubectl_ng/_delete.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_formatters.py` & `kubectl_ng-0.9.2/kubectl_ng/_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_get.py` & `kubectl_ng-0.9.2/kubectl_ng/_get.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_version.py` & `kubectl_ng-0.9.2/kubectl_ng/_version.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/_wait.py` & `kubectl_ng-0.9.2/kubectl_ng/_wait.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/cli.py` & `kubectl_ng-0.9.2/kubectl_ng/cli.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/tests/test_create_delete.py` & `kubectl_ng-0.9.2/kubectl_ng/tests/test_create_delete.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/tests/test_formatters.py` & `kubectl_ng-0.9.2/kubectl_ng/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/kubectl_ng/tests/test_version.py` & `kubectl_ng-0.9.2/kubectl_ng/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.9.1/pyproject.toml` & `kubectl_ng-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kubectl-ng"
-version = "0.9.1"
+version = "0.9.2"
 description = ""
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 readme = "README.md"
 packages = [{include = "kubectl_ng"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `kubectl_ng-0.9.1/PKG-INFO` & `kubectl_ng-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubectl-ng
-Version: 0.9.1
+Version: 0.9.2
 Summary: 
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

