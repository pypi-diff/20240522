# Comparing `tmp/upils-0.6.0.tar.gz` & `tmp/upils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upils-0.6.0.tar", max compression
+gzip compressed data, was "upils-0.7.0.tar", max compression
```

## Comparing `upils-0.6.0.tar` & `upils-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      846 2023-10-17 05:07:27.339608 upils-0.6.0/README.md
--rw-r--r--   0        0        0      551 2024-04-22 06:52:19.826932 upils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-17 05:07:27.341060 upils-0.6.0/upils/__init__.py
--rw-r--r--   0        0        0     1946 2024-04-22 06:21:27.721220 upils-0.6.0/upils/datetime.py
--rw-r--r--   0        0        0     1808 2023-11-22 08:11:56.912117 upils-0.6.0/upils/logging.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 upils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      846 2024-05-22 06:32:08.294419 upils-0.7.0/README.md
+-rw-r--r--   0        0        0      551 2024-05-22 07:26:47.529930 upils-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 06:32:08.295204 upils-0.7.0/upils/__init__.py
+-rw-r--r--   0        0        0     1946 2024-05-22 06:32:08.295342 upils-0.7.0/upils/datetime.py
+-rw-r--r--   0        0        0      187 2024-05-22 07:14:56.466929 upils-0.7.0/upils/list.py
+-rw-r--r--   0        0        0     1808 2024-05-22 06:32:08.295467 upils-0.7.0/upils/logging.py
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 upils-0.7.0/PKG-INFO
```

### Comparing `upils-0.6.0/README.md` & `upils-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `upils-0.6.0/pyproject.toml` & `upils-0.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upils"
-version = "0.6.0"
+version = "0.7.0"
 description = "Unified Python Utils. Requires python 3.10 and later"
 authors = [
     "Aslam Hadi Harsono <aslam.hadi@kumparan.com>",
     "Malik Fajar Mubarok <malik.fajar@kumparan.com>",
     "Niti Cahyaning Utami <niti.utami@kumparan.com>"
 ]
 readme = "README.md"
```

### Comparing `upils-0.6.0/upils/datetime.py` & `upils-0.7.0/upils/datetime.py`

 * *Files identical despite different names*

### Comparing `upils-0.6.0/upils/logging.py` & `upils-0.7.0/upils/logging.py`

 * *Files identical despite different names*

### Comparing `upils-0.6.0/PKG-INFO` & `upils-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: upils
-Version: 0.6.0
+Version: 0.7.0
 Summary: Unified Python Utils. Requires python 3.10 and later
 Author: Aslam Hadi Harsono
 Author-email: aslam.hadi@kumparan.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pytz (>=2022.1,<2023.0)
 Description-Content-Type: text/markdown
 
 # Unified Python Utils
 
 Collection of python library utils
```

