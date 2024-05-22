# Comparing `tmp/tflite_micro-0.dev20240518003142-cp311-cp311-manylinux_2_28_x86_64.whl.zip` & `tmp/tflite_micro-0.dev20240520175645-cp311-cp311-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 777075 bytes, number of entries: 12
--r-xr-xr-x  2.0 unx     1241 b- defN 24-May-18 13:12 tflite_micro/__init__.py
--r-xr-xr-x  2.0 unx  3344568 b- defN 24-May-18 13:15 tflite_micro/python/tflite_micro/_runtime.so
--r-xr-xr-x  2.0 unx       45 b- defN 24-May-18 13:12 tflite_micro/python/tflite_micro/_version.py
--r-xr-xr-x  2.0 unx     1796 b- defN 24-May-18 13:12 tflite_micro/python/tflite_micro/postinstall_check.py
--r-xr-xr-x  2.0 unx     9906 b- defN 24-May-18 13:12 tflite_micro/python/tflite_micro/runtime.py
--r-xr-xr-x  2.0 unx     3164 b- defN 24-May-18 13:12 tflite_micro/python/tflite_micro/sine_float.tflite
--r-xr-xr-x  2.0 unx   637385 b- defN 24-May-18 13:13 tflite_micro/tensorflow/lite/python/schema_py_generated.py
--r-xr-xr-x  2.0 unx     1631 b- defN 24-May-18 13:12 tflite_micro/tensorflow/lite/python/schema_util.py
--r-xr-xr-x  2.0 unx    14383 b- defN 24-May-18 13:12 tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py
-?rw-------  2.0 unx      113 b- defN 24-May-18 13:15 tflite_micro-0.dev20240518003142.dist-info/WHEEL
-?rw-------  2.0 unx      478 b- defN 24-May-18 13:15 tflite_micro-0.dev20240518003142.dist-info/METADATA
-?rw-------  2.0 unx     1200 b- defN 24-May-18 13:15 tflite_micro-0.dev20240518003142.dist-info/RECORD
-12 files, 4015910 bytes uncompressed, 775005 bytes compressed:  80.7%
+Zip file size: 777078 bytes, number of entries: 12
+-r-xr-xr-x  2.0 unx     1241 b- defN 24-May-21 13:15 tflite_micro/__init__.py
+-r-xr-xr-x  2.0 unx  3344568 b- defN 24-May-21 13:19 tflite_micro/python/tflite_micro/_runtime.so
+-r-xr-xr-x  2.0 unx       45 b- defN 24-May-21 13:15 tflite_micro/python/tflite_micro/_version.py
+-r-xr-xr-x  2.0 unx     1796 b- defN 24-May-21 13:15 tflite_micro/python/tflite_micro/postinstall_check.py
+-r-xr-xr-x  2.0 unx     9906 b- defN 24-May-21 13:15 tflite_micro/python/tflite_micro/runtime.py
+-r-xr-xr-x  2.0 unx     3164 b- defN 24-May-21 13:15 tflite_micro/python/tflite_micro/sine_float.tflite
+-r-xr-xr-x  2.0 unx   637385 b- defN 24-May-21 13:16 tflite_micro/tensorflow/lite/python/schema_py_generated.py
+-r-xr-xr-x  2.0 unx     1631 b- defN 24-May-21 13:15 tflite_micro/tensorflow/lite/python/schema_util.py
+-r-xr-xr-x  2.0 unx    14383 b- defN 24-May-21 13:15 tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py
+?rw-------  2.0 unx      113 b- defN 24-May-21 13:19 tflite_micro-0.dev20240520175645.dist-info/WHEEL
+?rw-------  2.0 unx      478 b- defN 24-May-21 13:19 tflite_micro-0.dev20240520175645.dist-info/METADATA
+?rw-------  2.0 unx     1200 b- defN 24-May-21 13:19 tflite_micro-0.dev20240520175645.dist-info/RECORD
+12 files, 4015910 bytes uncompressed, 775008 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -21,17 +21,17 @@
 
 Filename: tflite_micro/tensorflow/lite/python/schema_util.py
 Comment: 
 
 Filename: tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py
 Comment: 
 
-Filename: tflite_micro-0.dev20240518003142.dist-info/WHEEL
+Filename: tflite_micro-0.dev20240520175645.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_micro-0.dev20240518003142.dist-info/METADATA
+Filename: tflite_micro-0.dev20240520175645.dist-info/METADATA
 Comment: 
 
-Filename: tflite_micro-0.dev20240518003142.dist-info/RECORD
+Filename: tflite_micro-0.dev20240520175645.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_micro/python/tflite_micro/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.dev20240518003142-g6028493"
+__version__ = "0.dev20240520175645-g8e22946"
```

## Comparing `tflite_micro-0.dev20240518003142.dist-info/RECORD` & `tflite_micro-0.dev20240520175645.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tflite_micro/__init__.py,sha256=fjz_YqLilIRTfAnsshkOiF_EJVVnq5-f8UpLHBSl7mg,1241
 tflite_micro/python/tflite_micro/_runtime.so,sha256=bxNm6kPEUYirxpQ6-wLHs8eWoYUx57vlfvAlJFLGd2s,3344568
-tflite_micro/python/tflite_micro/_version.py,sha256=Tt2DIyam8tG92QgMZ6SaOyjnNSe3_4Mkd8naLbF4-2E,45
+tflite_micro/python/tflite_micro/_version.py,sha256=KVqyNSy8p5yHyL2hgcXVP1LkidQ8QKkTVXz1JXMreEs,45
 tflite_micro/python/tflite_micro/postinstall_check.py,sha256=txtw1er-0lCsMnicKOkRsP9RU0fZ73U6t2wGOE-D9wc,1796
 tflite_micro/python/tflite_micro/runtime.py,sha256=_AHamRV4YML5GuYfU1q_cfeeApAY_xbk6wMOE_OuEhU,9906
 tflite_micro/python/tflite_micro/sine_float.tflite,sha256=7pOYYxlco3zgY7GOFPuCqg2Y22WWukEJV1f2tWDaEHA,3164
 tflite_micro/tensorflow/lite/python/schema_py_generated.py,sha256=KpNyltLm7nrFMDMdW6CmaTBsoV9vN5gIAF8jYA18b3g,637385
 tflite_micro/tensorflow/lite/python/schema_util.py,sha256=M1LrSqMKK3e3SKsg-98ovSOkWO4-ly91FFu2JI32TZk,1631
 tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py,sha256=whDjbHdpQx3_1fEue2Wb5GTqj1U2NrUvqWzK-kC65bA,14383
-tflite_micro-0.dev20240518003142.dist-info/METADATA,sha256=-icxMKypves9piPLLr553A7su_JIzD_hiJYpdsCZMzQ,478
-tflite_micro-0.dev20240518003142.dist-info/RECORD,,
-tflite_micro-0.dev20240518003142.dist-info/WHEEL,sha256=qeKfpRMWEkf6-wLErlsQMeI6ob4StU6OQRW53pZ_1Pk,113
+tflite_micro-0.dev20240520175645.dist-info/METADATA,sha256=iqiE62rBv0UkIo-6d_NUYkX0gjfFgxz85EhXsc7o9Wc,478
+tflite_micro-0.dev20240520175645.dist-info/RECORD,,
+tflite_micro-0.dev20240520175645.dist-info/WHEEL,sha256=qeKfpRMWEkf6-wLErlsQMeI6ob4StU6OQRW53pZ_1Pk,113
```

