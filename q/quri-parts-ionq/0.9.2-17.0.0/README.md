# Comparing `tmp/quri_parts_ionq-0.9.2.tar.gz` & `tmp/quri_parts_ionq-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_ionq-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_ionq-17.0.0.tar", max compression
```

## Comparing `quri_parts_ionq-0.9.2.tar` & `quri_parts_ionq-17.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/LICENSE
--rw-r--r--   0        0        0      252 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/README.md
--rw-r--r--   0        0        0     1178 2023-03-29 07:37:29.174996 quri_parts_ionq-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:28.338991 quri_parts_ionq-0.9.2/quri_parts/ionq/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/__init__.py
--rw-r--r--   0        0        0      637 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/__init__.py
--rw-r--r--   0        0        0      680 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/gate_names.py
--rw-r--r--   0        0        0     3335 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/gates.py
--rw-r--r--   0        0        0     1370 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/transpile/__init__.py
--rw-r--r--   0        0        0     5534 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/transpile/ionq_native_transpiler.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.870951 quri_parts_ionq-0.9.2/quri_parts/ionq/py.typed
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 quri_parts_ionq-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/LICENSE
+-rw-r--r--   0        0        0      252 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/README.md
+-rw-r--r--   0        0        0     1179 2024-03-19 02:11:28.258013 quri_parts_ionq-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:27.650016 quri_parts_ionq-17.0.0/quri_parts/ionq/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/__init__.py
+-rw-r--r--   0        0        0      680 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/gate_names.py
+-rw-r--r--   0        0        0     3335 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/gates.py
+-rw-r--r--   0        0        0     1370 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     5534 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/transpile/ionq_native_transpiler.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.294138 quri_parts_ionq-17.0.0/quri_parts/ionq/py.typed
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 quri_parts_ionq-17.0.0/PKG-INFO
```

### Comparing `quri_parts_ionq-0.9.2/LICENSE` & `quri_parts_ionq-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_ionq-0.9.2/pyproject.toml` & `quri_parts_ionq-17.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-ionq"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use IonQ with QIRI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <support@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/__init__.py` & `quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/gate_names.py` & `quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/gate_names.py`

 * *Files identical despite different names*

### Comparing `quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/gates.py` & `quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/transpile/__init__.py` & `quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_ionq-0.9.2/quri_parts/ionq/circuit/transpile/ionq_native_transpiler.py` & `quri_parts_ionq-17.0.0/quri_parts/ionq/circuit/transpile/ionq_native_transpiler.py`

 * *Files identical despite different names*

### Comparing `quri_parts_ionq-0.9.2/PKG-INFO` & `quri_parts_ionq-17.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-ionq
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use IonQ with QIRI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: support@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

