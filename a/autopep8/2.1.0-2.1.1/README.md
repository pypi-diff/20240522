# Comparing `tmp/autopep8-2.1.0.tar.gz` & `tmp/autopep8-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopep8-2.1.0.tar", last modified: Sun Mar 17 10:46:46 2024, max compression
+gzip compressed data, was "autopep8-2.1.1.tar", last modified: Wed May 22 12:08:38 2024, max compression
```

## Comparing `autopep8-2.1.0.tar` & `autopep8-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 hattori    (502) staff       (20)        0 2024-03-17 10:46:46.007305 autopep8-2.1.0/
--rw-r--r--   0 hattori    (502) staff       (20)     2003 2020-12-17 05:43:31.000000 autopep8-2.1.0/AUTHORS.rst
--rw-r--r--   0 hattori    (502) staff       (20)     1181 2018-09-01 15:05:18.000000 autopep8-2.1.0/LICENSE
--rw-r--r--   0 hattori    (502) staff       (20)      760 2024-03-17 03:22:20.000000 autopep8-2.1.0/MANIFEST.in
--rw-r--r--   0 hattori    (502) staff       (20)    16967 2024-03-17 10:46:46.006980 autopep8-2.1.0/PKG-INFO
--rw-r--r--   0 hattori    (502) staff       (20)    15766 2024-03-17 10:30:20.000000 autopep8-2.1.0/README.rst
-drwxr-xr-x   0 hattori    (502) staff       (20)        0 2024-03-17 10:46:46.006431 autopep8-2.1.0/autopep8.egg-info/
--rw-r--r--   0 hattori    (502) staff       (20)    16967 2024-03-17 10:46:45.000000 autopep8-2.1.0/autopep8.egg-info/PKG-INFO
--rw-r--r--   0 hattori    (502) staff       (20)      512 2024-03-17 10:46:45.000000 autopep8-2.1.0/autopep8.egg-info/SOURCES.txt
--rw-r--r--   0 hattori    (502) staff       (20)        1 2024-03-17 10:46:45.000000 autopep8-2.1.0/autopep8.egg-info/dependency_links.txt
--rw-r--r--   0 hattori    (502) staff       (20)       43 2024-03-17 10:46:45.000000 autopep8-2.1.0/autopep8.egg-info/entry_points.txt
--rw-r--r--   0 hattori    (502) staff       (20)       54 2024-03-17 10:46:45.000000 autopep8-2.1.0/autopep8.egg-info/requires.txt
--rw-r--r--   0 hattori    (502) staff       (20)        9 2024-03-17 10:46:45.000000 autopep8-2.1.0/autopep8.egg-info/top_level.txt
--rwxr-xr-x   0 hattori    (502) staff       (20)   155184 2024-03-17 10:40:56.000000 autopep8-2.1.0/autopep8.py
--rw-r--r--   0 hattori    (502) staff       (20)     1437 2024-03-17 03:22:20.000000 autopep8-2.1.0/pyproject.toml
--rw-r--r--   0 hattori    (502) staff       (20)       67 2024-03-17 10:46:46.007811 autopep8-2.1.0/setup.cfg
-drwxr-xr-x   0 hattori    (502) staff       (20)        0 2024-03-17 10:46:46.004541 autopep8-2.1.0/test/
--rw-r--r--   0 hattori    (502) staff       (20)        0 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/__init__.py
--rw-r--r--   0 hattori    (502) staff       (20)       27 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/bad_encoding.py
--rw-r--r--   0 hattori    (502) staff       (20)       30 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/bad_encoding2.py
--rw-r--r--   0 hattori    (502) staff       (20)    44753 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/e101_example.py
--rw-r--r--   0 hattori    (502) staff       (20)     2190 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/example.py
-drwxr-xr-x   0 hattori    (502) staff       (20)        0 2024-03-17 10:46:46.004871 autopep8-2.1.0/test/fake_configuration/
--rw-r--r--   0 hattori    (502) staff       (20)       21 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/fake_configuration/.pep8
-drwxr-xr-x   0 hattori    (502) staff       (20)        0 2024-03-17 10:46:46.005989 autopep8-2.1.0/test/fake_pycodestyle_configuration/
--rw-r--r--   0 hattori    (502) staff       (20)       35 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/fake_pycodestyle_configuration/tox.ini
--rw-r--r--   0 hattori    (502) staff       (20)       29 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/iso_8859_1.py
--rwxr-xr-x   0 hattori    (502) staff       (20)   250373 2024-03-17 10:30:31.000000 autopep8-2.1.0/test/test_autopep8.py
--rwxr-xr-x   0 hattori    (502) staff       (20)     2939 2018-09-01 15:05:18.000000 autopep8-2.1.0/test/test_suite.py
--rw-r--r--   0 hattori    (502) staff       (20)      291 2024-03-17 03:22:20.000000 autopep8-2.1.0/tox.ini
+drwxr-xr-x   0 hideohattori   (501) staff       (20)        0 2024-05-22 12:08:38.035898 autopep8-2.1.1/
+-rw-r--r--   0 hideohattori   (501) staff       (20)     2003 2024-04-14 12:52:47.000000 autopep8-2.1.1/AUTHORS.rst
+-rw-r--r--   0 hideohattori   (501) staff       (20)     1181 2024-04-14 12:52:47.000000 autopep8-2.1.1/LICENSE
+-rw-r--r--   0 hideohattori   (501) staff       (20)      760 2024-04-14 12:52:47.000000 autopep8-2.1.1/MANIFEST.in
+-rw-r--r--   0 hideohattori   (501) staff       (20)    16967 2024-05-22 12:08:38.035810 autopep8-2.1.1/PKG-INFO
+-rw-r--r--   0 hideohattori   (501) staff       (20)    15766 2024-04-14 12:52:47.000000 autopep8-2.1.1/README.rst
+drwxr-xr-x   0 hideohattori   (501) staff       (20)        0 2024-05-22 12:08:38.035628 autopep8-2.1.1/autopep8.egg-info/
+-rw-r--r--   0 hideohattori   (501) staff       (20)    16967 2024-05-22 12:08:38.000000 autopep8-2.1.1/autopep8.egg-info/PKG-INFO
+-rw-r--r--   0 hideohattori   (501) staff       (20)      525 2024-05-22 12:08:38.000000 autopep8-2.1.1/autopep8.egg-info/SOURCES.txt
+-rw-r--r--   0 hideohattori   (501) staff       (20)        1 2024-05-22 12:08:38.000000 autopep8-2.1.1/autopep8.egg-info/dependency_links.txt
+-rw-r--r--   0 hideohattori   (501) staff       (20)       43 2024-05-22 12:08:38.000000 autopep8-2.1.1/autopep8.egg-info/entry_points.txt
+-rw-r--r--   0 hideohattori   (501) staff       (20)       54 2024-05-22 12:08:38.000000 autopep8-2.1.1/autopep8.egg-info/requires.txt
+-rw-r--r--   0 hideohattori   (501) staff       (20)        9 2024-05-22 12:08:38.000000 autopep8-2.1.1/autopep8.egg-info/top_level.txt
+-rwxr-xr-x   0 hideohattori   (501) staff       (20)   155326 2024-05-22 11:55:28.000000 autopep8-2.1.1/autopep8.py
+-rw-r--r--   0 hideohattori   (501) staff       (20)     1437 2024-05-22 11:54:38.000000 autopep8-2.1.1/pyproject.toml
+-rw-r--r--   0 hideohattori   (501) staff       (20)       67 2024-05-22 12:08:38.036055 autopep8-2.1.1/setup.cfg
+drwxr-xr-x   0 hideohattori   (501) staff       (20)        0 2024-05-22 12:08:38.035144 autopep8-2.1.1/test/
+-rw-r--r--   0 hideohattori   (501) staff       (20)        0 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/__init__.py
+-rwxr-xr-x   0 hideohattori   (501) staff       (20)     8844 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/acid.py
+-rw-r--r--   0 hideohattori   (501) staff       (20)       27 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/bad_encoding.py
+-rw-r--r--   0 hideohattori   (501) staff       (20)       30 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/bad_encoding2.py
+-rw-r--r--   0 hideohattori   (501) staff       (20)    44753 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/e101_example.py
+-rw-r--r--   0 hideohattori   (501) staff       (20)     2190 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/example.py
+drwxr-xr-x   0 hideohattori   (501) staff       (20)        0 2024-05-22 12:08:38.035356 autopep8-2.1.1/test/fake_configuration/
+-rw-r--r--   0 hideohattori   (501) staff       (20)       21 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/fake_configuration/.pep8
+drwxr-xr-x   0 hideohattori   (501) staff       (20)        0 2024-05-22 12:08:38.035478 autopep8-2.1.1/test/fake_pycodestyle_configuration/
+-rw-r--r--   0 hideohattori   (501) staff       (20)       35 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/fake_pycodestyle_configuration/tox.ini
+-rw-r--r--   0 hideohattori   (501) staff       (20)       29 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/iso_8859_1.py
+-rwxr-xr-x   0 hideohattori   (501) staff       (20)   250373 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/test_autopep8.py
+-rwxr-xr-x   0 hideohattori   (501) staff       (20)     2939 2024-04-14 12:52:47.000000 autopep8-2.1.1/test/test_suite.py
+-rw-r--r--   0 hideohattori   (501) staff       (20)      291 2024-04-14 12:52:47.000000 autopep8-2.1.1/tox.ini
```

### Comparing `autopep8-2.1.0/AUTHORS.rst` & `autopep8-2.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/LICENSE` & `autopep8-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/MANIFEST.in` & `autopep8-2.1.1/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 include AUTHORS.rst
 include LICENSE
 include README.rst
 include test/__init__.py
