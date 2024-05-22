# Comparing `tmp/functions-framework-3.5.0.tar.gz` & `tmp/functions_framework-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functions-framework-3.5.0.tar", last modified: Tue Nov 28 23:10:01 2023, max compression
+gzip compressed data, was "functions_framework-3.6.0.tar", last modified: Tue Apr 30 22:45:16 2024, max compression
```

## Comparing `functions-framework-3.5.0.tar` & `functions_framework-3.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.629592 functions-framework-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-28 23:09:54.000000 functions-framework-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2023-11-28 23:10:01.629592 functions-framework-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15243 2023-11-28 23:09:54.000000 functions-framework-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-28 23:10:01.629592 functions-framework-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-11-28 23:09:54.000000 functions-framework-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.613592 functions-framework-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.617592 functions-framework-3.5.0/src/functions_framework/
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/_function_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.621592 functions-framework-3.5.0/src/functions_framework/_http/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/_http/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/_http/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/_typed_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/background_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    14586 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/event_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/functions_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.625592 functions-framework-3.5.0/src/functions_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-28 23:10:01.000000 functions-framework-3.5.0/src/functions_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.621592 functions-framework-3.5.0/src/google/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.621592 functions-framework-3.5.0/src/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.621592 functions-framework-3.5.0/src/google/cloud/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/functions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.621592 functions-framework-3.5.0/src/google/cloud/functions_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/functions_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/functions_v1/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.625592 functions-framework-3.5.0/src/google/cloud/functions_v1beta2/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/functions_v1beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-28 23:09:54.000000 functions-framework-3.5.0/src/google/cloud/functions_v1beta2/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 23:10:01.625592 functions-framework-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_cloud_event_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22960 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_decorator_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_function_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19289 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_typed_event_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2023-11-28 23:09:54.000000 functions-framework-3.5.0/tests/test_view_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.290922 functions_framework-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 22:45:09.000000 functions_framework-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-30 22:45:16.290922 functions_framework-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-04-30 22:45:09.000000 functions_framework-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 22:45:16.290922 functions_framework-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-30 22:45:09.000000 functions_framework-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.278922 functions_framework-3.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.282922 functions_framework-3.6.0/src/functions_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/_function_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.286922 functions_framework-3.6.0/src/functions_framework/_http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/_http/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/_http/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/_typed_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/background_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/event_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/functions_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.290922 functions_framework-3.6.0/src/functions_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 22:45:16.000000 functions_framework-3.6.0/src/functions_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.286922 functions_framework-3.6.0/src/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.286922 functions_framework-3.6.0/src/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.286922 functions_framework-3.6.0/src/google/cloud/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/functions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.286922 functions_framework-3.6.0/src/google/cloud/functions_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/functions_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/functions_v1/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.286922 functions_framework-3.6.0/src/google/cloud/functions_v1beta2/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/functions_v1beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 22:45:09.000000 functions_framework-3.6.0/src/google/cloud/functions_v1beta2/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:45:16.290922 functions_framework-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_cloud_event_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22960 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_decorator_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_function_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_typed_event_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-30 22:45:09.000000 functions_framework-3.6.0/tests/test_view_functions.py
```

### Comparing `functions-framework-3.5.0/LICENSE` & `functions_framework-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/PKG-INFO` & `functions_framework-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: functions-framework
-Version: 3.5.0
+Version: 3.6.0
 Summary: An open source FaaS (Function as a service) framework for writing portable Python functions -- brought to you by the Google Cloud Functions team.
 Home-page: https://github.com/googlecloudplatform/functions-framework-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 Keywords: functions-framework
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask<4.0,>=1.0
 Requires-Dist: click<9.0,>=7.0
 Requires-Dist: watchdog>=1.0.0
 Requires-Dist: gunicorn>=19.2.0; platform_system != "Windows"
```

### Comparing `functions-framework-3.5.0/README.md` & `functions_framework-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/setup.py` & `functions_framework-3.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,32 +21,31 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="functions-framework",
-    version="3.5.0",
+    version="3.6.0",
     description="An open source FaaS (Function as a service) framework for writing portable Python functions -- brought to you by the Google Cloud Functions team.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/googlecloudplatform/functions-framework-python",
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable ",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="functions-framework",
     packages=find_packages(where="src"),
     package_data={"functions_framework": ["py.typed"]},
     namespace_packages=["google", "google.cloud"],
     package_dir={"": "src"},
     python_requires=">=3.5, <4",
