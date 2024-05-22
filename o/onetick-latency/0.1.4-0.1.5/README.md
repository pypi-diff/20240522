# Comparing `tmp/onetick_latency-0.1.4.tar.gz` & `tmp/onetick_latency-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.4.tar", last modified: Wed May 22 13:51:03 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.5.tar", last modified: Wed May 22 15:10:02 2024, max compression
```

## Comparing `onetick_latency-0.1.4.tar` & `onetick_latency-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.4/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.4/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-22 12:58:34.000000 onetick_latency-0.1.4/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.4/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 13:51:03.000000 onetick_latency-0.1.4/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.4/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2024-05-22 13:43:15.000000 onetick_latency-0.1.4/pythonAPI/creds.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3000 2024-05-22 13:47:36.000000 onetick_latency-0.1.4/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 13:51:03.344421 onetick_latency-0.1.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 13:50:26.000000 onetick_latency-0.1.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:10:02.954241 onetick_latency-0.1.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 15:10:02.954241 onetick_latency-0.1.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:10:02.954241 onetick_latency-0.1.5/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.5/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.5/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-22 14:20:59.000000 onetick_latency-0.1.5/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.5/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:10:02.954241 onetick_latency-0.1.5/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 15:10:02.000000 onetick_latency-0.1.5/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2024-05-22 15:10:02.000000 onetick_latency-0.1.5/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 15:10:02.000000 onetick_latency-0.1.5/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 15:10:02.000000 onetick_latency-0.1.5/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 15:10:02.000000 onetick_latency-0.1.5/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:10:02.954241 onetick_latency-0.1.5/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.5/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-22 13:17:27.000000 onetick_latency-0.1.5/pythonAPI/auth.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2024-05-22 15:07:25.000000 onetick_latency-0.1.5/pythonAPI/creds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3000 2024-05-22 13:47:36.000000 onetick_latency-0.1.5/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 15:10:02.954241 onetick_latency-0.1.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 15:09:22.000000 onetick_latency-0.1.5/setup.py
```

### Comparing `onetick_latency-0.1.4/PKG-INFO` & `onetick_latency-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.4/README.md` & `onetick_latency-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.4/modules/cross_over_controller.py` & `onetick_latency-0.1.5/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.4/modules/latency_module.py` & `onetick_latency-0.1.5/modules/latency_module.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.4/modules/volume_analyser.py` & `onetick_latency-0.1.5/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.4/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.5/onetick_latency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.4/pythonAPI/creds.py` & `onetick_latency-0.1.5/pythonAPI/creds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import onetick.query as otq
-
 dir_home = "/home/ubuntu/onetick-onboarding/onetick"
 current_dir = "/home/ubuntu/projects/onetick_latency"
 
 try:
-    from auth import username_authentication, password_authentication
+    from pythonAPI.auth import username_authentication, password_authentication
 except ImportError:
     raise ImportError("Please create an auth.py file with your username and password. "
                       "Refer to auth_example.py for an example.")
 
 env = os.environ[
     "ONE_TICK_CONFIG"
 ] = f"{dir_home}/client_data/config/one_tick_config.txt"  # point to OneTick main config file on your local machine
```

### Comparing `onetick_latency-0.1.4/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.5/pythonAPI/runnbboquote.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.4/setup.py` & `onetick_latency-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.4',
+    version='0.1.5',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

