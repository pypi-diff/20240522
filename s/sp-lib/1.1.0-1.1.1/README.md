# Comparing `tmp/sp_lib-1.1.0-py3-none-any.whl.zip` & `tmp/sp_lib-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10479 bytes, number of entries: 7
--rw-r--r--  2.0 unx       52 b- defN 24-May-22 05:28 sp_lib/__init__.py
+Zip file size: 10474 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       52 b- defN 24-May-22 06:08 sp_lib/__init__.py
 -rw-r--r--  2.0 unx    36162 b- defN 24-May-22 05:28 sp_lib/amazon_sp_api.py
--rw-r--r--  2.0 unx     1067 b- defN 24-May-22 05:41 sp_lib-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1698 b- defN 24-May-22 05:41 sp_lib-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-22 05:41 sp_lib-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-22 05:41 sp_lib-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      534 b- defN 24-May-22 05:41 sp_lib-1.1.0.dist-info/RECORD
-7 files, 39612 bytes uncompressed, 9535 bytes compressed:  75.9%
+-rw-r--r--  2.0 unx     1067 b- defN 24-May-22 06:16 sp_lib-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1697 b- defN 24-May-22 06:16 sp_lib-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 06:16 sp_lib-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-22 06:16 sp_lib-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      534 b- defN 24-May-22 06:16 sp_lib-1.1.1.dist-info/RECORD
+7 files, 39611 bytes uncompressed, 9530 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sp_lib/__init__.py
 Comment: 
 
 Filename: sp_lib/amazon_sp_api.py
 Comment: 
 
-Filename: sp_lib-1.1.0.dist-info/LICENSE
+Filename: sp_lib-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: sp_lib-1.1.0.dist-info/METADATA
+Filename: sp_lib-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sp_lib-1.1.0.dist-info/WHEEL
+Filename: sp_lib-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sp_lib-1.1.0.dist-info/top_level.txt
+Filename: sp_lib-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sp_lib-1.1.0.dist-info/RECORD
+Filename: sp_lib-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sp_lib/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .amazon_sp_api import *
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
```

## Comparing `sp_lib-1.1.0.dist-info/LICENSE` & `sp_lib-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sp_lib-1.1.0.dist-info/METADATA` & `sp_lib-1.1.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sp-lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: sp_lib: please see README
 Home-page: https://github.com/greenroomy/amazon_sp_api
 Download-URL: https://github.com/greenroomy/amazon_sp_api/
 Author: Shinji Uetsuki
 Author-email: greenroom1973@gmail.com
 Maintainer: Shinji Uetsuki
 Maintainer-email: greenroom1973@gmail.com
 License: MIT license
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.2)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: urllib3 (>=1.26.15)
 Requires-Dist: pandas (>=1.2.4)
 
 # Description
```

