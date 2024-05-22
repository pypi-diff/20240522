# Comparing `tmp/outputdecorator-0.0.1.tar.gz` & `tmp/outputdecorator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outputdecorator-0.0.1.tar", last modified: Tue May 21 10:33:59 2024, max compression
+gzip compressed data, was "outputdecorator-0.0.2.tar", last modified: Wed May 22 13:36:11 2024, max compression
```

## Comparing `outputdecorator-0.0.1.tar` & `outputdecorator-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-21 10:33:59.415312 outputdecorator-0.0.1/
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1499 2024-05-21 10:20:57.000000 outputdecorator-0.0.1/LICENSE
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)       94 2024-05-21 09:48:50.000000 outputdecorator-0.0.1/MANIFEST.in
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     2329 2024-05-21 10:33:59.415312 outputdecorator-0.0.1/PKG-INFO
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1216 2024-05-21 10:30:18.000000 outputdecorator-0.0.1/README.md
-drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-21 10:33:59.415312 outputdecorator-0.0.1/output_decorator/
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      337 2024-05-21 10:33:57.000000 outputdecorator-0.0.1/output_decorator/__init__.py
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      743 2024-05-21 10:16:18.000000 outputdecorator-0.0.1/output_decorator/decorators.py
-drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-21 10:33:59.415312 outputdecorator-0.0.1/outputdecorator.egg-info/
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     2329 2024-05-21 10:33:59.000000 outputdecorator-0.0.1/outputdecorator.egg-info/PKG-INFO
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      319 2024-05-21 10:33:59.000000 outputdecorator-0.0.1/outputdecorator.egg-info/SOURCES.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-21 10:33:59.000000 outputdecorator-0.0.1/outputdecorator.egg-info/dependency_links.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-21 10:33:59.000000 outputdecorator-0.0.1/outputdecorator.egg-info/not-zip-safe
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)       17 2024-05-21 10:33:59.000000 outputdecorator-0.0.1/outputdecorator.egg-info/top_level.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)        0 2024-05-21 09:48:49.000000 outputdecorator-0.0.1/requirements.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1168 2024-05-21 10:33:59.415312 outputdecorator-0.0.1/setup.cfg
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      343 2024-05-21 09:50:01.000000 outputdecorator-0.0.1/setup.py
+drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-22 13:36:11.045935 outputdecorator-0.0.2/
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1499 2024-05-21 10:20:57.000000 outputdecorator-0.0.2/LICENSE
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)       94 2024-05-21 09:48:50.000000 outputdecorator-0.0.2/MANIFEST.in
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     3311 2024-05-22 13:36:11.045935 outputdecorator-0.0.2/PKG-INFO
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     2136 2024-05-22 13:35:36.000000 outputdecorator-0.0.2/README.md
+drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-22 13:36:11.045935 outputdecorator-0.0.2/output_decorator/
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      406 2024-05-22 13:35:36.000000 outputdecorator-0.0.2/output_decorator/__init__.py
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      812 2024-05-21 10:39:48.000000 outputdecorator-0.0.2/output_decorator/decorators.py
+drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-22 13:36:11.045935 outputdecorator-0.0.2/outputdecorator.egg-info/
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     3311 2024-05-22 13:36:11.000000 outputdecorator-0.0.2/outputdecorator.egg-info/PKG-INFO
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      319 2024-05-22 13:36:11.000000 outputdecorator-0.0.2/outputdecorator.egg-info/SOURCES.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-22 13:36:11.000000 outputdecorator-0.0.2/outputdecorator.egg-info/dependency_links.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-22 13:36:11.000000 outputdecorator-0.0.2/outputdecorator.egg-info/not-zip-safe
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)       17 2024-05-22 13:36:11.000000 outputdecorator-0.0.2/outputdecorator.egg-info/top_level.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)        0 2024-05-21 09:48:49.000000 outputdecorator-0.0.2/requirements.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1230 2024-05-22 13:36:11.045935 outputdecorator-0.0.2/setup.cfg
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      343 2024-05-21 09:50:01.000000 outputdecorator-0.0.2/setup.py
```

### Comparing `outputdecorator-0.0.1/LICENSE` & `outputdecorator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `outputdecorator-0.0.1/output_decorator/decorators.py` & `outputdecorator-0.0.2/output_decorator/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # --------------------------------------------------------
 # Licensed under the terms of the BSD 3-Clause License
 # (see LICENSE for details).
 # Copyright © 2024, A.A. Suvorov
 # All rights reserved.
 # --------------------------------------------------------
+"""Output Decorator - Library for decorating strings in CLI apps """
 import shutil
 
 
 class StringDecorator:
     @classmethod
     def term_width(cls):
         return shutil.get_terminal_size()[0]
```

### Comparing `outputdecorator-0.0.1/setup.cfg` & `outputdecorator-0.0.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = outputdecorator
 version = attr: output_decorator.__version__
 author = A.A. Suvorov
 author_email = saneksking@gmail.com
-description = ''
+description = 'Output Decorator - Library for decorating strings in CLI apps/'
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/saneksking
 project_urls = 
 	Documentation = https://github.com/saneksking/outputdecorator/blob/master/README.md
 	Release notes = https://github.com/saneksking/outputdecorator/releases
 license = BSD 3-Clause License
```

