# Comparing `tmp/onetick_latency-0.1.3.tar.gz` & `tmp/onetick_latency-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.3.tar", last modified: Wed May 22 13:20:00 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.4.tar", last modified: Wed May 22 13:51:03 2024, max compression
```

## Comparing `onetick_latency-0.1.3.tar` & `onetick_latency-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.577139 onetick_latency-0.1.3/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.3/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.3/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-22 12:58:34.000000 onetick_latency-0.1.3/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.3/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.577139 onetick_latency-0.1.3/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.3/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-21 20:30:57.000000 onetick_latency-0.1.3/pythonAPI/auth.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3031 2024-05-22 13:17:53.000000 onetick_latency-0.1.3/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-05-21 20:16:37.000000 onetick_latency-0.1.3/pythonAPI/security_credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 13:18:48.000000 onetick_latency-0.1.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.4/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.4/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-22 12:58:34.000000 onetick_latency-0.1.4/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.4/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.4/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2024-05-22 13:43:15.000000 onetick_latency-0.1.4/pythonAPI/creds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3000 2024-05-22 13:47:36.000000 onetick_latency-0.1.4/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 13:50:26.000000 onetick_latency-0.1.4/setup.py
```

### Comparing `onetick_latency-0.1.3/PKG-INFO` & `onetick_latency-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.3/README.md` & `onetick_latency-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.3/modules/cross_over_controller.py` & `onetick_latency-0.1.4/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.3/modules/latency_module.py` & `onetick_latency-0.1.4/modules/latency_module.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.3/modules/volume_analyser.py` & `onetick_latency-0.1.4/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.3/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.4/onetick_latency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.3/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.4/pythonAPI/runnbboquote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import onetick.query as otq
-from onetick_latency.creds import dir_home, current_dir, username_authentication, password_authentication
+from pythonAPI.creds import dir_home, current_dir, username_authentication
 import pandas as pd
 import time
 import datetime as dt
 import pytz
 
 class OneTickQueryRunner:
```

### Comparing `onetick_latency-0.1.3/setup.py` & `onetick_latency-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.3',
+    version='0.1.4',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

