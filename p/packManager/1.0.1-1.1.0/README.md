# Comparing `tmp/packmanager-1.0.1.tar.gz` & `tmp/packmanager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packmanager-1.0.1.tar", last modified: Wed May 22 11:29:54 2024, max compression
+gzip compressed data, was "packmanager-1.1.0.tar", last modified: Wed May 22 11:57:28 2024, max compression
```

## Comparing `packmanager-1.0.1.tar` & `packmanager-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 11:29:54.942419 packmanager-1.0.1/
--rw-rw-rw-   0        0        0       85 2024-05-22 11:29:16.000000 packmanager-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      913 2024-05-22 11:29:54.939419 packmanager-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-05-22 10:00:43.000000 packmanager-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 11:29:54.936417 packmanager-1.0.1/packManager.egg-info/
--rw-rw-rw-   0        0        0      913 2024-05-22 11:29:54.000000 packmanager-1.0.1/packManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-22 11:29:54.000000 packmanager-1.0.1/packManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:29:54.000000 packmanager-1.0.1/packManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:29:54.000000 packmanager-1.0.1/packManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-05-22 10:02:38.000000 packmanager-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 11:29:54.942419 packmanager-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      855 2024-05-22 11:28:01.000000 packmanager-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:57:28.651924 packmanager-1.1.0/
+-rw-rw-rw-   0        0        0       85 2024-05-22 11:29:16.000000 packmanager-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      913 2024-05-22 11:57:28.651924 packmanager-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-22 10:00:43.000000 packmanager-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:57:28.643924 packmanager-1.1.0/packManager.egg-info/
+-rw-rw-rw-   0        0        0      913 2024-05-22 11:57:28.000000 packmanager-1.1.0/packManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-22 11:57:28.000000 packmanager-1.1.0/packManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:57:28.000000 packmanager-1.1.0/packManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:57:28.000000 packmanager-1.1.0/packManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-22 10:02:38.000000 packmanager-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:57:28.651924 packmanager-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      855 2024-05-22 11:56:03.000000 packmanager-1.1.0/setup.py
```

### Comparing `packmanager-1.0.1/PKG-INFO` & `packmanager-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packManager
-Version: 1.0.1
+Version: 1.1.0
 Summary: A package manager for python
 Home-page: https://chicken-muggets.github.io/packManager/
 Author: Chicken Muggets
 License: MIT
 Project-URL: Documentation, https://github.com/chicken-muggets/PackInst/wiki
 Project-URL: Source, https://github.com/chicken-muggets/PackInst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `packmanager-1.0.1/packManager.egg-info/PKG-INFO` & `packmanager-1.1.0/packManager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packManager
-Version: 1.0.1
+Version: 1.1.0
 Summary: A package manager for python
 Home-page: https://chicken-muggets.github.io/packManager/
 Author: Chicken Muggets
 License: MIT
 Project-URL: Documentation, https://github.com/chicken-muggets/PackInst/wiki
 Project-URL: Source, https://github.com/chicken-muggets/PackInst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `packmanager-1.0.1/setup.py` & `packmanager-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="packManager",
-    version="1.0.1",
+    version="1.1.0",
     description="A package manager for python",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://chicken-muggets.github.io/packManager/",
     author="Chicken Muggets",
     license="MIT",
     project_urls={
```

