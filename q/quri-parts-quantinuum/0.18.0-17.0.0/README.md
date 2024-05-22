# Comparing `tmp/quri_parts_quantinuum-0.18.0.tar.gz` & `tmp/quri_parts_quantinuum-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_quantinuum-0.18.0.tar", max compression
+gzip compressed data, was "quri_parts_quantinuum-17.0.0.tar", max compression
```

## Comparing `quri_parts_quantinuum-0.18.0.tar` & `quri_parts_quantinuum-17.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/LICENSE
--rw-r--r--   0        0        0      276 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/README.md
--rw-r--r--   0        0        0     1134 2024-05-22 06:07:55.207469 quri_parts_quantinuum-0.18.0/pyproject.toml
--rw-r--r--   0        0        0       34 2024-05-22 06:07:54.559477 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/NOTICE
--rw-r--r--   0        0        0        0 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/__init__.py
--rw-r--r--   0        0        0      621 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/__init__.py
--rw-r--r--   0        0        0      651 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/gate_names.py
--rw-r--r--   0        0        0     2867 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/gates.py
--rw-r--r--   0        0        0     1794 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/transpile/__init__.py
--rw-r--r--   0        0        0     6901 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py
--rw-r--r--   0        0        0        0 2024-05-22 06:07:18.871923 quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/py.typed
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 quri_parts_quantinuum-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/LICENSE
+-rw-r--r--   0        0        0      276 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/README.md
+-rw-r--r--   0        0        0     1134 2024-03-19 02:11:32.353992 quri_parts_quantinuum-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:31.765995 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/__init__.py
+-rw-r--r--   0        0        0      621 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/__init__.py
+-rw-r--r--   0        0        0      651 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/gate_names.py
+-rw-r--r--   0        0        0     2867 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/gates.py
+-rw-r--r--   0        0        0     1794 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     6901 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.302138 quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/py.typed
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 quri_parts_quantinuum-17.0.0/PKG-INFO
```

### Comparing `quri_parts_quantinuum-0.18.0/LICENSE` & `quri_parts_quantinuum-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.18.0/pyproject.toml` & `quri_parts_quantinuum-17.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-quantinuum"
-version = "0.18.0"
+version = "17.0.0"
 description = "A plugin to use Quantinuum with QIRI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <support@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/__init__.py` & `quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/gate_names.py` & `quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/gate_names.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/gates.py` & `quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/transpile/__init__.py` & `quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.18.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py` & `quri_parts_quantinuum-17.0.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.18.0/PKG-INFO` & `quri_parts_quantinuum-17.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-quantinuum
-Version: 0.18.0
+Version: 17.0.0
 Summary: A plugin to use Quantinuum with QIRI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: support@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

