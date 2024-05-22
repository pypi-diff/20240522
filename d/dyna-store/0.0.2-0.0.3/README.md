# Comparing `tmp/dyna_store-0.0.2.tar.gz` & `tmp/dyna_store-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyna_store-0.0.2.tar", max compression
+gzip compressed data, was "dyna_store-0.0.3.tar", max compression
```

## Comparing `dyna_store-0.0.2.tar` & `dyna_store-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-22 12:51:53.015893 dyna_store-0.0.2/LICENSE
--rw-r--r--   0        0        0      650 2024-05-22 12:51:53.015893 dyna_store-0.0.2/README.md
--rw-r--r--   0        0        0       92 2024-05-22 12:51:53.015893 dyna_store-0.0.2/dyna_store/__init__.py
--rw-r--r--   0        0        0      733 2024-05-22 12:51:53.015893 dyna_store-0.0.2/dyna_store/inmemory.py
--rw-r--r--   0        0        0     5717 2024-05-22 12:51:53.015893 dyna_store-0.0.2/dyna_store/main.py
--rw-r--r--   0        0        0     1114 2024-05-22 12:51:53.015893 dyna_store-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 dyna_store-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-22 12:59:45.062490 dyna_store-0.0.3/LICENSE
+-rw-r--r--   0        0        0      650 2024-05-22 12:59:45.062490 dyna_store-0.0.3/README.md
+-rw-r--r--   0        0        0       92 2024-05-22 12:59:45.062490 dyna_store-0.0.3/dyna_store/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-22 12:59:45.062490 dyna_store-0.0.3/dyna_store/inmemory.py
+-rw-r--r--   0        0        0     5717 2024-05-22 12:59:45.062490 dyna_store-0.0.3/dyna_store/main.py
+-rw-r--r--   0        0        0     1112 2024-05-22 12:59:45.062490 dyna_store-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 dyna_store-0.0.3/PKG-INFO
```

### Comparing `dyna_store-0.0.2/LICENSE` & `dyna_store-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.2/README.md` & `dyna_store-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.2/dyna_store/inmemory.py` & `dyna_store-0.0.3/dyna_store/inmemory.py`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.2/dyna_store/main.py` & `dyna_store-0.0.3/dyna_store/main.py`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.2/pyproject.toml` & `dyna_store-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "dyna-store"
-version = "0.0.2"
+version = "0.0.3"
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
-numpy = "^1.26.4"
+numpy = "^1.22"
 pydantic = "^2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pyright = "^1.1.355"
```

### Comparing `dyna_store-0.0.2/PKG-INFO` & `dyna_store-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dyna-store
-Version: 0.0.2
+Version: 0.0.3
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
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pydantic (>=2,<3)
 Project-URL: Documentation, https://github.com/brightnetwork/dyna-store
 Project-URL: Repository, https://github.com/brightnetwork/dyna-store
 Description-Content-Type: text/markdown
 
 [![image](https://img.shields.io/pypi/v/dyna-store.svg)](https://pypi.python.org/pypi/dyna-store)
 [![image](https://img.shields.io/pypi/l/dyna-store.svg)](https://pypi.python.org/pypi/dyna-store)
```

