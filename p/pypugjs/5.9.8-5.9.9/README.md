# Comparing `tmp/pypugjs-5.9.8.tar.gz` & `tmp/pypugjs-5.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypugjs-5.9.8.tar", last modified: Wed Dec  9 05:51:08 2020, max compression
+gzip compressed data, was "dist/pypugjs-5.9.9.tar", last modified: Tue Mar  2 13:35:04 2021, max compression
```

## Comparing `pypugjs-5.9.8.tar` & `pypugjs-5.9.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.993323 pypugjs-5.9.8/
--rw-r--r--   0 andy       (501) staff       (20)       11 2020-12-09 05:50:43.000000 pypugjs-5.9.8/MANIFEST.in
--rw-r--r--   0 andy       (501) staff       (20)     9157 2020-12-09 05:51:08.993779 pypugjs-5.9.8/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     3786 2020-10-09 07:04:57.000000 pypugjs-5.9.8/README.rst
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.940788 pypugjs-5.9.8/docs/
--rw-r--r--   0 andy       (501) staff       (20)     2112 2020-10-09 07:04:57.000000 pypugjs-5.9.8/docs/HISTORY.rst
--rw-r--r--   0 andy       (501) staff       (20)     3158 2020-10-09 07:04:57.000000 pypugjs-5.9.8/docs/installation.rst
--rw-r--r--   0 andy       (501) staff       (20)      440 2020-10-09 07:25:46.000000 pypugjs-5.9.8/pyproject.toml
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.981824 pypugjs-5.9.8/pypugjs/
--rw-r--r--   0 andy       (501) staff       (20)      311 2020-12-09 05:51:04.000000 pypugjs-5.9.8/pypugjs/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    15610 2020-10-09 07:05:04.000000 pypugjs-5.9.8/pypugjs/compiler.py
--rw-r--r--   0 andy       (501) staff       (20)     2861 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/convert.py
--rw-r--r--   0 andy       (501) staff       (20)       49 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/exceptions.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.985922 pypugjs-5.9.8/pypugjs/ext/
--rw-r--r--   0 andy       (501) staff       (20)        0 2018-03-23 13:11:48.000000 pypugjs-5.9.8/pypugjs/ext/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.989680 pypugjs-5.9.8/pypugjs/ext/django/
--rw-r--r--   0 andy       (501) staff       (20)      113 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/django/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     3130 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/django/compiler.py
--rw-r--r--   0 andy       (501) staff       (20)     1854 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/django/loader.py
--rw-r--r--   0 andy       (501) staff       (20)     6389 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/django/templatetags.py
--rw-r--r--   0 andy       (501) staff       (20)     5788 2020-10-09 07:05:04.000000 pypugjs-5.9.8/pypugjs/ext/html.py
--rw-r--r--   0 andy       (501) staff       (20)     5373 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/jinja.py
--rw-r--r--   0 andy       (501) staff       (20)     3827 2020-10-09 07:05:04.000000 pypugjs-5.9.8/pypugjs/ext/mako.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.991011 pypugjs-5.9.8/pypugjs/ext/pyramid/
--rw-r--r--   0 andy       (501) staff       (20)     1511 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/pyramid/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.992350 pypugjs-5.9.8/pypugjs/ext/tornado/
--rw-r--r--   0 andy       (501) staff       (20)     3341 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/tornado/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     4207 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/ext/underscore.py
--rw-r--r--   0 andy       (501) staff       (20)      675 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/filters.py
--rw-r--r--   0 andy       (501) staff       (20)    23425 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/lexer.py
--rw-r--r--   0 andy       (501) staff       (20)     5329 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/nodes.py
--rw-r--r--   0 andy       (501) staff       (20)    10921 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/parser.py
--rw-r--r--   0 andy       (501) staff       (20)     4548 2020-11-26 12:26:44.000000 pypugjs-5.9.8/pypugjs/runtime.py
--rw-r--r--   0 andy       (501) staff       (20)     6653 2020-10-09 07:04:57.000000 pypugjs-5.9.8/pypugjs/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2020-12-09 05:51:08.983806 pypugjs-5.9.8/pypugjs.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     9157 2020-12-09 05:51:08.000000 pypugjs-5.9.8/pypugjs.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      772 2020-12-09 05:51:08.000000 pypugjs-5.9.8/pypugjs.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2020-12-09 05:51:08.000000 pypugjs-5.9.8/pypugjs.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       58 2020-12-09 05:51:08.000000 pypugjs-5.9.8/pypugjs.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)       12 2020-12-09 05:51:08.000000 pypugjs-5.9.8/pypugjs.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        8 2020-12-09 05:51:08.000000 pypugjs-5.9.8/pypugjs.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)      261 2020-12-09 05:51:08.995306 pypugjs-5.9.8/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     2267 2020-12-07 11:43:38.000000 pypugjs-5.9.8/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.570723 pypugjs-5.9.9/
+-rw-r--r--   0 andy       (501) staff       (20)       11 2020-12-09 05:50:43.000000 pypugjs-5.9.9/MANIFEST.in
+-rw-r--r--   0 andy       (501) staff       (20)     9157 2021-03-02 13:35:04.570930 pypugjs-5.9.9/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     3786 2020-10-09 07:04:57.000000 pypugjs-5.9.9/README.rst
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.559807 pypugjs-5.9.9/docs/
+-rw-r--r--   0 andy       (501) staff       (20)     2112 2020-10-09 07:04:57.000000 pypugjs-5.9.9/docs/HISTORY.rst
+-rw-r--r--   0 andy       (501) staff       (20)     3158 2020-10-09 07:04:57.000000 pypugjs-5.9.9/docs/installation.rst
+-rw-r--r--   0 andy       (501) staff       (20)      440 2020-10-09 07:25:46.000000 pypugjs-5.9.9/pyproject.toml
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.564897 pypugjs-5.9.9/pypugjs/
+-rw-r--r--   0 andy       (501) staff       (20)      311 2021-03-02 13:34:50.000000 pypugjs-5.9.9/pypugjs/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    15610 2020-10-09 07:05:04.000000 pypugjs-5.9.9/pypugjs/compiler.py
+-rw-r--r--   0 andy       (501) staff       (20)     2861 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/convert.py
+-rw-r--r--   0 andy       (501) staff       (20)       49 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/exceptions.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.568322 pypugjs-5.9.9/pypugjs/ext/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2018-03-23 13:11:48.000000 pypugjs-5.9.9/pypugjs/ext/__init__.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.569724 pypugjs-5.9.9/pypugjs/ext/django/
+-rw-r--r--   0 andy       (501) staff       (20)      113 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/django/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     3130 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/django/compiler.py
+-rw-r--r--   0 andy       (501) staff       (20)     1854 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/django/loader.py
+-rw-r--r--   0 andy       (501) staff       (20)     6389 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/django/templatetags.py
+-rw-r--r--   0 andy       (501) staff       (20)     5788 2020-10-09 07:05:04.000000 pypugjs-5.9.9/pypugjs/ext/html.py
+-rw-r--r--   0 andy       (501) staff       (20)     5373 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/jinja.py
+-rw-r--r--   0 andy       (501) staff       (20)     3827 2020-10-09 07:05:04.000000 pypugjs-5.9.9/pypugjs/ext/mako.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.570107 pypugjs-5.9.9/pypugjs/ext/pyramid/
+-rw-r--r--   0 andy       (501) staff       (20)     1511 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/pyramid/__init__.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.570463 pypugjs-5.9.9/pypugjs/ext/tornado/
+-rw-r--r--   0 andy       (501) staff       (20)     3341 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/tornado/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     4207 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/ext/underscore.py
+-rw-r--r--   0 andy       (501) staff       (20)      675 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/filters.py
+-rw-r--r--   0 andy       (501) staff       (20)    23425 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/lexer.py
+-rw-r--r--   0 andy       (501) staff       (20)     5329 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/nodes.py
+-rw-r--r--   0 andy       (501) staff       (20)    10921 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     4552 2021-03-02 13:34:50.000000 pypugjs-5.9.9/pypugjs/runtime.py
+-rw-r--r--   0 andy       (501) staff       (20)     6653 2020-10-09 07:04:57.000000 pypugjs-5.9.9/pypugjs/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2021-03-02 13:35:04.566721 pypugjs-5.9.9/pypugjs.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     9157 2021-03-02 13:35:04.000000 pypugjs-5.9.9/pypugjs.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      772 2021-03-02 13:35:04.000000 pypugjs-5.9.9/pypugjs.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2021-03-02 13:35:04.000000 pypugjs-5.9.9/pypugjs.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       58 2021-03-02 13:35:04.000000 pypugjs-5.9.9/pypugjs.egg-info/entry_points.txt
+-rw-r--r--   0 andy       (501) staff       (20)       12 2021-03-02 13:35:04.000000 pypugjs-5.9.9/pypugjs.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        8 2021-03-02 13:35:04.000000 pypugjs-5.9.9/pypugjs.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      261 2021-03-02 13:35:04.571636 pypugjs-5.9.9/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     2267 2020-12-07 11:43:38.000000 pypugjs-5.9.9/setup.py
```

### Comparing `pypugjs-5.9.8/PKG-INFO` & `pypugjs-5.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pypugjs
-Version: 5.9.8
+Version: 5.9.9
 Summary: PugJS syntax template adapter for Django, Jinja2, Mako and Tornado templates
 Home-page: https://github.com/kakulukia/pypugjs
 Author: Andy Grabow
 Author-email: andy@freilandkiwis.de
 License: MIT