```

### Comparing `functions-framework-3.5.0/src/functions_framework/__init__.py` & `functions_framework-3.6.0/src/functions_framework/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,17 +61,17 @@
     def write(self, out):
         payload = dict(severity=self.level, message=out.rstrip("\n"))
         return self.stderr.write(json.dumps(payload) + "\n")
 
 
 def cloud_event(func: CloudEventFunction) -> CloudEventFunction:
     """Decorator that registers cloudevent as user function signature type."""
-    _function_registry.REGISTRY_MAP[
-        func.__name__
-    ] = _function_registry.CLOUDEVENT_SIGNATURE_TYPE
+    _function_registry.REGISTRY_MAP[func.__name__] = (
+        _function_registry.CLOUDEVENT_SIGNATURE_TYPE
+    )
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
 
@@ -101,17 +101,17 @@
     else:
         input_type = args[0]
         return _typed
 
 
 def http(func: HTTPFunction) -> HTTPFunction:
     """Decorator that registers http as user function signature type."""
-    _function_registry.REGISTRY_MAP[
-        func.__name__
-    ] = _function_registry.HTTP_SIGNATURE_TYPE
+    _function_registry.REGISTRY_MAP[func.__name__] = (
+        _function_registry.HTTP_SIGNATURE_TYPE
+    )
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `functions-framework-3.5.0/src/functions_framework/__main__.py` & `functions_framework-3.6.0/src/functions_framework/__main__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/_cli.py` & `functions_framework-3.6.0/src/functions_framework/_cli.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/_function_registry.py` & `functions_framework-3.6.0/src/functions_framework/_function_registry.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/_http/__init__.py` & `functions_framework-3.6.0/src/functions_framework/_http/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/_http/flask.py` & `functions_framework-3.6.0/src/functions_framework/_http/flask.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/_http/gunicorn.py` & `functions_framework-3.6.0/src/functions_framework/_http/gunicorn.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 import gunicorn.app.base
 
 
 class GunicornApplication(gunicorn.app.base.BaseApplication):
     def __init__(self, app, host, port, debug, **options):
         self.options = {
             "bind": "%s:%s" % (host, port),
-            "workers": 1,
-            "threads": (os.cpu_count() or 1) * 4,
-            "timeout": 0,
+            "workers": os.environ.get("WORKERS", (os.cpu_count() or 1) * 4),
+            "threads": os.environ.get("THREADS", 1),
+            "timeout": os.environ.get("CLOUD_RUN_TIMEOUT_SECONDS", 300),
             "loglevel": "error",
             "limit_request_line": 0,
         }
         self.options.update(options)
         self.app = app
+
         super().__init__()
 
     def load_config(self):
         for key, value in self.options.items():
             self.cfg.set(key, value)
 
     def load(self):
```

### Comparing `functions-framework-3.5.0/src/functions_framework/_typed_event.py` & `functions_framework-3.6.0/src/functions_framework/_typed_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         raise FunctionsFrameworkException(
             "Functions using the @typed decorator must provide "
             "the type of the input parameter by specifying @typed(inputType) and/or using python "
             "type annotations 'def your_fn(in: inputType)'"
         )
 
     _function_registry.INPUT_TYPE_MAP[func.__name__] = input_type
-    _function_registry.REGISTRY_MAP[
-        func.__name__
-    ] = _function_registry.TYPED_SIGNATURE_TYPE
+    _function_registry.REGISTRY_MAP[func.__name__] = (
+        _function_registry.TYPED_SIGNATURE_TYPE
+    )
 
 
 """ Checks whether the response type of the typed function has a to_dict method"""
 
 
 def _validate_return_type(response):
     if not (hasattr(response, "to_dict") and callable(getattr(response, "to_dict"))):
