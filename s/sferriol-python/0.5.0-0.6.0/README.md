# Comparing `tmp/sferriol_python-0.5.0.tar.gz` & `tmp/sferriol_python-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sferriol_python-0.5.0.tar", last modified: Sun Apr 28 09:30:48 2024, max compression
+gzip compressed data, was "sferriol_python-0.6.0.tar", last modified: Wed May 22 08:42:58 2024, max compression
```

## Comparing `sferriol_python-0.5.0.tar` & `sferriol_python-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.090427 sferriol_python-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      747 2024-04-28 09:30:48.090427 sferriol_python-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-04-28 09:30:48.093427 sferriol_python-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.087427 sferriol_python-0.5.0/sferriol/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.089427 sferriol_python-0.5.0/sferriol/python/
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.089427 sferriol_python-0.5.0/sferriol/python/dictionary/
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/dictionary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/env.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/json.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/object.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/os.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.090427 sferriol_python-0.5.0/sferriol_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:42:58.973605 sferriol_python-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-22 08:42:58.973605 sferriol_python-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-22 08:42:58.975605 sferriol_python-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:42:58.970605 sferriol_python-0.6.0/sferriol/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:42:58.972605 sferriol_python-0.6.0/sferriol/python/
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/_asyncio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:42:58.972605 sferriol_python-0.6.0/sferriol/python/dictionary/
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/dictionary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/object.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-22 08:41:15.000000 sferriol_python-0.6.0/sferriol/python/os.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:42:58.973605 sferriol_python-0.6.0/sferriol_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-22 08:42:58.000000 sferriol_python-0.6.0/sferriol_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-22 08:42:58.000000 sferriol_python-0.6.0/sferriol_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 08:42:58.000000 sferriol_python-0.6.0/sferriol_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-22 08:42:58.000000 sferriol_python-0.6.0/sferriol_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 08:42:58.000000 sferriol_python-0.6.0/sferriol_python.egg-info/top_level.txt
```

### Comparing `sferriol_python-0.5.0/LICENSE` & `sferriol_python-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sferriol_python-0.5.0/PKG-INFO` & `sferriol_python-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sferriol-python
-Version: 0.5.0
+Version: 0.6.0
 Summary: python utilities
 Home-page: https://gitlab.in2p3.fr/sferriol-ip2i/sferriol-python
 Author: Sylvain Ferriol
 Author-email: s.ferriol@ipnl.in2p3.fr
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sferriol_python-0.5.0/setup.cfg` & `sferriol_python-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sferriol_python-0.5.0/sferriol/python/__init__.py` & `sferriol_python-0.6.0/sferriol/python/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import importlib.util
 import pathlib
 import time
 import types
 from typing import Any, Callable
 
+import _asyncio as asyncio
+
 
 def load_module_from_file(fpath):
     """
     Load a module from a python file. 
     The module name is the file name without file extension. 
     """
     name = module_name_from_file(fpath)
@@ -38,14 +40,15 @@
 
 
 def method(obj):
     """
     Decorator used to define a function as a new method of the object obj.
     The method name is the function name.
     """
+
     def _(func):
         name = func.__name__
         setattr(obj, name, types.MethodType(func, obj))
         return getattr(obj, name)
 
     return _
```

### Comparing `sferriol_python-0.5.0/sferriol/python/dictionary/__init__.py` & `sferriol_python-0.6.0/sferriol/python/dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `sferriol_python-0.5.0/sferriol/python/json.py` & `sferriol_python-0.6.0/sferriol/python/json.py`

 * *Files identical despite different names*

### Comparing `sferriol_python-0.5.0/sferriol/python/object.py` & `sferriol_python-0.6.0/sferriol/python/object.py`

 * *Files identical despite different names*

### Comparing `sferriol_python-0.5.0/sferriol_python.egg-info/PKG-INFO` & `sferriol_python-0.6.0/sferriol_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sferriol-python
-Version: 0.5.0
+Version: 0.6.0
 Summary: python utilities
 Home-page: https://gitlab.in2p3.fr/sferriol-ip2i/sferriol-python
 Author: Sylvain Ferriol
 Author-email: s.ferriol@ipnl.in2p3.fr
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

