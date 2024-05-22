# Comparing `tmp/keep_screen_alive-0.0.4.tar.gz` & `tmp/keep_screen_alive-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keep_screen_alive-0.0.4.tar", max compression
+gzip compressed data, was "keep_screen_alive-0.0.5.tar", max compression
```

## Comparing `keep_screen_alive-0.0.4.tar` & `keep_screen_alive-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      477 2023-06-27 19:45:21.990191 keep_screen_alive-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-07 11:46:26.196161 keep_screen_alive-0.0.4/keep_alive/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-12 18:52:51.866839 keep_screen_alive-0.0.4/keep_alive/run.py
--rw-r--r--   0        0        0      772 2023-06-27 19:47:46.877876 keep_screen_alive-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 keep_screen_alive-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      477 2023-06-27 19:45:21.990191 keep_screen_alive-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 11:46:26.196161 keep_screen_alive-0.0.5/keep_alive/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-12 18:52:51.866839 keep_screen_alive-0.0.5/keep_alive/run.py
+-rw-r--r--   0        0        0      788 2024-05-22 15:45:19.126093 keep_screen_alive-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 keep_screen_alive-0.0.5/PKG-INFO
```

### Comparing `keep_screen_alive-0.0.4/keep_alive/run.py` & `keep_screen_alive-0.0.5/keep_alive/run.py`

 * *Files identical despite different names*

### Comparing `keep_screen_alive-0.0.4/pyproject.toml` & `keep_screen_alive-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keep-screen-alive"
-version = "0.0.4"
+version = "0.0.5"
 description = "A thin wrapper around macos caffeinate to use a relative datetime"
 authors = ["Tim Willis"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "keep_alive"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -16,14 +16,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 dateparser = "^1.1.8"
+six = "^1.16.0"
 
 [tool.poetry.scripts]
 keep-alive = "keep_alive.run:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `keep_screen_alive-0.0.4/PKG-INFO` & `keep_screen_alive-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: keep-screen-alive
-Version: 0.0.4
+Version: 0.0.5
 Summary: A thin wrapper around macos caffeinate to use a relative datetime
 License: MIT
 Author: Tim Willis
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## Summary
 A simple command line wrapper for [caffeinate](https://ss64.com/osx/caffeinate.html) on macOS that provides a forward looking relative datetime interface.
 
 ## Install
```

