# Comparing `tmp/EAACommander-0.3.tar.gz` & `tmp/EAACommander-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EAACommander-0.3.tar", last modified: Tue May 21 23:17:27 2024, max compression
+gzip compressed data, was "EAACommander-0.4.tar", last modified: Tue May 21 23:42:51 2024, max compression
```

## Comparing `EAACommander-0.3.tar` & `EAACommander-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:17:27.995757 EAACommander-0.3/
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:17:27.994779 EAACommander-0.3/EAACommander/
--rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.3/EAACommander/__init__.py
--rw-r--r--   0 marko      (501) staff       (20)     2399 2024-05-21 23:07:34.000000 EAACommander-0.3/EAACommander/cli_client.py
--rw-r--r--   0 marko      (501) staff       (20)     5800 2024-05-21 19:12:54.000000 EAACommander-0.3/EAACommander/settings.py
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:17:27.995412 EAACommander-0.3/EAACommander.egg-info/
--rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 23:17:27.000000 EAACommander-0.3/EAACommander.egg-info/PKG-INFO
--rw-r--r--   0 marko      (501) staff       (20)      339 2024-05-21 23:17:27.000000 EAACommander-0.3/EAACommander.egg-info/SOURCES.txt
--rw-r--r--   0 marko      (501) staff       (20)        1 2024-05-21 23:17:27.000000 EAACommander-0.3/EAACommander.egg-info/dependency_links.txt
--rw-r--r--   0 marko      (501) staff       (20)       74 2024-05-21 23:17:27.000000 EAACommander-0.3/EAACommander.egg-info/entry_points.txt
--rw-r--r--   0 marko      (501) staff       (20)        4 2024-05-21 23:17:27.000000 EAACommander-0.3/EAACommander.egg-info/requires.txt
--rw-r--r--   0 marko      (501) staff       (20)       19 2024-05-21 23:17:27.000000 EAACommander-0.3/EAACommander.egg-info/top_level.txt
--rw-r--r--   0 marko      (501) staff       (20)       12 2024-05-21 19:12:54.000000 EAACommander-0.3/LICENSE
--rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 23:17:27.995648 EAACommander-0.3/PKG-INFO
--rw-r--r--   0 marko      (501) staff       (20)       67 2024-05-21 19:12:54.000000 EAACommander-0.3/README.md
--rw-r--r--   0 marko      (501) staff       (20)       38 2024-05-21 23:17:27.995794 EAACommander-0.3/setup.cfg
--rw-r--r--   0 marko      (501) staff       (20)      812 2024-05-21 23:13:40.000000 EAACommander-0.3/setup.py
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:17:27.995524 EAACommander-0.3/tests/
--rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.3/tests/__init__.py
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:42:51.599358 EAACommander-0.4/
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:42:51.598397 EAACommander-0.4/EAACommander/
+-rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 23:34:59.000000 EAACommander-0.4/EAACommander/__init__.py
+-rw-r--r--   0 marko      (501) staff       (20)     2399 2024-05-21 23:34:59.000000 EAACommander-0.4/EAACommander/cli_client.py
+-rw-r--r--   0 marko      (501) staff       (20)     5870 2024-05-21 23:35:44.000000 EAACommander-0.4/EAACommander/settings.py
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:42:51.599019 EAACommander-0.4/EAACommander.egg-info/
+-rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 23:42:51.000000 EAACommander-0.4/EAACommander.egg-info/PKG-INFO
+-rw-r--r--   0 marko      (501) staff       (20)      339 2024-05-21 23:42:51.000000 EAACommander-0.4/EAACommander.egg-info/SOURCES.txt
+-rw-r--r--   0 marko      (501) staff       (20)        1 2024-05-21 23:42:51.000000 EAACommander-0.4/EAACommander.egg-info/dependency_links.txt
+-rw-r--r--   0 marko      (501) staff       (20)       74 2024-05-21 23:42:51.000000 EAACommander-0.4/EAACommander.egg-info/entry_points.txt
+-rw-r--r--   0 marko      (501) staff       (20)        4 2024-05-21 23:42:51.000000 EAACommander-0.4/EAACommander.egg-info/requires.txt
+-rw-r--r--   0 marko      (501) staff       (20)       19 2024-05-21 23:42:51.000000 EAACommander-0.4/EAACommander.egg-info/top_level.txt
+-rw-r--r--   0 marko      (501) staff       (20)       12 2024-05-21 19:12:54.000000 EAACommander-0.4/LICENSE
+-rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 23:42:51.599242 EAACommander-0.4/PKG-INFO
+-rw-r--r--   0 marko      (501) staff       (20)       67 2024-05-21 19:12:54.000000 EAACommander-0.4/README.md
+-rw-r--r--   0 marko      (501) staff       (20)       38 2024-05-21 23:42:51.599393 EAACommander-0.4/setup.cfg
+-rw-r--r--   0 marko      (501) staff       (20)      880 2024-05-21 23:42:30.000000 EAACommander-0.4/setup.py
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 23:42:51.599125 EAACommander-0.4/tests/
+-rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.4/tests/__init__.py
```

### Comparing `EAACommander-0.3/EAACommander/cli_client.py` & `EAACommander-0.4/EAACommander/cli_client.py`

 * *Files identical despite different names*

### Comparing `EAACommander-0.3/EAACommander/settings.py` & `EAACommander-0.4/EAACommander/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import configparser
+import pkg_resources
 import curses
 
-CONFIG_FILE = "settings.ini"
+CONFIG_FILE = pkg_resources.resource_filename('EAACommander', 'settings.ini')
 
 # Function to load settings from the configuration file
 def load_settings():
     config = configparser.ConfigParser()
     config.read(CONFIG_FILE)
     return config
```

### Comparing `EAACommander-0.3/EAACommander.egg-info/PKG-INFO` & `EAACommander-0.4/EAACommander.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAACommander
-Version: 0.3
+Version: 0.4
 Summary: A tool for Electronically Assisted Astronomy (EAA) enthusiasts
 Home-page: https://github.com/MarkoZnidar/EAACommander/
 Author: Marko Žnidar
 Author-email: marko.znidar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EAACommander-0.3/PKG-INFO` & `EAACommander-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAACommander
-Version: 0.3
+Version: 0.4
 Summary: A tool for Electronically Assisted Astronomy (EAA) enthusiasts
 Home-page: https://github.com/MarkoZnidar/EAACommander/
 Author: Marko Žnidar
 Author-email: marko.znidar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EAACommander-0.3/setup.py` & `EAACommander-0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EAACommander',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'art',
     ],
     entry_points={
         'console_scripts': [
             'eaacommander=EAACommander.cli_client:main_entry_point',
         ],
     },
+    package_data={
+        'EAACommander': ['settings.ini'],
+    },
     author='Marko Žnidar',
     author_email='marko.znidar@gmail.com',
     description='A tool for Electronically Assisted Astronomy (EAA) enthusiasts',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MarkoZnidar/EAACommander/',
     classifiers=[
```

