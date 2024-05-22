# Comparing `tmp/ivande_combiner-0.0.7.tar.gz` & `tmp/ivande_combiner-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivande_combiner-0.0.7.tar", last modified: Wed May 22 04:37:32 2024, max compression
+gzip compressed data, was "ivande_combiner-0.0.8.tar", last modified: Wed May 22 04:46:09 2024, max compression
```

## Comparing `ivande_combiner-0.0.7.tar` & `ivande_combiner-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:32.603427 ivande_combiner-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 04:37:32.603427 ivande_combiner-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:32.599427 ivande_combiner-0.0.7/ivande_combiner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/ivande_combiner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/ivande_combiner/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:32.603427 ivande_combiner-0.0.7/ivande_combiner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 04:37:32.000000 ivande_combiner-0.0.7/ivande_combiner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 04:37:32.000000 ivande_combiner-0.0.7/ivande_combiner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:37:32.000000 ivande_combiner-0.0.7/ivande_combiner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 04:37:32.000000 ivande_combiner-0.0.7/ivande_combiner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 04:37:32.000000 ivande_combiner-0.0.7/ivande_combiner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:37:32.603427 ivande_combiner-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:32.603427 ivande_combiner-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 04:37:24.000000 ivande_combiner-0.0.7/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:46:09.852362 ivande_combiner-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 04:46:09.852362 ivande_combiner-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:46:09.852362 ivande_combiner-0.0.8/ivande_combiner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/ivande_combiner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/ivande_combiner/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:46:09.852362 ivande_combiner-0.0.8/ivande_combiner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 04:46:09.000000 ivande_combiner-0.0.8/ivande_combiner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 04:46:09.000000 ivande_combiner-0.0.8/ivande_combiner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:46:09.000000 ivande_combiner-0.0.8/ivande_combiner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 04:46:09.000000 ivande_combiner-0.0.8/ivande_combiner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 04:46:09.000000 ivande_combiner-0.0.8/ivande_combiner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:46:09.852362 ivande_combiner-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:46:09.852362 ivande_combiner-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 04:46:02.000000 ivande_combiner-0.0.8/tests/test_module.py
```

### Comparing `ivande_combiner-0.0.7/LICENSE.txt` & `ivande_combiner-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ivande_combiner-0.0.7/PKG-INFO` & `ivande_combiner-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivande_combiner
-Version: 0.0.7
+Version: 0.0.8
 Summary: basic functionality for classic sklearn ml
 Home-page: https://github.com/IvanDe83/ivande_combiner
 Author: IvanDe
 Author-email: ivande83@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ivande_combiner-0.0.7/ivande_combiner.egg-info/PKG-INFO` & `ivande_combiner-0.0.8/ivande_combiner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivande-combiner
-Version: 0.0.7
+Version: 0.0.8
 Summary: basic functionality for classic sklearn ml
 Home-page: https://github.com/IvanDe83/ivande_combiner
 Author: IvanDe
 Author-email: ivande83@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ivande_combiner-0.0.7/setup.py` & `ivande_combiner-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ivande_combiner",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     description="basic functionality for classic sklearn ml",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="IvanDe",
     author_email="ivande83@gmail.com",
     url="https://github.com/IvanDe83/ivande_combiner",
```

