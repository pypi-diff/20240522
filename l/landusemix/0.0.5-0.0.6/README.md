# Comparing `tmp/landusemix-0.0.5.tar.gz` & `tmp/landusemix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landusemix-0.0.5.tar", last modified: Wed May 22 02:01:04 2024, max compression
+gzip compressed data, was "landusemix-0.0.6.tar", last modified: Wed May 22 02:06:41 2024, max compression
```

## Comparing `landusemix-0.0.5.tar` & `landusemix-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.870686 landusemix-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:01:01.000000 landusemix-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:01:04.870686 landusemix-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 02:01:01.000000 landusemix-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.866686 landusemix-0.0.5/landusemix/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:01:01.000000 landusemix-0.0.5/landusemix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 02:01:01.000000 landusemix-0.0.5/landusemix/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 02:01:01.000000 landusemix-0.0.5/landusemix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.870686 landusemix-0.0.5/landusemix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:01:04.870686 landusemix-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 02:01:01.000000 landusemix-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.870686 landusemix-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:01.000000 landusemix-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 02:01:01.000000 landusemix-0.0.5/tests/test_landusemix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:06:41.869756 landusemix-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:06:38.000000 landusemix-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:06:41.869756 landusemix-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 02:06:38.000000 landusemix-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:06:41.865756 landusemix-0.0.6/landusemix/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:06:38.000000 landusemix-0.0.6/landusemix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 02:06:38.000000 landusemix-0.0.6/landusemix/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 02:06:38.000000 landusemix-0.0.6/landusemix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:06:41.869756 landusemix-0.0.6/landusemix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:06:41.000000 landusemix-0.0.6/landusemix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 02:06:41.000000 landusemix-0.0.6/landusemix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:06:41.000000 landusemix-0.0.6/landusemix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:06:41.000000 landusemix-0.0.6/landusemix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:06:41.000000 landusemix-0.0.6/landusemix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:06:41.869756 landusemix-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-22 02:06:38.000000 landusemix-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:06:41.869756 landusemix-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:06:38.000000 landusemix-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 02:06:38.000000 landusemix-0.0.6/tests/test_landusemix.py
```

### Comparing `landusemix-0.0.5/LICENSE` & `landusemix-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.5/PKG-INFO` & `landusemix-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.5/README.md` & `landusemix-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.5/landusemix/indices.py` & `landusemix-0.0.6/landusemix/indices.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.5/landusemix/utils.py` & `landusemix-0.0.6/landusemix/utils.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.5/landusemix.egg-info/PKG-INFO` & `landusemix-0.0.6/landusemix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.5/setup.py` & `landusemix-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import glob
 from setuptools import setup, find_packages
 
 setup(
     name="landusemix",
-    version="0.0.5",
+    version="0.0.6",
     author="Mehmet Ali Akyol",
     author_email="akyol.mehmet@metu.edu.tr",
     description="A package for calculating land use mix indices",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/makyol/landusemix",
     packages=find_packages(),
     include_package_data=True,
-    package_data={'landusemix': ['data/']},
+    package_data={'landusemix': glob.glob('landusemix/data/*')},
     install_requires=[
         'pandas',
         'geopandas',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `landusemix-0.0.5/tests/test_landusemix.py` & `landusemix-0.0.6/tests/test_landusemix.py`

 * *Files identical despite different names*

