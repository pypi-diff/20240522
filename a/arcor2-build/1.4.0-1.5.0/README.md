# Comparing `tmp/arcor2_build-1.4.0.tar.gz` & `tmp/arcor2_build-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_build-1.4.0.tar", last modified: Thu Apr 11 09:47:34 2024, max compression
+gzip compressed data, was "arcor2_build-1.5.0.tar", last modified: Wed May 22 07:51:40 2024, max compression
```

## Comparing `arcor2_build-1.4.0.tar` & `arcor2_build-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:34.957130 arcor2_build-1.4.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     8230 2024-04-11 09:47:34.957130 arcor2_build-1.4.0/PKG-INFO
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:34.949130 arcor2_build-1.4.0/arcor2_build/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/VERSION
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       96 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/py.typed
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:34.953130 arcor2_build-1.4.0/arcor2_build/scripts/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/scripts/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    24286 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/scripts/build.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:34.957130 arcor2_build-1.4.0/arcor2_build/source/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/source/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    10300 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/source/logic.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      918 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/source/object_types.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    17825 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/source/python_to_json.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    19211 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/arcor2_build/source/utils.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:34.953130 arcor2_build-1.4.0/arcor2_build.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     8230 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      594 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       65 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/entry_points.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      162 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       13 2024-04-11 09:47:34.000000 arcor2_build-1.4.0/arcor2_build.egg-info/top_level.txt
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/backend_shim.py
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-11 09:47:34.957130 arcor2_build-1.4.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     9139 2024-04-11 09:47:33.000000 arcor2_build-1.4.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     8322 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/PKG-INFO
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/arcor2_build/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/VERSION
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       96 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/py.typed
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/arcor2_build/scripts/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/scripts/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    24286 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/scripts/build.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/arcor2_build/source/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/source/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    10300 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/source/logic.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      918 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/source/object_types.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    17825 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/source/python_to_json.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    19211 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build/source/utils.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/arcor2_build.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     8322 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      594 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       65 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      162 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       13 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/arcor2_build.egg-info/top_level.txt
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/backend_shim.py
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-05-22 07:51:40.521385 arcor2_build-1.5.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     9231 2024-05-22 07:51:40.000000 arcor2_build-1.5.0/setup.py
```

### Comparing `arcor2_build-1.4.0/PKG-INFO` & `arcor2_build-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2_build
-Version: 1.4.0
+Version: 1.5.0
 Summary: ARCOR2 Build
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -24,14 +24,20 @@
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project service.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 - `ARCOR2_PROJECT_PATH=""` - can be set to an arbitrary value, not actually used.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.5.0] - 2024-05-22
+
+### Changed
+
+- Updated dependency on the Project Service (2.0.0).
+
 ## [1.4.0] - 2024-04-11
 
 ### Changed
 
 - Updated dependencies, switched to Python 3.11.
 
 ## [1.3.2] - 2024-02-01
```

### Comparing `arcor2_build-1.4.0/arcor2_build/scripts/build.py` & `arcor2_build-1.5.0/arcor2_build/scripts/build.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/arcor2_build/source/logic.py` & `arcor2_build-1.5.0/arcor2_build/source/logic.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/arcor2_build/source/object_types.py` & `arcor2_build-1.5.0/arcor2_build/source/object_types.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/arcor2_build/source/python_to_json.py` & `arcor2_build-1.5.0/arcor2_build/source/python_to_json.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/arcor2_build/source/utils.py` & `arcor2_build-1.5.0/arcor2_build/source/utils.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/arcor2_build.egg-info/PKG-INFO` & `arcor2_build-1.5.0/arcor2_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2-build
-Version: 1.4.0
+Version: 1.5.0
 Summary: ARCOR2 Build
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -24,14 +24,20 @@
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project service.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 - `ARCOR2_PROJECT_PATH=""` - can be set to an arbitrary value, not actually used.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.5.0] - 2024-05-22
+
+### Changed
+
+- Updated dependency on the Project Service (2.0.0).
+
 ## [1.4.0] - 2024-04-11
 
 ### Changed
 
 - Updated dependencies, switched to Python 3.11.
 
 ## [1.3.2] - 2024-02-01
```

### Comparing `arcor2_build-1.4.0/arcor2_build.egg-info/SOURCES.txt` & `arcor2_build-1.5.0/arcor2_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/backend_shim.py` & `arcor2_build-1.5.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.4.0/setup.py` & `arcor2_build-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project service.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 - `ARCOR2_PROJECT_PATH=""` - can be set to an arbitrary value, not actually used.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.5.0] - 2024-05-22
+
+### Changed
+
+- Updated dependency on the Project Service (2.0.0).
+
 ## [1.4.0] - 2024-04-11
 
 ### Changed
 
 - Updated dependencies, switched to Python 3.11.
 
 ## [1.3.2] - 2024-02-01
@@ -301,9 +307,9 @@
     },
     'packages': (
         'arcor2_build',
         'arcor2_build.scripts',
         'arcor2_build.source',
     ),
     'python_requires': '==3.11.*',
-    'version': '1.4.0',
+    'version': '1.5.0',
 })
```

