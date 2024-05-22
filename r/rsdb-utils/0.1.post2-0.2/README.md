# Comparing `tmp/rsdb_utils-0.1.post2.tar.gz` & `tmp/rsdb_utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsdb_utils-0.1.post2.tar", last modified: Wed May 22 12:25:36 2024, max compression
+gzip compressed data, was "rsdb_utils-0.2.tar", last modified: Wed May 22 14:35:12 2024, max compression
```

## Comparing `rsdb_utils-0.1.post2.tar` & `rsdb_utils-0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.074630 rsdb_utils-0.1.post2/
--rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.1.post2/LICENCE.txt
--rw-r--r--   0 romain    (1000) romain    (1000)    45543 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)     3938 2024-05-22 12:12:03.000000 rsdb_utils-0.1.post2/README.md
--rw-rw-r--   0 romain    (1000) romain    (1000)     1224 2024-05-22 12:25:09.000000 rsdb_utils-0.1.post2/pyproject.toml
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/rsdb_utils/
--rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.1.post2/rsdb_utils/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     7383 2024-05-22 11:43:12.000000 rsdb_utils-0.1.post2/rsdb_utils/utils.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/rsdb_utils.egg-info/
--rw-r--r--   0 romain    (1000) romain    (1000)    45543 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      263 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/top_level.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 12:25:36.074630 rsdb_utils-0.1.post2/setup.cfg
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/tests/
--rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.1.post2/tests/tests.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 14:35:12.499627 rsdb_utils-0.2/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.2/LICENCE.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       54 2024-05-22 13:30:20.000000 rsdb_utils-0.2/MANIFEST.in
+-rw-r--r--   0 romain    (1000) romain    (1000)    45537 2024-05-22 14:35:12.499627 rsdb_utils-0.2/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)     3938 2024-05-22 12:12:03.000000 rsdb_utils-0.2/README.md
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1246 2024-05-22 13:33:28.000000 rsdb_utils-0.2/pyproject.toml
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 14:35:12.499627 rsdb_utils-0.2/rsdb_utils/
+-rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.2/rsdb_utils/__init__.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 14:35:12.499627 rsdb_utils-0.2/rsdb_utils/rsdb-schema/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    26502 2024-05-22 13:26:55.000000 rsdb_utils-0.2/rsdb_utils/rsdb-schema/case_study_schema.json
+-rw-rw-r--   0 romain    (1000) romain    (1000)     7324 2024-05-22 14:32:36.000000 rsdb_utils-0.2/rsdb_utils/utils.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 14:35:12.499627 rsdb_utils-0.2/rsdb_utils.egg-info/
+-rw-r--r--   0 romain    (1000) romain    (1000)    45537 2024-05-22 14:35:12.000000 rsdb_utils-0.2/rsdb_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      321 2024-05-22 14:35:12.000000 rsdb_utils-0.2/rsdb_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 14:35:12.000000 rsdb_utils-0.2/rsdb_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 14:35:12.000000 rsdb_utils-0.2/rsdb_utils.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 14:35:12.000000 rsdb_utils-0.2/rsdb_utils.egg-info/top_level.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 14:35:12.499627 rsdb_utils-0.2/setup.cfg
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 14:35:12.499627 rsdb_utils-0.2/tests/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.2/tests/tests.py
```

### Comparing `rsdb_utils-0.1.post2/LICENCE.txt` & `rsdb_utils-0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1.post2/PKG-INFO` & `rsdb_utils-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.1.post2
+Version: 0.2
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rsdb_utils-0.1.post2/README.md` & `rsdb_utils-0.2/README.md`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1.post2/pyproject.toml` & `rsdb_utils-0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsdb-utils"
-version = "0.1.post2"
+version = "0.2"
 description = "Utils to process the Regime Shifts DataBase CSV and parquet files"
 readme = "README.md"
 authors = [{ name = "Romain Thomas", email = "romain.thomas@su.se" }]
 license = {file = "LICENCE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -35,12 +35,13 @@
     "jsonschema>=4.22.0",
     "tqdm>=4.50.0",
     "pyarrow"
 ]
 requires-python = ">=3.9"
 
 [tool.setuptools]
+include-package-data = true
 packages = ["rsdb_utils"]
 
 [project.urls]
 Homepage = "https://github.com/regimeshifts/rsdb-utils"
 "Project website" = "https://www.regimeshifts.org/"
```

### Comparing `rsdb_utils-0.1.post2/rsdb_utils/utils.py` & `rsdb_utils-0.2/rsdb_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # Romain THOMAS 2024
 # Stockholm Resilience Centre
 # GNU General Public License v3 (GPLv3)
 
 import json
 import warnings
+import pkgutil
 
 import pandas as pd
 import numpy as np
 
 from tqdm import tqdm
 
 import jsonref  # dereferencing of JSON Reference
 from jsonschema import Draft202012Validator
 
-# replace with API call, package data or GitHub http download and cache
-schema_path = "../rsdb-schema/case_study_schema.json"
+# Load the JSON schema from the package data with all the references (defs)
+schema_path = "rsdb-schema/case_study_schema.json"
+rs_cs_schema = jsonref.loads(pkgutil.get_data(__name__, schema_path).decode('utf-8'))
 
-# Load the JSON schema
-with open(schema_path) as f:
-    # rs_cs_schema = json.load(f)
-    rs_cs_schema = f.read()
-    rs_cs_schema = jsonref.loads(rs_cs_schema)
 first_level_fields_in_schema = list(rs_cs_schema['properties'].keys())
 # check if the schema is valid
 Draft202012Validator.check_schema(rs_cs_schema)
 # create the JSON schema validator
 rs_cs_validator = Draft202012Validator(rs_cs_schema)
```

### Comparing `rsdb_utils-0.1.post2/rsdb_utils.egg-info/PKG-INFO` & `rsdb_utils-0.2/rsdb_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.1.post2
+Version: 0.2
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rsdb_utils-0.1.post2/tests/tests.py` & `rsdb_utils-0.2/tests/tests.py`

 * *Files identical despite different names*

