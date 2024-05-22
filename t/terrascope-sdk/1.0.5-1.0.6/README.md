# Comparing `tmp/terrascope-sdk-1.0.5.tar.gz` & `tmp/terrascope-sdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/marticenicks/repos/terrascope_sdk/dist/.tmp-hrh1dn2w/terrascope-sdk-1.0.5.tar", last modified: Tue Dec 13 12:19:03 2022, max compression
+gzip compressed data, was "terrascope-sdk-1.0.6.tar", last modified: Thu Feb  9 15:31:31 2023, max compression
```

## Comparing `terrascope-sdk-1.0.5.tar` & `terrascope-sdk-1.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/
--rw-r--r--   0 marticenicks   (503) staff       (20)     1061 2022-09-20 12:17:07.000000 terrascope-sdk-1.0.5/LICENSE
--rw-r--r--   0 marticenicks   (503) staff       (20)     2562 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/PKG-INFO
--rw-r--r--   0 marticenicks   (503) staff       (20)      846 2022-12-05 14:48:31.000000 terrascope-sdk-1.0.5/README.md
--rw-r--r--   0 marticenicks   (503) staff       (20)      990 2022-12-13 12:18:07.000000 terrascope-sdk-1.0.5/pyproject.toml
--rw-r--r--   0 marticenicks   (503) staff       (20)       38 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/setup.cfg
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/__init__.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/sdk/__init__.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/__init__.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    27404 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/algorithm.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    27647 2022-12-13 12:13:36.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/analysis.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    13852 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/aoi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     6456 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/credit.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     3496 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/data.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     2353 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/permission.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    15627 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/result.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     2760 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/toi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     4178 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/user.py
--rw-r--r--   0 marticenicks   (503) staff       (20)      851 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/visualization.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/__init__.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    15398 2022-12-13 12:18:07.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/algorithm.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     7091 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/analysis.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     6766 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/toi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     5280 2022-12-05 14:48:26.000000 terrascope-sdk-1.0.5/terrascope/sdk/terrascope_sdk.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/__init__.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     5752 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/io.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1396 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/sdk_support.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/
--rw-r--r--   0 marticenicks   (503) staff       (20)     2562 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marticenicks   (503) staff       (20)     1293 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marticenicks   (503) staff       (20)        1 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marticenicks   (503) staff       (20)      113 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/requires.txt
--rw-r--r--   0 marticenicks   (503) staff       (20)       44 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/tests/
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/tests/integration/
--rw-r--r--   0 marticenicks   (503) staff       (20)    46388 2022-12-05 14:48:26.000000 terrascope-sdk-1.0.5/tests/integration/test_algorithm.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1193 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_algorithm_builder.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    47447 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_analysis.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1111 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_analysis_builder.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     6127 2022-10-07 20:45:48.000000 terrascope-sdk-1.0.5/tests/integration/test_aoi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     8417 2022-12-05 13:22:22.000000 terrascope-sdk-1.0.5/tests/integration/test_credit.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1325 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_data.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     5982 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_permission.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     7021 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_result.py
--rw-r--r--   0 marticenicks   (503) staff       (20)      990 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_sdk_support.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    13125 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_toi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)      152 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_visualization.py
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.153617 terrascope-sdk-1.0.6/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     1061 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/LICENSE
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     2562 2023-02-09 15:31:31.153034 terrascope-sdk-1.0.6/PKG-INFO
+-rw-r--r--   0 nicholashyland   (501) staff       (20)      846 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/README.md
+-rw-r--r--   0 nicholashyland   (501) staff       (20)      990 2023-02-09 15:31:13.000000 terrascope-sdk-1.0.6/pyproject.toml
+-rw-r--r--   0 nicholashyland   (501) staff       (20)       38 2023-02-09 15:31:31.153818 terrascope-sdk-1.0.6/setup.cfg
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.128960 terrascope-sdk-1.0.6/terrascope/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.6/terrascope/__init__.py
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.129441 terrascope-sdk-1.0.6/terrascope/sdk/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.6/terrascope/sdk/__init__.py
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.135423 terrascope-sdk-1.0.6/terrascope/sdk/api/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/__init__.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    27404 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/algorithm.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    28071 2023-02-09 15:23:53.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/analysis.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    13852 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/aoi.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     6456 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/credit.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     3496 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/data.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     2353 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/permission.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    15627 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/result.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     2760 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/toi.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     4178 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/user.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)      851 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/api/visualization.py
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.137797 terrascope-sdk-1.0.6/terrascope/sdk/builder/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/terrascope/sdk/builder/__init__.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    15498 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/builder/algorithm.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     7091 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/builder/analysis.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     6766 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/builder/toi.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     5280 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/terrascope_sdk.py
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.139751 terrascope-sdk-1.0.6/terrascope/sdk/tools/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.6/terrascope/sdk/tools/__init__.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     5752 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/tools/io.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     1396 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/terrascope/sdk/tools/sdk_support.py
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.142676 terrascope-sdk-1.0.6/terrascope_sdk.egg-info/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     2562 2023-02-09 15:31:31.000000 terrascope-sdk-1.0.6/terrascope_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     1293 2023-02-09 15:31:31.000000 terrascope-sdk-1.0.6/terrascope_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholashyland   (501) staff       (20)        1 2023-02-09 15:31:31.000000 terrascope-sdk-1.0.6/terrascope_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholashyland   (501) staff       (20)      113 2023-02-09 15:31:31.000000 terrascope-sdk-1.0.6/terrascope_sdk.egg-info/requires.txt
+-rw-r--r--   0 nicholashyland   (501) staff       (20)       44 2023-02-09 15:31:31.000000 terrascope-sdk-1.0.6/terrascope_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.127681 terrascope-sdk-1.0.6/tests/
+drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:31:31.152140 terrascope-sdk-1.0.6/tests/integration/
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    46388 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/tests/integration/test_algorithm.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     3065 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/tests/integration/test_algorithm_builder.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    22029 2023-02-09 15:30:02.000000 terrascope-sdk-1.0.6/tests/integration/test_analysis.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     1111 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/tests/integration/test_analysis_builder.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     6127 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/tests/integration/test_aoi.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     8417 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/tests/integration/test_credit.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     1325 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/tests/integration/test_data.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     5982 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/tests/integration/test_permission.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)     7021 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/tests/integration/test_result.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)      990 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/tests/integration/test_sdk_support.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)    13125 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.6/tests/integration/test_toi.py
+-rw-r--r--   0 nicholashyland   (501) staff       (20)      152 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.6/tests/integration/test_visualization.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `terrascope-sdk-1.0.5/LICENSE` & `terrascope-sdk-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/PKG-INFO` & `terrascope-sdk-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrascope-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: A software development kit for developing projects on TerraScope
 Author-email: "Martice E. Nicks III" <martice.nicks@orbitalinsight.com>
 License: Copyright 2022 Orbital Insight, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `terrascope-sdk-1.0.5/README.md` & `terrascope-sdk-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/pyproject.toml` & `terrascope-sdk-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terrascope-sdk"
 
 
