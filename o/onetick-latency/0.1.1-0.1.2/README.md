# Comparing `tmp/onetick_latency-0.1.1.tar.gz` & `tmp/onetick_latency-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.1.tar", last modified: Tue May 21 20:40:00 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.2.tar", last modified: Tue May 21 20:44:45 2024, max compression
```

## Comparing `onetick_latency-0.1.1.tar` & `onetick_latency-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:40:00.615295 onetick_latency-0.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-21 20:40:00.615295 onetick_latency-0.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:40:00.615295 onetick_latency-0.1.1/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.1/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.1/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8128 2024-05-17 14:52:06.000000 onetick_latency-0.1.1/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.1/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:40:00.615295 onetick_latency-0.1.1/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-21 20:40:00.000000 onetick_latency-0.1.1/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-05-21 20:40:00.000000 onetick_latency-0.1.1/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-21 20:40:00.000000 onetick_latency-0.1.1/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-21 20:40:00.000000 onetick_latency-0.1.1/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-21 20:40:00.000000 onetick_latency-0.1.1/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:40:00.615295 onetick_latency-0.1.1/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.1/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-21 20:30:57.000000 onetick_latency-0.1.1/pythonAPI/auth.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2024-05-21 20:30:57.000000 onetick_latency-0.1.1/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-05-21 20:16:37.000000 onetick_latency-0.1.1/pythonAPI/security_credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-21 20:40:00.615295 onetick_latency-0.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-21 20:38:28.000000 onetick_latency-0.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.562859 onetick_latency-0.1.2/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.2/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.2/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8128 2024-05-17 14:52:06.000000 onetick_latency-0.1.2/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.2/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.2/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-21 20:30:57.000000 onetick_latency-0.1.2/pythonAPI/auth.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3133 2024-05-21 20:44:01.000000 onetick_latency-0.1.2/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-05-21 20:16:37.000000 onetick_latency-0.1.2/pythonAPI/security_credentials.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-21 20:44:43.000000 onetick_latency-0.1.2/setup.py
```

### Comparing `onetick_latency-0.1.1/PKG-INFO` & `onetick_latency-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.1/README.md` & `onetick_latency-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.1/modules/cross_over_controller.py` & `onetick_latency-0.1.2/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.1/modules/latency_module.py` & `onetick_latency-0.1.2/modules/latency_module.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.1/modules/volume_analyser.py` & `onetick_latency-0.1.2/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.1/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.2/onetick_latency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.1/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.2/pythonAPI/runnbboquote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import os
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 import onetick.query as otq
-from creds import dir_home, current_dir, username_authentication, password_authentication
+from onetick_latency.creds import dir_home, current_dir, username_authentication, password_authentication
 import pandas as pd
 import time
 import datetime as dt
 import pytz
 
 class OneTickQueryRunner:
```

### Comparing `onetick_latency-0.1.1/setup.py` & `onetick_latency-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.1',
+    version='0.1.2',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

