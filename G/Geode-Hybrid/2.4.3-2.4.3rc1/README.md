# Comparing `tmp/Geode_Hybrid-2.4.3-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Hybrid-2.4.3rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 171914 bytes, number of entries: 8
--rw-r--r--  2.0 unx       66 b- defN 24-May-22 00:36 geode_hybrid/__init__.py
--rw-r--r--  2.0 unx      225 b- defN 24-May-22 00:36 geode_hybrid/brep.py
--rwxr-xr-x  2.0 unx   130456 b- defN 24-May-22 00:36 geode_hybrid/lib64/geode_hybrid_py_brep.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   266752 b- defN 24-May-22 00:36 geode_hybrid/lib64/libGeode-Hybrid_brep.so
--rw-r--r--  2.0 unx     2200 b- defN 24-May-22 00:36 Geode_Hybrid-2.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 24-May-22 00:36 Geode_Hybrid-2.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-22 00:36 Geode_Hybrid-2.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      704 b- defN 24-May-22 00:36 Geode_Hybrid-2.4.3.dist-info/RECORD
-8 files, 400519 bytes uncompressed, 170676 bytes compressed:  57.4%
+Zip file size: 1557764 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      170 b- defN 24-May-21 18:49 geode_hybrid/__init__.py
+-rw-rw-rw-  2.0 fat      234 b- defN 24-May-21 18:49 geode_hybrid/brep.py
+-rw-rw-rw-  2.0 fat  3856896 b- defN 24-May-21 18:50 geode_hybrid/bin/Geode-Hybrid_brep.dll
+-rw-rw-rw-  2.0 fat   126464 b- defN 24-May-21 18:50 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2273 b- defN 24-May-21 18:50 Geode_Hybrid-2.4.3rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-21 18:50 Geode_Hybrid-2.4.3rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-21 18:50 Geode_Hybrid-2.4.3rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      700 b- defN 24-May-21 18:50 Geode_Hybrid-2.4.3rc1.dist-info/RECORD
+8 files, 3986850 bytes uncompressed, 1556538 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: geode_hybrid/__init__.py
 Comment: 
 
 Filename: geode_hybrid/brep.py
 Comment: 
 
-Filename: geode_hybrid/lib64/geode_hybrid_py_brep.cpython-39-x86_64-linux-gnu.so
+Filename: geode_hybrid/bin/Geode-Hybrid_brep.dll
 Comment: 
 
-Filename: geode_hybrid/lib64/libGeode-Hybrid_brep.so
+Filename: geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Hybrid-2.4.3.dist-info/METADATA
+Filename: Geode_Hybrid-2.4.3rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Hybrid-2.4.3.dist-info/WHEEL
+Filename: Geode_Hybrid-2.4.3rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Hybrid-2.4.3.dist-info/top_level.txt
+Filename: Geode_Hybrid-2.4.3rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Hybrid-2.4.3.dist-info/RECORD
+Filename: Geode_Hybrid-2.4.3rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_hybrid/__init__.py

```diff
@@ -1,3 +1,6 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .brep import *
```

## geode_hybrid/brep.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_numerics
-import geode_simplex
-
-from .lib64.geode_hybrid_py_brep import *
-HybridBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_numerics
+import geode_simplex
+
+from .bin.geode_hybrid_py_brep import *
+HybridBRepLibrary.initialize()
```

## Comparing `Geode_Hybrid-2.4.3.dist-info/METADATA` & `Geode_Hybrid-2.4.3rc1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-Metadata-Version: 2.1
-Name: Geode-Hybrid
-Version: 2.4.3
-Summary: Hybrid remeshing Geode-solutions OpenGeode module
-Home-page: https://github.com/Geode-solutions/Geode-Hybrid
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.10.0
-Requires-Dist: geode-common ==31.*,>=31.1.0
-Requires-Dist: geode-numerics ==4.*,>=4.3.3
-Requires-Dist: geode-simplex ==6.*,>=6.8.0
-Requires-Dist: opengeode-core ==14.*,>=14.20.0
-Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
-
-<h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Template for creating your own OpenGeode private module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-ModuleTemplate_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-ModuleTemplate_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://geode-solutions.com/#slack">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2024, Geode-solutions
+Metadata-Version: 2.1
+Name: Geode-Hybrid
+Version: 2.4.3rc1
+Summary: Hybrid remeshing Geode-solutions OpenGeode module
+Home-page: https://github.com/Geode-solutions/Geode-Hybrid
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Requires-Dist: geode-background ==7.*,>=7.10.0rc1
+Requires-Dist: geode-common ==31.*,>=31.1.0
+Requires-Dist: geode-numerics ==4.*,>=4.3.3
+Requires-Dist: geode-simplex ==6.*,>=6.8.0rc1
+Requires-Dist: opengeode-core ==14.*,>=14.20.0
+Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
+
+<h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Template for creating your own OpenGeode private module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-ModuleTemplate_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-ModuleTemplate_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://geode-solutions.com/#slack">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2024, Geode-solutions
+
+
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.4.3 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.4.3rc1 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
-solutions.com License: Proprietary Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.10.0 Requires-Dist: geode-common
-==31.*,>=31.1.0 Requires-Dist: geode-numerics ==4.*,>=4.3.3 Requires-Dist:
-geode-simplex ==6.*,>=6.8.0 Requires-Dist: opengeode-core ==14.*,>=14.20.0
-Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
+solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
+text/markdown Requires-Dist: geode-background ==7.*,>=7.10.0rc1 Requires-Dist:
+geode-common ==31.*,>=31.1.0 Requires-Dist: geode-numerics ==4.*,>=4.3.3
+Requires-Dist: geode-simplex ==6.*,>=6.8.0rc1 Requires-Dist: opengeode-core
+==14.*,>=14.20.0 Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
          ************ GGeeooddee--MMoodduulleeTTeemmppllaattee__pprriivvaatteebbyy GGeeooddee--ssoolluuttiioonnss ************
        ******** TTeemmppllaattee ffoorr ccrreeaattiinngg yyoouurr oowwnn OOppeennGGeeooddee pprriivvaattee mmoodduullee ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