-version = "1.0.5"
+version = "1.0.6"
 
 
 authors = [
     { name = "Martice E. Nicks III", email = "martice.nicks@orbitalinsight.com" },
 ]
 description = "A software development kit for developing projects on TerraScope"
 readme = "README.md"
```

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/algorithm.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/algorithm.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/analysis.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from typing import List
 
 from google.protobuf.timestamp_pb2 import Timestamp
 from terrascope_api import TerrascopeAsyncClient
-from terrascope_api.models.analysis_computation_pb2 import AnalysisComputationCreateRequest, \
-    AnalysisComputationRunRequest, AnalysisComputation, \
-    AnalysisComputationGetRequest, AnalysisComputationListRequest
-from terrascope_api.models.analysis_config_pb2 import AnalysisConfigCreateRequest, AnalysisConfigGetRequest, \
-    AnalysisConfigListRequest, AnalysisConfig
-from terrascope_api.models.analysis_pb2 import Analysis, AnalysisCreateRequest, \
-    AnalysisGetRequest, AnalysisListRequest
-from terrascope_api.models.analysis_version_pb2 import AnalysisVersionListRequest, AnalysisVersionGetRequest, \
-    AnalysisVersionCreateRequest, AnalysisVersion
+from terrascope_api.models.analysis_computation_pb2 import (
+    AnalysisComputationCreateRequest, AnalysisComputationRunRequest, AnalysisComputation, AnalysisComputationGetRequest,
+    AnalysisComputationListRequest
+)
+from terrascope_api.models.analysis_config_pb2 import (
+    AnalysisConfigCreateRequest, AnalysisConfigGetRequest, AnalysisConfigListRequest, AnalysisConfigDeactivateRequest,
+    AnalysisConfig
+)
+from terrascope_api.models.analysis_pb2 import (
+    Analysis, AnalysisCreateRequest, AnalysisGetRequest, AnalysisListRequest
+)
+from terrascope_api.models.analysis_version_pb2 import (
+    AnalysisVersionListRequest, AnalysisVersionGetRequest, AnalysisVersionCreateRequest, AnalysisVersion
+)
 from terrascope_api.models.common_models_pb2 import Pagination
 
 from terrascope.sdk.builder.analysis import AnalysisManifest, AnalysisConfiguration
 from terrascope.sdk.tools.sdk_support import SDKSupport
 
 
 class APIAnalysis:
@@ -407,24 +412,32 @@
         for, metadata can be retrieved, and can still be used in new analysis_computations, but they are no longer
         actively supported.
         :param analysis_config_ids:
         :return:
         """
         pass
 
-    async def deactivate(self, analysis_config_ids: List):
+    async def deactivate(self, analysis_config_ids: List[str]):
         """
         Deactivate the specific configuration of an analysis_version. Deactivated analysis_configs will no longer
         show up in searches, but metadata can still be retrieved for deactivated analysis_configs via the get endpoint.
         Deactivated analysis_configs cannot be used in any new analysis_computations, but existing analysis_computations
          will continue to function properly.
         :param analysis_config_ids:
         :return:
         """
-        pass
+        import pdb
+        pdb.set_trace()
+        analysis_config_deactivate_request = AnalysisConfigDeactivateRequest(
+            ids=analysis_config_ids
+        )
+        analysis_config_deactivate_response = await self.__client.api.analysis_config.deactivate(
+            analysis_config_deactivate_request, timeout=self.__timeout)
+
+        return analysis_config_deactivate_response
 
     async def delete(self, analysis_config_ids: List):
         """
         Delete the specified analysis_config, if and only if it has not been used to create an analysis_computation.
         Once an analysis_config has been used to create an analysis_computation it can never be deleted.
         The user must have permission to access the specified analysis.
         :param analysis_config_ids:
```

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/aoi.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/aoi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/credit.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/credit.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/data.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/data.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/permission.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/permission.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/result.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/result.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/toi.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/toi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/user.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/user.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/api/visualization.py` & `terrascope-sdk-1.0.6/terrascope/sdk/api/visualization.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/builder/algorithm.py` & `terrascope-sdk-1.0.6/terrascope/sdk/builder/algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class DataSource(Enum):
     # Ping Sources
     GEOLOCATION = "geolocation_pings"
     SAFEGRAPH = "safegraph_pings"
     XMODE = "xmode_pings"
     CUEBIQ = "cuebiq_pings"
     BLOGWATCHER = "blogwatcher_pings"
