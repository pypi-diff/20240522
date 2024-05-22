# Comparing `tmp/tgedr-dataops-0.0.8.tar.gz` & `tmp/tgedr-dataops-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgedr-dataops-0.0.8.tar", last modified: Thu Feb  1 09:53:03 2024, max compression
+gzip compressed data, was "tgedr-dataops-0.0.9.tar", last modified: Thu Feb  1 09:58:14 2024, max compression
```

## Comparing `tgedr-dataops-0.0.8.tar` & `tgedr-dataops-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:53:03.598631 tgedr-dataops-0.0.8/
--rw-r--r--   0 runner     (501) staff       (20)     1211 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      509 2024-02-01 09:53:03.598147 tgedr-dataops-0.0.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)       39 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/README.md
--rw-r--r--   0 runner     (501) staff       (20)      404 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-02-01 09:53:03.598711 tgedr-dataops-0.0.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      903 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:53:03.590620 tgedr-dataops-0.0.8/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:53:03.593176 tgedr-dataops-0.0.8/src/tgedr/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:53:03.595518 tgedr-dataops-0.0.8/src/tgedr/dataops/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1405 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/chain.py
--rw-r--r--   0 runner     (501) staff       (20)     3204 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/etl.py
--rw-r--r--   0 runner     (501) staff       (20)      710 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/processor.py
--rw-r--r--   0 runner     (501) staff       (20)      885 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/sink.py
--rw-r--r--   0 runner     (501) staff       (20)      897 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/source.py
--rw-r--r--   0 runner     (501) staff       (20)     4136 2024-02-01 09:51:08.000000 tgedr-dataops-0.0.8/src/tgedr/dataops/utils_reflection.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:53:03.597664 tgedr-dataops-0.0.8/src/tgedr_dataops.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      509 2024-02-01 09:53:03.000000 tgedr-dataops-0.0.8/src/tgedr_dataops.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      472 2024-02-01 09:53:03.000000 tgedr-dataops-0.0.8/src/tgedr_dataops.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-01 09:53:03.000000 tgedr-dataops-0.0.8/src/tgedr_dataops.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       25 2024-02-01 09:53:03.000000 tgedr-dataops-0.0.8/src/tgedr_dataops.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-02-01 09:53:03.000000 tgedr-dataops-0.0.8/src/tgedr_dataops.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:58:14.154606 tgedr-dataops-0.0.9/
+-rw-r--r--   0 runner     (501) staff       (20)     1211 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      511 2024-02-01 09:58:14.153978 tgedr-dataops-0.0.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)       39 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      404 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-02-01 09:58:14.154716 tgedr-dataops-0.0.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      905 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:58:14.143415 tgedr-dataops-0.0.9/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:58:14.146487 tgedr-dataops-0.0.9/src/tgedr/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:58:14.149941 tgedr-dataops-0.0.9/src/tgedr/dataops/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1405 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/chain.py
+-rw-r--r--   0 runner     (501) staff       (20)     3204 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/etl.py
+-rw-r--r--   0 runner     (501) staff       (20)      710 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/processor.py
+-rw-r--r--   0 runner     (501) staff       (20)      885 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/sink.py
+-rw-r--r--   0 runner     (501) staff       (20)      897 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/source.py
+-rw-r--r--   0 runner     (501) staff       (20)     4136 2024-02-01 09:56:37.000000 tgedr-dataops-0.0.9/src/tgedr/dataops/utils_reflection.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-01 09:58:14.153280 tgedr-dataops-0.0.9/src/tgedr_dataops.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      511 2024-02-01 09:58:14.000000 tgedr-dataops-0.0.9/src/tgedr_dataops.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      472 2024-02-01 09:58:14.000000 tgedr-dataops-0.0.9/src/tgedr_dataops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-01 09:58:14.000000 tgedr-dataops-0.0.9/src/tgedr_dataops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       27 2024-02-01 09:58:14.000000 tgedr-dataops-0.0.9/src/tgedr_dataops.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-02-01 09:58:14.000000 tgedr-dataops-0.0.9/src/tgedr_dataops.egg-info/top_level.txt
```

### Comparing `tgedr-dataops-0.0.8/LICENSE` & `tgedr-dataops-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tgedr-dataops-0.0.8/setup.py` & `tgedr-dataops-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 
 from setuptools import setup, find_namespace_packages
 
 logger = logging.getLogger(__name__)
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 logging.info(f"building version: {VERSION}")
 
 setup(
     name='tgedr-dataops',
     version=VERSION,
     description='data operations related code',
     url='https://github.com/jtviegas-sandbox/dataops',
@@ -21,13 +21,13 @@
     'Programming Language :: Python :: 3.10'
     ],
     keywords='data engineering mlops ml',
     include_package_data=True,
     package_dir={"": "src"},
     packages=find_namespace_packages(where="src"),
     install_requires=[
-        "pyarrow==14",
+        "pyarrow==15.*",
         "pyspark==3.5"
     ],
     python_requires='>=3.9',
     # package_data={'sample': ['package_data.dat'],},
 )
```

### Comparing `tgedr-dataops-0.0.8/src/tgedr/dataops/chain.py` & `tgedr-dataops-0.0.9/src/tgedr/dataops/chain.py`

 * *Files identical despite different names*

### Comparing `tgedr-dataops-0.0.8/src/tgedr/dataops/etl.py` & `tgedr-dataops-0.0.9/src/tgedr/dataops/etl.py`

 * *Files identical despite different names*

### Comparing `tgedr-dataops-0.0.8/src/tgedr/dataops/processor.py` & `tgedr-dataops-0.0.9/src/tgedr/dataops/processor.py`

 * *Files identical despite different names*

### Comparing `tgedr-dataops-0.0.8/src/tgedr/dataops/sink.py` & `tgedr-dataops-0.0.9/src/tgedr/dataops/sink.py`

 * *Files identical despite different names*

### Comparing `tgedr-dataops-0.0.8/src/tgedr/dataops/source.py` & `tgedr-dataops-0.0.9/src/tgedr/dataops/source.py`

 * *Files identical despite different names*

### Comparing `tgedr-dataops-0.0.8/src/tgedr/dataops/utils_reflection.py` & `tgedr-dataops-0.0.9/src/tgedr/dataops/utils_reflection.py`

 * *Files identical despite different names*

