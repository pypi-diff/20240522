# Comparing `tmp/intensity_logger-0.1.1.tar.gz` & `tmp/intensity_logger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intensity_logger-0.1.1.tar", last modified: Wed May 22 07:31:55 2024, max compression
+gzip compressed data, was "intensity_logger-0.1.2.tar", last modified: Wed May 22 07:36:56 2024, max compression
```

## Comparing `intensity_logger-0.1.1.tar` & `intensity_logger-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 07:31:55.767248 intensity_logger-0.1.1/
--rw-rw-rw-   0        0        0     1085 2024-05-22 07:11:41.000000 intensity_logger-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3761 2024-05-22 07:31:55.766162 intensity_logger-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2024-05-22 07:31:22.000000 intensity_logger-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 07:31:55.741059 intensity_logger-0.1.1/intensity_logger/
--rw-rw-rw-   0        0        0       26 2024-05-22 07:17:22.000000 intensity_logger-0.1.1/intensity_logger/__init__.py
--rw-rw-rw-   0        0        0     1523 2024-05-22 07:26:12.000000 intensity_logger-0.1.1/intensity_logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:31:55.764791 intensity_logger-0.1.1/intensity_logger.egg-info/
--rw-rw-rw-   0        0        0     3761 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 07:29:53.000000 intensity_logger-0.1.1/intensity_logger.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 07:31:55.767248 intensity_logger-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1234 2024-05-22 07:30:34.000000 intensity_logger-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:56.886387 intensity_logger-0.1.2/
+-rw-rw-rw-   0        0        0     1085 2024-05-22 07:11:41.000000 intensity_logger-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3761 2024-05-22 07:36:56.885381 intensity_logger-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2024-05-22 07:36:33.000000 intensity_logger-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:56.863155 intensity_logger-0.1.2/intensity_logger/
+-rw-rw-rw-   0        0        0       26 2024-05-22 07:17:22.000000 intensity_logger-0.1.2/intensity_logger/__init__.py
+-rw-rw-rw-   0        0        0     2177 2024-05-22 07:35:50.000000 intensity_logger-0.1.2/intensity_logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:56.884920 intensity_logger-0.1.2/intensity_logger.egg-info/
+-rw-rw-rw-   0        0        0     3761 2024-05-22 07:36:56.000000 intensity_logger-0.1.2/intensity_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-22 07:36:56.000000 intensity_logger-0.1.2/intensity_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:36:56.000000 intensity_logger-0.1.2/intensity_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 07:29:53.000000 intensity_logger-0.1.2/intensity_logger.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-05-22 07:36:56.000000 intensity_logger-0.1.2/intensity_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:36:56.886387 intensity_logger-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2024-05-22 07:35:56.000000 intensity_logger-0.1.2/setup.py
```

### Comparing `intensity_logger-0.1.1/LICENSE` & `intensity_logger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intensity_logger-0.1.1/PKG-INFO` & `intensity_logger-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intensity-logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A logging utility for Python applications with customizable intensity
 Home-page: https://github.com/idkconsole/intensity-logger
 Author: idkconsole, eagledev1337, homicide3301
 Author-email: idkconsole@proton.me
 Keywords: logging logger intensity color logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,15 +45,15 @@
 - Optional custom intensity to convert messages to uppercase.
 - Lightweight and easy to integrate into any Python project.
 
 ## Installation
 You can install Intensity Logger via pip:
 
 ```bash
-pip install intensity-logger==0.1.1
+pip install intensity-logger==0.1.2
 ```
 
 ## Usage
 ## Basic Usage
 
 Here's a basic example to get you started with Intensity Logger:
```

### Comparing `intensity_logger-0.1.1/README.md` & `intensity_logger-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 - Optional custom intensity to convert messages to uppercase.
 - Lightweight and easy to integrate into any Python project.
 
 ## Installation
 You can install Intensity Logger via pip:
 
 ```bash
-pip install intensity-logger==0.1.1
+pip install intensity-logger==0.1.2
 ```
 
 ## Usage
 ## Basic Usage
 
 Here's a basic example to get you started with Intensity Logger:
```

### Comparing `intensity_logger-0.1.1/intensity_logger.egg-info/PKG-INFO` & `intensity_logger-0.1.2/intensity_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intensity-logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A logging utility for Python applications with customizable intensity
 Home-page: https://github.com/idkconsole/intensity-logger
 Author: idkconsole, eagledev1337, homicide3301
 Author-email: idkconsole@proton.me
 Keywords: logging logger intensity color logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,15 +45,15 @@
 - Optional custom intensity to convert messages to uppercase.
 - Lightweight and easy to integrate into any Python project.
 
 ## Installation
 You can install Intensity Logger via pip:
 
 ```bash
-pip install intensity-logger==0.1.1
+pip install intensity-logger==0.1.2
 ```
 
 ## Usage
 ## Basic Usage
 
 Here's a basic example to get you started with Intensity Logger:
```

### Comparing `intensity_logger-0.1.1/setup.py` & `intensity_logger-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='intensity-logger',
-    version='0.1.1',
+    version='0.1.2',
     author='idkconsole, eagledev1337, homicide3301',
     author_email='idkconsole@proton.me',
     description='A logging utility for Python applications with customizable intensity',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/idkconsole/intensity-logger',
     packages=find_packages(),
```