```

### Comparing `functions-framework-3.5.0/src/functions_framework/background_event.py` & `functions_framework-3.6.0/src/functions_framework/background_event.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/event_conversion.py` & `functions_framework-3.6.0/src/functions_framework/event_conversion.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework/exceptions.py` & `functions_framework-3.6.0/src/functions_framework/exceptions.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/functions_framework.egg-info/PKG-INFO` & `functions_framework-3.6.0/src/functions_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: functions-framework
-Version: 3.5.0
+Version: 3.6.0
 Summary: An open source FaaS (Function as a service) framework for writing portable Python functions -- brought to you by the Google Cloud Functions team.
 Home-page: https://github.com/googlecloudplatform/functions-framework-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 Keywords: functions-framework
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask<4.0,>=1.0
 Requires-Dist: click<9.0,>=7.0
 Requires-Dist: watchdog>=1.0.0
 Requires-Dist: gunicorn>=19.2.0; platform_system != "Windows"
```

### Comparing `functions-framework-3.5.0/src/functions_framework.egg-info/SOURCES.txt` & `functions_framework-3.6.0/src/functions_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/__init__.py` & `functions_framework-3.6.0/src/google/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/__init__.py` & `functions_framework-3.6.0/src/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/functions/__init__.py` & `functions_framework-3.6.0/src/google/cloud/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/functions/context.py` & `functions_framework-3.6.0/src/google/cloud/functions/context.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/functions_v1/__init__.py` & `functions_framework-3.6.0/src/google/cloud/functions_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/functions_v1/context.py` & `functions_framework-3.6.0/src/google/cloud/functions_v1/context.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/functions_v1beta2/__init__.py` & `functions_framework-3.6.0/src/google/cloud/functions_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/src/google/cloud/functions_v1beta2/context.py` & `functions_framework-3.6.0/src/google/cloud/functions_v1beta2/context.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_cli.py` & `functions_framework-3.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_cloud_event_functions.py` & `functions_framework-3.6.0/tests/test_cloud_event_functions.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_convert.py` & `functions_framework-3.6.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_decorator_functions.py` & `functions_framework-3.6.0/tests/test_decorator_functions.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_function_registry.py` & `functions_framework-3.6.0/tests/test_function_registry.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_functions.py` & `functions_framework-3.6.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_http.py` & `functions_framework-3.6.0/tests/test_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,25 +93,25 @@
     gunicorn_app = functions_framework._http.gunicorn.GunicornApplication(
         app, host, port, debug, **options
     )
 
     assert gunicorn_app.app == app
     assert gunicorn_app.options == {
         "bind": "%s:%s" % (host, port),
-        "workers": 1,
-        "threads": os.cpu_count() * 4,
-        "timeout": 0,
+        "workers": os.cpu_count() * 4,
+        "threads": 1,
+        "timeout": 300,
         "loglevel": "error",
         "limit_request_line": 0,
     }
 
     assert gunicorn_app.cfg.bind == ["1.2.3.4:1234"]
-    assert gunicorn_app.cfg.workers == 1
-    assert gunicorn_app.cfg.threads == os.cpu_count() * 4
-    assert gunicorn_app.cfg.timeout == 0
+    assert gunicorn_app.cfg.workers == os.cpu_count() * 4
+    assert gunicorn_app.cfg.threads == 1
+    assert gunicorn_app.cfg.timeout == 300
     assert gunicorn_app.load() == app
 
 
 @pytest.mark.parametrize("debug", [True, False])
 def test_flask_application(debug):
     app = pretend.stub(run=pretend.call_recorder(lambda *a, **kw: None))
     host = pretend.stub()
```

### Comparing `functions-framework-3.5.0/tests/test_main.py` & `functions_framework-3.6.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_samples.py` & `functions_framework-3.6.0/tests/test_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     @pytest.mark.slow_integration_test
     def test_cloud_run_http(self):
         client = docker.from_env()
         self.stop_all_containers(client)
 
         TAG = "cloud_run_http"
-        client.images.build(path=str(EXAMPLES_DIR / "cloud_run_http"), tag={TAG})
+        client.images.build(path=str(EXAMPLES_DIR / "cloud_run_http"), tag=TAG)
         container = client.containers.run(image=TAG, detach=True, ports={8080: 8080})
         timeout = 10
         success = False
         while success == False and timeout > 0:
             try:
                 response = requests.get("http://localhost:8080")
                 if response.text == "Hello world!":
```

### Comparing `functions-framework-3.5.0/tests/test_typed_event_functions.py` & `functions_framework-3.6.0/tests/test_typed_event_functions.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.5.0/tests/test_view_functions.py` & `functions_framework-3.6.0/tests/test_view_functions.py`

 * *Files identical despite different names*

