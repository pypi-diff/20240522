# Comparing `tmp/apeboiy-0.0.6.tar.gz` & `tmp/apeboiy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeboiy-0.0.6.tar", last modified: Wed May 22 14:01:53 2024, max compression
+gzip compressed data, was "apeboiy-0.0.7.tar", last modified: Wed May 22 14:06:23 2024, max compression
```

## Comparing `apeboiy-0.0.6.tar` & `apeboiy-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:01:53.150241 apeboiy-0.0.6/
--rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.6/LICENSE
--rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:01:53.150047 apeboiy-0.0.6/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.6/README.md
--rw-r--r--   0 iccy       (501) staff       (20)      621 2024-05-22 14:01:35.000000 apeboiy-0.0.6/pyproject.toml
--rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 14:01:53.150278 apeboiy-0.0.6/setup.cfg
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:01:53.147959 apeboiy-0.0.6/src/
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:01:53.148745 apeboiy-0.0.6/src/apeboiy/
--rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.6/src/apeboiy/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.6/src/apeboiy/example.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:01:53.149592 apeboiy-0.0.6/src/apeboiy/plyreader/
--rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 14:01:35.000000 apeboiy-0.0.6/src/apeboiy/plyreader/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)     3507 2024-05-22 13:45:12.000000 apeboiy-0.0.6/src/apeboiy/plyreader/reader.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:01:53.149848 apeboiy-0.0.6/src/apeboiy.egg-info/
--rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:01:53.000000 apeboiy-0.0.6/src/apeboiy.egg-info/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      319 2024-05-22 14:01:53.000000 apeboiy-0.0.6/src/apeboiy.egg-info/SOURCES.txt
--rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 14:01:53.000000 apeboiy-0.0.6/src/apeboiy.egg-info/dependency_links.txt
--rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 14:01:53.000000 apeboiy-0.0.6/src/apeboiy.egg-info/requires.txt
--rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 14:01:53.000000 apeboiy-0.0.6/src/apeboiy.egg-info/top_level.txt
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:06:23.289451 apeboiy-0.0.7/
+-rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.7/LICENSE
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:06:23.289246 apeboiy-0.0.7/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.7/README.md
+-rw-r--r--   0 iccy       (501) staff       (20)      621 2024-05-22 14:05:02.000000 apeboiy-0.0.7/pyproject.toml
+-rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 14:06:23.289490 apeboiy-0.0.7/setup.cfg
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:06:23.286329 apeboiy-0.0.7/src/
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:06:23.287396 apeboiy-0.0.7/src/apeboiy/
+-rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.7/src/apeboiy/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.7/src/apeboiy/example.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:06:23.288623 apeboiy-0.0.7/src/apeboiy/ply/
+-rw-r--r--   0 iccy       (501) staff       (20)       22 2024-05-22 14:05:02.000000 apeboiy-0.0.7/src/apeboiy/ply/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)     3504 2024-05-22 14:04:38.000000 apeboiy-0.0.7/src/apeboiy/ply/_reader.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:06:23.288998 apeboiy-0.0.7/src/apeboiy.egg-info/
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:06:23.000000 apeboiy-0.0.7/src/apeboiy.egg-info/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      308 2024-05-22 14:06:23.000000 apeboiy-0.0.7/src/apeboiy.egg-info/SOURCES.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 14:06:23.000000 apeboiy-0.0.7/src/apeboiy.egg-info/dependency_links.txt
+-rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 14:06:23.000000 apeboiy-0.0.7/src/apeboiy.egg-info/requires.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 14:06:23.000000 apeboiy-0.0.7/src/apeboiy.egg-info/top_level.txt
```

### Comparing `apeboiy-0.0.6/LICENSE` & `apeboiy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.6/PKG-INFO` & `apeboiy-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apeboiy-0.0.6/pyproject.toml` & `apeboiy-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apeboiy"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { "name"="AppleBoiy", "email"="contact.chaipat@gmail.com"}
 ]
 description = "Shared AppleBoiy's packages."
 readme = "README.md"
 keywords = ["appleboiy", "shared", "packages"]
 requires-python = ">=3.8"
```

### Comparing `apeboiy-0.0.6/src/apeboiy/plyreader/reader.py` & `apeboiy-0.0.7/src/apeboiy/ply/_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import struct
 
 import numpy as np
 
 
-class PLYReader:
+class Reader:
     """
     Class to read PLY files. The class can read in ASCII 1.0 and little-endian binary 1.0 files.
 
     usage:
     reader = PLYReader("file.ply")
     reader.read() # read the file
```

### Comparing `apeboiy-0.0.6/src/apeboiy.egg-info/PKG-INFO` & `apeboiy-0.0.7/src/apeboiy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