-Download-URL: https://github.com/kakulukia/pypugjs/tarball/5.9.8
+Download-URL: https://github.com/kakulukia/pypugjs/tarball/5.9.9
 Description: PyPugJS |PyPiPackage|_ |BuildStatus|_ |Coverage|_
         ===================================================
         
         .. |PyPiPackage| image:: https://badge.fury.io/py/pypugjs.svg
         .. _PyPiPackage: https://badge.fury.io/py/pypugjs
         
         .. |BuildStatus| image:: https://travis-ci.org/kakulukia/pypugjs.svg
```

### Comparing `pypugjs-5.9.8/README.rst` & `pypugjs-5.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/docs/HISTORY.rst` & `pypugjs-5.9.9/docs/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/docs/installation.rst` & `pypugjs-5.9.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/compiler.py` & `pypugjs-5.9.9/pypugjs/compiler.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/convert.py` & `pypugjs-5.9.9/pypugjs/convert.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/django/compiler.py` & `pypugjs-5.9.9/pypugjs/ext/django/compiler.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/django/loader.py` & `pypugjs-5.9.9/pypugjs/ext/django/loader.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/django/templatetags.py` & `pypugjs-5.9.9/pypugjs/ext/django/templatetags.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/html.py` & `pypugjs-5.9.9/pypugjs/ext/html.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/jinja.py` & `pypugjs-5.9.9/pypugjs/ext/jinja.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/mako.py` & `pypugjs-5.9.9/pypugjs/ext/mako.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/pyramid/__init__.py` & `pypugjs-5.9.9/pypugjs/ext/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/tornado/__init__.py` & `pypugjs-5.9.9/pypugjs/ext/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/ext/underscore.py` & `pypugjs-5.9.9/pypugjs/ext/underscore.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/filters.py` & `pypugjs-5.9.9/pypugjs/filters.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/lexer.py` & `pypugjs-5.9.9/pypugjs/lexer.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/nodes.py` & `pypugjs-5.9.9/pypugjs/nodes.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/parser.py` & `pypugjs-5.9.9/pypugjs/parser.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs/runtime.py` & `pypugjs-5.9.9/pypugjs/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import six
 from six.moves import reduce
 
 from chardet.universaldetector import UniversalDetector
 import io
 
 try:
