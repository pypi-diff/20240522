# Comparing `tmp/cdindex-1.0.8.tar.gz` & `tmp/cdindex-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdindex-1.0.8.tar", last modified: Thu Jul 20 13:08:30 2017, max compression
+gzip compressed data, was "dist/cdindex-1.0.9.tar", last modified: Thu Jul 20 13:13:16 2017, max compression
```

## Comparing `cdindex-1.0.8.tar` & `cdindex-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:08:30.000000 cdindex-1.0.8/
-drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:08:30.000000 cdindex-1.0.8/cdindex/
--rw-r--r--   0 funk       (501) staff       (20)       50 2016-01-16 17:14:30.000000 cdindex-1.0.8/cdindex/__init__.py
--rw-r--r--   0 funk       (501) staff       (20)    12875 2017-07-20 12:56:09.000000 cdindex-1.0.8/cdindex/cdindex.py
--rw-r--r--   0 funk       (501) staff       (20)    12395 2017-07-20 13:03:40.000000 cdindex-1.0.8/cdindex/pycdindex.c
--rw-r--r--   0 funk       (501) staff       (20)     1358 2017-07-20 00:21:19.000000 cdindex-1.0.8/cdindex/time_utilities.py
-drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:08:30.000000 cdindex-1.0.8/cdindex.egg-info/
--rw-r--r--   0 funk       (501) staff       (20)        1 2017-07-20 13:08:29.000000 cdindex-1.0.8/cdindex.egg-info/dependency_links.txt
--rw-r--r--   0 funk       (501) staff       (20)      271 2017-07-20 13:08:29.000000 cdindex-1.0.8/cdindex.egg-info/PKG-INFO
--rw-r--r--   0 funk       (501) staff       (20)      305 2017-07-20 13:08:29.000000 cdindex-1.0.8/cdindex.egg-info/SOURCES.txt
--rw-r--r--   0 funk       (501) staff       (20)        8 2017-07-20 13:08:29.000000 cdindex-1.0.8/cdindex.egg-info/top_level.txt
--rw-r--r--   0 funk       (501) staff       (20)       34 2017-06-29 00:55:22.000000 cdindex-1.0.8/MANIFEST.in
--rw-r--r--   0 funk       (501) staff       (20)      271 2017-07-20 13:08:30.000000 cdindex-1.0.8/PKG-INFO
--rw-r--r--   0 funk       (501) staff       (20)     2997 2017-07-12 12:36:07.000000 cdindex-1.0.8/README.rst
--rw-r--r--   0 funk       (501) staff       (20)       59 2017-07-20 13:08:30.000000 cdindex-1.0.8/setup.cfg
--rw-r--r--   0 funk       (501) staff       (20)      962 2017-07-20 13:07:34.000000 cdindex-1.0.8/setup.py
-drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:08:30.000000 cdindex-1.0.8/src/
--rw-r--r--   0 funk       (501) staff       (20)     4486 2017-07-20 12:54:48.000000 cdindex-1.0.8/src/cdindex.c
--rw-r--r--   0 funk       (501) staff       (20)     1249 2017-07-20 13:07:23.000000 cdindex-1.0.8/src/cdindex.h
--rw-r--r--   0 funk       (501) staff       (20)     4891 2017-07-20 12:21:08.000000 cdindex-1.0.8/src/graph.c
--rw-r--r--   0 funk       (501) staff       (20)     2565 2017-07-20 12:20:12.000000 cdindex-1.0.8/src/main.c
--rw-r--r--   0 funk       (501) staff       (20)     2379 2017-07-20 12:19:40.000000 cdindex-1.0.8/src/utility.c
+drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:13:16.000000 cdindex-1.0.9/
+drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:13:16.000000 cdindex-1.0.9/cdindex/
+-rw-r--r--   0 funk       (501) staff       (20)       50 2016-01-16 17:14:30.000000 cdindex-1.0.9/cdindex/__init__.py
+-rw-r--r--   0 funk       (501) staff       (20)    12875 2017-07-20 12:56:09.000000 cdindex-1.0.9/cdindex/cdindex.py
+-rw-r--r--   0 funk       (501) staff       (20)    12395 2017-07-20 13:03:40.000000 cdindex-1.0.9/cdindex/pycdindex.c
+-rw-r--r--   0 funk       (501) staff       (20)     1358 2017-07-20 00:21:19.000000 cdindex-1.0.9/cdindex/time_utilities.py
+drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:13:16.000000 cdindex-1.0.9/cdindex.egg-info/
+-rw-r--r--   0 funk       (501) staff       (20)        1 2017-07-20 13:13:16.000000 cdindex-1.0.9/cdindex.egg-info/dependency_links.txt
+-rw-r--r--   0 funk       (501) staff       (20)      271 2017-07-20 13:13:16.000000 cdindex-1.0.9/cdindex.egg-info/PKG-INFO
+-rw-r--r--   0 funk       (501) staff       (20)      305 2017-07-20 13:13:16.000000 cdindex-1.0.9/cdindex.egg-info/SOURCES.txt
+-rw-r--r--   0 funk       (501) staff       (20)        8 2017-07-20 13:13:16.000000 cdindex-1.0.9/cdindex.egg-info/top_level.txt
+-rw-r--r--   0 funk       (501) staff       (20)       34 2017-06-29 00:55:22.000000 cdindex-1.0.9/MANIFEST.in
+-rw-r--r--   0 funk       (501) staff       (20)      271 2017-07-20 13:13:16.000000 cdindex-1.0.9/PKG-INFO
+-rw-r--r--   0 funk       (501) staff       (20)     2997 2017-07-12 12:36:07.000000 cdindex-1.0.9/README.rst
+-rw-r--r--   0 funk       (501) staff       (20)       59 2017-07-20 13:13:16.000000 cdindex-1.0.9/setup.cfg
+-rw-r--r--   0 funk       (501) staff       (20)      962 2017-07-20 13:09:55.000000 cdindex-1.0.9/setup.py
+drwxr-xr-x   0 funk       (501) staff       (20)        0 2017-07-20 13:13:16.000000 cdindex-1.0.9/src/
+-rw-r--r--   0 funk       (501) staff       (20)     4486 2017-07-20 12:54:48.000000 cdindex-1.0.9/src/cdindex.c
+-rw-r--r--   0 funk       (501) staff       (20)     1256 2017-07-20 13:12:28.000000 cdindex-1.0.9/src/cdindex.h
+-rw-r--r--   0 funk       (501) staff       (20)     4891 2017-07-20 12:21:08.000000 cdindex-1.0.9/src/graph.c
+-rw-r--r--   0 funk       (501) staff       (20)     2565 2017-07-20 12:20:12.000000 cdindex-1.0.9/src/main.c
+-rw-r--r--   0 funk       (501) staff       (20)     2379 2017-07-20 12:19:40.000000 cdindex-1.0.9/src/utility.c
```

### Comparing `cdindex-1.0.8/cdindex/cdindex.py` & `cdindex-1.0.9/cdindex/cdindex.py`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/cdindex/pycdindex.c` & `cdindex-1.0.9/cdindex/pycdindex.c`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/cdindex/time_utilities.py` & `cdindex-1.0.9/cdindex/time_utilities.py`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/README.rst` & `cdindex-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/setup.py` & `cdindex-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __author__ = "Russell J. Funk"
 __copyright__ = "Copyright (C) 2017"
 
 # built in modules
 from setuptools import setup, Extension, find_packages
 
 setup(name="cdindex",
-    version="1.0.8",
+    version="1.0.9",
     description="Package for computing the cdindex.",
     author="Russell J. Funk",
     author_email="russellfunk@gmail.com",
     url="http://www.cdindex.info",
     license="GNU General Public License (GPL)",
     ext_modules=[
                   Extension("cdindex._cdindex",
```

### Comparing `cdindex-1.0.8/src/cdindex.c` & `cdindex-1.0.9/src/cdindex.c`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/src/cdindex.h` & `cdindex-1.0.9/src/cdindex.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 void add_vertex(Graph *graph, long long int id, long long int timestamp);
 void add_edge(Graph *graph, long long int source_id, long long int target_id);
 void free_graph(Graph *graph);
 
 /* function prototypes for cdindex.c */
 double cdindex(Graph *graph, long long int id, long long int time_delta);
 double mcdindex(Graph *graph, long long int id, long long int time_delta);
-double iindex(Graph *graph, long long int id, long long int time_delta);
+long long int iindex(Graph *graph, long long int id, long long int time_delta);
```

### Comparing `cdindex-1.0.8/src/graph.c` & `cdindex-1.0.9/src/graph.c`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/src/main.c` & `cdindex-1.0.9/src/main.c`

 * *Files identical despite different names*

### Comparing `cdindex-1.0.8/src/utility.c` & `cdindex-1.0.9/src/utility.c`

 * *Files identical despite different names*

