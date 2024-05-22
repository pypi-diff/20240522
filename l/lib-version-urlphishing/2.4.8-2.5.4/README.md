# Comparing `tmp/lib_version_urlphishing-2.4.8.tar.gz` & `tmp/lib_version_urlphishing-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.4.8.tar", max compression
+gzip compressed data, was "lib_version_urlphishing-2.5.4.tar", max compression
```

## Comparing `lib_version_urlphishing-2.4.8.tar` & `lib_version_urlphishing-2.5.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2024-05-21 19:11:37.808376 lib_version_urlphishing-2.4.8/README.md
--rw-r--r--   0        0        0        0 2024-05-21 19:11:37.808376 lib_version_urlphishing-2.4.8/lib_version_URLPhishing/__init__.py
--rw-r--r--   0        0        0       22 2024-05-21 19:11:38.076376 lib_version_urlphishing-2.4.8/lib_version_URLPhishing/version.py
--rw-r--r--   0        0        0      337 2024-05-21 19:11:37.808376 lib_version_urlphishing-2.4.8/lib_version_URLPhishing/version_util.py
--rw-r--r--   0        0        0      827 2024-05-21 19:11:57.312391 lib_version_urlphishing-2.4.8/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-05-22 19:00:29.652028 lib_version_urlphishing-2.5.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 19:00:29.652028 lib_version_urlphishing-2.5.4/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-22 19:00:29.912028 lib_version_urlphishing-2.5.4/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      337 2024-05-22 19:00:29.652028 lib_version_urlphishing-2.5.4/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      827 2024-05-22 19:00:45.124048 lib_version_urlphishing-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.5.4/PKG-INFO
```

### Comparing `lib_version_urlphishing-2.4.8/pyproject.toml` & `lib_version_urlphishing-2.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-version-urlphishing"
-version = "2.4.8"
+version = "2.5.4"
 description = "A library to manage and track versions of software components"
 authors = ["Marianna Louizidou <M.Louizidou@student.tudelft.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `lib_version_urlphishing-2.4.8/PKG-INFO` & `lib_version_urlphishing-2.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-version-urlphishing
-Version: 2.4.8
+Version: 2.5.4
 Summary: A library to manage and track versions of software components
 License: Apache-2.0
 Author: Marianna Louizidou
 Author-email: M.Louizidou@student.tudelft.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

