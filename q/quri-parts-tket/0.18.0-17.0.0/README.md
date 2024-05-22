# Comparing `tmp/quri_parts_tket-0.18.0.tar.gz` & `tmp/quri_parts_tket-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_tket-0.18.0.tar", max compression
+gzip compressed data, was "quri_parts_tket-17.0.0.tar", max compression
```

## Comparing `quri_parts_tket-0.18.0.tar` & `quri_parts_tket-17.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11358 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/LICENSE
--rw-r--r--   0        0        0      341 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/README.md
--rw-r--r--   0        0        0     1103 2024-05-22 06:07:57.403442 quri_parts_tket-0.18.0/pyproject.toml
--rw-r--r--   0        0        0       34 2024-05-22 06:07:56.763450 quri_parts_tket-0.18.0/quri_parts/tket/NOTICE
--rw-r--r--   0        0        0        0 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/quri_parts/tket/__init__.py
--rw-r--r--   0        0        0      725 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/quri_parts/tket/circuit/__init__.py
--rw-r--r--   0        0        0     5581 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/quri_parts/tket/circuit/circuit_converter.py
--rw-r--r--   0        0        0     4510 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/quri_parts/tket/circuit/tket_circuit_converter.py
--rw-r--r--   0        0        0     4572 2024-05-22 06:07:18.875923 quri_parts_tket-0.18.0/quri_parts/tket/circuit/transpile/__init__.py
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 quri_parts_tket-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/LICENSE
+-rw-r--r--   0        0        0      341 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/README.md
+-rw-r--r--   0        0        0     1103 2024-03-19 02:11:34.409981 quri_parts_tket-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:33.821984 quri_parts_tket-17.0.0/quri_parts/tket/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/quri_parts/tket/__init__.py
+-rw-r--r--   0        0        0      725 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/quri_parts/tket/circuit/__init__.py
+-rw-r--r--   0        0        0     5581 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/quri_parts/tket/circuit/circuit_converter.py
+-rw-r--r--   0        0        0     4510 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/quri_parts/tket/circuit/tket_circuit_converter.py
+-rw-r--r--   0        0        0     4572 2024-03-19 02:11:01.306138 quri_parts_tket-17.0.0/quri_parts/tket/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 quri_parts_tket-17.0.0/PKG-INFO
```

### Comparing `quri_parts_tket-0.18.0/LICENSE` & `quri_parts_tket-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.18.0/pyproject.toml` & `quri_parts_tket-17.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-tket"
-version = "0.18.0"
+version = "17.0.0"
 description = "A plugin to use tket with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_tket-0.18.0/quri_parts/tket/circuit/__init__.py` & `quri_parts_tket-17.0.0/quri_parts/tket/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.18.0/quri_parts/tket/circuit/circuit_converter.py` & `quri_parts_tket-17.0.0/quri_parts/tket/circuit/circuit_converter.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.18.0/quri_parts/tket/circuit/tket_circuit_converter.py` & `quri_parts_tket-17.0.0/quri_parts/tket/circuit/tket_circuit_converter.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.18.0/quri_parts/tket/circuit/transpile/__init__.py` & `quri_parts_tket-17.0.0/quri_parts/tket/circuit/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.18.0/PKG-INFO` & `quri_parts_tket-17.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-tket
-Version: 0.18.0
+Version: 17.0.0
 Summary: A plugin to use tket with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

