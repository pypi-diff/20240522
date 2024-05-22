# Comparing `tmp/PheTK-0.1.40.tar.gz` & `tmp/PheTK-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PheTK-0.1.40.tar", last modified: Wed May 15 03:01:46 2024, max compression
+gzip compressed data, was "PheTK-0.1.41.tar", last modified: Wed May 22 10:00:49 2024, max compression
```

## Comparing `PheTK-0.1.40.tar` & `PheTK-0.1.41.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.284661 PheTK-0.1.40/
--rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.40/LICENSE
--rw-r--r--   0 trantac  (1207383791) 1360859114    17202 2024-05-15 03:01:46.284440 PheTK-0.1.40/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114    16920 2024-05-15 03:00:29.000000 PheTK-0.1.40/README.md
--rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-05-15 03:01:46.284758 PheTK-0.1.40/setup.cfg
--rw-r--r--   0 trantac  (1207383791) 1360859114      950 2024-05-15 03:00:29.000000 PheTK-0.1.40/setup.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.239976 PheTK-0.1.40/src/
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.248034 PheTK-0.1.40/src/PheTK/
--rw-r--r--   0 trantac  (1207383791) 1360859114    16590 2024-05-15 03:00:29.000000 PheTK-0.1.40/src/PheTK/Cohort.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.40/src/PheTK/Demo.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/PheWAS.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/Phecode.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/Plot.py
--rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.40/src/PheTK/__init__.py
--rw-r--r--   0 trantac  (1207383791) 1360859114      526 2024-05-12 19:15:55.000000 PheTK-0.1.40/src/PheTK/_paths.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/_queries.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.40/src/PheTK/_utils.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.277615 PheTK-0.1.40/src/PheTK/phecode/
--rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.40/src/PheTK/phecode/phecode12.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.40/src/PheTK/phecode/phecodeX.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.40/src/PheTK/phecode/phecodeX_WHO.csv
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.252902 PheTK-0.1.40/src/PheTK.egg-info/
--rw-r--r--   0 trantac  (1207383791) 1360859114    17202 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/SOURCES.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/dependency_links.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114      120 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/requires.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/top_level.txt
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-22 10:00:49.011824 PheTK-0.1.41/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.41/LICENSE
+-rw-r--r--   0 trantac  (1207383791) 1360859114    17362 2024-05-22 10:00:49.011546 PheTK-0.1.41/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114    17080 2024-05-22 09:56:40.000000 PheTK-0.1.41/README.md
+-rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-05-22 10:00:49.011872 PheTK-0.1.41/setup.cfg
+-rw-r--r--   0 trantac  (1207383791) 1360859114      959 2024-05-22 10:00:12.000000 PheTK-0.1.41/setup.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-22 10:00:48.969527 PheTK-0.1.41/src/
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-22 10:00:48.975176 PheTK-0.1.41/src/PheTK/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16590 2024-05-15 03:00:29.000000 PheTK-0.1.41/src/PheTK/Cohort.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.41/src/PheTK/Demo.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-05-15 02:39:18.000000 PheTK-0.1.41/src/PheTK/PheWAS.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-05-15 02:39:18.000000 PheTK-0.1.41/src/PheTK/Phecode.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-05-15 02:39:18.000000 PheTK-0.1.41/src/PheTK/Plot.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.41/src/PheTK/__init__.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114      526 2024-05-12 19:15:55.000000 PheTK-0.1.41/src/PheTK/_paths.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-05-15 02:39:18.000000 PheTK-0.1.41/src/PheTK/_queries.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.41/src/PheTK/_utils.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-22 10:00:49.003396 PheTK-0.1.41/src/PheTK/phecode/
+-rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.41/src/PheTK/phecode/phecode12.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.41/src/PheTK/phecode/phecodeX.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.41/src/PheTK/phecode/phecodeX_WHO.csv
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-22 10:00:48.976806 PheTK-0.1.41/src/PheTK.egg-info/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    17362 2024-05-22 10:00:48.000000 PheTK-0.1.41/src/PheTK.egg-info/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-05-22 10:00:48.000000 PheTK-0.1.41/src/PheTK.egg-info/SOURCES.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-05-22 10:00:48.000000 PheTK-0.1.41/src/PheTK.egg-info/dependency_links.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114      129 2024-05-22 10:00:48.000000 PheTK-0.1.41/src/PheTK.egg-info/requires.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-05-22 10:00:48.000000 PheTK-0.1.41/src/PheTK.egg-info/top_level.txt
```

### Comparing `PheTK-0.1.40/LICENSE` & `PheTK-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/PKG-INFO` & `PheTK-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PheTK
-Version: 0.1.40
+Version: 0.1.41
 Summary: The Phenotype Toolkit
 Home-page: https://github.com/nhgritctran/PheTK
 Author: Tam Tran
 Author-email: PheTK@mail.nih.gov
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -13,14 +13,17 @@
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
 Current version: 0.1.40
 
 ## Changelog:
 
