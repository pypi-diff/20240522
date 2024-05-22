# Comparing `tmp/ddx_python-0.1.6-cp38-abi3-manylinux_2_24_x86_64.whl.zip` & `tmp/ddx_python-0.2.0-cp310-cp310-macosx_10_12_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 203111 bytes, number of entries: 5
--rw-r--r--  4.6 unx      839 b- defN 22-Feb-22 19:47 ddx_python-0.1.6.dist-info/METADATA
--rw-r--r--  4.6 unx      107 b- defN 22-Feb-22 19:47 ddx_python-0.1.6.dist-info/WHEEL
--rw-r--r--  4.6 unx       56 b- defN 22-Feb-22 19:47 ddx_python/__init__.py
--rwxr-xr-x  4.6 unx   461272 b- defN 22-Feb-22 19:47 ddx_python/ddx_python.abi3.so
--rw-r--r--  4.6 unx      380 b- defN 22-Feb-22 19:47 ddx_python-0.1.6.dist-info/RECORD
-5 files, 462654 bytes uncompressed, 202407 bytes compressed:  56.3%
+Zip file size: 764566 bytes, number of entries: 5
+-rw-r--r--  4.6 unx      839 b- defN 24-May-22 00:27 ddx_python-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 24-May-22 00:27 ddx_python-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      123 b- defN 24-May-22 00:27 ddx_python/__init__.py
+-rwxr-xr-x  4.6 unx  1971292 b- defN 24-May-22 00:27 ddx_python/ddx_python.cpython-310-darwin.so
+-rw-r--r--  4.6 unx      396 b- defN 24-May-22 00:27 ddx_python-0.2.0.dist-info/RECORD
+5 files, 1972756 bytes uncompressed, 763834 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: ddx_python-0.1.6.dist-info/METADATA
+Filename: ddx_python-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: ddx_python-0.1.6.dist-info/WHEEL
+Filename: ddx_python-0.2.0.dist-info/WHEEL
 Comment: 
 
 Filename: ddx_python/__init__.py
 Comment: 
 
-Filename: ddx_python/ddx_python.abi3.so
+Filename: ddx_python/ddx_python.cpython-310-darwin.so
 Comment: 
 
-Filename: ddx_python-0.1.6.dist-info/RECORD
+Filename: ddx_python-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddx_python/__init__.py

```diff
@@ -1,3 +1,5 @@
 from .ddx_python import *
 
 __doc__ = ddx_python.__doc__
+if hasattr(ddx_python, "__all__"):
+    __all__ = ddx_python.__all__
```

## Comparing `ddx_python-0.1.6.dist-info/METADATA` & `ddx_python-0.2.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ddx_python
-Version: 0.1.6
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # DDX-Python
```

