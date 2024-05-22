# Comparing `tmp/tracing_auto_instrumentation-0.0.2.tar.gz` & `tmp/tracing_auto_instrumentation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracing_auto_instrumentation-0.0.2.tar", last modified: Wed May 22 14:10:57 2024, max compression
+gzip compressed data, was "tracing_auto_instrumentation-0.0.3.tar", last modified: Wed May 22 16:59:13 2024, max compression
```

## Comparing `tracing_auto_instrumentation-0.0.2.tar` & `tracing_auto_instrumentation-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2024-05-22 14:10:57.315520 tracing_auto_instrumentation-0.0.2/
--rw-r--r--   0 jonathan   (501) staff       (20)    11357 2024-05-21 22:11:21.000000 tracing_auto_instrumentation-0.0.2/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)      527 2024-05-22 14:10:57.315290 tracing_auto_instrumentation-0.0.2/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      869 2024-05-22 14:10:48.000000 tracing_auto_instrumentation-0.0.2/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       35 2024-05-22 14:00:20.000000 tracing_auto_instrumentation-0.0.2/requirements.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2024-05-22 14:10:57.315555 tracing_auto_instrumentation-0.0.2/setup.cfg
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2024-05-22 14:10:57.312741 tracing_auto_instrumentation-0.0.2/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2024-05-22 14:10:57.313925 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/
--rw-r--r--   0 jonathan   (501) staff       (20)      340 2024-05-22 13:16:25.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5577 2024-05-22 13:17:45.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/ibm.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5495 2024-05-22 00:49:45.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/langchain_instrumentor.py
--rw-r--r--   0 jonathan   (501) staff       (20)     6532 2024-05-22 00:49:27.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/llama_index_callback_handler.py
--rw-r--r--   0 jonathan   (501) staff       (20)    14532 2024-05-22 13:22:43.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/openai.py
--rw-r--r--   0 jonathan   (501) staff       (20)      626 2024-05-21 22:33:09.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/wrap_utils.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2024-05-22 14:10:57.315033 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)      527 2024-05-22 14:10:57.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      617 2024-05-22 14:10:57.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2024-05-22 14:10:57.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       36 2024-05-22 14:10:57.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       29 2024-05-22 14:10:57.000000 tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.018581 tracing_auto_instrumentation-0.0.3/
+-rw-r--r--   0 rossdancraig   (501) staff       (20)    11357 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/LICENSE
+-rw-r--r--   0 rossdancraig   (501) staff       (20)      527 2024-05-22 16:59:13.018372 tracing_auto_instrumentation-0.0.3/PKG-INFO
+-rw-r--r--   0 rossdancraig   (501) staff       (20)      870 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/pyproject.toml
+-rw-r--r--   0 rossdancraig   (501) staff       (20)       35 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/requirements.txt
+-rw-r--r--   0 rossdancraig   (501) staff       (20)       38 2024-05-22 16:59:13.018766 tracing_auto_instrumentation-0.0.3/setup.cfg
+drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.015218 tracing_auto_instrumentation-0.0.3/src/
+drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.017031 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/
+-rw-r--r--   0 rossdancraig   (501) staff       (20)      340 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/__init__.py
+-rw-r--r--   0 rossdancraig   (501) staff       (20)     7205 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/ibm.py
+-rw-r--r--   0 rossdancraig   (501) staff       (20)     5495 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/langchain_instrumentor.py
+-rw-r--r--   0 rossdancraig   (501) staff       (20)     6532 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/llama_index_callback_handler.py
+-rw-r--r--   0 rossdancraig   (501) staff       (20)    14532 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/openai.py
+-rw-r--r--   0 rossdancraig   (501) staff       (20)      626 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/wrap_utils.py
+drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.018139 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/
+-rw-r--r--   0 rossdancraig   (501) staff       (20)      527 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 rossdancraig   (501) staff       (20)      617 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 rossdancraig   (501) staff       (20)        1 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 rossdancraig   (501) staff       (20)       36 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 rossdancraig   (501) staff       (20)       29 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/top_level.txt
```

### Comparing `tracing_auto_instrumentation-0.0.2/LICENSE` & `tracing_auto_instrumentation-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.2/PKG-INFO` & `tracing_auto_instrumentation-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracing_auto_instrumentation
-Version: 0.0.2
+Version: 0.0.3
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/tracing_auto_instrumentation
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/tracing_auto_instrumentation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tracing_auto_instrumentation-0.0.2/pyproject.toml` & `tracing_auto_instrumentation-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "tracing_auto_instrumentation"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="LastMile AI" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -35,8 +35,8 @@
     | .hg
     | .mypy_cache
     | .tox
     | venv
     | buck-out
     | dist
   )/
-'''
+'''
```

### Comparing `tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/langchain_instrumentor.py` & `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/langchain_instrumentor.py`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/llama_index_callback_handler.py` & `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/llama_index_callback_handler.py`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/openai.py` & `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation/wrap_utils.py` & `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/wrap_utils.py`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/PKG-INFO` & `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracing_auto_instrumentation
-Version: 0.0.2
+Version: 0.0.3
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/tracing_auto_instrumentation
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/tracing_auto_instrumentation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tracing_auto_instrumentation-0.0.2/src/tracing_auto_instrumentation.egg-info/SOURCES.txt` & `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

