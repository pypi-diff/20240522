# Comparing `tmp/lib_version_urlphishing-2.5.4.tar.gz` & `tmp/lib_version_urlphishing-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.5.4.tar", max compression
+gzip compressed data, was "lib_version_urlphishing-2.5.7.tar", max compression
```

## Comparing `lib_version_urlphishing-2.5.4.tar` & `lib_version_urlphishing-2.5.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2024-05-22 19:00:29.652028 lib_version_urlphishing-2.5.4/README.md
--rw-r--r--   0        0        0        0 2024-05-22 19:00:29.652028 lib_version_urlphishing-2.5.4/lib_version_URLPhishing/__init__.py
--rw-r--r--   0        0        0       22 2024-05-22 19:00:29.912028 lib_version_urlphishing-2.5.4/lib_version_URLPhishing/version.py
--rw-r--r--   0        0        0      337 2024-05-22 19:00:29.652028 lib_version_urlphishing-2.5.4/lib_version_URLPhishing/version_util.py
--rw-r--r--   0        0        0      827 2024-05-22 19:00:45.124048 lib_version_urlphishing-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-05-22 19:23:45.310305 lib_version_urlphishing-2.5.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 19:23:45.310305 lib_version_urlphishing-2.5.7/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-22 19:23:45.578309 lib_version_urlphishing-2.5.7/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      337 2024-05-22 19:23:45.314305 lib_version_urlphishing-2.5.7/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      843 2024-05-22 19:24:01.050522 lib_version_urlphishing-2.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.5.7/PKG-INFO
```

### Comparing `lib_version_urlphishing-2.5.4/pyproject.toml` & `lib_version_urlphishing-2.5.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-version-urlphishing"
-version = "2.5.4"
+version = "2.5.7"
 description = "A library to manage and track versions of software components"
 authors = ["Marianna Louizidou <M.Louizidou@student.tudelft.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 
 
 
@@ -21,11 +21,12 @@
 Homepage = "https://github.com/REMLA24-TEAM-15/lib-version"
 Issues = "https://github.com/REMLA24-TEAM-15/lib-version/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 flake8 = "^3.9"
+pdoc = "14.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lib_version_urlphishing-2.5.4/PKG-INFO` & `lib_version_urlphishing-2.5.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lib-version-urlphishing
-Version: 2.5.4
+Version: 2.5.7
 Summary: A library to manage and track versions of software components
 License: Apache-2.0
 Author: Marianna Louizidou
 Author-email: M.Louizidou@student.tudelft.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flake8 (>=3.9,<4.0)
+Requires-Dist: pdoc (==14.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Homepage, https://github.com/REMLA24-TEAM-15/lib-version
 Project-URL: Issues, https://github.com/REMLA24-TEAM-15/lib-version/issues
 Description-Content-Type: text/markdown
 
 lib_version_URLPhishing is a version-aware library that can can be asked for the version of the library.
```

