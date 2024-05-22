# Comparing `tmp/finch_tensor-0.1.8.tar.gz` & `tmp/finch_tensor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finch_tensor-0.1.8.tar", max compression
+gzip compressed data, was "finch_tensor-0.1.9.tar", max compression
```

## Comparing `finch_tensor-0.1.8.tar` & `finch_tensor-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/LICENSE
--rw-r--r--   0        0        0     1851 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/README.md
--rw-r--r--   0        0        0      522 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1365 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/__init__.py
--rw-r--r--   0        0        0      842 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/compiled.py
--rw-r--r--   0        0        0      532 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/dtypes.py
--rw-r--r--   0        0        0      246 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/julia.py
--rw-r--r--   0        0        0     2066 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/levels.py
--rw-r--r--   0        0        0    21685 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/tensor.py
--rw-r--r--   0        0        0      287 2024-03-29 09:46:26.048858 finch_tensor-0.1.8/src/finch/typing.py
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 finch_tensor-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1851 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/README.md
+-rw-r--r--   0        0        0      522 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1731 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/compiled.py
+-rw-r--r--   0        0        0      532 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/dtypes.py
+-rw-r--r--   0        0        0      432 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/julia.py
+-rw-r--r--   0        0        0     2066 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/levels.py
+-rw-r--r--   0        0        0    21685 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/tensor.py
+-rw-r--r--   0        0        0      287 2024-04-11 12:56:22.094720 finch_tensor-0.1.9/src/finch/typing.py
+-rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 finch_tensor-0.1.9/PKG-INFO
```

### Comparing `finch_tensor-0.1.8/LICENSE` & `finch_tensor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `finch_tensor-0.1.8/README.md` & `finch_tensor-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `finch_tensor-0.1.8/pyproject.toml` & `finch_tensor-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finch-tensor"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Willow Ahrens <willow.marie.ahrens@gmail.com>"]
 readme = "README.md"
 packages = [{include = "finch", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `finch_tensor-0.1.8/src/finch/__init__.py` & `finch_tensor-0.1.9/src/finch/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,16 +21,32 @@
     permute_dims,
     multiply,
     sum,
     prod,
     add,
     subtract,
     divide,
+    floor_divide,
+    pow,
     positive,
     negative,
+    abs,
+    cos,
+    cosh,
+    acos,
+    acosh,
+    sin,
+    sinh,
+    asin,
+    asinh,
+    tan,
+    tanh,
+    atan,
+    atanh,
+    atan2,
 )
 from .compiled import (
     lazy,
     compiled,
     compute,
 )
 from .dtypes import (
@@ -92,10 +108,26 @@
     "compute",
     "sum",
     "prod",
     "add",
     "subtract",
     "multiply",
     "divide",
+    "floor_divide",
+    "pow",
     "positive",
     "negative",
+    "abs",
+    "cos",
+    "cosh",
+    "acos",
+    "acosh",
+    "sin",
+    "sinh",
+    "asin",
+    "asinh",
+    "tan",
+    "tanh",
+    "atan",
+    "atanh",
+    "atan2",
 ]
```

### Comparing `finch_tensor-0.1.8/src/finch/compiled.py` & `finch_tensor-0.1.9/src/finch/compiled.py`

 * *Files identical despite different names*

### Comparing `finch_tensor-0.1.8/src/finch/dtypes.py` & `finch_tensor-0.1.9/src/finch/dtypes.py`

 * *Files identical despite different names*

### Comparing `finch_tensor-0.1.8/src/finch/levels.py` & `finch_tensor-0.1.9/src/finch/levels.py`

 * *Files identical despite different names*

### Comparing `finch_tensor-0.1.8/src/finch/tensor.py` & `finch_tensor-0.1.9/src/finch/tensor.py`

 * *Files identical despite different names*

### Comparing `finch_tensor-0.1.8/PKG-INFO` & `finch_tensor-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-tensor
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Willow Ahrens
 Author-email: willow.marie.ahrens@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

