# Comparing `tmp/landusemix-0.0.4.tar.gz` & `tmp/landusemix-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landusemix-0.0.4.tar", last modified: Wed May 22 01:52:39 2024, max compression
+gzip compressed data, was "landusemix-0.0.5.tar", last modified: Wed May 22 02:01:04 2024, max compression
```

## Comparing `landusemix-0.0.4.tar` & `landusemix-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 01:52:36.000000 landusemix-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 01:52:39.173718 landusemix-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 01:52:36.000000 landusemix-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/landusemix/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 01:52:36.000000 landusemix-0.0.4/landusemix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 01:52:36.000000 landusemix-0.0.4/landusemix/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 01:52:36.000000 landusemix-0.0.4/landusemix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/landusemix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:52:39.173718 landusemix-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 01:52:36.000000 landusemix-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:36.000000 landusemix-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 01:52:36.000000 landusemix-0.0.4/tests/test_landusemix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.870686 landusemix-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:01:01.000000 landusemix-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:01:04.870686 landusemix-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 02:01:01.000000 landusemix-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.866686 landusemix-0.0.5/landusemix/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:01:01.000000 landusemix-0.0.5/landusemix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 02:01:01.000000 landusemix-0.0.5/landusemix/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 02:01:01.000000 landusemix-0.0.5/landusemix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.870686 landusemix-0.0.5/landusemix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:01:04.000000 landusemix-0.0.5/landusemix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:01:04.870686 landusemix-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 02:01:01.000000 landusemix-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:04.870686 landusemix-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:01:01.000000 landusemix-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 02:01:01.000000 landusemix-0.0.5/tests/test_landusemix.py
```

### Comparing `landusemix-0.0.4/LICENSE` & `landusemix-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.4/PKG-INFO` & `landusemix-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.4/README.md` & `landusemix-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.4/landusemix/indices.py` & `landusemix-0.0.5/landusemix/indices.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.4/landusemix/utils.py` & `landusemix-0.0.5/landusemix/utils.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.4/landusemix.egg-info/PKG-INFO` & `landusemix-0.0.5/landusemix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.4/setup.py` & `landusemix-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="landusemix",
-    version="0.0.4",
+    version="0.0.5",
     author="Mehmet Ali Akyol",
     author_email="akyol.mehmet@metu.edu.tr",
     description="A package for calculating land use mix indices",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/makyol/landusemix",
     packages=find_packages(),
     include_package_data=True,
+    package_data={'landusemix': ['data/']},
     install_requires=[
         'pandas',
         'geopandas',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `landusemix-0.0.4/tests/test_landusemix.py` & `landusemix-0.0.5/tests/test_landusemix.py`

 * *Files identical despite different names*

