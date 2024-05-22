# Comparing `tmp/jeeves_shell-2.3.2.tar.gz` & `tmp/jeeves_shell-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.3.2.tar", max compression
+gzip compressed data, was "jeeves_shell-2.3.3.tar", max compression
```

## Comparing `jeeves_shell-2.3.2.tar` & `jeeves_shell-2.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2030 2023-11-04 21:23:57.440241 jeeves_shell-2.3.2/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.3.2/jeeves_shell/__init__.py
--rw-r--r--   0        0        0     1314 2023-11-05 21:49:27.161312 jeeves_shell-2.3.2/jeeves_shell/cli.py
--rw-r--r--   0        0        0     4795 2023-09-08 10:23:09.998753 jeeves_shell-2.3.2/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.3.2/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0     1942 2023-11-05 21:49:27.161312 jeeves_shell-2.3.2/jeeves_shell/errors.py
--rw-r--r--   0        0        0      255 2023-09-07 14:40:21.896746 jeeves_shell-2.3.2/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.3.2/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1910 2023-11-05 21:49:27.161312 jeeves_shell-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 jeeves_shell-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2030 2024-05-22 18:46:26.830986 jeeves_shell-2.3.3/README.md
+-rw-r--r--   0        0        0       39 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0     1314 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     4795 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0     1942 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      255 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2024-05-22 18:46:26.842984 jeeves_shell-2.3.3/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1903 2024-05-22 19:40:42.923648 jeeves_shell-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 jeeves_shell-2.3.3/PKG-INFO
```

### Comparing `jeeves_shell-2.3.2/README.md` & `jeeves_shell-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.3.2/jeeves_shell/cli.py` & `jeeves_shell-2.3.3/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.3.2/jeeves_shell/discover.py` & `jeeves_shell-2.3.3/jeeves_shell/discover.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.3.2/jeeves_shell/errors.py` & `jeeves_shell-2.3.3/jeeves_shell/errors.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.3.2/pyproject.toml` & `jeeves_shell-2.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jeeves-shell"
 description = "Pythonic replacement for GNU Make"
-version = "2.3.2"
+version = "2.3.3"
 license = "MIT"
 
 authors = []
 
 readme = "README.md"
 
 repository = "https://github.com/jeeves-sh/jeeves-shell"
@@ -27,19 +27,19 @@
 
 [tool.poetry.scripts]
 j = "jeeves_shell.cli:app"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-typer = "^0.9.0"
-documented = "^0.1.4"
-funcy = "^2.0"
-rich = {version = "^13.3.5"}
-sh = {version = "^2.0.4", optional = true}
+typer = ">=0.9.0"
+documented = ">=0.1.4"
+funcy = ">=2.0"
+rich = ">=13.3.5"
+sh = {version = ">=2.0.4", optional = true}
 
 [tool.poetry.extras]
 all = ["sh"]
 
 [tool.poetry.group.dev.dependencies]
 m2r2 = "^0.2"
 mkdocstrings = "^0.19.1"
```

### Comparing `jeeves_shell-2.3.2/PKG-INFO` & `jeeves_shell-2.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: jeeves-shell
-Version: 2.3.2
+Version: 2.3.3
 Summary: Pythonic replacement for GNU Make
 Home-page: https://github.com/jeeves-sh/jeeves-shell
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
-Requires-Dist: documented (>=0.1.4,<0.2.0)
-Requires-Dist: funcy (>=2.0,<3.0)
-Requires-Dist: rich (>=13.3.5,<14.0.0)
-Requires-Dist: sh (>=2.0.4,<3.0.0) ; extra == "all"
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: documented (>=0.1.4)
+Requires-Dist: funcy (>=2.0)
+Requires-Dist: rich (>=13.3.5)
+Requires-Dist: sh (>=2.0.4) ; extra == "all"
+Requires-Dist: typer (>=0.9.0)
 Project-URL: Repository, https://github.com/jeeves-sh/jeeves-shell
 Description-Content-Type: text/markdown
 
 # Jeeves Shell
 
 [![Build Status](https://github.com/jeeves-sh/jeeves-shell/workflows/test/badge.svg?branch=master&event=push)](https://github.com/jeeves-sh/jeeves-shell/actions?query=workflow%3Atest)
 [![codecov](https://codecov.io/gh/jeeves-sh/jeeves-shell/branch/master/graph/badge.svg)](https://codecov.io/gh/jeeves-sh/jeeves-shell)
```

