# Comparing `tmp/Geode_Explicit-4.8.0rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.8.1rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3139253 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 24-May-21 18:41 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 24-May-21 18:41 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 24-May-21 18:41 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  4021248 b- defN 24-May-21 18:42 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33792 b- defN 24-May-21 18:42 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3715072 b- defN 24-May-21 18:42 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   147456 b- defN 24-May-21 18:42 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   135680 b- defN 24-May-21 18:42 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2212 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/RECORD
-12 files, 8057419 bytes uncompressed, 3137329 bytes compressed:  61.1%
+Zip file size: 361355 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       89 b- defN 24-May-22 14:17 geode_explicit/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 24-May-22 14:17 geode_explicit/brep.py
+-rw-r--r--  2.0 unx      240 b- defN 24-May-22 14:17 geode_explicit/section.py
+-rwxr-xr-x  2.0 unx   159296 b- defN 24-May-22 14:17 geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   138752 b- defN 24-May-22 14:17 geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   467952 b- defN 24-May-22 14:17 geode_explicit/lib64/libGeode-Explicit_brep.so
+-rwxr-xr-x  2.0 unx    35352 b- defN 24-May-22 14:17 geode_explicit/lib64/libGeode-Explicit_common.so
+-rwxr-xr-x  2.0 unx    77016 b- defN 24-May-22 14:17 geode_explicit/lib64/libGeode-Explicit_section.so
+-rw-r--r--  2.0 unx     2149 b- defN 24-May-22 14:17 Geode_Explicit-4.8.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 24-May-22 14:17 Geode_Explicit-4.8.1rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-22 14:17 Geode_Explicit-4.8.1rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1166 b- defN 24-May-22 14:17 Geode_Explicit-4.8.1rc1.dist-info/RECORD
+12 files, 882391 bytes uncompressed, 359351 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: geode_explicit/brep.py
 Comment: 
 
 Filename: geode_explicit/section.py
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_brep.dll
+Filename: geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_common.dll
+Filename: geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_section.dll
+Filename: geode_explicit/lib64/libGeode-Explicit_brep.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_common.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_section.so
 Comment: 
 
-Filename: Geode_Explicit-4.8.0rc1.dist-info/METADATA
+Filename: Geode_Explicit-4.8.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.8.0rc1.dist-info/WHEEL
+Filename: Geode_Explicit-4.8.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.8.0rc1.dist-info/top_level.txt
+Filename: Geode_Explicit-4.8.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.8.0rc1.dist-info/RECORD
+Filename: Geode_Explicit-4.8.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .section import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+from .section import *
+from .brep import *
```

## geode_explicit/brep.py

```diff
@@ -1,12 +1,12 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_inspector
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_brep import *
-ExplicitBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_inspector
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_brep import *
+ExplicitBRepLibrary.initialize()
```

## geode_explicit/section.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_section import *
-ExplicitSectionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_section import *
+ExplicitSectionLibrary.initialize()
```

## Comparing `Geode_Explicit-4.8.0rc1.dist-info/RECORD` & `Geode_Explicit-4.8.1rc1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-geode_explicit/__init__.py,sha256=3IEZJDMtMfFSTtDJOl8tpLIg5P9Iytnx2bE1I6Gg8qo,194
-geode_explicit/brep.py,sha256=i4sDZvKY0NnpwATBxQHOq2egAGLbxDH5u4iZqCHMOlk,271
-geode_explicit/section.py,sha256=k_Q35aAqi_ZAP004Xc86lQf4FSYA2u0kU6y1_iR9Ahk,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=bLx4Q0rkjOE__X5IgHlQU2LoAXPLtGhAAo70L225eNo,4021248
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=G7E6Cf7ImDf-VxhGxBBRpG9LiqEV88Vr41xwdEPf4dM,33792
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=S8xclsfFmxXN3uu50wWJ9sfcl_dF56KhAqiqfnXfU_w,3715072
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=JrLaFChWK8AbnEfQ1hHi_Y7LxwR70vzyjFSBWONzP4c,147456
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=si6Bgvpf9Y7tzPG7eGzgza_OPPqNQT-XTsDkTHkCzLY,135680
-Geode_Explicit-4.8.0rc1.dist-info/METADATA,sha256=C3sEXm4LwaAzkzjKuofXHAom6JP0RHHIXDmUdCY7pRs,2212
-Geode_Explicit-4.8.0rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Explicit-4.8.0rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.8.0rc1.dist-info/RECORD,,
+geode_explicit/__init__.py,sha256=08Jv_j6l55nLaa6-0g_1kSAFNTm8bJxZIhj1Su7ykhg,89
+geode_explicit/brep.py,sha256=AGSr4GiHYA2yA300pQq5aSAPY-cKbjxOzdYukAtEJNw,261
+geode_explicit/section.py,sha256=iYPIWWs6fo3bNWTBkUqJ7-J0FI9w3mXN3NovuSZaL6o,240
+geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so,sha256=5itAf4Jh7J91y49Z3dYCdmndtWca6B_i-jiokua5Us8,159296
+geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so,sha256=MRMmXLmu0lL0Wsmd4a9MYqfVUnZox1Dv8R3EIz3BTD0,138752
+geode_explicit/lib64/libGeode-Explicit_brep.so,sha256=DUUfQCezyyzI8SitVX4hsSl8k_bcrkjxtpsGV0fFcdg,467952
+geode_explicit/lib64/libGeode-Explicit_common.so,sha256=55qL92sF6QA6u0Cqr8q9w8C06XWkJiWIkQQdedqJ8UU,35352
+geode_explicit/lib64/libGeode-Explicit_section.so,sha256=5A3OxoY5n2FOCQE9dd9cg1gLEkgDL1p1hTFwaf9msic,77016
+Geode_Explicit-4.8.1rc1.dist-info/METADATA,sha256=Pnx31nGK8wKJUsRP51AuSRnU7tW6cD8A3SfxPVA6Qf4,2149
+Geode_Explicit-4.8.1rc1.dist-info/WHEEL,sha256=cPiEulY4lHJMdGCxx29HxfDkwhV9C6172sJgZUA9dSs,103
+Geode_Explicit-4.8.1rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.8.1rc1.dist-info/RECORD,,
```

