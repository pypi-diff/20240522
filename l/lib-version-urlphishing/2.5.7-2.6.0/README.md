# Comparing `tmp/lib_version_urlphishing-2.5.7.tar.gz` & `tmp/lib_version_urlphishing-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.5.7.tar", max compression
+gzip compressed data, was "lib_version_urlphishing-2.6.0.tar", max compression
```

## Comparing `lib_version_urlphishing-2.5.7.tar` & `lib_version_urlphishing-2.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2024-05-22 19:23:45.310305 lib_version_urlphishing-2.5.7/README.md
--rw-r--r--   0        0        0        0 2024-05-22 19:23:45.310305 lib_version_urlphishing-2.5.7/lib_version_URLPhishing/__init__.py
--rw-r--r--   0        0        0       22 2024-05-22 19:23:45.578309 lib_version_urlphishing-2.5.7/lib_version_URLPhishing/version.py
--rw-r--r--   0        0        0      337 2024-05-22 19:23:45.314305 lib_version_urlphishing-2.5.7/lib_version_URLPhishing/version_util.py
--rw-r--r--   0        0        0      843 2024-05-22 19:24:01.050522 lib_version_urlphishing-2.5.7/pyproject.toml
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.5.7/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-05-22 19:40:41.193661 lib_version_urlphishing-2.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 19:40:41.193661 lib_version_urlphishing-2.6.0/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-22 19:40:41.449661 lib_version_urlphishing-2.6.0/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      337 2024-05-22 19:40:41.193661 lib_version_urlphishing-2.6.0/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      843 2024-05-22 19:40:55.285672 lib_version_urlphishing-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.6.0/PKG-INFO
```

### Comparing `lib_version_urlphishing-2.5.7/pyproject.toml` & `lib_version_urlphishing-2.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-version-urlphishing"
-version = "2.5.7"
+version = "2.6.0"
 description = "A library to manage and track versions of software components"
 authors = ["Marianna Louizidou <M.Louizidou@student.tudelft.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `lib_version_urlphishing-2.5.7/PKG-INFO` & `lib_version_urlphishing-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-version-urlphishing
-Version: 2.5.7
+Version: 2.6.0
 Summary: A library to manage and track versions of software components
 License: Apache-2.0
 Author: Marianna Louizidou
 Author-email: M.Louizidou@student.tudelft.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

