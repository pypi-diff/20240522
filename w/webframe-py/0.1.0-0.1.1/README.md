# Comparing `tmp/webframe-py-0.1.0.tar.gz` & `tmp/webframe_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\webframe-py-0.1.0.tar", last modified: Sat May 18 17:51:21 2024, max compression
+gzip compressed data, was "dist\webframe_py-0.1.1.tar", last modified: Wed May 22 16:38:22 2024, max compression
```

## Comparing `webframe-py-0.1.0.tar` & `webframe_py-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 17:51:21.896309 webframe-py-0.1.0/
--rw-rw-rw-   0        0        0      722 2024-05-18 17:51:21.896309 webframe-py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-18 17:51:21.896309 webframe-py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4026 2024-05-18 17:41:27.000000 webframe-py-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 17:51:21.896309 webframe-py-0.1.0/webframe_py.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-18 17:51:21.000000 webframe-py-0.1.0/webframe_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-05-18 17:51:21.000000 webframe-py-0.1.0/webframe_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 17:51:21.000000 webframe-py-0.1.0/webframe_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-18 17:51:21.000000 webframe-py-0.1.0/webframe_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 17:51:21.000000 webframe-py-0.1.0/webframe_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 16:38:22.802558 webframe_py-0.1.1/
+-rw-rw-rw-   0        0        0      950 2024-05-22 16:38:22.801481 webframe_py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-18 18:51:19.000000 webframe_py-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:38:22.802558 webframe_py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4036 2024-05-22 16:35:55.000000 webframe_py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:38:22.761097 webframe_py-0.1.1/webframe_py/
+-rw-rw-rw-   0        0        0        0 2024-05-22 16:35:39.000000 webframe_py-0.1.1/webframe_py/__init__.py
+-rw-rw-rw-   0        0        0     4063 2024-05-18 17:13:37.000000 webframe_py-0.1.1/webframe_py/app.py
+-rw-rw-rw-   0        0        0      708 2024-05-18 12:01:31.000000 webframe_py-0.1.1/webframe_py/middleware.py
+-rw-rw-rw-   0        0        0      982 2024-05-18 17:57:26.000000 webframe_py-0.1.1/webframe_py/response.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:38:22.800486 webframe_py-0.1.1/webframe_py.egg-info/
+-rw-rw-rw-   0        0        0      950 2024-05-22 16:38:22.000000 webframe_py-0.1.1/webframe_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-22 16:38:22.000000 webframe_py-0.1.1/webframe_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:38:22.000000 webframe_py-0.1.1/webframe_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-22 16:38:22.000000 webframe_py-0.1.1/webframe_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 16:38:22.000000 webframe_py-0.1.1/webframe_py.egg-info/top_level.txt
```

### Comparing `webframe-py-0.1.0/PKG-INFO` & `webframe_py-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
-Name: webframe-py
-Version: 0.1.0
-Summary: Python Web framework for learning purposes 
+Name: webframe_py
+Version: 0.1.1
+Summary: Python Web framework for all to build projects easily
 Home-page: https://github.com/me/myproject
 Author: Abdumalikov Asadbek
 Author-email: ali.backenddev@gmail.com
 License: MIT
-Description: Python Web framework for learning purposes 
+Description: 
+        # Python Web Framework built for all users to create projects easier
+        
+        ![Purpose](https://img.shields.io/badge/:purpose-learning-teal)
+        ![PyPI - Version](https://img.shields.io/pypi/v/webframe-py)
+        
+        
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `webframe-py-0.1.0/setup.py` & `webframe_py-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
-NAME = 'webframe-py'
-DESCRIPTION = 'Python Web framework for learning purposes '
+NAME = 'webframe_py'
+DESCRIPTION = 'Python Web framework for all to build projects easily'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'ali.backenddev@gmail.com'
 AUTHOR = 'Abdumalikov Asadbek'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

### Comparing `webframe-py-0.1.0/webframe_py.egg-info/PKG-INFO` & `webframe_py-0.1.1/webframe_py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
 Name: webframe-py
-Version: 0.1.0
-Summary: Python Web framework for learning purposes 
+Version: 0.1.1
+Summary: Python Web framework for all to build projects easily
 Home-page: https://github.com/me/myproject
 Author: Abdumalikov Asadbek
 Author-email: ali.backenddev@gmail.com
 License: MIT
-Description: Python Web framework for learning purposes 
+Description: 
+        # Python Web Framework built for all users to create projects easier
+        
+        ![Purpose](https://img.shields.io/badge/:purpose-learning-teal)
+        ![PyPI - Version](https://img.shields.io/pypi/v/webframe-py)
+        
+        
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

