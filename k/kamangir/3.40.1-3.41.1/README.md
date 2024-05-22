# Comparing `tmp/kamangir-3.40.1.tar.gz` & `tmp/kamangir-3.41.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kamangir-3.40.1.tar", last modified: Tue May 21 02:53:18 2024, max compression
+gzip compressed data, was "kamangir-3.41.1.tar", last modified: Wed May 22 02:19:10 2024, max compression
```

## Comparing `kamangir-3.40.1.tar` & `kamangir-3.41.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:53:18.876500 kamangir-3.40.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.40.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.40.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-21 02:53:18.875905 kamangir-3.40.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3243 2024-05-21 02:52:53.000000 kamangir-3.40.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:53:18.873636 kamangir-3.40.1/kamangir/
--rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-21 02:53:15.000000 kamangir-3.40.1/kamangir/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4623 2024-05-21 02:51:34.000000 kamangir-3.40.1/kamangir/content.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:53:18.875432 kamangir-3.40.1/kamangir.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      303 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      475 2024-05-20 22:39:45.000000 kamangir-3.40.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 02:53:18.876599 kamangir-3.40.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-20 01:29:24.000000 kamangir-3.40.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:19:10.723890 kamangir-3.41.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.41.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.41.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-22 02:19:10.723425 kamangir-3.41.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3243 2024-05-21 02:52:53.000000 kamangir-3.41.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:19:10.720869 kamangir-3.41.1/kamangir/
+-rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-22 02:19:04.000000 kamangir-3.41.1/kamangir/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4623 2024-05-22 02:18:49.000000 kamangir-3.41.1/kamangir/content.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:19:10.722896 kamangir-3.41.1/kamangir.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      303 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      430 2024-05-22 02:17:19.000000 kamangir-3.41.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-22 02:19:10.723987 kamangir-3.41.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-20 01:29:24.000000 kamangir-3.41.1/setup.py
```

### Comparing `kamangir-3.40.1/LICENSE` & `kamangir-3.41.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kamangir-3.40.1/PKG-INFO` & `kamangir-3.41.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kamangir
-Version: 3.40.1
+Version: 3.41.1
 Summary: kamangir.net
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 My name is [Arash](http://kamangir.net/); I mix [ai](https://github.com/kamangir/roofAI), [cloud](https://github.com/kamangir/hubble), and [mathematics](https://github.com/kamangir/giza) into minimal forms that seek survival.
```

### Comparing `kamangir-3.40.1/README.md` & `kamangir-3.41.1/README.md`

 * *Files identical despite different names*

### Comparing `kamangir-3.40.1/kamangir/__main__.py` & `kamangir-3.41.1/kamangir/__main__.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.40.1/kamangir/content.py` & `kamangir-3.41.1/kamangir/content.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.40.1/kamangir/functions.py` & `kamangir-3.41.1/kamangir/functions.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.40.1/kamangir.egg-info/PKG-INFO` & `kamangir-3.41.1/kamangir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kamangir
-Version: 3.40.1
+Version: 3.41.1
 Summary: kamangir.net
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 My name is [Arash](http://kamangir.net/); I mix [ai](https://github.com/kamangir/roofAI), [cloud](https://github.com/kamangir/hubble), and [mathematics](https://github.com/kamangir/giza) into minimal forms that seek survival.
```

