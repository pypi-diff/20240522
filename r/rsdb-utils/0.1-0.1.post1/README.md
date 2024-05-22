# Comparing `tmp/rsdb_utils-0.1.tar.gz` & `tmp/rsdb_utils-0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsdb_utils-0.1.tar", last modified: Wed May 22 11:59:40 2024, max compression
+gzip compressed data, was "rsdb_utils-0.1.post1.tar", last modified: Wed May 22 12:14:17 2024, max compression
```

## Comparing `rsdb_utils-0.1.tar` & `rsdb_utils-0.1.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 11:59:40.095019 rsdb_utils-0.1/
--rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.1/LICENCE.txt
--rw-r--r--   0 romain    (1000) romain    (1000)    45160 2024-05-22 11:59:40.095019 rsdb_utils-0.1/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)     3564 2024-05-22 11:56:53.000000 rsdb_utils-0.1/README.md
--rw-rw-r--   0 romain    (1000) romain    (1000)     1215 2024-05-22 11:59:32.000000 rsdb_utils-0.1/pyproject.toml
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 11:59:40.095019 rsdb_utils-0.1/rsdb_utils/
--rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.1/rsdb_utils/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     7383 2024-05-22 11:43:12.000000 rsdb_utils-0.1/rsdb_utils/utils.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 11:59:40.095019 rsdb_utils-0.1/rsdb_utils.egg-info/
--rw-r--r--   0 romain    (1000) romain    (1000)    45160 2024-05-22 11:59:40.000000 rsdb_utils-0.1/rsdb_utils.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      263 2024-05-22 11:59:40.000000 rsdb_utils-0.1/rsdb_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 11:59:40.000000 rsdb_utils-0.1/rsdb_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 11:59:40.000000 rsdb_utils-0.1/rsdb_utils.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 11:59:40.000000 rsdb_utils-0.1/rsdb_utils.egg-info/top_level.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 11:59:40.095019 rsdb_utils-0.1/setup.cfg
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 11:59:40.095019 rsdb_utils-0.1/tests/
--rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.1/tests/tests.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.1.post1/LICENCE.txt
+-rw-r--r--   0 romain    (1000) romain    (1000)    45540 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)     3938 2024-05-22 12:12:03.000000 rsdb_utils-0.1.post1/README.md
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1221 2024-05-22 12:12:58.000000 rsdb_utils-0.1.post1/pyproject.toml
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/rsdb_utils/
+-rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.1.post1/rsdb_utils/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     7383 2024-05-22 11:43:12.000000 rsdb_utils-0.1.post1/rsdb_utils/utils.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/rsdb_utils.egg-info/
+-rw-r--r--   0 romain    (1000) romain    (1000)    45540 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      263 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/top_level.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 12:14:17.065647 rsdb_utils-0.1.post1/setup.cfg
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/tests/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.1.post1/tests/tests.py
```

### Comparing `rsdb_utils-0.1/LICENCE.txt` & `rsdb_utils-0.1.post1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1/PKG-INFO` & `rsdb_utils-0.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.1
+Version: 0.1.post1
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -704,14 +704,16 @@
 
 Functionalities:
 
   - Import the database from a CSV or parquet file in a pandas DataFrame
   - Save the database in a CSV or parquet file from a pandas DataFrame
   - Check the database (a DataFrame) with the json schema or the Regime Shifts DataBase
 
+Code repository: [https://github.com/regimeshifts/rsdb-utils](https://github.com/regimeshifts/rsdb-utils)
+
 Licence: GNU General Public License v3 (GPLv3)
 
 ## Installation
 
 ### From Python
 In a terminal:
 ```bash
@@ -851,15 +853,25 @@
 
 ```bash
 pytest tests/tests.py
 ```
 
 ### Build
 
-In the development virtual environment:
+In the development virtual environment, install:
 ```bash
 pip install build twine
 ```
 
+Then build the package:
+```bash
+python3 -m build
+```
+
+Configure your pypi access token and publish the package version:
+```bash
+twine upload dist/rsdb_utils-0.1.tar.gz dist/rsdb_utils-0.1-py3-none-any.whl
+```
+Once published, a version cannot be re-uploaded.
 
 Romain THOMAS 2024  
 Stockholm Resilience Centre
```

### Comparing `rsdb_utils-0.1/README.md` & `rsdb_utils-0.1.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Functionalities:
 
   - Import the database from a CSV or parquet file in a pandas DataFrame
   - Save the database in a CSV or parquet file from a pandas DataFrame
   - Check the database (a DataFrame) with the json schema or the Regime Shifts DataBase
 
+Code repository: [https://github.com/regimeshifts/rsdb-utils](https://github.com/regimeshifts/rsdb-utils)
+
 Licence: GNU General Public License v3 (GPLv3)
 
 ## Installation
 
 ### From Python
 In a terminal:
 ```bash
@@ -151,15 +153,25 @@
 
 ```bash
 pytest tests/tests.py
 ```
 
 ### Build
 
-In the development virtual environment:
+In the development virtual environment, install:
 ```bash
 pip install build twine
 ```
 
+Then build the package:
+```bash
+python3 -m build
+```
+
+Configure your pypi access token and publish the package version:
+```bash
+twine upload dist/rsdb_utils-0.1.tar.gz dist/rsdb_utils-0.1-py3-none-any.whl
+```
+Once published, a version cannot be re-uploaded.
 
 Romain THOMAS 2024  
 Stockholm Resilience Centre
```

### Comparing `rsdb_utils-0.1/pyproject.toml` & `rsdb_utils-0.1.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsdb-utils"
-version = "0.1"
+version = "0.1.post1"
 description = "Utils to process the Regime Shifts DataBase CSV and parquet files"
 readme = "README.md"
 authors = [{ name = "Romain Thomas", email = "romain.thomas@su.se" }]
 license = {file = "LICENCE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `rsdb_utils-0.1/rsdb_utils/utils.py` & `rsdb_utils-0.1.post1/rsdb_utils/utils.py`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1/rsdb_utils.egg-info/PKG-INFO` & `rsdb_utils-0.1.post1/rsdb_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.1
+Version: 0.1.post1
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -704,14 +704,16 @@
 
 Functionalities:
 
   - Import the database from a CSV or parquet file in a pandas DataFrame
   - Save the database in a CSV or parquet file from a pandas DataFrame
   - Check the database (a DataFrame) with the json schema or the Regime Shifts DataBase
 
+Code repository: [https://github.com/regimeshifts/rsdb-utils](https://github.com/regimeshifts/rsdb-utils)
+
 Licence: GNU General Public License v3 (GPLv3)
 
 ## Installation
 
 ### From Python
 In a terminal:
 ```bash
@@ -851,15 +853,25 @@
 
 ```bash
 pytest tests/tests.py
 ```
 
 ### Build
 
-In the development virtual environment:
+In the development virtual environment, install:
 ```bash
 pip install build twine
 ```
 
+Then build the package:
+```bash
+python3 -m build
+```
+
+Configure your pypi access token and publish the package version:
+```bash
+twine upload dist/rsdb_utils-0.1.tar.gz dist/rsdb_utils-0.1-py3-none-any.whl
+```
+Once published, a version cannot be re-uploaded.
 
 Romain THOMAS 2024  
 Stockholm Resilience Centre
```

### Comparing `rsdb_utils-0.1/tests/tests.py` & `rsdb_utils-0.1.post1/tests/tests.py`

 * *Files identical despite different names*

