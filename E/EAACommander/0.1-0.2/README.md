# Comparing `tmp/EAACommander-0.1.tar.gz` & `tmp/EAACommander-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EAACommander-0.1.tar", last modified: Tue May 21 22:27:30 2024, max compression
+gzip compressed data, was "EAACommander-0.2.tar", last modified: Tue May 21 22:50:25 2024, max compression
```

## Comparing `EAACommander-0.1.tar` & `EAACommander-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:27:30.544192 EAACommander-0.1/
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:27:30.542916 EAACommander-0.1/EAACommander/
--rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.1/EAACommander/__init__.py
--rw-r--r--   0 marko      (501) staff       (20)     2253 2024-05-21 19:12:54.000000 EAACommander-0.1/EAACommander/cli_client.py
--rw-r--r--   0 marko      (501) staff       (20)     5800 2024-05-21 19:12:54.000000 EAACommander-0.1/EAACommander/settings.py
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:27:30.543632 EAACommander-0.1/EAACommander.egg-info/
--rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 22:27:30.000000 EAACommander-0.1/EAACommander.egg-info/PKG-INFO
--rw-r--r--   0 marko      (501) staff       (20)      339 2024-05-21 22:27:30.000000 EAACommander-0.1/EAACommander.egg-info/SOURCES.txt
--rw-r--r--   0 marko      (501) staff       (20)        1 2024-05-21 22:27:30.000000 EAACommander-0.1/EAACommander.egg-info/dependency_links.txt
--rw-r--r--   0 marko      (501) staff       (20)       62 2024-05-21 22:27:30.000000 EAACommander-0.1/EAACommander.egg-info/entry_points.txt
--rw-r--r--   0 marko      (501) staff       (20)        4 2024-05-21 22:27:30.000000 EAACommander-0.1/EAACommander.egg-info/requires.txt
--rw-r--r--   0 marko      (501) staff       (20)       19 2024-05-21 22:27:30.000000 EAACommander-0.1/EAACommander.egg-info/top_level.txt
--rw-r--r--   0 marko      (501) staff       (20)       12 2024-05-21 19:12:54.000000 EAACommander-0.1/LICENSE
--rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 22:27:30.544012 EAACommander-0.1/PKG-INFO
--rw-r--r--   0 marko      (501) staff       (20)       67 2024-05-21 19:12:54.000000 EAACommander-0.1/README.md
--rw-r--r--   0 marko      (501) staff       (20)       38 2024-05-21 22:27:30.544244 EAACommander-0.1/setup.cfg
--rw-r--r--   0 marko      (501) staff       (20)      800 2024-05-21 22:25:50.000000 EAACommander-0.1/setup.py
-drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:27:30.543742 EAACommander-0.1/tests/
--rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.1/tests/__init__.py
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:50:25.434202 EAACommander-0.2/
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:50:25.433235 EAACommander-0.2/EAACommander/
+-rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.2/EAACommander/__init__.py
+-rw-r--r--   0 marko      (501) staff       (20)     2351 2024-05-21 22:48:47.000000 EAACommander-0.2/EAACommander/cli_client.py
+-rw-r--r--   0 marko      (501) staff       (20)     5800 2024-05-21 19:12:54.000000 EAACommander-0.2/EAACommander/settings.py
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:50:25.433848 EAACommander-0.2/EAACommander.egg-info/
+-rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 22:50:25.000000 EAACommander-0.2/EAACommander.egg-info/PKG-INFO
+-rw-r--r--   0 marko      (501) staff       (20)      339 2024-05-21 22:50:25.000000 EAACommander-0.2/EAACommander.egg-info/SOURCES.txt
+-rw-r--r--   0 marko      (501) staff       (20)        1 2024-05-21 22:50:25.000000 EAACommander-0.2/EAACommander.egg-info/dependency_links.txt
+-rw-r--r--   0 marko      (501) staff       (20)       62 2024-05-21 22:50:25.000000 EAACommander-0.2/EAACommander.egg-info/entry_points.txt
+-rw-r--r--   0 marko      (501) staff       (20)        4 2024-05-21 22:50:25.000000 EAACommander-0.2/EAACommander.egg-info/requires.txt
+-rw-r--r--   0 marko      (501) staff       (20)       19 2024-05-21 22:50:25.000000 EAACommander-0.2/EAACommander.egg-info/top_level.txt
+-rw-r--r--   0 marko      (501) staff       (20)       12 2024-05-21 19:12:54.000000 EAACommander-0.2/LICENSE
+-rw-r--r--   0 marko      (501) staff       (20)      540 2024-05-21 22:50:25.434086 EAACommander-0.2/PKG-INFO
+-rw-r--r--   0 marko      (501) staff       (20)       67 2024-05-21 19:12:54.000000 EAACommander-0.2/README.md
+-rw-r--r--   0 marko      (501) staff       (20)       38 2024-05-21 22:50:25.434238 EAACommander-0.2/setup.cfg
+-rw-r--r--   0 marko      (501) staff       (20)      800 2024-05-21 22:48:10.000000 EAACommander-0.2/setup.py
+drwxr-xr-x   0 marko      (501) staff       (20)        0 2024-05-21 22:50:25.433958 EAACommander-0.2/tests/
+-rw-r--r--   0 marko      (501) staff       (20)        0 2024-05-21 19:12:54.000000 EAACommander-0.2/tests/__init__.py
```

### Comparing `EAACommander-0.1/EAACommander/cli_client.py` & `EAACommander-0.2/EAACommander/cli_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import curses
 from art import text2art
-from settings import load_settings, display_message, settings
+
+try:
+    from .settings import load_settings, display_message, settings
+except ImportError:
+    from settings import load_settings, display_message, settings
+
 
 TITLE = "EAA Commander"
 
 def check_health(stdscr):
     config = load_settings()
     hostname = config['Server'].get('Hostname', 'astro')
     port = config['Server'].get('Port', '50000')
```

### Comparing `EAACommander-0.1/EAACommander/settings.py` & `EAACommander-0.2/EAACommander/settings.py`

 * *Files identical despite different names*

### Comparing `EAACommander-0.1/EAACommander.egg-info/PKG-INFO` & `EAACommander-0.2/EAACommander.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAACommander
-Version: 0.1
+Version: 0.2
 Summary: A tool for Electronically Assisted Astronomy (EAA) enthusiasts
 Home-page: https://github.com/MarkoZnidar/EAACommander/
 Author: Marko Žnidar
 Author-email: marko.znidar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EAACommander-0.1/PKG-INFO` & `EAACommander-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAACommander
-Version: 0.1
+Version: 0.2
 Summary: A tool for Electronically Assisted Astronomy (EAA) enthusiasts
 Home-page: https://github.com/MarkoZnidar/EAACommander/
 Author: Marko Žnidar
 Author-email: marko.znidar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EAACommander-0.1/setup.py` & `EAACommander-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EAACommander',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'art',
     ],
     entry_points={
         'console_scripts': [
             'eaacommander=EAACommander.cli_client:main',
```