-    from collections import Mapping as MappingType
+    from collections.abc import Mapping as MappingType
 except ImportError:
     import UserDict
 
     MappingType = (UserDict.UserDict, UserDict.DictMixin, dict)
 
 
 def escape(s):
```

### Comparing `pypugjs-5.9.8/pypugjs/utils.py` & `pypugjs-5.9.9/pypugjs/utils.py`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/pypugjs.egg-info/PKG-INFO` & `pypugjs-5.9.9/pypugjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pypugjs
-Version: 5.9.8
+Version: 5.9.9
 Summary: PugJS syntax template adapter for Django, Jinja2, Mako and Tornado templates
 Home-page: https://github.com/kakulukia/pypugjs
 Author: Andy Grabow
 Author-email: andy@freilandkiwis.de
 License: MIT
-Download-URL: https://github.com/kakulukia/pypugjs/tarball/5.9.8
+Download-URL: https://github.com/kakulukia/pypugjs/tarball/5.9.9
 Description: PyPugJS |PyPiPackage|_ |BuildStatus|_ |Coverage|_
         ===================================================
         
         .. |PyPiPackage| image:: https://badge.fury.io/py/pypugjs.svg
         .. _PyPiPackage: https://badge.fury.io/py/pypugjs
         
         .. |BuildStatus| image:: https://travis-ci.org/kakulukia/pypugjs.svg
```

### Comparing `pypugjs-5.9.8/pypugjs.egg-info/SOURCES.txt` & `pypugjs-5.9.9/pypugjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypugjs-5.9.8/setup.py` & `pypugjs-5.9.9/setup.py`

 * *Files identical despite different names*

