# Comparing `tmp/hspatial-4.0.1.tar.gz` & `tmp/hspatial-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspatial-4.0.1.tar", last modified: Mon Apr 22 12:46:24 2024, max compression
+gzip compressed data, was "hspatial-4.1.0.tar", last modified: Wed May 22 18:21:22 2024, max compression
```

## Comparing `hspatial-4.0.1.tar` & `hspatial-4.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.127708 hspatial-4.0.1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3678 2024-04-22 12:21:42.000000 hspatial-4.0.1/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      710 2022-03-05 20:41:09.000000 hspatial-4.0.1/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:09.000000 hspatial-4.0.1/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5253 2024-04-22 12:46:24.127708 hspatial-4.0.1/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      723 2022-03-05 20:41:09.000000 hspatial-4.0.1/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.123708 hspatial-4.0.1/docs/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.123708 hspatial-4.0.1/docs/_build/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.123708 hspatial-4.0.1/docs/_build/html/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.123708 hspatial-4.0.1/docs/_build/html/_static/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      286 2023-03-29 08:31:27.000000 hspatial-4.0.1/docs/_build/html/_static/file.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7791 2021-06-13 20:22:59.000000 hspatial-4.0.1/docs/_build/html/_static/forkme_right_darkblue_121621.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2023-03-29 08:31:27.000000 hspatial-4.0.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2023-03-29 08:31:27.000000 hspatial-4.0.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9376 2024-04-13 14:14:35.000000 hspatial-4.0.1/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1370 2022-03-05 20:41:09.000000 hspatial-4.0.1/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:09.000000 hspatial-4.0.1/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      214 2022-03-05 20:41:09.000000 hspatial-4.0.1/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1013 2022-03-05 20:41:09.000000 hspatial-4.0.1/docs/testutils.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5336 2022-03-05 20:41:09.000000 hspatial-4.0.1/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.127708 hspatial-4.0.1/hspatial/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      141 2024-04-22 12:45:44.000000 hspatial-4.0.1/hspatial/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10333 2022-03-05 20:41:09.000000 hspatial-4.0.1/hspatial/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15422 2024-04-14 14:13:33.000000 hspatial-4.0.1/hspatial/hspatial.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1023 2022-03-05 20:41:09.000000 hspatial-4.0.1/hspatial/test.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.127708 hspatial-4.0.1/hspatial.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5253 2024-04-22 12:46:24.000000 hspatial-4.0.1/hspatial.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      673 2024-04-22 12:46:24.000000 hspatial-4.0.1/hspatial.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-22 12:46:24.000000 hspatial-4.0.1/hspatial.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       49 2024-04-22 12:46:24.000000 hspatial-4.0.1/hspatial.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-31 20:38:47.000000 hspatial-4.0.1/hspatial.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       84 2024-04-22 12:46:24.000000 hspatial-4.0.1/hspatial.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        9 2024-04-22 12:46:24.000000 hspatial-4.0.1/hspatial.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-22 12:46:24.127708 hspatial-4.0.1/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1711 2024-04-22 12:21:42.000000 hspatial-4.0.1/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-22 12:46:24.127708 hspatial-4.0.1/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:09.000000 hspatial-4.0.1/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    23026 2022-03-05 20:41:09.000000 hspatial-4.0.1/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    29125 2024-04-14 14:08:06.000000 hspatial-4.0.1/tests/test_hspatial.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.587901 hspatial-4.1.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3786 2024-05-22 18:17:50.000000 hspatial-4.1.0/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      710 2022-03-05 20:41:09.000000 hspatial-4.1.0/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:09.000000 hspatial-4.1.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5361 2024-05-22 18:21:22.587901 hspatial-4.1.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      723 2022-03-05 20:41:09.000000 hspatial-4.1.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.583901 hspatial-4.1.0/docs/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.583901 hspatial-4.1.0/docs/_build/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.583901 hspatial-4.1.0/docs/_build/html/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.587901 hspatial-4.1.0/docs/_build/html/_static/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      286 2023-03-29 08:31:27.000000 hspatial-4.1.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7791 2021-06-13 20:22:59.000000 hspatial-4.1.0/docs/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2023-03-29 08:31:27.000000 hspatial-4.1.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2023-03-29 08:31:27.000000 hspatial-4.1.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9450 2024-05-22 17:52:15.000000 hspatial-4.1.0/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1370 2022-03-05 20:41:09.000000 hspatial-4.1.0/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:09.000000 hspatial-4.1.0/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      214 2022-03-05 20:41:09.000000 hspatial-4.1.0/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1013 2022-03-05 20:41:09.000000 hspatial-4.1.0/docs/testutils.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5336 2022-03-05 20:41:09.000000 hspatial-4.1.0/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.587901 hspatial-4.1.0/hspatial/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      141 2024-05-22 18:19:58.000000 hspatial-4.1.0/hspatial/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10333 2022-03-05 20:41:09.000000 hspatial-4.1.0/hspatial/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15922 2024-05-22 18:16:05.000000 hspatial-4.1.0/hspatial/hspatial.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1023 2022-03-05 20:41:09.000000 hspatial-4.1.0/hspatial/test.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.587901 hspatial-4.1.0/hspatial.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5361 2024-05-22 18:21:22.000000 hspatial-4.1.0/hspatial.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      673 2024-05-22 18:21:22.000000 hspatial-4.1.0/hspatial.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-05-22 18:21:22.000000 hspatial-4.1.0/hspatial.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       49 2024-05-22 18:21:22.000000 hspatial-4.1.0/hspatial.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-31 20:38:47.000000 hspatial-4.1.0/hspatial.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       84 2024-05-22 18:21:22.000000 hspatial-4.1.0/hspatial.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        9 2024-05-22 18:21:22.000000 hspatial-4.1.0/hspatial.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-05-22 18:21:22.587901 hspatial-4.1.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1711 2024-04-22 12:21:42.000000 hspatial-4.1.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-05-22 18:21:22.587901 hspatial-4.1.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:09.000000 hspatial-4.1.0/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    23026 2022-03-05 20:41:09.000000 hspatial-4.1.0/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    29578 2024-05-22 18:00:19.000000 hspatial-4.1.0/tests/test_hspatial.py
```

### Comparing `hspatial-4.0.1/HISTORY.rst` & `hspatial-4.1.0/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+4.1.0 (2024-05-22)
+==================
+
+- extract_point_from_raster() now also accepts a GDALRaster object.
+
 4.0.1 (2024-04-22)
 ==================
 
 - Updated requirements to be compatible with Django 4 and 5.
 
 4.0.0 (2024-04-14)
 ==================
