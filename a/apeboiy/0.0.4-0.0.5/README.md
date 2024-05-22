# Comparing `tmp/apeboiy-0.0.4.tar.gz` & `tmp/apeboiy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeboiy-0.0.4.tar", last modified: Wed May 22 13:57:58 2024, max compression
+gzip compressed data, was "apeboiy-0.0.5.tar", last modified: Wed May 22 13:59:53 2024, max compression
```

## Comparing `apeboiy-0.0.4.tar` & `apeboiy-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:57:58.653044 apeboiy-0.0.4/
--rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.4/LICENSE
--rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 13:57:58.652869 apeboiy-0.0.4/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.4/README.md
--rw-r--r--   0 iccy       (501) staff       (20)      621 2024-05-22 13:57:40.000000 apeboiy-0.0.4/pyproject.toml
--rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 13:57:58.653086 apeboiy-0.0.4/setup.cfg
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:57:58.650370 apeboiy-0.0.4/src/
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:57:58.651359 apeboiy-0.0.4/src/apeboiy/
--rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.4/src/apeboiy/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.4/src/apeboiy/example.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:57:58.652373 apeboiy-0.0.4/src/apeboiy/plyreader/
--rw-r--r--   0 iccy       (501) staff       (20)       30 2024-05-22 13:57:00.000000 apeboiy-0.0.4/src/apeboiy/plyreader/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)     3507 2024-05-22 13:45:12.000000 apeboiy-0.0.4/src/apeboiy/plyreader/_reader.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:57:58.652672 apeboiy-0.0.4/src/apeboiy.egg-info/
--rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 13:57:58.000000 apeboiy-0.0.4/src/apeboiy.egg-info/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      320 2024-05-22 13:57:58.000000 apeboiy-0.0.4/src/apeboiy.egg-info/SOURCES.txt
--rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 13:57:58.000000 apeboiy-0.0.4/src/apeboiy.egg-info/dependency_links.txt
--rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 13:57:58.000000 apeboiy-0.0.4/src/apeboiy.egg-info/requires.txt
--rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 13:57:58.000000 apeboiy-0.0.4/src/apeboiy.egg-info/top_level.txt
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:59:53.664051 apeboiy-0.0.5/
+-rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.5/LICENSE
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 13:59:53.663841 apeboiy-0.0.5/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.5/README.md
+-rw-r--r--   0 iccy       (501) staff       (20)      621 2024-05-22 13:59:44.000000 apeboiy-0.0.5/pyproject.toml
+-rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 13:59:53.664097 apeboiy-0.0.5/setup.cfg
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:59:53.661481 apeboiy-0.0.5/src/
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:59:53.662264 apeboiy-0.0.5/src/apeboiy/
+-rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.5/src/apeboiy/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.5/src/apeboiy/example.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:59:53.663252 apeboiy-0.0.5/src/apeboiy/plyreader/
+-rw-r--r--   0 iccy       (501) staff       (20)       29 2024-05-22 13:59:44.000000 apeboiy-0.0.5/src/apeboiy/plyreader/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)     3507 2024-05-22 13:45:12.000000 apeboiy-0.0.5/src/apeboiy/plyreader/reader.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 13:59:53.663573 apeboiy-0.0.5/src/apeboiy.egg-info/
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 13:59:53.000000 apeboiy-0.0.5/src/apeboiy.egg-info/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      319 2024-05-22 13:59:53.000000 apeboiy-0.0.5/src/apeboiy.egg-info/SOURCES.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 13:59:53.000000 apeboiy-0.0.5/src/apeboiy.egg-info/dependency_links.txt
+-rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 13:59:53.000000 apeboiy-0.0.5/src/apeboiy.egg-info/requires.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 13:59:53.000000 apeboiy-0.0.5/src/apeboiy.egg-info/top_level.txt
```

### Comparing `apeboiy-0.0.4/LICENSE` & `apeboiy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.4/PKG-INFO` & `apeboiy-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apeboiy-0.0.4/pyproject.toml` & `apeboiy-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apeboiy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { "name"="AppleBoiy", "email"="contact.chaipat@gmail.com"}
 ]
 description = "Shared AppleBoiy's packages."
 readme = "README.md"
 keywords = ["appleboiy", "shared", "packages"]
 requires-python = ">=3.8"
```

### Comparing `apeboiy-0.0.4/src/apeboiy/plyreader/_reader.py` & `apeboiy-0.0.5/src/apeboiy/plyreader/reader.py`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.4/src/apeboiy.egg-info/PKG-INFO` & `apeboiy-0.0.5/src/apeboiy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

