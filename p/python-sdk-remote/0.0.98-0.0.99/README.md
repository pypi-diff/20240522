# Comparing `tmp/python_sdk_remote-0.0.98.tar.gz` & `tmp/python_sdk_remote-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sdk_remote-0.0.98.tar", last modified: Fri May 17 16:11:47 2024, max compression
+gzip compressed data, was "python_sdk_remote-0.0.99.tar", last modified: Sun May 19 08:22:02 2024, max compression
```

## Comparing `python_sdk_remote-0.0.98.tar` & `python_sdk_remote-0.0.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:11:47.812288 python_sdk_remote-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-17 16:11:47.812288 python_sdk_remote-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:11:47.808288 python_sdk_remote-0.0.98/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:11:47.812288 python_sdk_remote-0.0.98/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/http_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:11:47.812288 python_sdk_remote-0.0.98/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-17 16:11:47.000000 python_sdk_remote-0.0.98/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 16:11:47.000000 python_sdk_remote-0.0.98/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:11:47.000000 python_sdk_remote-0.0.98/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 16:11:47.000000 python_sdk_remote-0.0.98/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 16:11:47.000000 python_sdk_remote-0.0.98/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:11:47.812288 python_sdk_remote-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-17 16:11:37.000000 python_sdk_remote-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:22:02.650246 python_sdk_remote-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-19 08:22:02.650246 python_sdk_remote-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:22:02.646246 python_sdk_remote-0.0.99/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:22:02.650246 python_sdk_remote-0.0.99/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:22:02.650246 python_sdk_remote-0.0.99/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-19 08:22:02.000000 python_sdk_remote-0.0.99/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-19 08:22:02.000000 python_sdk_remote-0.0.99/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:22:02.000000 python_sdk_remote-0.0.99/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 08:22:02.000000 python_sdk_remote-0.0.99/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 08:22:02.000000 python_sdk_remote-0.0.99/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:22:02.650246 python_sdk_remote-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-19 08:21:54.000000 python_sdk_remote-0.0.99/setup.py
```

### Comparing `python_sdk_remote-0.0.98/PKG-INFO` & `python_sdk_remote-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.98/README.md` & `python_sdk_remote-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/constants.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/http_response.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/http_response.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/mini_logger.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/our_object.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/unified_json.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/utilities.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/utilities.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote/src/validate_environment.py` & `python_sdk_remote-0.0.99/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote.egg-info/PKG-INFO` & `python_sdk_remote-0.0.99/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.98/python_sdk_remote.egg-info/SOURCES.txt` & `python_sdk_remote-0.0.99/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.98/setup.py` & `python_sdk_remote-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.98',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.99',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

