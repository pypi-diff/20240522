# Comparing `tmp/georeader-spaceml-1.1.2.tar.gz` & `tmp/georeader-spaceml-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georeader-spaceml-1.1.2.tar", last modified: Fri May 17 07:19:40 2024, max compression
+gzip compressed data, was "georeader-spaceml-1.1.3.tar", last modified: Wed May 22 11:04:37 2024, max compression
```

## Comparing `georeader-spaceml-1.1.2.tar` & `georeader-spaceml-1.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/LICENSE
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6803 2024-05-02 07:50:25.000000 georeader-spaceml-1.1.2/README.md
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.028694 georeader-spaceml-1.1.2/georeader/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.1.2/georeader/SolarIrradiance_Thuillier.csv
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2180 2024-05-02 10:15:20.000000 georeader-spaceml-1.1.2/georeader/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.1.2/georeader/abstract_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5394 2024-05-10 11:53:41.000000 georeader-spaceml-1.1.2/georeader/dataarray.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28666 2024-05-02 05:57:00.000000 georeader-spaceml-1.1.2/georeader/geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9257 2024-02-28 17:48:55.000000 georeader-spaceml-1.1.2/georeader/griddata.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11516 2024-03-01 12:59:18.000000 georeader-spaceml-1.1.2/georeader/mosaic.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11134 2024-01-09 11:32:45.000000 georeader-spaceml-1.1.2/georeader/plot.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    35477 2024-03-05 14:52:32.000000 georeader-spaceml-1.1.2/georeader/rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/rasterize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34265 2024-04-03 08:10:54.000000 georeader-spaceml-1.1.2/georeader/read.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/georeader/readers/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57165 2024-05-02 07:44:41.000000 georeader-spaceml-1.1.2/georeader/readers/S2_SAFE_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/readers/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.1.2/georeader/readers/download_pv_product.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2454 2024-02-28 16:40:43.000000 georeader-spaceml-1.1.2/georeader/readers/download_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10780 2024-05-17 06:24:46.000000 georeader-spaceml-1.1.2/georeader/readers/ee_image.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14387 2024-05-17 05:51:47.000000 georeader-spaceml-1.1.2/georeader/readers/ee_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    33154 2024-04-10 11:36:43.000000 georeader-spaceml-1.1.2/georeader/readers/emit.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12527 2024-03-01 21:44:02.000000 georeader-spaceml-1.1.2/georeader/readers/prisma.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18752 2024-05-02 08:23:57.000000 georeader-spaceml-1.1.2/georeader/readers/probav_image_operational.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/readers/query_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/readers/scihubcopernicus_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13869 2024-05-02 10:11:31.000000 georeader-spaceml-1.1.2/georeader/readers/spotvgt_image_operational.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3014 2024-05-17 07:17:50.000000 georeader-spaceml-1.1.2/georeader/readers/tileserver.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12969 2024-03-04 07:44:43.000000 georeader-spaceml-1.1.2/georeader/reflectance.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.1.2/georeader/save.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.1.2/georeader/save_cog.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/slices.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.1.2/georeader/vectorize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11423 2024-04-03 08:56:42.000000 georeader-spaceml-1.1.2/georeader/window_utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1171 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/SOURCES.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/dependency_links.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      513 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/requires.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/top_level.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/setup.cfg
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2780 2023-12-19 08:18:42.000000 georeader-spaceml-1.1.2/setup.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/tests/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/tests/test_geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/tests/test_rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/tests/test_xarray_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-22 11:04:37.906112 georeader-spaceml-1.1.3/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/LICENSE
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-22 11:04:37.906112 georeader-spaceml-1.1.3/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6803 2024-05-02 07:50:25.000000 georeader-spaceml-1.1.3/README.md
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-22 11:04:37.898112 georeader-spaceml-1.1.3/georeader/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.1.3/georeader/SolarIrradiance_Thuillier.csv
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2180 2024-05-22 11:04:17.000000 georeader-spaceml-1.1.3/georeader/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.1.3/georeader/abstract_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5394 2024-05-10 11:53:41.000000 georeader-spaceml-1.1.3/georeader/dataarray.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28666 2024-05-02 05:57:00.000000 georeader-spaceml-1.1.3/georeader/geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9257 2024-02-28 17:48:55.000000 georeader-spaceml-1.1.3/georeader/griddata.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11516 2024-03-01 12:59:18.000000 georeader-spaceml-1.1.3/georeader/mosaic.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11134 2024-01-09 11:32:45.000000 georeader-spaceml-1.1.3/georeader/plot.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    35477 2024-03-05 14:52:32.000000 georeader-spaceml-1.1.3/georeader/rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/georeader/rasterize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34265 2024-04-03 08:10:54.000000 georeader-spaceml-1.1.3/georeader/read.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-22 11:04:37.902112 georeader-spaceml-1.1.3/georeader/readers/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57165 2024-05-02 07:44:41.000000 georeader-spaceml-1.1.3/georeader/readers/S2_SAFE_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/georeader/readers/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.1.3/georeader/readers/download_pv_product.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2454 2024-02-28 16:40:43.000000 georeader-spaceml-1.1.3/georeader/readers/download_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10780 2024-05-17 06:24:46.000000 georeader-spaceml-1.1.3/georeader/readers/ee_image.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14599 2024-05-22 11:02:33.000000 georeader-spaceml-1.1.3/georeader/readers/ee_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    33154 2024-04-10 11:36:43.000000 georeader-spaceml-1.1.3/georeader/readers/emit.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12527 2024-03-01 21:44:02.000000 georeader-spaceml-1.1.3/georeader/readers/prisma.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18752 2024-05-02 08:23:57.000000 georeader-spaceml-1.1.3/georeader/readers/probav_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/georeader/readers/query_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/georeader/readers/scihubcopernicus_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13869 2024-05-02 10:11:31.000000 georeader-spaceml-1.1.3/georeader/readers/spotvgt_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3014 2024-05-17 07:17:50.000000 georeader-spaceml-1.1.3/georeader/readers/tileserver.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12969 2024-03-04 07:44:43.000000 georeader-spaceml-1.1.3/georeader/reflectance.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.1.3/georeader/save.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.1.3/georeader/save_cog.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/georeader/slices.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.1.3/georeader/vectorize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11423 2024-04-03 08:56:42.000000 georeader-spaceml-1.1.3/georeader/window_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-22 11:04:37.902112 georeader-spaceml-1.1.3/georeader_spaceml.egg-info/
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-22 11:04:37.000000 georeader-spaceml-1.1.3/georeader_spaceml.egg-info/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1171 2024-05-22 11:04:37.000000 georeader-spaceml-1.1.3/georeader_spaceml.egg-info/SOURCES.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2024-05-22 11:04:37.000000 georeader-spaceml-1.1.3/georeader_spaceml.egg-info/dependency_links.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      513 2024-05-22 11:04:37.000000 georeader-spaceml-1.1.3/georeader_spaceml.egg-info/requires.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2024-05-22 11:04:37.000000 georeader-spaceml-1.1.3/georeader_spaceml.egg-info/top_level.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2024-05-22 11:04:37.906112 georeader-spaceml-1.1.3/setup.cfg
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2780 2023-12-19 08:18:42.000000 georeader-spaceml-1.1.3/setup.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-22 11:04:37.902112 georeader-spaceml-1.1.3/tests/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/tests/test_geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/tests/test_rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.3/tests/test_xarray_utils.py
```

### Comparing `georeader-spaceml-1.1.2/LICENSE` & `georeader-spaceml-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/PKG-INFO` & `georeader-spaceml-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georeader-spaceml
-Version: 1.1.2
+Version: 1.1.3
 Summary: Lightweight reader for raster files
 Home-page: https://github.com/spaceml-org/georeader
 Author: Gonzalo Mateo-Garcia
 Keywords: raster reading,rasterio
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `georeader-spaceml-1.1.2/README.md` & `georeader-spaceml-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/SolarIrradiance_Thuillier.csv` & `georeader-spaceml-1.1.3/georeader/SolarIrradiance_Thuillier.csv`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/__init__.py` & `georeader-spaceml-1.1.3/georeader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 import math
 from typing import Tuple, Any, Union
 from shapely.geometry.base import BaseGeometry
 from shapely import Geometry
 from shapely.geometry import shape, mapping
 import rasterio.warp
