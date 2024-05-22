# Comparing `tmp/clisync-1.3.0.tar.gz` & `tmp/clisync-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clisync-1.3.0.tar", last modified: Thu May  2 20:06:30 2024, max compression
+gzip compressed data, was "clisync-1.3.1.tar", last modified: Wed May 22 16:19:35 2024, max compression
```

## Comparing `clisync-1.3.0.tar` & `clisync-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.877676 clisync-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.869675 clisync-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-02 20:06:21.000000 clisync-1.3.0/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-02 20:06:21.000000 clisync-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-02 20:06:21.000000 clisync-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 20:06:21.000000 clisync-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-02 20:06:30.873675 clisync-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-02 20:06:21.000000 clisync-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/clisync/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-02 20:06:21.000000 clisync-1.3.0/clisync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-02 20:06:21.000000 clisync-1.3.0/clisync/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-02 20:06:21.000000 clisync-1.3.0/clisync/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/clisync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:06:26.000000 clisync-1.3.0/clisync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/demo/clisyncdemo/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/clisyncdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/clisyncdemo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/clisyncdemo/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 20:06:21.000000 clisync-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 20:06:21.000000 clisync-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:06:30.877676 clisync-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 20:06:21.000000 clisync-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.834296 clisync-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.830296 clisync-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.830296 clisync-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-22 16:19:28.000000 clisync-1.3.1/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-22 16:19:28.000000 clisync-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-22 16:19:28.000000 clisync-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 16:19:28.000000 clisync-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-22 16:19:35.834296 clisync-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-22 16:19:28.000000 clisync-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.830296 clisync-1.3.1/clisync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-22 16:19:28.000000 clisync-1.3.1/clisync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-22 16:19:28.000000 clisync-1.3.1/clisync/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-22 16:19:28.000000 clisync-1.3.1/clisync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.834296 clisync-1.3.1/clisync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-22 16:19:35.000000 clisync-1.3.1/clisync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-22 16:19:35.000000 clisync-1.3.1/clisync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:19:35.000000 clisync-1.3.1/clisync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:19:32.000000 clisync-1.3.1/clisync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 16:19:35.000000 clisync-1.3.1/clisync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 16:19:35.000000 clisync-1.3.1/clisync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.834296 clisync-1.3.1/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-22 16:19:28.000000 clisync-1.3.1/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:35.834296 clisync-1.3.1/demo/clisyncdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 16:19:28.000000 clisync-1.3.1/demo/clisyncdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:28.000000 clisync-1.3.1/demo/clisyncdemo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-22 16:19:28.000000 clisync-1.3.1/demo/clisyncdemo/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 16:19:28.000000 clisync-1.3.1/demo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 16:19:28.000000 clisync-1.3.1/demo/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 16:19:28.000000 clisync-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 16:19:28.000000 clisync-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:19:35.834296 clisync-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-22 16:19:28.000000 clisync-1.3.1/setup.py
```

### Comparing `clisync-1.3.0/.github/workflows/pypi_release.yml` & `clisync-1.3.1/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/.gitignore` & `clisync-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/LICENSE` & `clisync-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/PKG-INFO` & `clisync-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clisync
-Version: 1.3.0
+Version: 1.3.1
 Summary: Generate click commands from your project
 Home-page: https://clisync.surge.sh
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `clisync-1.3.0/README.md` & `clisync-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/clisync/__init__.py` & `clisync-1.3.1/clisync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 import click
 from typing import List, Union
 import importlib
 
 from clisync.utils import list_static_method, cli_callback, cli_doc
```

### Comparing `clisync-1.3.0/clisync/shell.py` & `clisync-1.3.1/clisync/shell.py`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/clisync/utils.py` & `clisync-1.3.1/clisync/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import List, get_type_hints, Union
-import importlib
+from typing import List, get_type_hints
 import click
 import re
 
 
 def get_method_description(method: callable):
     """Get the first line of the method docstring as the description.
     If the method has no docstring, return an empty string.
@@ -62,15 +61,15 @@
     """
     params = []
     helps = get_method_description(method)
     param_docs = get_params_from_docstring(method.__doc__)
     annotations = get_type_hints(method)
     return_in_annots = "return" in annotations
     for idx, (key, value) in enumerate(annotations.items()):
-        if key == "return" or key in method._overriden_kwargs:
+        if key == "return" or (hasattr(method, "_overriden_kwargs") and key in method._overriden_kwargs):
             continue
         default_value = None
         di = len(annotations) - len(method.__defaults__ or []) - int(return_in_annots)
         if method.__defaults__ and len(method.__defaults__) > 0 and idx >= di:
             default_value = method.__defaults__[idx - di]
         multiple = False
         if str(value).startswith("typing.Optional"):
@@ -88,15 +87,15 @@
             default_value = False
         param = click.Option(
             [f"--{key}"],
             default=default_value,
             prompt_required=default_value is None,
             type=value,
             multiple=multiple,
-            help=param_docs.get(key, f""),
+            help=param_docs.get(key, ""),
             show_default=True,
             is_flag=value == bool,
         )
         params.append(param)
     return helps, list(reversed(params))
```

### Comparing `clisync-1.3.0/clisync.egg-info/PKG-INFO` & `clisync-1.3.1/clisync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clisync
-Version: 1.3.0
+Version: 1.3.1
 Summary: Generate click commands from your project
 Home-page: https://clisync.surge.sh
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `clisync-1.3.0/demo/clisyncdemo/__init__.py` & `clisync-1.3.1/demo/clisyncdemo/__init__.py`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/demo/clisyncdemo/objects.py` & `clisync-1.3.1/demo/clisyncdemo/objects.py`

 * *Files identical despite different names*

### Comparing `clisync-1.3.0/setup.py` & `clisync-1.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
```

