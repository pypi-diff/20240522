# Comparing `tmp/timeout_sampler-0.0.8.tar.gz` & `tmp/timeout_sampler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeout_sampler-0.0.8.tar", max compression
+gzip compressed data, was "timeout_sampler-0.0.9.tar", max compression
```

## Comparing `timeout_sampler-0.0.8.tar` & `timeout_sampler-0.0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      491 2024-02-15 13:56:12.196603 timeout_sampler-0.0.8/README.md
--rw-r--r--   0        0        0     1339 2024-02-15 13:56:16.593566 timeout_sampler-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7294 2024-02-15 13:56:12.197603 timeout_sampler-0.0.8/timeout_sampler/__init__.py
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 timeout_sampler-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      491 2024-02-20 09:22:13.770832 timeout_sampler-0.0.9/README.md
+-rw-r--r--   0        0        0     1339 2024-02-20 09:22:18.427783 timeout_sampler-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7294 2024-02-20 09:22:13.771832 timeout_sampler-0.0.9/timeout_sampler/__init__.py
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 timeout_sampler-0.0.9/PKG-INFO
```

### Comparing `timeout_sampler-0.0.8/pyproject.toml` & `timeout_sampler-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "timeout-sampler"
-version = "0.0.8"
+version = "0.0.9"
 description = "Timeout utility class to wait for any function output and interact with it in given time"
 authors = ["Meni Yakove <myakove@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/RedHatQE/timeout-sampler"
 documentation = "https://github.com/RedHatQE/timeout-sampler"
 packages = [{ include = "timeout_sampler" }]
```

### Comparing `timeout_sampler-0.0.8/timeout_sampler/__init__.py` & `timeout_sampler-0.0.9/timeout_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `timeout_sampler-0.0.8/PKG-INFO` & `timeout_sampler-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeout-sampler
-Version: 0.0.8
+Version: 0.0.9
 Summary: Timeout utility class to wait for any function output and interact with it in given time
 Home-page: https://github.com/RedHatQE/timeout-sampler
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

