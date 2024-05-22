# Comparing `tmp/vr180_convert-0.4.0.tar.gz` & `tmp/vr180_convert-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vr180_convert-0.4.0.tar", max compression
+gzip compressed data, was "vr180_convert-0.4.1.tar", max compression
```

## Comparing `vr180_convert-0.4.0.tar` & `vr180_convert-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-05-20 02:32:27.636149 vr180_convert-0.4.0/LICENSE
--rw-r--r--   0        0        0    10741 2024-05-20 02:32:27.636149 vr180_convert-0.4.0/README.md
--rw-r--r--   0        0        0     3837 2024-05-20 02:32:28.760145 vr180_convert-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      707 2024-05-20 02:32:28.760145 vr180_convert-0.4.0/src/vr180_convert/__init__.py
--rw-r--r--   0        0        0      113 2024-05-20 02:32:27.652149 vr180_convert-0.4.0/src/vr180_convert/__main__.py
--rw-r--r--   0        0        0    12703 2024-05-20 02:32:27.652149 vr180_convert-0.4.0/src/vr180_convert/cli.py
--rw-r--r--   0        0        0        0 2024-05-20 02:32:27.652149 vr180_convert-0.4.0/src/vr180_convert/py.typed
--rw-r--r--   0        0        0    12090 2024-05-20 02:32:27.652149 vr180_convert-0.4.0/src/vr180_convert/remapper.py
--rw-r--r--   0        0        0     1889 2024-05-20 02:32:27.652149 vr180_convert-0.4.0/src/vr180_convert/testing.py
--rw-r--r--   0        0        0    20213 2024-05-20 02:32:27.652149 vr180_convert-0.4.0/src/vr180_convert/transformer.py
--rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-22 11:55:39.673391 vr180_convert-0.4.1/LICENSE
+-rw-r--r--   0        0        0    10741 2024-05-22 11:55:39.673391 vr180_convert-0.4.1/README.md
+-rw-r--r--   0        0        0     3837 2024-05-22 11:55:40.789401 vr180_convert-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-05-22 11:55:40.789401 vr180_convert-0.4.1/src/vr180_convert/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-22 11:55:39.689391 vr180_convert-0.4.1/src/vr180_convert/__main__.py
+-rw-r--r--   0        0        0    12703 2024-05-22 11:55:39.689391 vr180_convert-0.4.1/src/vr180_convert/cli.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:55:39.689391 vr180_convert-0.4.1/src/vr180_convert/py.typed
+-rw-r--r--   0        0        0    12090 2024-05-22 11:55:39.689391 vr180_convert-0.4.1/src/vr180_convert/remapper.py
+-rw-r--r--   0        0        0     1889 2024-05-22 11:55:39.689391 vr180_convert-0.4.1/src/vr180_convert/testing.py
+-rw-r--r--   0        0        0    20213 2024-05-22 11:55:39.689391 vr180_convert-0.4.1/src/vr180_convert/transformer.py
+-rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.4.1/PKG-INFO
```

### Comparing `vr180_convert-0.4.0/LICENSE` & `vr180_convert-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.4.0/README.md` & `vr180_convert-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.4.0/pyproject.toml` & `vr180_convert-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vr180-convert"
-version = "0.4.0"
+version = "0.4.1"
 description = "Simple VR180 image converter"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/vr180-convert"
 documentation = "https://vr180-convert.readthedocs.io"
 classifiers = [
```

### Comparing `vr180_convert-0.4.0/src/vr180_convert/__init__.py` & `vr180_convert-0.4.1/src/vr180_convert/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 from .remapper import apply, apply_lr, get_map
 from .transformer import (
     DenormalizeTransformer,
     EquirectangularEncoder,
     Euclidean3DRotator,
     Euclidean3DTransformer,
     FisheyeDecoder,
```

### Comparing `vr180_convert-0.4.0/src/vr180_convert/cli.py` & `vr180_convert-0.4.1/src/vr180_convert/cli.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.4.0/src/vr180_convert/remapper.py` & `vr180_convert-0.4.1/src/vr180_convert/remapper.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.4.0/src/vr180_convert/testing.py` & `vr180_convert-0.4.1/src/vr180_convert/testing.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.4.0/src/vr180_convert/transformer.py` & `vr180_convert-0.4.1/src/vr180_convert/transformer.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.4.0/PKG-INFO` & `vr180_convert-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vr180-convert
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple VR180 image converter
 Home-page: https://github.com/34j/vr180-convert
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vr180-convert Version: 0.4.0 Summary: Simple VR180
+Metadata-Version: 2.1 Name: vr180-convert Version: 0.4.1 Summary: Simple VR180
 image converter Home-page: https://github.com/34j/vr180-convert License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

