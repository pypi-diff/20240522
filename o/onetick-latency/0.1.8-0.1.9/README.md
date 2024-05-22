# Comparing `tmp/onetick_latency-0.1.8.tar.gz` & `tmp/onetick_latency-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.8.tar", last modified: Wed May 22 17:41:30 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.9.tar", last modified: Wed May 22 17:44:18 2024, max compression
```

## Comparing `onetick_latency-0.1.8.tar` & `onetick_latency-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2024-05-22 17:28:52.000000 onetick_latency-0.1.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.8/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.8/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8181 2024-05-22 17:40:57.000000 onetick_latency-0.1.8/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.8/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      366 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.8/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-22 15:56:30.000000 onetick_latency-0.1.8/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 17:40:57.000000 onetick_latency-0.1.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:44:18.008412 onetick_latency-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:44:18.008412 onetick_latency-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2024-05-22 17:28:52.000000 onetick_latency-0.1.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:44:18.004413 onetick_latency-0.1.9/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.9/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.9/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8181 2024-05-22 17:40:57.000000 onetick_latency-0.1.9/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.9/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:44:18.008412 onetick_latency-0.1.9/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:44:17.000000 onetick_latency-0.1.9/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      366 2024-05-22 17:44:17.000000 onetick_latency-0.1.9/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 17:44:17.000000 onetick_latency-0.1.9/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 17:44:17.000000 onetick_latency-0.1.9/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 17:44:17.000000 onetick_latency-0.1.9/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:44:18.008412 onetick_latency-0.1.9/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.9/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-22 15:56:30.000000 onetick_latency-0.1.9/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 17:44:18.008412 onetick_latency-0.1.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 17:44:14.000000 onetick_latency-0.1.9/setup.py
```

### Comparing `onetick_latency-0.1.8/PKG-INFO` & `onetick_latency-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.8/README.md` & `onetick_latency-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.8/modules/cross_over_controller.py` & `onetick_latency-0.1.9/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.8/modules/latency_module.py` & `onetick_latency-0.1.9/modules/latency_module.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.8/modules/volume_analyser.py` & `onetick_latency-0.1.9/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.8/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.9/onetick_latency.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.8/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.9/pythonAPI/runnbboquote.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.8/setup.py` & `onetick_latency-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.8',
+    version='0.1.9',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

