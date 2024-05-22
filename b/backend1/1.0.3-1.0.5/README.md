# Comparing `tmp/backend1-1.0.3.tar.gz` & `tmp/backend1-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend1-1.0.3.tar", max compression
+gzip compressed data, was "backend1-1.0.5.tar", max compression
```

## Comparing `backend1-1.0.3.tar` & `backend1-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      111 2024-05-22 02:18:02.771098 backend1-1.0.3/README.md
--rw-r--r--   0        0        0     1298 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/auth/auth_bearer.py
--rw-r--r--   0        0        0      928 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/auth/auth_handler.py
--rw-r--r--   0        0        0      771 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/db/database.py
--rw-r--r--   0        0        0      313 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/db/schemas.py
--rw-r--r--   0        0        0      763 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/main.py
--rw-r--r--   0        0        0      316 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/models/users.py
--rw-r--r--   0        0        0      434 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/operations/users.py
--rw-r--r--   0        0        0     1828 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/routers/table.py
--rw-r--r--   0        0        0     1049 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/routers/test.py
--rw-r--r--   0        0        0     1157 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/routers/users.py
--rw-r--r--   0        0        0      296 2024-05-22 02:18:02.771098 backend1-1.0.3/backend1/utils/utilities.py
--rw-r--r--   0        0        0      645 2024-05-22 02:18:17.935173 backend1-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 backend1-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      111 2024-05-22 02:21:55.578277 backend1-1.0.5/README.md
+-rw-r--r--   0        0        0     1298 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/auth/auth_bearer.py
+-rw-r--r--   0        0        0      928 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/auth/auth_handler.py
+-rw-r--r--   0        0        0      771 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/db/database.py
+-rw-r--r--   0        0        0      313 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/db/schemas.py
+-rw-r--r--   0        0        0      763 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/main.py
+-rw-r--r--   0        0        0      316 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/models/users.py
+-rw-r--r--   0        0        0      434 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/operations/users.py
+-rw-r--r--   0        0        0     1828 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/routers/table.py
+-rw-r--r--   0        0        0     1049 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/routers/test.py
+-rw-r--r--   0        0        0     1157 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/routers/users.py
+-rw-r--r--   0        0        0      296 2024-05-22 02:21:55.578277 backend1-1.0.5/backend1/utils/utilities.py
+-rw-r--r--   0        0        0      645 2024-05-22 02:22:09.150308 backend1-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 backend1-1.0.5/PKG-INFO
```

### Comparing `backend1-1.0.3/backend1/auth/auth_bearer.py` & `backend1-1.0.5/backend1/auth/auth_bearer.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/backend1/auth/auth_handler.py` & `backend1-1.0.5/backend1/auth/auth_handler.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/backend1/db/database.py` & `backend1-1.0.5/backend1/db/database.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/backend1/main.py` & `backend1-1.0.5/backend1/main.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/backend1/routers/table.py` & `backend1-1.0.5/backend1/routers/table.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/backend1/routers/test.py` & `backend1-1.0.5/backend1/routers/test.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/backend1/routers/users.py` & `backend1-1.0.5/backend1/routers/users.py`

 * *Files identical despite different names*

### Comparing `backend1-1.0.3/pyproject.toml` & `backend1-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backend1"
-version = "1.0.3"
+version = "1.0.5"
 description = "This a demo project"
 authors = ["sukruth grandhi <sukruthgrandhiofficial@gmail.com>"]
 readme = "README.md"
 packages = [{include = "backend1"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `backend1-1.0.3/PKG-INFO` & `backend1-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend1
-Version: 1.0.3
+Version: 1.0.5
 Summary: This a demo project
 Author: sukruth grandhi
 Author-email: sukruthgrandhiofficial@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

