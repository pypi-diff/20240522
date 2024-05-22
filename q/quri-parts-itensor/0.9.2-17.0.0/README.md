# Comparing `tmp/quri_parts_itensor-0.9.2.tar.gz` & `tmp/quri_parts_itensor-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_itensor-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_itensor-17.0.0.tar", max compression
```

## Comparing `quri_parts_itensor-0.9.2.tar` & `quri_parts_itensor-17.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      443 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/README.md
--rw-r--r--   0        0        0     1156 2023-03-29 07:37:30.087001 quri_parts_itensor-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:29.306997 quri_parts_itensor-0.9.2/quri_parts/itensor/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/__init__.py
--rw-r--r--   0        0        0     4661 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/circuit/__init__.py
--rw-r--r--   0        0        0     6404 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/estimator.py
--rw-r--r--   0        0        0     3772 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/library.jl
--rw-r--r--   0        0        0      431 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/load_itensor.py
--rw-r--r--   0        0        0     1241 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/py.typed
--rw-r--r--   0        0        0     2364 2023-03-29 07:37:19.870951 quri_parts_itensor-0.9.2/quri_parts/itensor/sampler.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 quri_parts_itensor-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      443 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/README.md
+-rw-r--r--   0        0        0     1157 2024-03-19 02:11:28.938010 quri_parts_itensor-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:28.346013 quri_parts_itensor-17.0.0/quri_parts/itensor/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/__init__.py
+-rw-r--r--   0        0        0     5778 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/circuit/__init__.py
+-rw-r--r--   0        0        0    10851 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/estimator.py
+-rw-r--r--   0        0        0     3772 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/library.jl
+-rw-r--r--   0        0        0     1125 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/load_itensor.py
+-rw-r--r--   0        0        0     1783 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/operator/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/py.typed
+-rw-r--r--   0        0        0     4719 2024-03-19 02:11:01.294138 quri_parts_itensor-17.0.0/quri_parts/itensor/sampler.py
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 quri_parts_itensor-17.0.0/PKG-INFO
```

### Comparing `quri_parts_itensor-0.9.2/pyproject.toml` & `quri_parts_itensor-17.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-itensor"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use ITensor with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_itensor-0.9.2/quri_parts/itensor/library.jl` & `quri_parts_itensor-17.0.0/quri_parts/itensor/library.jl`

 * *Files identical despite different names*

### Comparing `quri_parts_itensor-0.9.2/PKG-INFO` & `quri_parts_itensor-17.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-itensor
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use ITensor with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