+include test/acid.py
 include test/bad_encoding.py
 include test/bad_encoding2.py
 include test/e101_example.py
 include test/example
 include test/example/x.py
 include test/example.py
 include test/iso_8859_1.py
@@ -18,13 +19,12 @@
 exclude CONTRIBUTING.rst
 exclude Makefile
 exclude coveralls.bash
 exclude hooks
 exclude hooks/pre-push
 exclude install_hooks.bash
 exclude test/.gitignore
-exclude test/acid.py
 exclude test/acid_pypi.py
 exclude test/suite
 exclude test/suite/out
 exclude test/vim_autopep8.py
 exclude update_readme.py
```

### Comparing `autopep8-2.1.0/PKG-INFO` & `autopep8-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopep8
-Version: 2.1.0
+Version: 2.1.1
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide
 Author-email: Hideo Hattori <hhatto.jp@gmail.com>
 Project-URL: Repository, https://github.com/hhatto/autopep8
 Keywords: automation,pep8,format,pycodestyle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `autopep8-2.1.0/README.rst` & `autopep8-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/autopep8.egg-info/PKG-INFO` & `autopep8-2.1.1/autopep8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopep8
-Version: 2.1.0
+Version: 2.1.1
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide
 Author-email: Hideo Hattori <hhatto.jp@gmail.com>
 Project-URL: Repository, https://github.com/hhatto/autopep8
 Keywords: automation,pep8,format,pycodestyle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `autopep8-2.1.0/autopep8.egg-info/SOURCES.txt` & `autopep8-2.1.1/autopep8.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 autopep8.egg-info/PKG-INFO
 autopep8.egg-info/SOURCES.txt
 autopep8.egg-info/dependency_links.txt
 autopep8.egg-info/entry_points.txt
 autopep8.egg-info/requires.txt
 autopep8.egg-info/top_level.txt
 test/__init__.py