-    SPIRE = "spire"
+    SPIRE = "spire_pings"
     CUEBIQ_WORKBENCH = "cuebiq-workbench_pings"
     WEJO = "wejo_pings"
     HAWKEYE360 = "hawkeye360_pings"
     OTONOMO = "otonomo_pings"
     ADSBX = "adsbx_pings"
     EXACTEARTH = "exact-earth_pings"
     EXACTEARTH_NMEA = "exact-earth_nmea-pings"
@@ -52,15 +52,15 @@
 
     # Imagery Sources
     IMAGERY = "imagery_imagery"
     PLANET_REORTHOTILE = "planet_REOrthoTile"
     PLANET_PSORTHOTILE = "planet_OSOrthoTile"
     PLANET_PSSCENE4BAND = "planet_PSScene4Band"
     PLANET_SKYSATSCENE = "planet_SkySatScene"
-    PLANET_SKYSATCOLLECT = "planet_SkySatCollection"
+    PLANET_SKYSATCOLLECT = "planet_SkySatCollect"
     AIRBUS_SPOT7 = "airbus_SPOT7"
     AIRBUS_PHR1A = "airbus_PHR1A"
     AIRBUS_PHR1B = "airbus_PHR1B"
 
 
 class ReleaseStatus(Enum):
     DEV = "DEV"
@@ -201,14 +201,16 @@
         entry = {
             "data_type_name": data_type_name.value
         }
         if 'min_count' in kwargs.keys():
             entry['min_count'] = kwargs['min_count']
         if 'max_count' in kwargs.keys():
             entry['max_count'] = kwargs['max_count']
+        if 'parameters' in kwargs.keys():
+            entry['parameters'] = kwargs['parameters']
 
         self.__inputs.append(entry.copy())
         self.__required['inputs'] = True
 
     # Container Parameters
     def container_parameters_required(self, image: str, command: List):
         self.container_parameters_image(image=image)
```

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/builder/analysis.py` & `terrascope-sdk-1.0.6/terrascope/sdk/builder/analysis.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/builder/toi.py` & `terrascope-sdk-1.0.6/terrascope/sdk/builder/toi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/terrascope_sdk.py` & `terrascope-sdk-1.0.6/terrascope/sdk/terrascope_sdk.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/tools/io.py` & `terrascope-sdk-1.0.6/terrascope/sdk/tools/io.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope/sdk/tools/sdk_support.py` & `terrascope-sdk-1.0.6/terrascope/sdk/tools/sdk_support.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/terrascope_sdk.egg-info/PKG-INFO` & `terrascope-sdk-1.0.6/terrascope_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrascope-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: A software development kit for developing projects on TerraScope
 Author-email: "Martice E. Nicks III" <martice.nicks@orbitalinsight.com>
 License: Copyright 2022 Orbital Insight, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `terrascope-sdk-1.0.5/terrascope_sdk.egg-info/SOURCES.txt` & `terrascope-sdk-1.0.6/terrascope_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_algorithm.py` & `terrascope-sdk-1.0.6/tests/integration/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_analysis_builder.py` & `terrascope-sdk-1.0.6/tests/integration/test_analysis_builder.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_aoi.py` & `terrascope-sdk-1.0.6/tests/integration/test_aoi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_credit.py` & `terrascope-sdk-1.0.6/tests/integration/test_credit.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_data.py` & `terrascope-sdk-1.0.6/tests/integration/test_data.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_permission.py` & `terrascope-sdk-1.0.6/tests/integration/test_permission.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_result.py` & `terrascope-sdk-1.0.6/tests/integration/test_result.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_sdk_support.py` & `terrascope-sdk-1.0.6/tests/integration/test_sdk_support.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.5/tests/integration/test_toi.py` & `terrascope-sdk-1.0.6/tests/integration/test_toi.py`

 * *Files identical despite different names*