```

### Comparing `georeader-spaceml-1.1.2/georeader/abstract_reader.py` & `georeader-spaceml-1.1.3/georeader/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/dataarray.py` & `georeader-spaceml-1.1.3/georeader/dataarray.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/geotensor.py` & `georeader-spaceml-1.1.3/georeader/geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/griddata.py` & `georeader-spaceml-1.1.3/georeader/griddata.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/mosaic.py` & `georeader-spaceml-1.1.3/georeader/mosaic.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/plot.py` & `georeader-spaceml-1.1.3/georeader/plot.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/rasterio_reader.py` & `georeader-spaceml-1.1.3/georeader/rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/rasterize.py` & `georeader-spaceml-1.1.3/georeader/rasterize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/read.py` & `georeader-spaceml-1.1.3/georeader/read.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/S2_SAFE_reader.py` & `georeader-spaceml-1.1.3/georeader/readers/S2_SAFE_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/download_pv_product.py` & `georeader-spaceml-1.1.3/georeader/readers/download_pv_product.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/download_utils.py` & `georeader-spaceml-1.1.3/georeader/readers/download_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/ee_image.py` & `georeader-spaceml-1.1.3/georeader/readers/ee_image.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/ee_query.py` & `georeader-spaceml-1.1.3/georeader/readers/ee_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,23 +74,27 @@
     if return_collection:
         return geodf, img_col
 
     return geodf
 
 def figure_out_collection_landsat(tile:str) -> str:
     if tile.startswith("LC08") or tile.startswith("LO08"):
-        if tile.endswith("T1_RT") or tile.endswith("T1"):
+        if tile.endswith("T1_RT") or tile.endswith("T1") or tile.endswith("RT"):
             return "LANDSAT/LC08/C02/T1_RT_TOA"
         elif tile.endswith("T2"):
             return "LANDSAT/LC08/C02/T2_TOA"
