# Comparing `tmp/antspyt1w-0.9.2.tar.gz` & `tmp/antspyt1w-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspyt1w-0.9.2.tar", last modified: Wed May  8 13:23:01 2024, max compression
+gzip compressed data, was "antspyt1w-0.9.3.tar", last modified: Wed May 22 14:53:30 2024, max compression
```

## Comparing `antspyt1w-0.9.2.tar` & `antspyt1w-0.9.3.tar`

### file list

```diff
@@ -1,30 +1,18 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.601569 antspyt1w-0.9.2/
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.597228 antspyt1w-0.9.2/.circleci/
--rw-r--r--   0 stnava     (501) staff       (20)      760 2021-12-05 18:20:06.000000 antspyt1w-0.9.2/.circleci/config.yml
--rw-r--r--   0 stnava     (501) staff       (20)     1924 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/.gitignore
--rw-r--r--   0 stnava     (501) staff       (20)      119 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/.gitmodules
--rw-r--r--   0 stnava     (501) staff       (20)      519 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/Dockerfile
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)     3409 2024-05-08 13:23:01.601263 antspyt1w-0.9.2/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     3078 2023-12-14 01:09:11.000000 antspyt1w-0.9.2/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.597831 antspyt1w-0.9.2/antspyt1w/
--rw-r--r--   0 stnava     (501) staff       (20)     1573 2023-03-14 13:16:41.000000 antspyt1w-0.9.2/antspyt1w/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   134414 2024-05-08 13:17:46.000000 antspyt1w-0.9.2/antspyt1w/get_data.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.600932 antspyt1w-0.9.2/antspyt1w.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     3409 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      471 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2022-10-05 13:41:34.000000 antspyt1w-0.9.2/antspyt1w.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)       10 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.598967 antspyt1w-0.9.2/docs/
--rw-r--r--   0 stnava     (501) staff       (20)   103244 2023-05-15 15:46:35.000000 antspyt1w-0.9.2/docs/antspyt1w_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      133 2022-01-13 15:53:02.000000 antspyt1w-0.9.2/requirements.txt
--rw-r--r--   0 stnava     (501) staff       (20)       38 2024-05-08 13:23:01.601641 antspyt1w-0.9.2/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      522 2024-05-08 13:09:59.000000 antspyt1w-0.9.2/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.600686 antspyt1w-0.9.2/tests/
--rw-r--r--   0 stnava     (501) staff       (20)      987 2022-03-11 22:33:25.000000 antspyt1w-0.9.2/tests/test_deep_hipp.py
--rw-r--r--   0 stnava     (501) staff       (20)      948 2022-03-12 15:08:32.000000 antspyt1w-0.9.2/tests/test_mtl.py
--rw-r--r--   0 stnava     (501) staff       (20)      675 2022-01-11 18:52:31.000000 antspyt1w-0.9.2/tests/test_rbp.py
--rw-r--r--   0 stnava     (501) staff       (20)     1382 2022-03-18 13:56:41.000000 antspyt1w-0.9.2/tests/test_reference_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      541 2022-01-09 15:31:19.000000 antspyt1w-0.9.2/tests/test_tissueseg.py
--rw-r--r--   0 stnava     (501) staff       (20)     1143 2022-01-04 12:49:35.000000 antspyt1w-0.9.2/tests/test_wmh.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:53:30.415238 antspyt1w-0.9.3/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-17 22:27:29.000000 antspyt1w-0.9.3/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)     3923 2024-05-22 14:53:30.415077 antspyt1w-0.9.3/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     3247 2024-05-22 14:48:25.000000 antspyt1w-0.9.3/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:53:30.413977 antspyt1w-0.9.3/antspyt1w/
+-rw-r--r--   0 stnava     (501) staff       (20)     1573 2023-03-14 13:16:41.000000 antspyt1w-0.9.3/antspyt1w/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   134414 2024-05-08 13:17:46.000000 antspyt1w-0.9.3/antspyt1w/get_data.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:53:30.414895 antspyt1w-0.9.3/antspyt1w.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)     3923 2024-05-22 14:53:30.000000 antspyt1w-0.9.3/antspyt1w.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      291 2024-05-22 14:53:30.000000 antspyt1w-0.9.3/antspyt1w.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2024-05-22 14:53:30.000000 antspyt1w-0.9.3/antspyt1w.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)      162 2024-05-22 14:53:30.000000 antspyt1w-0.9.3/antspyt1w.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       10 2024-05-22 14:53:30.000000 antspyt1w-0.9.3/antspyt1w.egg-info/top_level.txt
+-rw-r--r--   0 stnava     (501) staff       (20)      763 2024-05-22 14:47:25.000000 antspyt1w-0.9.3/pyproject.toml
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2024-05-22 14:53:30.415273 antspyt1w-0.9.3/setup.cfg
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:53:30.414746 antspyt1w-0.9.3/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)       73 2024-05-22 12:44:22.000000 antspyt1w-0.9.3/tests/test_00_setup.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1382 2022-03-18 13:56:41.000000 antspyt1w-0.9.3/tests/test_reference_run.py
```

### Comparing `antspyt1w-0.9.2/LICENSE` & `antspyt1w-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.2/PKG-INFO` & `antspyt1w-0.9.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: antspyt1w
-Version: 0.9.2
-Summary: T1w human neuroimage processing with antspyx
-Home-page: https://github.com/stnava/ANTsPyT1w
-Author: Avants, Gosselin, Tustison
-Author-email: stnava@gmail.com
-License: Apache 2.0
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENSE
-
 # ANTsPyT1w
 
 [![CircleCI](https://circleci.com/gh/stnava/ANTsPyT1w/tree/master.svg?style=svg)](https://circleci.com/gh/stnava/ANTsPyT1w/tree/master)
 
 ## reference processing for t1-weighted neuroimages (human)
 
 the outputs of these processes can be used for data inspection/cleaning/triage
@@ -113,11 +102,16 @@
 ```python
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
 ```
 
 ## to publish a release
 
+before doing this - make sure you have a recent run of `pip-compile pyproject.toml`
+
 ```
-python3 -m build
-python -m twine upload -u username -p password  dist/*
+rm -r -f build/ antspyt1w.egg-info/ dist/
+python3 -m  build .
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository antspyt1w dist/*
 ```
+
```

### Comparing `antspyt1w-0.9.2/antspyt1w/__init__.py` & `antspyt1w-0.9.3/antspyt1w/__init__.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.2/antspyt1w/get_data.py` & `antspyt1w-0.9.3/antspyt1w/get_data.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.2/antspyt1w.egg-info/PKG-INFO` & `antspyt1w-0.9.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 Metadata-Version: 2.1
 Name: antspyt1w
-Version: 0.9.2
+Version: 0.9.3
 Summary: T1w human neuroimage processing with antspyx
-Home-page: https://github.com/stnava/ANTsPyT1w
-Author: Avants, Gosselin, Tustison
-Author-email: stnava@gmail.com
+Author-email: "Avants, Gosselin, Tustison" <stnava@gmail.com>
 License: Apache 2.0
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/stnava/ANTsPyT1w
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: h5py>=3.10.0
+Requires-Dist: numpy>=1.19.4
+Requires-Dist: pandas>=1.0.1
+Requires-Dist: antspyx>=0.2.7
+Requires-Dist: antspynet>=0.2.5
+Requires-Dist: tensorflow-probability[tf]
+Requires-Dist: pathlib
+Requires-Dist: PyNomaly>=0.3.3
+Requires-Dist: pytest>=8.0.1
+Requires-Dist: scipy
+Requires-Dist: pillow
+Requires-Dist: matplotlib
 
 # ANTsPyT1w
 
 [![CircleCI](https://circleci.com/gh/stnava/ANTsPyT1w/tree/master.svg?style=svg)](https://circleci.com/gh/stnava/ANTsPyT1w/tree/master)
 
 ## reference processing for t1-weighted neuroimages (human)
 
@@ -113,11 +125,16 @@
 ```python
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
 ```
 
 ## to publish a release
 
+before doing this - make sure you have a recent run of `pip-compile pyproject.toml`
+
 ```
-python3 -m build
-python -m twine upload -u username -p password  dist/*
+rm -r -f build/ antspyt1w.egg-info/ dist/
+python3 -m  build .
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository antspyt1w dist/*
 ```
+
```

### Comparing `antspyt1w-0.9.2/tests/test_reference_run.py` & `antspyt1w-0.9.3/tests/test_reference_run.py`

 * *Files identical despite different names*

