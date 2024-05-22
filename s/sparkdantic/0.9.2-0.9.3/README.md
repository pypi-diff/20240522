# Comparing `tmp/sparkdantic-0.9.2.tar.gz` & `tmp/sparkdantic-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkdantic-0.9.2.tar", max compression
+gzip compressed data, was "sparkdantic-0.9.3.tar", max compression
```

## Comparing `sparkdantic-0.9.2.tar` & `sparkdantic-0.9.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3187 2023-09-11 09:29:06.289857 sparkdantic-0.9.2/README.md
--rw-r--r--   0        0        0     1142 2023-09-11 09:29:06.289857 sparkdantic-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      184 2023-09-11 09:29:06.293857 sparkdantic-0.9.2/src/sparkdantic/__init__.py
--rw-r--r--   0        0        0     2093 2023-09-11 09:29:06.293857 sparkdantic-0.9.2/src/sparkdantic/generation.py
--rw-r--r--   0        0        0    10033 2023-09-11 09:29:06.293857 sparkdantic-0.9.2/src/sparkdantic/model.py
--rw-r--r--   0        0        0     3898 1970-01-01 00:00:00.000000 sparkdantic-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3187 2023-09-12 09:42:01.446117 sparkdantic-0.9.3/README.md
+-rw-r--r--   0        0        0     1142 2023-09-12 09:42:01.446117 sparkdantic-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-09-12 09:42:01.446117 sparkdantic-0.9.3/src/sparkdantic/__init__.py
+-rw-r--r--   0        0        0     4095 2023-09-12 09:42:01.446117 sparkdantic-0.9.3/src/sparkdantic/generation.py
+-rw-r--r--   0        0        0    10033 2023-09-12 09:42:01.446117 sparkdantic-0.9.3/src/sparkdantic/model.py
+-rw-r--r--   0        0        0     3898 1970-01-01 00:00:00.000000 sparkdantic-0.9.3/PKG-INFO
```

### Comparing `sparkdantic-0.9.2/README.md` & `sparkdantic-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ##  SparkDantic
 
 [![codecov](https://codecov.io/gh/mitchelllisle/sparkdantic/graph/badge.svg?token=O6PPQX4FEX)](https://codecov.io/gh/mitchelllisle/sparkdantic)
 [![PyPI version](https://badge.fury.io/py/sparkdantic.svg)](https://badge.fury.io/py/sparkdantic)
 
-> 1️⃣ version: 0.9.2
+> 1️⃣ version: 0.9.3
 
 > ✍️ author: Mitchell Lisle
 
 # PySpark Model Conversion Tool
 
 This Python module provides a utility for converting Pydantic models to PySpark schemas. It's implemented as a class 
 named `SparkModel` that extends the Pydantic's `BaseModel`.
```

### Comparing `sparkdantic-0.9.2/pyproject.toml` & `sparkdantic-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkdantic"
-version = "0.9.2"
+version = "0.9.3"
 description = "A pydantic -> spark schema library"
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sparkdantic", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9,<4.0.0"
@@ -30,15 +30,15 @@
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.4"
 mkdocs-gen-files = ">=0.4,<0.6"
 mkdocs-literate-nav = "^0.6.0"
-mkdocstrings = {extras = ["python"], version = ">=0.20,<0.23"}
+mkdocstrings = {extras = ["python"], version = ">=0.20,<0.24"}
 mkautodoc = "^0.2.0"
 pymdown-extensions = "^10.0.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-dotenv = "^0.5.2"
```

### Comparing `sparkdantic-0.9.2/src/sparkdantic/model.py` & `sparkdantic-0.9.3/src/sparkdantic/model.py`

 * *Files identical despite different names*

### Comparing `sparkdantic-0.9.2/PKG-INFO` & `sparkdantic-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdantic
-Version: 0.9.2
+Version: 0.9.3
 Summary: A pydantic -> spark schema library
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 
 ##  SparkDantic
 
 [![codecov](https://codecov.io/gh/mitchelllisle/sparkdantic/graph/badge.svg?token=O6PPQX4FEX)](https://codecov.io/gh/mitchelllisle/sparkdantic)
 [![PyPI version](https://badge.fury.io/py/sparkdantic.svg)](https://badge.fury.io/py/sparkdantic)
 
-> 1️⃣ version: 0.9.2
+> 1️⃣ version: 0.9.3
 
 > ✍️ author: Mitchell Lisle
 
 # PySpark Model Conversion Tool
 
 This Python module provides a utility for converting Pydantic models to PySpark schemas. It's implemented as a class 
 named `SparkModel` that extends the Pydantic's `BaseModel`.
```

