# Comparing `tmp/printmate-1.3.0.9.tar.gz` & `tmp/printmate-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printmate-1.3.0.9.tar", last modified: Wed May 22 20:49:44 2024, max compression
+gzip compressed data, was "printmate-1.3.1.tar", last modified: Wed May 22 20:50:33 2024, max compression
```

## Comparing `printmate-1.3.0.9.tar` & `printmate-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:49:44.894216 printmate-1.3.0.9/
--rw-rw-rw-   0        0        0      310 2024-05-22 20:49:44.891224 printmate-1.3.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.3.0.9/license
-drwxrwxrwx   0        0        0        0 2024-05-22 20:49:44.888911 printmate-1.3.0.9/printmate.egg-info/
--rw-rw-rw-   0        0        0      310 2024-05-22 20:49:44.000000 printmate-1.3.0.9/printmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-22 20:49:44.000000 printmate-1.3.0.9/printmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:49:44.000000 printmate-1.3.0.9/printmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-22 20:49:44.000000 printmate-1.3.0.9/printmate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 20:49:44.000000 printmate-1.3.0.9/printmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:49:44.000000 printmate-1.3.0.9/printmate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:49:44.894216 printmate-1.3.0.9/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-22 20:49:28.000000 printmate-1.3.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:50:33.475888 printmate-1.3.1/
+-rw-rw-rw-   0        0        0      308 2024-05-22 20:50:33.471368 printmate-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.3.1/license
+drwxrwxrwx   0        0        0        0 2024-05-22 20:50:33.471368 printmate-1.3.1/printmate.egg-info/
+-rw-rw-rw-   0        0        0      308 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:50:33.475888 printmate-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 20:50:21.000000 printmate-1.3.1/setup.py
```

### Comparing `printmate-1.3.0.9/license` & `printmate-1.3.1/license`

 * *Files identical despite different names*

### Comparing `printmate-1.3.0.9/setup.py` & `printmate-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='printmate',
-    version='1.3.0.9',
+    version='1.3.1',
     packages=find_packages(),
     install_requires=[
         "colorama"],
     entry_points={
         'console_scripts': [
             'printmate = printmate.__main__:main',
         ],
```

