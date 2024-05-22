# Comparing `tmp/styxdefs-0.1.0.tar.gz` & `tmp/styxdefs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styxdefs-0.1.0.tar", max compression
+gzip compressed data, was "styxdefs-0.1.1.tar", max compression
```

## Comparing `styxdefs-0.1.0.tar` & `styxdefs-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2024-05-21 20:59:46.677555 styxdefs-0.1.0/LICENSE
--rw-r--r--   0        0        0      870 2024-05-21 20:59:46.677555 styxdefs-0.1.0/README.md
--rw-r--r--   0        0        0     1563 2024-05-21 20:59:46.681555 styxdefs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      418 2024-05-21 20:59:46.681555 styxdefs-0.1.0/src/styxdefs/__init__.py
--rw-r--r--   0        0        0     2720 2024-05-21 20:59:46.681555 styxdefs-0.1.0/src/styxdefs/runner.py
--rw-r--r--   0        0        0     2354 2024-05-21 20:59:46.681555 styxdefs-0.1.0/src/styxdefs/types.py
--rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 styxdefs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-21 21:29:50.928169 styxdefs-0.1.1/LICENSE
+-rw-r--r--   0        0        0      870 2024-05-21 21:29:50.928169 styxdefs-0.1.1/README.md
+-rw-r--r--   0        0        0     1564 2024-05-21 21:29:50.928169 styxdefs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      418 2024-05-21 21:29:50.928169 styxdefs-0.1.1/src/styxdefs/__init__.py
+-rw-r--r--   0        0        0     2720 2024-05-21 21:29:50.928169 styxdefs-0.1.1/src/styxdefs/runner.py
+-rw-r--r--   0        0        0     2354 2024-05-21 21:29:50.928169 styxdefs-0.1.1/src/styxdefs/types.py
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 styxdefs-0.1.1/PKG-INFO
```

### Comparing `styxdefs-0.1.0/LICENSE` & `styxdefs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.0/README.md` & `styxdefs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.0/pyproject.toml` & `styxdefs-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "styxdefs"
-version = "0.1.0"
+version = "0.1.1"
 description = "Styx definitions and minimal runtime"
 authors = ["Florian Rupprecht <33600480+nx10@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "styxdefs", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "~3.11"
+python = ">=3.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 mypy = "^1.10.0"
 pre-commit = "^3.7.1"
 pytest-cov = "^5.0.0"
 ruff = "^0.4.4"
```

### Comparing `styxdefs-0.1.0/src/styxdefs/runner.py` & `styxdefs-0.1.1/src/styxdefs/runner.py`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.0/src/styxdefs/types.py` & `styxdefs-0.1.1/src/styxdefs/types.py`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.0/PKG-INFO` & `styxdefs-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: styxdefs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Styx definitions and minimal runtime
 License: MIT
 Author: Florian Rupprecht
 Author-email: 33600480+nx10@users.noreply.github.com
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Styx definitions and minimal runtime
 
 [![Build](https://github.com/childmindresearch/styxdefs/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/styxdefs/actions/workflows/test.yaml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/childmindresearch/styxdefs/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/styxdefs)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

