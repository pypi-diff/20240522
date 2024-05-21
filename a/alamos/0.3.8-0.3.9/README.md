# Comparing `tmp/alamos-0.3.8.tar.gz` & `tmp/alamos-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alamos-0.3.8.tar", max compression
+gzip compressed data, was "alamos-0.3.9.tar", max compression
```

## Comparing `alamos-0.3.8.tar` & `alamos-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-18 05:34:31.798167 alamos-0.3.8/README.md
--rw-r--r--   0        0        0      493 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/__init__.py
--rw-r--r--   0        0        0     1240 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/dev/__init__.py
--rw-r--r--   0        0        0     1221 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/environment.py
--rw-r--r--   0        0        0     4455 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/instrumentation.py
--rw-r--r--   0        0        0     1708 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/log.py
--rw-r--r--   0        0        0     1001 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/meta.py
--rw-r--r--   0        0        0      988 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/noop.py
--rw-r--r--   0        0        0     6530 2024-04-18 05:34:31.798167 alamos-0.3.8/alamos/trace.py
--rw-r--r--   0        0        0      613 2024-04-18 05:34:42.030215 alamos-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 14:21:30.774753 alamos-0.3.9/README.md
+-rw-r--r--   0        0        0      493 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/dev/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/environment.py
+-rw-r--r--   0        0        0     4455 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/instrumentation.py
+-rw-r--r--   0        0        0     1708 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/log.py
+-rw-r--r--   0        0        0     1001 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/meta.py
+-rw-r--r--   0        0        0      988 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/noop.py
+-rw-r--r--   0        0        0     6530 2024-04-19 14:21:30.774753 alamos-0.3.9/alamos/trace.py
+-rw-r--r--   0        0        0      613 2024-04-19 14:21:41.602752 alamos-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.9/PKG-INFO
```

### Comparing `alamos-0.3.8/alamos/dev/__init__.py` & `alamos-0.3.9/alamos/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/alamos/environment.py` & `alamos-0.3.9/alamos/environment.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/alamos/instrumentation.py` & `alamos-0.3.9/alamos/instrumentation.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/alamos/log.py` & `alamos-0.3.9/alamos/log.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/alamos/meta.py` & `alamos-0.3.9/alamos/meta.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/alamos/noop.py` & `alamos-0.3.9/alamos/noop.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/alamos/trace.py` & `alamos-0.3.9/alamos/trace.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.8/pyproject.toml` & `alamos-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alamos"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["Emiliano Bonilla <ebonilla@synnaxlabs.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.0"
```

### Comparing `alamos-0.3.8/PKG-INFO` & `alamos-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alamos
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: Emiliano Bonilla
 Author-email: ebonilla@synnaxlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

