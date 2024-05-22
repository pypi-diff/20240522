# Comparing `tmp/apeboiy-0.0.2.tar.gz` & `tmp/apeboiy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeboiy-0.0.2.tar", last modified: Wed May 22 12:21:58 2024, max compression
+gzip compressed data, was "apeboiy-0.0.3.tar", last modified: Wed May 22 13:52:31 2024, max compression
```

## Comparing `apeboiy-0.0.2.tar` & `apeboiy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.658276 apeboiy-0.0.2/
--rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.2/LICENSE
--rw-r--r--   0 iccy       (501) staff       (20)      714 2024-05-22 12:21:58.658078 apeboiy-0.0.2/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.2/README.md
--rw-r--r--   0 iccy       (501) staff       (20)      573 2024-05-22 12:21:55.000000 apeboiy-0.0.2/pyproject.toml
--rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 12:21:58.658311 apeboiy-0.0.2/setup.cfg
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.656051 apeboiy-0.0.2/src/
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.657046 apeboiy-0.0.2/src/apeboiy/
--rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.2/src/apeboiy/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.2/src/apeboiy/example.py
--rw-r--r--   0 iccy       (501) staff       (20)     3258 2024-05-22 12:19:49.000000 apeboiy-0.0.2/src/apeboiy/plyreader.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.657900 apeboiy-0.0.2/src/apeboiy.egg-info/
--rw-r--r--   0 iccy       (501) staff       (20)      714 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      278 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/SOURCES.txt
--rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/dependency_links.txt
--rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/requires.txt
--rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/top_level.txt
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:52:31.465417 apeboiy-0.0.3/
+-rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.3/LICENSE
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 13:52:31.465215 apeboiy-0.0.3/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.3/README.md
+-rw-r--r--   0 iccy       (501) staff       (20)      621 2024-05-22 13:52:29.000000 apeboiy-0.0.3/pyproject.toml
+-rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 13:52:31.465457 apeboiy-0.0.3/setup.cfg
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:52:31.462411 apeboiy-0.0.3/src/
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:52:31.463418 apeboiy-0.0.3/src/apeboiy/
+-rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.3/src/apeboiy/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.3/src/apeboiy/example.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:52:31.464633 apeboiy-0.0.3/src/apeboiy/plyreader/
+-rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 13:45:12.000000 apeboiy-0.0.3/src/apeboiy/plyreader/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)     3507 2024-05-22 13:45:12.000000 apeboiy-0.0.3/src/apeboiy/plyreader/__reader.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:52:31.464998 apeboiy-0.0.3/src/apeboiy.egg-info/
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 13:52:31.000000 apeboiy-0.0.3/src/apeboiy.egg-info/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      321 2024-05-22 13:52:31.000000 apeboiy-0.0.3/src/apeboiy.egg-info/SOURCES.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 13:52:31.000000 apeboiy-0.0.3/src/apeboiy.egg-info/dependency_links.txt
+-rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 13:52:31.000000 apeboiy-0.0.3/src/apeboiy.egg-info/requires.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 13:52:31.000000 apeboiy-0.0.3/src/apeboiy.egg-info/top_level.txt
```

### Comparing `apeboiy-0.0.2/LICENSE` & `apeboiy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.2/PKG-INFO` & `apeboiy-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
+Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.21.0
 
 # Example Package
```

### Comparing `apeboiy-0.0.2/pyproject.toml` & `apeboiy-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "apeboiy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="AppleBoiy", email="contact.chaipat@gmail.com" },
+    { "name"="AppleBoiy", "email"="contact.chaipat@gmail.com"}
 ]
 description = "Shared AppleBoiy's packages."
 readme = "README.md"
-requires-python = ">=3.8.10"
+keywords = ["appleboiy", "shared", "packages"]
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests>=2.25.1",
```

### Comparing `apeboiy-0.0.2/src/apeboiy/plyreader.py` & `apeboiy-0.0.3/src/apeboiy/plyreader/__reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import os
 import struct
 
 import numpy as np
 
 
 class PLYReader:
+    """
+    Class to read PLY files. The class can read in ASCII 1.0 and little-endian binary 1.0 files.
+
+    usage:
+    reader = PLYReader("file.ply")
+    reader.read() # read the file
+
+    # get the vertices
+    vertices = reader.vertices
+    """
     def __init__(self, filename):
         self.__name = filename
         self.__header = "ply\n"
         self.__vertex_count = 0
         self.__format = None
         self.__vertices = {
             "Position": np.zeros((0, 3), dtype=np.float64),  # (x, y, z
```

### Comparing `apeboiy-0.0.2/src/apeboiy.egg-info/PKG-INFO` & `apeboiy-0.0.3/src/apeboiy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
+Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.21.0
 
 # Example Package
```

