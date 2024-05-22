# Comparing `tmp/bitlinear-1.2.5.tar.gz` & `tmp/bitlinear-2.0.0.tar.gz`

## Comparing `bitlinear-1.2.5.tar` & `bitlinear-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.5/bitlinear/__init__.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bitlinear-1.2.5/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.5/bitlinear/kernels.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.5/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.5/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/__init__.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/kernels.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/measures.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.0/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.0/PKG-INFO
```

### Comparing `bitlinear-1.2.5/bitlinear/kernels.py` & `bitlinear-2.0.0/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.5/LICENSE` & `bitlinear-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.5/README.md` & `bitlinear-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.5/pyproject.toml` & `bitlinear-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.2.5"
+version = "2.0.0"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.2.5/PKG-INFO` & `bitlinear-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.2.5
+Version: 2.0.0
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

