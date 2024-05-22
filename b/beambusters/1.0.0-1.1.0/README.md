# Comparing `tmp/beambusters-1.0.0.tar.gz` & `tmp/beambusters-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.0.0.tar", max compression
+gzip compressed data, was "beambusters-1.1.0.tar", max compression
```

## Comparing `beambusters-1.0.0.tar` & `beambusters-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-22 11:53:46.335508 beambusters-1.0.0/LICENSE
--rw-r--r--   0        0        0      630 2024-05-22 11:53:46.335508 beambusters-1.0.0/README.md
--rwxr-xr-x   0        0        0        0 2024-05-22 11:53:46.335508 beambusters-1.0.0/beambusters/__init__.py
--rw-r--r--   0        0        0    11833 2024-05-22 11:53:46.335508 beambusters-1.0.0/beambusters/main.py
--rwxr-xr-x   0        0        0     3170 2024-05-22 11:53:46.335508 beambusters-1.0.0/beambusters/settings.py
--rwxr-xr-x   0        0        0      143 2024-05-22 11:53:46.335508 beambusters-1.0.0/beambusters/utils.py
--rw-r--r--   0        0        0     2010 2024-05-22 11:53:55.803454 beambusters-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 beambusters-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 12:05:01.019777 beambusters-1.1.0/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-22 12:05:01.019777 beambusters-1.1.0/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/__init__.py
+-rw-r--r--   0        0        0    11833 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/main.py
+-rwxr-xr-x   0        0        0     3170 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/settings.py
+-rwxr-xr-x   0        0        0      143 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/utils.py
+-rw-r--r--   0        0        0     2026 2024-05-22 12:05:09.019782 beambusters-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.1.0/PKG-INFO
```

### Comparing `beambusters-1.0.0/LICENSE` & `beambusters-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.0.0/README.md` & `beambusters-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.0.0/beambusters/main.py` & `beambusters-1.1.0/beambusters/main.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.0.0/beambusters/settings.py` & `beambusters-1.1.0/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.0.0/pyproject.toml` & `beambusters-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
 
@@ -88,12 +88,13 @@
 tomlkit = "0.12.3"
 trove-classifiers = "2024.2.23"
 typing-extensions = "4.10.0"
 tzdata = "2024.1"
 urllib3 = "2.2.1"
 virtualenv = "20.25.1"
 zipp = "3.17.0"
+bblib = "2.0.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beambusters-1.0.0/PKG-INFO` & `beambusters-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: abstract (==2022.7.10)
 Requires-Dist: base32hex (==1.0.2)
+Requires-Dist: bblib (==2.0.3)
 Requires-Dist: black (==24.1.1)
 Requires-Dist: build (==1.0.3)
 Requires-Dist: cachecontrol (==0.14.0)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: cffi (==1.16.0)
 Requires-Dist: charset-normalizer (==3.3.2)
 Requires-Dist: cleo (==2.1.0)
```