```

### Comparing `hspatial-4.0.1/LICENSE` & `hspatial-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/PKG-INFO` & `hspatial-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspatial
-Version: 4.0.1
+Version: 4.1.0
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/hspatial
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: hspatial
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,14 +49,19 @@
 * Documentation: https://hspatial.readthedocs.io.
 
 
 =======
 History
 =======
 
+4.1.0 (2024-05-22)
+==================
+
+- extract_point_from_raster() now also accepts a GDALRaster object.
+
 4.0.1 (2024-04-22)
 ==================
 
 - Updated requirements to be compatible with Django 4 and 5.
 
 4.0.0 (2024-04-14)
 ==================
```

### Comparing `hspatial-4.0.1/README.rst` & `hspatial-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/docs/_build/html/_static/forkme_right_darkblue_121621.png` & `hspatial-4.1.0/docs/_build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/docs/api.rst` & `hspatial-4.1.0/docs/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,19 @@
    examines the recorded list and checks whether it has been
    calculated from all available data (occasionally more data becomes
    available between subsequent runs); if yes, the function returns
    without doing anything.
 
 .. function:: hspatial.extract_point_from_raster(point, data_source, band_number=1)
 
-   *data_source* is a GDAL raster. *point* is either an OGR point, or a
-   GeoDjango point object.  The function returns the value of the pixel
-   of the specified band of *data_source* in which the *point* falls.
+   *data_source* is either a GDAL data source with a raster or a
+   GeoDjango :class:`GDALRaster` object. *point* is either an OGR point,
+   or a GeoDjango point object.  The function returns the value of the
+   pixel of the specified band of *data_source* in which the *point*
+   falls.
 
    *point* and *data_source* need not be in the same reference system,
    but they must both have an appropriate spatial reference defined.
 
    If the *point* does not fall in the raster, :exc:`RuntimeError` is
    raised.
```

### Comparing `hspatial-4.0.1/docs/conf.py` & `hspatial-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/docs/testutils.rst` & `hspatial-4.1.0/docs/testutils.rst`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/docs/usage.rst` & `hspatial-4.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/hspatial/cli.py` & `hspatial-4.1.0/hspatial/cli.py`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/hspatial/hspatial.py` & `hspatial-4.1.0/hspatial/hspatial.py`

 * *Files 7% similar despite different names*

```diff
@@ -260,34 +260,50 @@
 
 
 def extract_point_from_raster(point, data_source, band_number=1):
     """Return floating-point value that corresponds to given point."""
     pppoint = PassepartoutPoint(point)
 
     # Convert point co-ordinates so that they are in same projection as raster