+___version 0.1.41 (22 May 2024):___
+- Added polars version <= 0.20.26 as dependency requirement since polars version 0.20.27 could cause multithreading issue.
+
 ___version 0.1.40 (14 May 2024):___
 - Fixed an incorrect printout text check in `.by_genotype()` in Cohort module when a variant is not found. 
 This is only an aesthetic fix to avoid confusion, and does not affect previously generated cohorts.
 
 ___version 0.1.39 (02 May 2024):___
 - Added lxml as a required dependency during installation as it might not be preinstalled in some platforms.
```

### Comparing `PheTK-0.1.40/README.md` & `PheTK-0.1.41/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
 Current version: 0.1.40
 
 ## Changelog:
 
+___version 0.1.41 (22 May 2024):___
+- Added polars version <= 0.20.26 as dependency requirement since polars version 0.20.27 could cause multithreading issue.
+
 ___version 0.1.40 (14 May 2024):___
 - Fixed an incorrect printout text check in `.by_genotype()` in Cohort module when a variant is not found. 
 This is only an aesthetic fix to avoid confusion, and does not affect previously generated cohorts.
 
 ___version 0.1.39 (02 May 2024):___
 - Added lxml as a required dependency during installation as it might not be preinstalled in some platforms.
```

### Comparing `PheTK-0.1.40/setup.py` & `PheTK-0.1.41/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read contents of the README.md file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PheTK',
-    version='0.1.40',
+    version='0.1.41',
     python_requires='>=3.7',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={
         '': ['*.*'],
         'PheTK': ['phecode/*'],
     },
@@ -27,13 +27,13 @@
         "google-cloud-bigquery",
         "hail",
         "lifelines",
         "lxml",
         "matplotlib",
         "numpy",
         "pandas",
-        "polars",
+        "polars<=0.20.26",
         "pyarrow",
         "statsmodels",
         "tqdm"
     ]
 )
```

### Comparing `PheTK-0.1.40/src/PheTK/Cohort.py` & `PheTK-0.1.41/src/PheTK/Cohort.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/Demo.py` & `PheTK-0.1.41/src/PheTK/Demo.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/PheWAS.py` & `PheTK-0.1.41/src/PheTK/PheWAS.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/Phecode.py` & `PheTK-0.1.41/src/PheTK/Phecode.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/Plot.py` & `PheTK-0.1.41/src/PheTK/Plot.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/_paths.py` & `PheTK-0.1.41/src/PheTK/_paths.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/_queries.py` & `PheTK-0.1.41/src/PheTK/_queries.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/_utils.py` & `PheTK-0.1.41/src/PheTK/_utils.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/phecode/phecode12.csv` & `PheTK-0.1.41/src/PheTK/phecode/phecode12.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/phecode/phecodeX.csv` & `PheTK-0.1.41/src/PheTK/phecode/phecodeX.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK/phecode/phecodeX_WHO.csv` & `PheTK-0.1.41/src/PheTK/phecode/phecodeX_WHO.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.40/src/PheTK.egg-info/PKG-INFO` & `PheTK-0.1.41/src/PheTK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PheTK
-Version: 0.1.40
+Version: 0.1.41
 Summary: The Phenotype Toolkit
 Home-page: https://github.com/nhgritctran/PheTK
 Author: Tam Tran
 Author-email: PheTK@mail.nih.gov
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -13,14 +13,17 @@
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
 Current version: 0.1.40
 
 ## Changelog:
 
+___version 0.1.41 (22 May 2024):___
+- Added polars version <= 0.20.26 as dependency requirement since polars version 0.20.27 could cause multithreading issue.
+
 ___version 0.1.40 (14 May 2024):___
 - Fixed an incorrect printout text check in `.by_genotype()` in Cohort module when a variant is not found. 
 This is only an aesthetic fix to avoid confusion, and does not affect previously generated cohorts.
 
 ___version 0.1.39 (02 May 2024):___
 - Added lxml as a required dependency during installation as it might not be preinstalled in some platforms.
```

