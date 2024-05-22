# Comparing `tmp/fengwo-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/fengwo-0.0.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2175912 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      172 b- defN 24-May-19 12:37 fengwo/__init__.py
--rw-rw-rw-  2.0 fat  5151744 b- defN 23-Feb-08 01:35 fengwo/libcrypto-3-x64.dll
--rw-rw-rw-  2.0 fat   782848 b- defN 24-May-19 12:09 fengwo/pyML.pyd
--rw-rw-rw-  2.0 fat      529 b- defN 24-May-19 12:37 fengwo-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 12:37 fengwo-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-19 12:37 fengwo-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      526 b- defN 24-May-19 12:37 fengwo-0.0.1.dist-info/RECORD
-7 files, 5935918 bytes uncompressed, 2174992 bytes compressed:  63.4%
+Zip file size: 2176932 bytes, number of entries: 7
+?rw-------  2.0 fat      172 b- defN 24-May-22 20:06 fengwo/__init__.py
+?rw-------  2.0 fat  5151744 b- defN 24-May-22 20:06 fengwo/libcrypto-3-x64.dll
+?rw-------  2.0 fat   784384 b- defN 24-May-22 20:06 fengwo/pyML.pyd
+?rw-------  2.0 fat      540 b- defN 24-May-22 20:06 fengwo-0.0.2.dist-info/METADATA
+?rw-------  2.0 fat       99 b- defN 24-May-22 20:06 fengwo-0.0.2.dist-info/WHEEL
+?rw-------  2.0 fat        7 b- defN 24-May-22 20:06 fengwo-0.0.2.dist-info/top_level.txt
+?rw-------  2.0 fat      526 b- defN 24-May-22 20:06 fengwo-0.0.2.dist-info/RECORD
+7 files, 5937472 bytes uncompressed, 2176012 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: fengwo/libcrypto-3-x64.dll
 Comment: 
 
 Filename: fengwo/pyML.pyd
 Comment: 
 
-Filename: fengwo-0.0.1.dist-info/METADATA
+Filename: fengwo-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: fengwo-0.0.1.dist-info/WHEEL
+Filename: fengwo-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: fengwo-0.0.1.dist-info/top_level.txt
+Filename: fengwo-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fengwo-0.0.1.dist-info/RECORD
+Filename: fengwo-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fengwo/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .pyML import *
-version='0.0.1'
+version='0.0.2'
 author='燕山飞雪'
 author_email='kogj@163.com'
 description='仿通达信公式的量化函数库'
 url='https://www.fengwo.run'
```

## Comparing `fengwo-0.0.1.dist-info/METADATA` & `fengwo-0.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: fengwo
-Version: 0.0.1
+Version: 0.0.2
 Summary: 仿通达信公式的量化函数库
 Home-page: https://www.fengwo.run
 Author: 燕山飞雪
 Author-email: kogj@163.com
 License: UNKNOWN
 Platform: Windows
+Platform: linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
 
 仿通达信公式的量化函数库
```