+        else:
+            raise ValueError(f"Tile of Landsat-8 {tile} not recognized")
     elif tile.startswith("LC09") or tile.startswith("LO09"):
         if tile.endswith("T1"):
             return "LANDSAT/LC09/C02/T1_TOA"
         elif tile.endswith("T2"):
             return "LANDSAT/LC09/C02/T2_TOA"
+        else:
+            raise ValueError(f"Tile of Landsat-9 {tile} not recognized")
     else:
         raise ValueError(f"Tile {tile} not recognized")
 
 
 def query(area:Union[MultiPolygon,Polygon],
           date_start:datetime, date_end:datetime,
           producttype:str='S2', filter_duplicates:bool=True,
@@ -152,15 +156,16 @@
     else:
         raise NotImplementedError(f"Unknown product type {producttype}")
 
     img_col = ee.ImageCollection(image_collection_name).filterDate(date_start.replace(tzinfo=None),
                                                                    date_end.replace(tzinfo=None)).filterBounds(
         pol)
     if "T1" in image_collection_name:
-        image_collection_name_t2 = image_collection_name.replace("T1_RT", "T2").replace("T1","T2")
+        # Add tier 2 data to the query
+        image_collection_name_t2 = image_collection_name.replace("T1_RT", "T2").replace("T1", "T2")
         img_col_t1 = ee.ImageCollection(image_collection_name_t2).filterDate(date_start.replace(tzinfo=None),
                                                                      date_end.replace(tzinfo=None)).filterBounds(
             pol)
         img_col = img_col.merge(img_col_t1)
     
     if (producttype == "Landsat") or (producttype == "both"):
         img_col_l9 = ee.ImageCollection("LANDSAT/LC09/C02/T1_TOA").filterDate(date_start.replace(tzinfo=None),
@@ -178,18 +183,16 @@
     geodf = img_collection_to_feature_collection(img_col,
                                                  ["system:time_start"] + list(keys_query.keys()) + extra_metadata_keys,
                                                 as_geopandas=True, band_crs="B2")
 
     geodf.rename(keys_query, axis=1, inplace=True)
 
     if geodf.shape[0] > 0:
-        if (producttype == "Landsat") or (producttype == "both"):
+        if (producttype == "Landsat") or (producttype == "both") or (producttype == "L8") or (producttype == "L9"):
             geodf["collection_name"] = geodf["title"].apply(figure_out_collection_landsat)
-        else:
-            geodf["collection_name"] = image_collection_name
 
     img_col = img_col.map(lambda x: _rename_add_properties(x, keys_query))
 
     if producttype == "both":
         img_col_s2 = ee.ImageCollection("COPERNICUS/S2_HARMONIZED").filterDate(date_start.replace(tzinfo=None),
                                                                               date_end.replace(
                                                                                   tzinfo=None)).filterBounds(
```

### Comparing `georeader-spaceml-1.1.2/georeader/readers/emit.py` & `georeader-spaceml-1.1.3/georeader/readers/emit.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/prisma.py` & `georeader-spaceml-1.1.3/georeader/readers/prisma.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/probav_image_operational.py` & `georeader-spaceml-1.1.3/georeader/readers/probav_image_operational.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/query_utils.py` & `georeader-spaceml-1.1.3/georeader/readers/query_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/scihubcopernicus_query.py` & `georeader-spaceml-1.1.3/georeader/readers/scihubcopernicus_query.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/spotvgt_image_operational.py` & `georeader-spaceml-1.1.3/georeader/readers/spotvgt_image_operational.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/readers/tileserver.py` & `georeader-spaceml-1.1.3/georeader/readers/tileserver.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/reflectance.py` & `georeader-spaceml-1.1.3/georeader/reflectance.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/save.py` & `georeader-spaceml-1.1.3/georeader/save.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/slices.py` & `georeader-spaceml-1.1.3/georeader/slices.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/vectorize.py` & `georeader-spaceml-1.1.3/georeader/vectorize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader/window_utils.py` & `georeader-spaceml-1.1.3/georeader/window_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader_spaceml.egg-info/PKG-INFO` & `georeader-spaceml-1.1.3/georeader_spaceml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georeader-spaceml
-Version: 1.1.2
+Version: 1.1.3
 Summary: Lightweight reader for raster files
 Home-page: https://github.com/spaceml-org/georeader
 Author: Gonzalo Mateo-Garcia
 Keywords: raster reading,rasterio
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `georeader-spaceml-1.1.2/georeader_spaceml.egg-info/SOURCES.txt` & `georeader-spaceml-1.1.3/georeader_spaceml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/georeader_spaceml.egg-info/requires.txt` & `georeader-spaceml-1.1.3/georeader_spaceml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/setup.py` & `georeader-spaceml-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/tests/test_geotensor.py` & `georeader-spaceml-1.1.3/tests/test_geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/tests/test_rasterio_reader.py` & `georeader-spaceml-1.1.3/tests/test_rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.2/tests/test_xarray_utils.py` & `georeader-spaceml-1.1.3/tests/test_xarray_utils.py`

 * *Files identical despite different names*

