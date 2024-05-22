# Comparing `tmp/landusemix-0.0.7.tar.gz` & `tmp/landusemix-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landusemix-0.0.7.tar", last modified: Wed May 22 02:22:24 2024, max compression
+gzip compressed data, was "landusemix-0.0.8.tar", last modified: Wed May 22 02:34:33 2024, max compression
```

## Comparing `landusemix-0.0.7.tar` & `landusemix-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.224805 landusemix-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:22:21.000000 landusemix-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 02:22:21.000000 landusemix-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:22:24.224805 landusemix-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 02:22:21.000000 landusemix-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.216805 landusemix-0.0.7/landusemix/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.220805 landusemix-0.0.7/landusemix/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.220805 landusemix-0.0.7/landusemix/data/geojson/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/geojson/half.geojson
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/geojson/multiple.geojson
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/geojson/one.geojson
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.216805 landusemix-0.0.7/landusemix/data/shapefiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.220805 landusemix-0.0.7/landusemix/data/shapefiles/half/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.prj
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.qix
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.shp
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/half/half.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.220805 landusemix-0.0.7/landusemix/data/shapefiles/multiple/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/multiple/multiple.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/multiple/multiple.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/multiple/multiple.prj
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/multiple/multiple.qix
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/multiple/multiple.shp
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/multiple/multiple.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.220805 landusemix-0.0.7/landusemix/data/shapefiles/one/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/one/one.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/one/one.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/one/one.prj
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/one/one.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/one/one.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/data/shapefiles/one/one.shx
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 02:22:21.000000 landusemix-0.0.7/landusemix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.224805 landusemix-0.0.7/landusemix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:22:24.000000 landusemix-0.0.7/landusemix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-22 02:22:24.000000 landusemix-0.0.7/landusemix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:22:24.000000 landusemix-0.0.7/landusemix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:22:24.000000 landusemix-0.0.7/landusemix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:22:24.000000 landusemix-0.0.7/landusemix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:22:24.224805 landusemix-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-22 02:22:21.000000 landusemix-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:24.224805 landusemix-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:21.000000 landusemix-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 02:22:21.000000 landusemix-0.0.7/tests/test_landusemix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.795222 landusemix-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:34:24.000000 landusemix-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 02:34:24.000000 landusemix-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:34:33.795222 landusemix-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 02:34:24.000000 landusemix-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.791222 landusemix-0.0.8/landusemix/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.791222 landusemix-0.0.8/landusemix/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.791222 landusemix-0.0.8/landusemix/data/geojson/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/geojson/half.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/geojson/multiple.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/geojson/one.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.795222 landusemix-0.0.8/landusemix/data/shapefiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.prj
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.qix
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/half.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/multiple.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/multiple.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/multiple.prj
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/multiple.qix
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/multiple.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/multiple.shx
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/one.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/one.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/one.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/one.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/data/shapefiles/one.shx
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 02:34:24.000000 landusemix-0.0.8/landusemix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.795222 landusemix-0.0.8/landusemix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 02:34:33.000000 landusemix-0.0.8/landusemix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 02:34:33.000000 landusemix-0.0.8/landusemix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:34:33.000000 landusemix-0.0.8/landusemix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:34:33.000000 landusemix-0.0.8/landusemix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:34:33.000000 landusemix-0.0.8/landusemix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:34:33.795222 landusemix-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-22 02:34:24.000000 landusemix-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:33.795222 landusemix-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:34:24.000000 landusemix-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 02:34:24.000000 landusemix-0.0.8/tests/test_landusemix.py
```

### Comparing `landusemix-0.0.7/LICENSE` & `landusemix-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/PKG-INFO` & `landusemix-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.7/README.md` & `landusemix-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix/data/geojson/half.geojson` & `landusemix-0.0.8/landusemix/data/geojson/half.geojson`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix/data/geojson/multiple.geojson` & `landusemix-0.0.8/landusemix/data/geojson/multiple.geojson`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix/data/shapefiles/half/half.qmd` & `landusemix-0.0.8/landusemix/data/shapefiles/half.qmd`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix/data/shapefiles/one/one.qmd` & `landusemix-0.0.8/landusemix/data/shapefiles/one.qmd`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix/indices.py` & `landusemix-0.0.8/landusemix/indices.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix/utils.py` & `landusemix-0.0.8/landusemix/utils.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.7/landusemix.egg-info/PKG-INFO` & `landusemix-0.0.8/landusemix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.7/tests/test_landusemix.py` & `landusemix-0.0.8/tests/test_landusemix.py`

 * *Files identical despite different names*

