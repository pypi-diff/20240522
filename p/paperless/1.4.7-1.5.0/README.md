# Comparing `tmp/paperless-1.4.7.tar.gz` & `tmp/paperless-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperless-1.4.7.tar", last modified: Wed May 22 13:24:17 2024, max compression
+gzip compressed data, was "paperless-1.5.0.tar", last modified: Wed May 22 16:06:43 2024, max compression
```

## Comparing `paperless-1.4.7.tar` & `paperless-1.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 13:24:13.000000 paperless-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 13:24:13.000000 paperless-1.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 13:24:17.164464 paperless-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 13:24:13.000000 paperless-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.160464 paperless-1.4.7/paperless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/kernels/kernel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/kernels/kernel_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/notebook/notebook_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/paperless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless/serverless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/serverless/serverless_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 13:24:13.000000 paperless-1.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:24:17.164464 paperless-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 13:24:13.000000 paperless-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 13:24:13.000000 paperless-1.4.7/tests/test_e2e_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:06:39.000000 paperless-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 16:06:39.000000 paperless-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 16:06:43.903568 paperless-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 16:06:39.000000 paperless-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.899568 paperless-1.5.0/paperless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/kernels/kernel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/kernels/kernel_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/notebook/notebook_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/paperless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless/serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/serverless/serverless_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:06:39.000000 paperless-1.5.0/paperless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/paperless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 16:06:43.000000 paperless-1.5.0/paperless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 16:06:39.000000 paperless-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:06:43.903568 paperless-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 16:06:39.000000 paperless-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:06:43.903568 paperless-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 16:06:39.000000 paperless-1.5.0/tests/test_e2e_test.py
```

### Comparing `paperless-1.4.7/LICENSE` & `paperless-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/PKG-INFO` & `paperless-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperless
-Version: 1.4.7
+Version: 1.5.0
 Summary: A papermill implementation to run notebooks inside dataproc serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: papermill
```

### Comparing `paperless-1.4.7/README.md` & `paperless-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/paperless/__main__.py` & `paperless-1.5.0/paperless/__main__.py`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/paperless/kernels/kernel_client.py` & `paperless-1.5.0/paperless/kernels/kernel_client.py`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/paperless/kernels/kernel_manager.py` & `paperless-1.5.0/paperless/kernels/kernel_manager.py`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/paperless/paperless.py` & `paperless-1.5.0/paperless/paperless.py`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/paperless/serverless/serverless_manager.py` & `paperless-1.5.0/paperless/serverless/serverless_manager.py`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/paperless.egg-info/PKG-INFO` & `paperless-1.5.0/paperless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperless
-Version: 1.4.7
+Version: 1.5.0
 Summary: A papermill implementation to run notebooks inside dataproc serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: papermill
```

### Comparing `paperless-1.4.7/paperless.egg-info/SOURCES.txt` & `paperless-1.5.0/paperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperless-1.4.7/setup.py` & `paperless-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="paperless",
-    version="1.4.7",
+    version="1.5.0",
     description="A papermill implementation to run notebooks inside dataproc serverless",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     py_modules = ['paperless', 'app'],
     python_requires=">=3.10",
     packages=find_packages(exclude=("tests",)),
```

