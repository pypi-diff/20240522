# Comparing `tmp/uploadthing_py-0.3.1.tar.gz` & `tmp/uploadthing_py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.3.1.tar", max compression
+gzip compressed data, was "uploadthing_py-0.3.2.tar", max compression
```

## Comparing `uploadthing_py-0.3.1.tar` & `uploadthing_py-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2538 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/README.md
--rw-r--r--   0        0        0      627 2024-05-21 23:06:08.828448 uploadthing_py-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      663 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/builder.py
--rw-r--r--   0        0        0        0 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/py.typed
--rw-r--r--   0        0        0    11603 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/request_handler.py
--rw-r--r--   0        0        0     3719 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/types.py
--rw-r--r--   0        0        0     5561 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/utapi.py
--rw-r--r--   0        0        0     1385 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/utils.py
--rw-r--r--   0        0        0     2893 1970-01-01 00:00:00.000000 uploadthing_py-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2538 2024-05-21 23:09:33.156553 uploadthing_py-0.3.2/README.md
+-rw-r--r--   0        0        0      627 2024-05-21 23:09:45.848638 uploadthing_py-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      663 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/builder.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/py.typed
+-rw-r--r--   0        0        0    11603 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/request_handler.py
+-rw-r--r--   0        0        0     3719 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5561 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0     1385 2024-05-21 23:09:33.160553 uploadthing_py-0.3.2/uploadthing_py/utils.py
+-rw-r--r--   0        0        0     2893 1970-01-01 00:00:00.000000 uploadthing_py-0.3.2/PKG-INFO
```

### Comparing `uploadthing_py-0.3.1/README.md` & `uploadthing_py-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/pyproject.toml` & `uploadthing_py-0.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uploadthing.py"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python SDK for UploadThing"
 authors = ["juliusmarminge <julius0216@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "uploadthing_py" }]
 license = "MIT"
```

### Comparing `uploadthing_py-0.3.1/uploadthing_py/__init__.py` & `uploadthing_py-0.3.2/uploadthing_py/__init__.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/uploadthing_py/builder.py` & `uploadthing_py-0.3.2/uploadthing_py/builder.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/uploadthing_py/request_handler.py` & `uploadthing_py-0.3.2/uploadthing_py/request_handler.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/uploadthing_py/types.py` & `uploadthing_py-0.3.2/uploadthing_py/types.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/uploadthing_py/utapi.py` & `uploadthing_py-0.3.2/uploadthing_py/utapi.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/uploadthing_py/utils.py` & `uploadthing_py-0.3.2/uploadthing_py/utils.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.1/PKG-INFO` & `uploadthing_py-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploadthing.py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for UploadThing
 License: MIT
 Author: juliusmarminge
 Author-email: julius0216@outlook.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

