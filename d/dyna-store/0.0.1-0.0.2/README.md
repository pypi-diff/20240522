# Comparing `tmp/dyna_store-0.0.1.tar.gz` & `tmp/dyna_store-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyna_store-0.0.1.tar", max compression
+gzip compressed data, was "dyna_store-0.0.2.tar", max compression
```

## Comparing `dyna_store-0.0.1.tar` & `dyna_store-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-21 16:50:56.834085 dyna_store-0.0.1/LICENSE
--rw-r--r--   0        0        0      650 2024-05-21 16:50:56.834085 dyna_store-0.0.1/README.md
--rw-r--r--   0        0        0       92 2024-05-21 16:50:56.834085 dyna_store-0.0.1/dyna_store/__init__.py
--rw-r--r--   0        0        0      733 2024-05-21 16:50:56.834085 dyna_store-0.0.1/dyna_store/inmemory.py
--rw-r--r--   0        0        0     5717 2024-05-21 16:50:56.834085 dyna_store-0.0.1/dyna_store/main.py
--rw-r--r--   0        0        0     1118 2024-05-21 16:50:56.838085 dyna_store-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 dyna_store-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-22 12:51:53.015893 dyna_store-0.0.2/LICENSE
+-rw-r--r--   0        0        0      650 2024-05-22 12:51:53.015893 dyna_store-0.0.2/README.md
+-rw-r--r--   0        0        0       92 2024-05-22 12:51:53.015893 dyna_store-0.0.2/dyna_store/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-22 12:51:53.015893 dyna_store-0.0.2/dyna_store/inmemory.py
+-rw-r--r--   0        0        0     5717 2024-05-22 12:51:53.015893 dyna_store-0.0.2/dyna_store/main.py
+-rw-r--r--   0        0        0     1114 2024-05-22 12:51:53.015893 dyna_store-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 dyna_store-0.0.2/PKG-INFO
```

### Comparing `dyna_store-0.0.1/LICENSE` & `dyna_store-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.1/README.md` & `dyna_store-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.1/dyna_store/inmemory.py` & `dyna_store-0.0.2/dyna_store/inmemory.py`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.1/dyna_store/main.py` & `dyna_store-0.0.2/dyna_store/main.py`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.1/pyproject.toml` & `dyna_store-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "dyna-store"
-version = "0.0.1"
+version = "0.0.2"
 description = "Dynamic metadata storage"
 authors = ["brightnetwork <dev@brightnetwork.co.uk>"]
 repository = "https://github.com/brightnetwork/dyna-store"
 homepage = "https://github.com/brightnetwork/dyna-store"
 documentation = "https://github.com/brightnetwork/dyna-store"
 keywords = ["id", "meta", "store", "high-cardinality", "metadata"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
-pydantic = "^2.7.1"
+pydantic = "^2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pyright = "^1.1.355"
 pytest-cov = "^4.1.0"
```

### Comparing `dyna_store-0.0.1/PKG-INFO` & `dyna_store-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dyna-store
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dynamic metadata storage
 Home-page: https://github.com/brightnetwork/dyna-store
 License: MIT
 Keywords: id,meta,store,high-cardinality,metadata
 Author: brightnetwork
 Author-email: dev@brightnetwork.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: pydantic (>=2,<3)
 Project-URL: Documentation, https://github.com/brightnetwork/dyna-store
 Project-URL: Repository, https://github.com/brightnetwork/dyna-store
 Description-Content-Type: text/markdown
 
 [![image](https://img.shields.io/pypi/v/dyna-store.svg)](https://pypi.python.org/pypi/dyna-store)
 [![image](https://img.shields.io/pypi/l/dyna-store.svg)](https://pypi.python.org/pypi/dyna-store)
 [![image](https://img.shields.io/pypi/pyversions/dyna-store.svg)](https://pypi.python.org/pypi/dyna-store)
```

