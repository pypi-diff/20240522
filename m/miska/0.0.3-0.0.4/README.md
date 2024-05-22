# Comparing `tmp/miska-0.0.3.tar.gz` & `tmp/miska-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miska-0.0.3.tar", last modified: Tue May 21 08:59:23 2024, max compression
+gzip compressed data, was "miska-0.0.4.tar", last modified: Wed May 22 15:29:45 2024, max compression
```

## Comparing `miska-0.0.3.tar` & `miska-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.175150 miska-0.0.3/
--rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.3/LICENSE
--rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-21 08:59:23.174150 miska-0.0.3/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.3/README.rst
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.169150 miska-0.0.3/miska/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/__init__.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.171150 miska-0.0.3/miska/http/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/http/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.3/miska/http/rs.py
--rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.3/miska/mixins.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1828 2024-05-21 08:55:25.000000 miska-0.0.3/miska/registries.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.172150 miska-0.0.3/miska/types/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/types/__init__.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.173150 miska-0.0.3/miska/types/network/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/types/network/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.3/miska/types/network/bgp.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.173150 miska-0.0.3/miska.egg-info/
--rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      379 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/SOURCES.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/dependency_links.txt
--rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/requires.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/top_level.txt
--rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-21 08:57:50.000000 miska-0.0.3/pyproject.toml
--rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-21 08:59:23.175150 miska-0.0.3/setup.cfg
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.173150 miska-0.0.3/tests/
--rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-21 08:54:48.000000 miska-0.0.3/tests/test_registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.819277 miska-0.0.4/
+-rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.4/LICENSE
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-22 15:29:45.818277 miska-0.0.4/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.4/README.rst
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.813278 miska-0.0.4/miska/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1215 2024-05-22 15:28:25.000000 miska-0.0.4/miska/dataclasses.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.815277 miska-0.0.4/miska/http/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/http/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.4/miska/http/rs.py
+-rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.4/miska/mixins.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1828 2024-05-22 15:28:18.000000 miska-0.0.4/miska/registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.816277 miska-0.0.4/miska/types/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/types/__init__.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.816277 miska-0.0.4/miska/types/network/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/types/network/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.4/miska/types/network/bgp.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.817278 miska-0.0.4/miska.egg-info/
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      400 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/SOURCES.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/dependency_links.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/requires.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/top_level.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-22 15:28:25.000000 miska-0.0.4/pyproject.toml
+-rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-22 15:29:45.819277 miska-0.0.4/setup.cfg
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.817278 miska-0.0.4/tests/
+-rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-21 08:54:48.000000 miska-0.0.4/tests/test_registries.py
```

### Comparing `miska-0.0.3/LICENSE` & `miska-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `miska-0.0.3/PKG-INFO` & `miska-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.3
+Version: 0.0.4
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `miska-0.0.3/README.rst` & `miska-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `miska-0.0.3/miska/http/rs.py` & `miska-0.0.4/miska/http/rs.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.3/miska/registries.py` & `miska-0.0.4/miska/registries.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.3/miska/types/network/bgp.py` & `miska-0.0.4/miska/types/network/bgp.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.3/miska.egg-info/PKG-INFO` & `miska-0.0.4/miska.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.3
+Version: 0.0.4
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `miska-0.0.3/pyproject.toml` & `miska-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "miska"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Dima Burmistrov", email="pyctrl.dev@gmail.com" },
 ]
 description = "An exceptional library"
 readme = "README.rst"
 license = {file = "LICENSE"}
```