-    target_srs_wkt = data_source.GetProjection()
+    try:
+        target_srs_wkt = data_source.GetProjection()
+    except AttributeError:
+        target_srs_wkt = data_source.srs.wkt
     try:
         pppoint = pppoint.transform_to(target_srs_wkt)
     except GDALException:
         raise RuntimeError("Couldn't convert point to raster's CRS")
     infinities = (float("inf"), float("-inf"))
     if pppoint.x in infinities or pppoint.y in infinities:
         raise RuntimeError("Couldn't convert point to raster's CRS")
 
     # Convert geographic co-ordinates to pixel co-ordinates
-    forward_transform = Affine.from_gdal(*data_source.GetGeoTransform())
+    try:
+        forward_transform = Affine.from_gdal(*data_source.GetGeoTransform())
+    except AttributeError:
+        forward_transform = Affine.from_gdal(*data_source.geotransform)
     reverse_transform = ~forward_transform
     px, py = reverse_transform * (pppoint.x, pppoint.y)
     px, py = int(px), int(py)
 
     # Extract pixel value
-    band = data_source.GetRasterBand(band_number)
-    structval = band.ReadRaster(px, py, 1, 1, buf_type=gdal.GDT_Float32)
+    try:
+        band = data_source.GetRasterBand(band_number)
+    except AttributeError:
+        band = data_source.bands[band_number - 1]
+    try:
+        structval = band.ReadRaster(px, py, 1, 1, buf_type=gdal.GDT_Float32)
+    except AttributeError:
+        structval = band.data(offset=(px, py), size=(1, 1))
     result = struct.unpack("f", structval)[0]
-    if result == band.GetNoDataValue():
+    try:
+        nodata_value = band.GetNoDataValue()
+    except AttributeError:
+        nodata_value = band.nodata_value
+    if result == nodata_value:
         result = float("nan")
     return result
 
 
 class PointTimeseries:
     def __init__(self, point, **kwargs):
         self.point = point
```

### Comparing `hspatial-4.0.1/hspatial/test.py` & `hspatial-4.1.0/hspatial/test.py`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/hspatial.egg-info/PKG-INFO` & `hspatial-4.1.0/hspatial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspatial
-Version: 4.0.1
+Version: 4.1.0
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/hspatial
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: hspatial
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,14 +49,19 @@
 * Documentation: https://hspatial.readthedocs.io.
 
 
 =======
 History
 =======
 
+4.1.0 (2024-05-22)
+==================
+
+- extract_point_from_raster() now also accepts a GDALRaster object.
+
 4.0.1 (2024-04-22)
 ==================
 
 - Updated requirements to be compatible with Django 4 and 5.
 
 4.0.0 (2024-04-14)
 ==================
```

### Comparing `hspatial-4.0.1/hspatial.egg-info/SOURCES.txt` & `hspatial-4.1.0/hspatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/setup.py` & `hspatial-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/tests/test_cli.py` & `hspatial-4.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hspatial-4.0.1/tests/test_hspatial.py` & `hspatial-4.1.0/tests/test_hspatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import textwrap
 from stat import S_IREAD, S_IRGRP, S_IROTH
 from time import sleep
 from unittest import TestCase
 
 import numpy as np
 import pandas as pd
+from django.contrib.gis.gdal import GDALRaster
 from django.contrib.gis.geos import Point as GeoDjangoPoint
 from htimeseries import HTimeseries, TzinfoFromString
 from osgeo import gdal, ogr, osr
 
 import hspatial
 from hspatial.test import setup_test_raster
 
@@ -390,14 +391,23 @@
         # We use co-ordinates almost to the common corner of the four lower left points,
         # only a little bit towards the center.
         point = hspatial.coordinates2point(22.01001, 37.98001)
         self.assertAlmostEqual(
             hspatial.extract_point_from_raster(point, self.fp), 2.2, places=2
         )
 
+    def test_middle_point_with_GDALRaster(self):
+        # Same as test_middle_point(), but uses GDALRaster object instead of a gdal
+        # data source.
+        point = hspatial.coordinates2point(22.01001, 37.98001)
+        gdal_raster_object = GDALRaster(self.filename)
+        self.assertAlmostEqual(
+            hspatial.extract_point_from_raster(point, gdal_raster_object), 2.2, places=2
+        )
+
     def test_bottom_left_point(self):
         # Use almost exactly same point as test_middle_point(), only slightly altered
         # so that we get bottom left point instead.
         point = hspatial.coordinates2point(22.00999, 37.97999)
         self.assertAlmostEqual(
             hspatial.extract_point_from_raster(point, self.fp), 3.1, places=2
         )
```

