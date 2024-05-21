# Comparing `tmp/hermes_cai-0.0.8.tar.gz` & `tmp/hermes_cai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermes_cai-0.0.8.tar", last modified: Mon May 20 22:35:12 2024, max compression
+gzip compressed data, was "hermes_cai-0.0.9.tar", last modified: Mon May 20 22:35:43 2024, max compression
```

## Comparing `hermes_cai-0.0.8.tar` & `hermes_cai-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:35:12.031408 hermes_cai-0.0.8/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       16 2024-05-20 22:15:52.000000 hermes_cai-0.0.8/MANIFEST.in
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 22:35:12.031222 hermes_cai-0.0.8/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 22:15:52.000000 hermes_cai-0.0.8/README.md
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        5 2024-05-20 22:35:10.000000 hermes_cai-0.0.8/VERSION
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:35:12.030254 hermes_cai-0.0.8/hermes_cai/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:15:52.000000 hermes_cai-0.0.8/hermes_cai/__init__.py
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 22:15:52.000000 hermes_cai-0.0.8/hermes_cai/constants.py
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      625 2024-05-20 20:17:08.000000 hermes_cai-0.0.8/hermes_cai/exceptions.py
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:35:12.030929 hermes_cai-0.0.8/hermes_cai.egg-info/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 22:35:12.000000 hermes_cai-0.0.8/hermes_cai.egg-info/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      246 2024-05-20 22:35:12.000000 hermes_cai-0.0.8/hermes_cai.egg-info/SOURCES.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 22:35:12.000000 hermes_cai-0.0.8/hermes_cai.egg-info/dependency_links.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 22:35:12.000000 hermes_cai-0.0.8/hermes_cai.egg-info/top_level.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 22:35:12.031617 hermes_cai-0.0.8/setup.cfg
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      868 2024-05-20 22:15:52.000000 hermes_cai-0.0.8/setup.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:35:43.063966 hermes_cai-0.0.9/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       16 2024-05-20 22:15:52.000000 hermes_cai-0.0.9/MANIFEST.in
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 22:35:43.063780 hermes_cai-0.0.9/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 22:15:52.000000 hermes_cai-0.0.9/README.md
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        5 2024-05-20 22:35:42.000000 hermes_cai-0.0.9/VERSION
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:35:43.060991 hermes_cai-0.0.9/hermes_cai/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:15:52.000000 hermes_cai-0.0.9/hermes_cai/__init__.py
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 22:15:52.000000 hermes_cai-0.0.9/hermes_cai/constants.py
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      625 2024-05-20 20:17:08.000000 hermes_cai-0.0.9/hermes_cai/exceptions.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:35:43.063232 hermes_cai-0.0.9/hermes_cai.egg-info/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 22:35:43.000000 hermes_cai-0.0.9/hermes_cai.egg-info/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      246 2024-05-20 22:35:43.000000 hermes_cai-0.0.9/hermes_cai.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 22:35:43.000000 hermes_cai-0.0.9/hermes_cai.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 22:35:43.000000 hermes_cai-0.0.9/hermes_cai.egg-info/top_level.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 22:35:43.064017 hermes_cai-0.0.9/setup.cfg
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      868 2024-05-20 22:15:52.000000 hermes_cai-0.0.9/setup.py
```

### Comparing `hermes_cai-0.0.8/PKG-INFO` & `hermes_cai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.8/README.md` & `hermes_cai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.8/hermes_cai/constants.py` & `hermes_cai-0.0.9/hermes_cai/constants.py`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.8/hermes_cai/exceptions.py` & `hermes_cai-0.0.9/hermes_cai/exceptions.py`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.8/hermes_cai.egg-info/PKG-INFO` & `hermes_cai-0.0.9/hermes_cai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.8/setup.py` & `hermes_cai-0.0.9/setup.py`

 * *Files identical despite different names*