+test/acid.py
 test/bad_encoding.py
 test/bad_encoding2.py
 test/e101_example.py
 test/example.py
 test/iso_8859_1.py
 test/test_autopep8.py
 test/test_suite.py
```

### Comparing `autopep8-2.1.0/autopep8.py` & `autopep8-2.1.1/autopep8.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 import argparse
 import codecs
 import collections
 import copy
 import difflib
 import fnmatch
+import importlib
 import inspect
 import io
 import itertools
 import keyword
 import locale
 import os
 import re
@@ -82,18 +83,17 @@
 import token
 import tokenize
 import warnings
 import ast
 from configparser import ConfigParser as SafeConfigParser, Error
 
 import pycodestyle
-from pycodestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -217,17 +217,14 @@
             not blank_before and
             logical_line.startswith(('def ', 'async def ')) and
             '(self' in logical_line
         ):
             yield (0, 'E301 expected 1 blank line, found 0')
 
 
-pycodestyle.register_check(extended_blank_lines)
-
-
 def continued_indentation(logical_line, tokens, indent_level, hang_closing,
                           indent_char, noqa):
     """Override pycodestyle's function to provide indentation information."""
     first_row = tokens[0][2][0]
     nrows = 1 + tokens[-1][2][0] - first_row
     if noqa or nrows == 1:
         return
@@ -411,15 +408,19 @@
         desired_indent = indent_level + 2 * DEFAULT_INDENT_SIZE
         if visual_indent:
             yield (pos, 'E129 {}'.format(desired_indent))
         else:
             yield (pos, 'E125 {}'.format(desired_indent))
 
 
+# NOTE: need reload with runpy and call twice
+#   see: https://github.com/hhatto/autopep8/issues/625
+importlib.reload(pycodestyle)
 del pycodestyle._checks['logical_line'][pycodestyle.continued_indentation]
+pycodestyle.register_check(extended_blank_lines)
 pycodestyle.register_check(continued_indentation)
 
 
 class FixPEP8(object):
 
     """Fix invalid code.
 
@@ -1089,16 +1090,19 @@
         if not logical:
             return []  # pragma: no cover
         logical_lines = logical[2]
 
         # Avoid applying this when indented.
         # https://docs.python.org/reference/compound_stmts.html
         for line in logical_lines:
-            if (result['id'] == 'E702' and ':' in line
-                    and STARTSWITH_INDENT_STATEMENT_REGEX.match(line)):
+            if (
+                result['id'] == 'E702'
+                and ':' in line
+                and pycodestyle.STARTSWITH_INDENT_STATEMENT_REGEX.match(line)
+            ):
                 if self.options.verbose:
                     print(
                         '---> avoid fixing {error} with '
                         'other compound statements'.format(error=result['id']),
                         file=sys.stderr
                     )
                 return []
```

### Comparing `autopep8-2.1.0/pyproject.toml` & `autopep8-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/test/e101_example.py` & `autopep8-2.1.1/test/e101_example.py`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/test/example.py` & `autopep8-2.1.1/test/example.py`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/test/test_autopep8.py` & `autopep8-2.1.1/test/test_autopep8.py`

 * *Files identical despite different names*

### Comparing `autopep8-2.1.0/test/test_suite.py` & `autopep8-2.1.1/test/test_suite.py`

 * *Files identical despite different names*

