# Comparing `tmp/quri_parts_stim-0.9.2.tar.gz` & `tmp/quri_parts_stim-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_stim-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_stim-17.0.0.tar", max compression
```

## Comparing `quri_parts_stim-0.9.2.tar` & `quri_parts_stim-17.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/LICENSE
--rw-r--r--   0        0        0      341 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/README.md
--rw-r--r--   0        0        0     1139 2023-03-29 07:37:35.603031 quri_parts_stim-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:34.823027 quri_parts_stim-0.9.2/quri_parts/stim/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/quri_parts/stim/__init__.py
--rw-r--r--   0        0        0     3519 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/quri_parts/stim/circuit/__init__.py
--rw-r--r--   0        0        0     4619 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/quri_parts/stim/estimator/__init__.py
--rw-r--r--   0        0        0     2036 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/quri_parts/stim/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/quri_parts/stim/py.typed
--rw-r--r--   0        0        0     2646 2023-03-29 07:37:19.878951 quri_parts_stim-0.9.2/quri_parts/stim/sampler/__init__.py
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 quri_parts_stim-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/LICENSE
+-rw-r--r--   0        0        0      341 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/README.md
+-rw-r--r--   0        0        0     1141 2024-03-19 02:11:33.733985 quri_parts_stim-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:33.121988 quri_parts_stim-17.0.0/quri_parts/stim/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/__init__.py
+-rw-r--r--   0        0        0     3519 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/circuit/__init__.py
+-rw-r--r--   0        0        0     4619 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/estimator/__init__.py
+-rw-r--r--   0        0        0     2036 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/operator/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/py.typed
+-rw-r--r--   0        0        0     2646 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/sampler/__init__.py
+-rw-r--r--   0        0        0     2342 2024-03-19 02:11:01.306138 quri_parts_stim-17.0.0/quri_parts/stim/simulator.py
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 quri_parts_stim-17.0.0/PKG-INFO
```

### Comparing `quri_parts_stim-0.9.2/LICENSE` & `quri_parts_stim-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_stim-0.9.2/pyproject.toml` & `quri_parts_stim-17.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-stim"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use Stim with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
@@ -24,15 +24,15 @@
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
 python = "^3.9.8"
 quri-parts-circuit = "*"
 quri-parts-core = "*"
-stim = "^1.9.0"
+stim = "^1.11.0"
 
 [tool.poetry.group.dev.dependencies]
 quri-parts-circuit = {path = "../circuit", develop = true}
 quri-parts-core = {path = "../core", develop = true}
 
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
```

### Comparing `quri_parts_stim-0.9.2/quri_parts/stim/circuit/__init__.py` & `quri_parts_stim-17.0.0/quri_parts/stim/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_stim-0.9.2/quri_parts/stim/estimator/__init__.py` & `quri_parts_stim-17.0.0/quri_parts/stim/estimator/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_stim-0.9.2/quri_parts/stim/operator/__init__.py` & `quri_parts_stim-17.0.0/quri_parts/stim/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_stim-0.9.2/quri_parts/stim/sampler/__init__.py` & `quri_parts_stim-17.0.0/quri_parts/stim/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_stim-0.9.2/PKG-INFO` & `quri_parts_stim-17.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-stim
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use Stim with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Dist: quri-parts-circuit
 Requires-Dist: quri-parts-core
-Requires-Dist: stim (>=1.9.0,<2.0.0)
+Requires-Dist: stim (>=1.11.0,<2.0.0)
 Project-URL: Documentation, https://quri-parts.qunasys.com
 Project-URL: Repository, https://github.com/QunaSys/quri-parts
 Description-Content-Type: text/markdown
 
 # QURI Parts Stim
 
 QURI Parts Stim is a support library for using Stim with QURI Parts.
```

