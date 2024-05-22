# Comparing `tmp/onetick_latency-0.1.7.tar.gz` & `tmp/onetick_latency-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.7.tar", last modified: Wed May 22 17:30:22 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.8.tar", last modified: Wed May 22 17:41:30 2024, max compression
```

## Comparing `onetick_latency-0.1.7.tar` & `onetick_latency-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2024-05-22 17:28:52.000000 onetick_latency-0.1.7/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.7/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.7/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8197 2024-05-22 17:28:52.000000 onetick_latency-0.1.7/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.7/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      366 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.7/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-22 15:56:30.000000 onetick_latency-0.1.7/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 17:29:23.000000 onetick_latency-0.1.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2024-05-22 17:28:52.000000 onetick_latency-0.1.8/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.8/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.8/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8181 2024-05-22 17:40:57.000000 onetick_latency-0.1.8/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.8/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      366 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 17:41:30.000000 onetick_latency-0.1.8/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.8/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-22 15:56:30.000000 onetick_latency-0.1.8/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 17:41:30.465296 onetick_latency-0.1.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 17:40:57.000000 onetick_latency-0.1.8/setup.py
```

### Comparing `onetick_latency-0.1.7/PKG-INFO` & `onetick_latency-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.7/README.md` & `onetick_latency-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.7/modules/cross_over_controller.py` & `onetick_latency-0.1.8/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.7/modules/latency_module.py` & `onetick_latency-0.1.8/modules/latency_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Developed by Alexandre Levert, NBC (National Bank du Canada)
 May 2024
 
 This module simulates network latency based on trading activity and high-activity periods identified
 by the VolumeAnalyser. It uses the DataFrame of trading data to adjust timestamps based on calculated latencies.
 """
 
-from onetick_latency.pythonAPI.runnbboquote import OneTickQueryRunner
+from pythonAPI.runnbboquote import OneTickQueryRunner
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from modules.volume_analyser import VolumeAnalyser
 from modules.cross_over_controller import CrossOverController
 
 MINUTES_IN_HOUR = 60
```

### Comparing `onetick_latency-0.1.7/modules/volume_analyser.py` & `onetick_latency-0.1.8/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.7/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.8/onetick_latency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.7/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.8/pythonAPI/runnbboquote.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.7/setup.py` & `onetick_latency-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.7',
+    version='0.1.8',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

