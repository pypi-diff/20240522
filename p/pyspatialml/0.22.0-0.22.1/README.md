# Comparing `tmp/pyspatialml-0.22.0.tar.gz` & `tmp/pyspatialml-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspatialml-0.22.0.tar", max compression
+gzip compressed data, was "pyspatialml-0.22.1.tar", max compression
```

## Comparing `pyspatialml-0.22.0.tar` & `pyspatialml-0.22.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0    35141 2024-05-18 03:17:44.578611 pyspatialml-0.22.0/LICENSE
--rw-r--r--   0        0        0    17229 2024-05-18 04:48:00.485702 pyspatialml-0.22.0/README.md
--rw-r--r--   0        0        0      700 2024-05-18 15:27:58.682263 pyspatialml-0.22.0/pyproject.toml
--rw-r--r--   0        0        0       64 2024-05-18 03:17:44.595025 pyspatialml-0.22.0/pyspatialml/__init__.py
--rw-r--r--   0        0        0      618 2024-05-18 04:03:54.249762 pyspatialml-0.22.0/pyspatialml/_extraction.py
--rw-r--r--   0        0        0     8831 2024-05-18 04:03:54.249907 pyspatialml-0.22.0/pyspatialml/_plotting.py
--rw-r--r--   0        0        0     8184 2024-05-18 03:17:44.595549 pyspatialml-0.22.0/pyspatialml/_prediction.py
--rw-r--r--   0        0        0     4227 2024-05-18 03:17:44.595630 pyspatialml-0.22.0/pyspatialml/_rasterbase.py
--rw-r--r--   0        0        0        0 2024-05-18 03:17:44.595692 pyspatialml-0.22.0/pyspatialml/datasets/__init__.py
--rw-r--r--   0        0        0    33305 2024-05-18 03:17:44.595866 pyspatialml-0.22.0/pyspatialml/datasets/chnl_dist.tif
--rw-r--r--   0        0        0    33297 2024-05-18 03:17:44.595974 pyspatialml-0.22.0/pyspatialml/datasets/dem.tif
--rw-r--r--   0        0        0    33300 2024-05-18 03:17:44.596068 pyspatialml-0.22.0/pyspatialml/datasets/dist.tif
--rw-r--r--   0        0        0    70166 2024-05-18 04:48:00.487953 pyspatialml-0.22.0/pyspatialml/datasets/extracted_pixels.txt
--rw-r--r--   0        0        0    33285 2024-05-18 03:17:44.596336 pyspatialml-0.22.0/pyspatialml/datasets/ffreq.tif
--rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596453 pyspatialml-0.22.0/pyspatialml/datasets/landimg2.tif
--rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596625 pyspatialml-0.22.0/pyspatialml/datasets/landimg3.tif
--rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596794 pyspatialml-0.22.0/pyspatialml/datasets/landimg4.tif
--rw-r--r--   0        0        0   870707 2024-05-18 03:17:44.598175 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_labelled_pixels.tif
--rw-r--r--   0        0        0   160290 2024-05-18 03:17:44.598833 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.dbf
--rw-r--r--   0        0        0      536 2024-05-18 04:48:00.498623 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.prj
--rw-r--r--   0        0        0    28100 2024-05-18 03:17:44.599051 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shp
--rw-r--r--   0        0        0     8100 2024-05-18 03:17:44.599156 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shx
--rw-r--r--   0        0        0     8938 2024-05-18 03:17:44.599287 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.dbf
--rw-r--r--   0        0        0      493 2024-05-18 04:48:00.498908 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.prj
--rw-r--r--   0        0        0     4756 2024-05-18 03:17:44.599434 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.shp
--rw-r--r--   0        0        0      372 2024-05-18 03:17:44.599484 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.shx
--rw-r--r--   0        0        0  4336805 2024-05-18 03:17:44.605376 pyspatialml-0.22.0/pyspatialml/datasets/landsat_multiband.tif
--rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.606729 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_10.tif
--rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.608015 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_20.tif
--rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.609461 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_30.tif
--rw-r--r--   0        0        0   869905 2024-05-18 03:17:44.610714 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_40.tif
--rw-r--r--   0        0        0   869905 2024-05-18 03:17:44.612145 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_50.tif
--rw-r--r--   0        0        0   435771 2024-05-18 03:17:44.613062 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_70.tif
--rw-r--r--   0        0        0    25062 2024-05-18 03:17:44.613170 pyspatialml-0.22.0/pyspatialml/datasets/meuse.dbf
--rw-r--r--   0        0        0      434 2024-05-18 04:48:00.499193 pyspatialml-0.22.0/pyspatialml/datasets/meuse.prj
--rw-r--r--   0        0        0      967 2024-05-18 04:48:00.499299 pyspatialml-0.22.0/pyspatialml/datasets/meuse.py
--rw-r--r--   0        0        0     4440 2024-05-18 03:17:44.613379 pyspatialml-0.22.0/pyspatialml/datasets/meuse.shp
--rw-r--r--   0        0        0     1340 2024-05-18 03:17:44.613445 pyspatialml-0.22.0/pyspatialml/datasets/meuse.shx
--rw-r--r--   0        0        0    33327 2024-05-18 03:17:44.613547 pyspatialml-0.22.0/pyspatialml/datasets/mrvbf.tif
--rw-r--r--   0        0        0      889 2024-05-18 04:48:00.499394 pyspatialml-0.22.0/pyspatialml/datasets/nc.py
--rw-r--r--   0        0        0    33293 2024-05-18 03:17:44.613729 pyspatialml-0.22.0/pyspatialml/datasets/rsp.tif
--rw-r--r--   0        0        0    33307 2024-05-18 03:17:44.613836 pyspatialml-0.22.0/pyspatialml/datasets/slope.tif
--rw-r--r--   0        0        0    33285 2024-05-18 03:17:44.613952 pyspatialml-0.22.0/pyspatialml/datasets/soil.tif
--rw-r--r--   0        0        0   869411 2024-05-18 03:17:44.614915 pyspatialml-0.22.0/pyspatialml/datasets/strata.tif
--rw-r--r--   0        0        0    33319 2024-05-18 03:17:44.615036 pyspatialml-0.22.0/pyspatialml/datasets/twi.tif
--rw-r--r--   0        0        0     8137 2024-05-18 04:48:00.499521 pyspatialml-0.22.0/pyspatialml/preprocessing.py
--rw-r--r--   0        0        0    95089 2024-05-18 04:48:00.499896 pyspatialml-0.22.0/pyspatialml/raster.py
--rw-r--r--   0        0        0    17937 2024-05-18 04:48:00.500055 pyspatialml-0.22.0/pyspatialml/rasterlayer.py
--rw-r--r--   0        0        0     1185 2024-05-18 03:17:44.615450 pyspatialml-0.22.0/pyspatialml/rasterstats.py
--rw-r--r--   0        0        0    15649 2024-05-18 03:17:44.615583 pyspatialml-0.22.0/pyspatialml/transformers.py
--rw-r--r--   0        0        0     1438 2024-05-18 03:17:44.615642 pyspatialml-0.22.0/pyspatialml/vector.py
--rw-r--r--   0        0        0    18404 1970-01-01 00:00:00.000000 pyspatialml-0.22.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2024-05-18 03:17:44.578611 pyspatialml-0.22.1/LICENSE
+-rw-r--r--   0        0        0    17229 2024-05-18 04:48:00.485702 pyspatialml-0.22.1/README.md
+-rw-r--r--   0        0        0      875 2024-05-22 21:41:40.510750 pyspatialml-0.22.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-18 03:17:44.595025 pyspatialml-0.22.1/pyspatialml/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-18 04:03:54.249762 pyspatialml-0.22.1/pyspatialml/_extraction.py
+-rw-r--r--   0        0        0     8831 2024-05-18 04:03:54.249907 pyspatialml-0.22.1/pyspatialml/_plotting.py
+-rw-r--r--   0        0        0     8184 2024-05-18 03:17:44.595549 pyspatialml-0.22.1/pyspatialml/_prediction.py
+-rw-r--r--   0        0        0     4227 2024-05-18 03:17:44.595630 pyspatialml-0.22.1/pyspatialml/_rasterbase.py
+-rw-r--r--   0        0        0        0 2024-05-18 03:17:44.595692 pyspatialml-0.22.1/pyspatialml/datasets/__init__.py
+-rw-r--r--   0        0        0    33305 2024-05-18 03:17:44.595866 pyspatialml-0.22.1/pyspatialml/datasets/chnl_dist.tif
+-rw-r--r--   0        0        0    33297 2024-05-18 03:17:44.595974 pyspatialml-0.22.1/pyspatialml/datasets/dem.tif
+-rw-r--r--   0        0        0    33300 2024-05-18 03:17:44.596068 pyspatialml-0.22.1/pyspatialml/datasets/dist.tif
+-rw-r--r--   0        0        0    70166 2024-05-18 04:48:00.487953 pyspatialml-0.22.1/pyspatialml/datasets/extracted_pixels.txt
+-rw-r--r--   0        0        0    33285 2024-05-18 03:17:44.596336 pyspatialml-0.22.1/pyspatialml/datasets/ffreq.tif
+-rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596453 pyspatialml-0.22.1/pyspatialml/datasets/landimg2.tif
+-rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596625 pyspatialml-0.22.1/pyspatialml/datasets/landimg3.tif
+-rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596794 pyspatialml-0.22.1/pyspatialml/datasets/landimg4.tif
+-rw-r--r--   0        0        0   870707 2024-05-18 03:17:44.598175 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_labelled_pixels.tif
+-rw-r--r--   0        0        0   160290 2024-05-18 03:17:44.598833 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.dbf
+-rw-r--r--   0        0        0      536 2024-05-18 04:48:00.498623 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.prj
+-rw-r--r--   0        0        0    28100 2024-05-18 03:17:44.599051 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.shp
+-rw-r--r--   0        0        0     8100 2024-05-18 03:17:44.599156 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.shx
+-rw-r--r--   0        0        0     8938 2024-05-18 03:17:44.599287 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_polygons.dbf
+-rw-r--r--   0        0        0      493 2024-05-18 04:48:00.498908 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_polygons.prj
+-rw-r--r--   0        0        0     4756 2024-05-18 03:17:44.599434 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_polygons.shp
+-rw-r--r--   0        0        0      372 2024-05-18 03:17:44.599484 pyspatialml-0.22.1/pyspatialml/datasets/landsat96_polygons.shx
+-rw-r--r--   0        0        0  4336805 2024-05-18 03:17:44.605376 pyspatialml-0.22.1/pyspatialml/datasets/landsat_multiband.tif
+-rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.606729 pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_10.tif
+-rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.608015 pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_20.tif
+-rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.609461 pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_30.tif
+-rw-r--r--   0        0        0   869905 2024-05-18 03:17:44.610714 pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_40.tif
+-rw-r--r--   0        0        0   869905 2024-05-18 03:17:44.612145 pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_50.tif
+-rw-r--r--   0        0        0   435771 2024-05-18 03:17:44.613062 pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_70.tif
+-rw-r--r--   0        0        0    25062 2024-05-18 03:17:44.613170 pyspatialml-0.22.1/pyspatialml/datasets/meuse.dbf
+-rw-r--r--   0        0        0      434 2024-05-18 04:48:00.499193 pyspatialml-0.22.1/pyspatialml/datasets/meuse.prj
+-rw-r--r--   0        0        0      967 2024-05-18 04:48:00.499299 pyspatialml-0.22.1/pyspatialml/datasets/meuse.py
+-rw-r--r--   0        0        0     4440 2024-05-18 03:17:44.613379 pyspatialml-0.22.1/pyspatialml/datasets/meuse.shp
+-rw-r--r--   0        0        0     1340 2024-05-18 03:17:44.613445 pyspatialml-0.22.1/pyspatialml/datasets/meuse.shx
+-rw-r--r--   0        0        0    33327 2024-05-18 03:17:44.613547 pyspatialml-0.22.1/pyspatialml/datasets/mrvbf.tif
+-rw-r--r--   0        0        0      889 2024-05-18 04:48:00.499394 pyspatialml-0.22.1/pyspatialml/datasets/nc.py
+-rw-r--r--   0        0        0    33293 2024-05-18 03:17:44.613729 pyspatialml-0.22.1/pyspatialml/datasets/rsp.tif
+-rw-r--r--   0        0        0    33307 2024-05-18 03:17:44.613836 pyspatialml-0.22.1/pyspatialml/datasets/slope.tif
+-rw-r--r--   0        0        0    33285 2024-05-18 03:17:44.613952 pyspatialml-0.22.1/pyspatialml/datasets/soil.tif
+-rw-r--r--   0        0        0   869411 2024-05-18 03:17:44.614915 pyspatialml-0.22.1/pyspatialml/datasets/strata.tif
+-rw-r--r--   0        0        0    33319 2024-05-18 03:17:44.615036 pyspatialml-0.22.1/pyspatialml/datasets/twi.tif
+-rw-r--r--   0        0        0     7281 2024-05-21 05:22:42.778777 pyspatialml-0.22.1/pyspatialml/locindexer.py
+-rw-r--r--   0        0        0     8139 2024-05-20 15:27:44.939767 pyspatialml-0.22.1/pyspatialml/preprocessing.py
+-rw-r--r--   0        0        0    88598 2024-05-21 05:23:07.660824 pyspatialml-0.22.1/pyspatialml/raster.py
+-rw-r--r--   0        0        0    17942 2024-05-20 15:27:44.940072 pyspatialml-0.22.1/pyspatialml/rasterlayer.py
+-rw-r--r--   0        0        0     1185 2024-05-18 03:17:44.615450 pyspatialml-0.22.1/pyspatialml/rasterstats.py
+-rw-r--r--   0        0        0    15646 2024-05-20 15:27:45.092043 pyspatialml-0.22.1/pyspatialml/transformers.py
+-rw-r--r--   0        0        0     1462 2024-05-20 15:27:44.940257 pyspatialml-0.22.1/pyspatialml/vector.py
+-rw-r--r--   0        0        0    18404 1970-01-01 00:00:00.000000 pyspatialml-0.22.1/PKG-INFO
```

### Comparing `pyspatialml-0.22.0/LICENSE` & `pyspatialml-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/README.md` & `pyspatialml-0.22.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyproject.toml` & `pyspatialml-0.22.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspatialml"
-version = "0.22.0"
+version = "0.22.1"
 description = "Machine learning classification and regression modelling for spatial raster data."
 authors = ["Steven Pawley <dr.stevenpawley@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://stevenpawley.github.io/Pyspatialml/"
 repository = "https://github.com/stevenpawley/Pyspatialml"
 
@@ -17,10 +17,19 @@
 scipy = "^1.13.0"
 shapely = "^2.0.4"
 pandas = "^2.2.2"
 matplotlib = "^3.9.0"
 scikit-learn = "^1.4.2"
 affine = "^2.4.0"
 
+[tool.poetry.group.dev.dependencies]
+quartodoc = "^0.7.2"
+jupyter = "^1.0.0"
+ipykernel = "^6.29.4"
+black = "^24.4.2"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.2.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyspatialml-0.22.0/pyspatialml/_extraction.py` & `pyspatialml-0.22.1/pyspatialml/_extraction.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/_plotting.py` & `pyspatialml-0.22.1/pyspatialml/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/_prediction.py` & `pyspatialml-0.22.1/pyspatialml/_prediction.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/_rasterbase.py` & `pyspatialml-0.22.1/pyspatialml/_rasterbase.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/chnl_dist.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/chnl_dist.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/dem.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/dem.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/dist.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/dist.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/extracted_pixels.txt` & `pyspatialml-0.22.1/pyspatialml/datasets/extracted_pixels.txt`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/ffreq.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/ffreq.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landimg2.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/landimg2.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landimg3.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/landimg3.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landimg4.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/landimg4.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_labelled_pixels.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_labelled_pixels.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.dbf` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.dbf`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.prj` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.prj`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shp` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.shp`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shx` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_points.shx`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.dbf` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_polygons.dbf`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.shp` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat96_polygons.shp`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/landsat_multiband.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/landsat_multiband.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_10.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_10.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_20.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_20.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_30.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_30.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_40.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_40.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_50.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_50.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_70.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/lsat7_2000_70.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/meuse.dbf` & `pyspatialml-0.22.1/pyspatialml/datasets/meuse.dbf`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/meuse.py` & `pyspatialml-0.22.1/pyspatialml/datasets/meuse.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/meuse.shp` & `pyspatialml-0.22.1/pyspatialml/datasets/meuse.shp`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/meuse.shx` & `pyspatialml-0.22.1/pyspatialml/datasets/meuse.shx`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/mrvbf.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/mrvbf.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/nc.py` & `pyspatialml-0.22.1/pyspatialml/datasets/nc.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/rsp.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/rsp.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/slope.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/slope.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/soil.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/soil.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/strata.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/strata.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/datasets/twi.tif` & `pyspatialml-0.22.1/pyspatialml/datasets/twi.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/preprocessing.py` & `pyspatialml-0.22.1/pyspatialml/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,22 +202,24 @@
                       in_place=True)
 
     return new_raster
 
 
 def _grid_distance(shape, rows, cols):
     """Generate buffer distances to x,y coordinates.
+
     Parameters
     ----------
     shape : tuple
         shape of numpy array (rows, cols) to create buffer distances within.
     rows : 1d numpy array
         array of row indexes.
     cols : 1d numpy array
         array of column indexes.
+
     Returns
     -------
     ndarray
         3d numpy array of euclidean grid distances to each x,y coordinate pair
         [band, row, col].
     """
```

### Comparing `pyspatialml-0.22.0/pyspatialml/raster.py` & `pyspatialml-0.22.1/pyspatialml/raster.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,252 +29,15 @@
     stack_constants,
 )
 from ._rasterbase import TempRasterLayer, _check_alignment, _fix_names, get_nodata_value
 from .rasterlayer import RasterLayer
 from .rasterstats import RasterStats
 from ._extraction import extract_by_chunk
 from .transformers import _apply_transformer
-
-
-class _LocIndexer(MutableMapping):
-    """Access pyspatialml.RasterLayer objects by using a key.
-
-    Represents a structure similar to a dict but allows access using a
-    list of keys (not just a single key).
-    """
-
-    def __init__(self, *args, **kw):
-        self.__dict__.update(*args, **kw)
-
-    def __getitem__(self, key):
-        """Defines the subset method for the _LocIndexer. Allows the
-        contained RasterLayer objects to be subset using a either
-        single, or multiple labels corresponding to the names of each
-        RasterLayer.
-
-        Parameters
-        ----------
-        key : a single str, or a list of str
-
-        Returns
-        -------
-        Returns a RasterLayer if only a single item is subset, or a
-        Raster if multiple items are subset.
-
-        """
-        if isinstance(key, str):
-            new = self.__dict__[key]
-        else:
-            selected = []
-
-            for i in key:
-                if i in self.names is False:
-                    raise KeyError("key not present in Raster object")
-                else:
-                    selected.append(self.__dict__[i])
-
-            new = Raster(selected)
-        return new
-
-    def __setitem__(self, key, value):
-        """Allows a RasterLayer object to be assigned to a name within
-        a Raster object. This automatically updates the indexer with
-        the layer, and adds the RasterLayer's name as an attribute in
-        the Raster.
-
-        Parameters
-        ----------
-        key : str
-            The key to use for the assignment:
-
-        value : pyspatialml.RasterLayer
-            A single RasterLayer object to assign to the key.
-        """
-        if isinstance(value, RasterLayer):
-            self.__dict__[key] = value
-        else:
-            raise ValueError("value is not a RasterLayer object")
-
-    def __iter__(self):
-        """Iterates through keys"""
-        return iter(self._keys)
-
-    def __len__(self):
-        """Number of layers in the indexer"""
-        return len(self.__dict__) - len(self._internal)
-
-    def __delitem__(self, key):
-        """Delete a key:value pair"""
-        self.__dict__.pop(key)
-
-    def __repr__(self):
-        print("Raster Object Containing {n} Layers".format(n=self.count))
-        meta = pd.DataFrame(
-            {
-                "attribute": ["names", "files", "rows", "cols", "res", "nodatavals"],
-                "values": [
-                    list(self.names),
-                    self.files,
-                    self.shape[0],
-                    self.shape[1],
-                    self.res,
-                    self.nodatavals,
-                ],
-            }
-        )
-        print(meta)
-
-        return ""
-
-    @property
-    def _keys(self):
-        d = {k: v for (k, v) in self.__dict__.items() if k not in self._internal}
-        return d.keys()
-
-    def _rename_inplace(self, old, new):
-        """Rename a RasterLayer from `old` to `new. This method renames
-        the layer in the indexer and renames the equivalent attribute
-        in the parent Raster object.
-
-        Parameters
-        ----------
-        old : str
-            Name of the existing key.
-
-        new : str
-            Name to use to rename the existing key.
-        """
-        # rename the index by rebuilding the dict
-        original_keys = list(self.__dict__.keys())
-        new_keys = [new if i == old else i for i in original_keys]
-        new_dict = dict(zip(new_keys, self.__dict__.values()))
-        self.__dict__ = new_dict
-
-        # update the internal name of a RasterLayer
-        self.__dict__[new].name = new
-
-    @property
-    def loc(self):
-        """Alias for the getter method of the indexer"""
-        return self
-
-    @loc.setter
-    def loc(self, key, value):
-        """Alias for the setter method if the indexer"""
-        self.__dict__[key] = value
-
-    @property
-    def iloc(self):
-        """Reference to an integer-based indexer to access the layers
-        by integer position rather than label"""
-        return _iLocIndexer(self)
-
-    @property
-    def names(self):
-        return self._keys
-
-    @names.setter
-    def names(self, value):
-        if isinstance(value, str):
-            value = [value]
-
-        if len(value) != self.count:
-            raise ValueError(
-                "Length of new names has to equal the number of layers in the Raster"
-            )
-
-        renamer = {old: new for (old, new) in zip(self.names, value)}
-        self.rename(renamer, in_place=True)
-
-
-class _iLocIndexer(object):
-    """Access pyspatialml.RasterLayer objects using an index position
-
-    A wrapper around _LocIndexer to enable integer-based indexing of
-    the items in the OrderedDict. Setting and getting items can occur
-    using a single index position, a list or tuple of positions, or a
-    slice of positions.
-
-    Methods
-    -------
-    __getitem__ : index
-        Subset RasterLayers using an integer index, a slice of indexes,
-        or a list/tuple of indexes. Returns a RasterLayer is a single
-        item is subset, or a Raster if multiple layers are subset.
-
-    __setitem__ : index, value
-        Assign a RasterLayer to a index position within the indexer.
-        The index can be a single integer position, a slice of
-        positions, or a list/tuple of positions. This method also
-        updates the parent Raster object's attributes with the names
-        of the new RasterLayers that were passed as the value.
-    """
-
-    def __init__(self, loc_indexer):
-        """Initiate a _iLocIndexer
-
-        Parameters
-        ----------
-        loc_indexer : pyspatialml.raster._LocIndexer
-            An instance of a _LocIndexer.
-        """
-        self._index = loc_indexer
-
-    def __setitem__(self, index, value):
-        if isinstance(index, int):
-            key = list(self._index.keys())[index]
-            self._index[key] = value
-
-        if isinstance(index, slice):
-            start = index.start
-            stop = index.stop
-            step = index.step
-
-            if start is None:
-                start = 0
-            if stop is None:
-                stop = self.count
-            if step is None:
-                step = 1
-
-            index = list(range(start, stop, step))
-
-        if isinstance(index, (list, tuple)):
-            for i, v in zip(index, value):
-                key = list(self._index.keys())[i]
-                self._index[key] = v
-
-    def __getitem__(self, index):
-        if isinstance(index, int):
-            key = list(self._index.keys())[index]
-            selected = self._index[key]
-
-        if isinstance(index, slice):
-            start = index.start
-            stop = index.stop
-            step = index.step
-
-            if start is None:
-                start = 0
-
-            if stop is None:
-                stop = self.count
-
-            if step is None:
-                step = 1
-
-            index = list(range(start, stop, step))
-
-        if isinstance(index, (list, tuple)):
-            key = []
-            for i in index:
-                key.append(list(self._index.keys())[i])
-            selected = Raster([self._index[k] for k in key])
-
-        return selected
+from .locindexer import _LocIndexer
 
 
 class Raster(_LocIndexer, RasterStats, RasterPlot):
     """Creates a collection of file-based GDAL-supported raster
     datasets that share a common coordinate reference system and
     geometry.
 
@@ -383,20 +146,19 @@
 
         src_layers = []
 
         # get temporary file name if file_path is None
         if file_path is None and isinstance(src, np.ndarray):
             file_path, tfile = self._tempfile(file_path)
             driver = "GTiff"
-
+        
         # initiate from numpy array
-        try:
+        if isinstance(src, np.ndarray):
             if src.ndim == 2:
                 src = src[np.newaxis]
-
             count, height, width = src.shape
 
             if in_memory is True:
                 memfile = MemoryFile()
                 dst = memfile.open(
                     height=height,
                     width=width,
@@ -404,161 +166,129 @@
                     driver=driver,
                     dtype=src.dtype,
                     crs=crs,
                     transform=transform,
                     nodata=nodata,
                 )
                 dst.write(src)
-
             else:
                 with rasterio.open(
                     file_path,
                     mode="w",
                     driver=driver,
                     height=height,
                     width=width,
                     count=count,
                     dtype=src.dtype,
                     crs=crs,
                     transform=transform,
                     nodata=nodata,
                 ) as dst:
                     dst.write(src)
-
                 dst = rasterio.open(file_path, "r")
 
             for i in range(dst.count):
                 band = rasterio.band(dst, i + 1)
                 rasterlayer = RasterLayer(band)
-
                 if in_memory is True:
                     rasterlayer.in_memory = True
-
                 src_layers.append(rasterlayer)
 
             if tfile is not None and in_memory is False:
                 for layer in src_layers:
                     layer._close = tfile.close
-
             self._layers = src_layers
             return
-
-        except:
-            pass
-
+        
         # from a single file path
-        try:
+        elif isinstance(src, str):
             src_layers = []
             r = rasterio.open(src, mode="r", driver=driver)
-
             for i in range(r.count):
                 band = rasterio.band(r, i + 1)
                 src_layers.append(RasterLayer(band))
-
-            self._layers = src_layers
-            return
-
-        except:
-            pass
-
-        # from a list of file paths
-        try:
-            src_layers = []
-
-            for f in src:
-                r = rasterio.open(f, mode="r", driver=driver)
-                for i in range(r.count):
-                    band = rasterio.band(r, i + 1)
-                    src_layers.append(RasterLayer(band))
-
             self._layers = src_layers
             return
 
-        except:
-            pass
-
-        # from a RasterLayer
-        try:
+        # from a single RasterLayer
+        elif isinstance(src, RasterLayer):
             self._layers = src
             self._rename_inplace(list(self.names)[0], src.name)
             return
 
-        except:
-            pass
-
-        # from a list of RasterLayers
-        try:
-            self._layers = src
-
-            for old, new in zip(self.names, src):
-                self._rename_inplace(old, new.name)
-            return
-
-        except:
-            pass
-
-        # from a Raster
-        try:
+        # from a single Raster
+        elif isinstance(src, Raster):
             self._layers = [i for i in src.values()]
-
             for old, new in zip(self.names, list(src.names)):
                 self._rename_inplace(old, new)
             return
 
-        except:
-            pass
-
         # from a single rasterio.io.datasetreader/writer
-        try:
+        elif isinstance(src, rasterio.io.DatasetReader):
             src_layers = []
-
             for i in range(src.count):
                 band = rasterio.band(src, i + 1)
                 src_layers.append(RasterLayer(band))
-
-            self._layers = src_layers
-            return
-
-        except:
-            pass
-
-        # from a list of rasterio.io.datasetreader
-        try:
-            src_layers = []
-
-            for r in src:
-                for i in range(r.count):
-                    band = rasterio.band(r, i + 1)
-                    src_layers.append(RasterLayer(band))
-
             self._layers = src_layers
             return
 
-        except:
-            pass
-
-        # from a single rasterio.band objects
-        try:
+        # from a single rasterio.band object
+        elif isinstance(src, rasterio.Band):
             self._layers = RasterLayer(src)
             return
 
-        except:
-            pass
-
-        try:
-            src_layers = []
-
-            for band in src:
-                src_layers.append(RasterLayer(band))
-
-            self._layers = src_layers
-            return
-
-        except:
-            pass
+        # from a list of objects
+        elif isinstance(src, list):
+            # list of file paths (str)
+            if all(isinstance(x, str) for x in src):
+                src_layers = []
+                for f in src:
+                    r = rasterio.open(f, mode="r", driver=driver)
+                    for i in range(r.count):
+                        band = rasterio.band(r, i + 1)
+                        src_layers.append(RasterLayer(band))
+
+                self._layers = src_layers
+                return
+
+            # list of RasterLayer objects
+            elif all(isinstance(x, RasterLayer) for x in src):
+                self._layers = src
+                for old, new in zip(self.names, src):
+                    self._rename_inplace(old, new.name)
+                return
+
+            # list of rasterio.io.datasetreader objects
+            elif all(isinstance(x, rasterio.io.DatasetReader) for x in src):
+                src_layers = []
+                for r in src:
+                    for i in range(r.count):
+                        band = rasterio.band(r, i + 1)
+                        src_layers.append(RasterLayer(band))
+                self._layers = src_layers
+                return
+        
+            # from a list of rasterio.band objects
+            elif all(isinstance(x, rasterio.Band) for x in src):
+                src_layers = []
+                for band in src:
+                    src_layers.append(RasterLayer(band))
+                self._layers = src_layers
+                return
+        else:
+            raise ValueError("Cannot create a Raster object from a mixture of inputs")
+        
+        # try:
+        #     src_layers = []
+        #     for band in src:
+        #         src_layers.append(RasterLayer(band))
+        #     self._layers = src_layers
+        #     return
+        # except:
+        #     pass
 
     @property
     def block_shape(self) -> Tuple[int, int]:
         """Return the block shape in (height, width) used to read windows from the
         Raster
         """
         return self._block_shape
```

### Comparing `pyspatialml-0.22.0/pyspatialml/rasterlayer.py` & `pyspatialml-0.22.1/pyspatialml/rasterlayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,16 +417,16 @@
         """Read method for a single RasterLayer.
 
         Reads the pixel values from a RasterLayer into a ndarray that
         always will have two dimensions in the order of (rows, columns).
 
         Parameters
         ----------
-        **kwargs : named arguments that can be passed to the the
-        rasterio.DatasetReader.read method.
+        **kwargs : named arguments that can be passed to the the 
+            rasterio.DatasetReader.read method.
         """
         if "resampling" in kwargs.keys():
             resampling_methods = [i.name for i in rasterio.enums.Resampling]
 
             if kwargs["resampling"] not in resampling_methods:
                 raise ValueError(
                     "Invalid resampling method. Resampling "
@@ -518,14 +518,15 @@
         legend=False,
         vmin=None,
         vmax=None,
         fig_kwds=None,
         legend_kwds=None,
     ):
         """Plot a RasterLayer using matplotlib.pyplot.imshow
+
         Parameters
         ----------
         cmap : str (default None)
             The name of a colormap recognized by matplotlib.
             Overrides the cmap attribute of the RasterLayer.
 
         norm : matplotlib.colors.Normalize (opt)
@@ -570,15 +571,14 @@
 
         legend_kwds : dict (optional, default None)
             Keyword arguments to pass to matplotlib.pyplot.colorbar().
 
         Returns
         -------
         ax : matplotlib axes instance
-
         """
 
         # some checks
         if fig_kwds is None:
             fig_kwds = {}
 
         if ax is None:
```

### Comparing `pyspatialml-0.22.0/pyspatialml/rasterstats.py` & `pyspatialml-0.22.1/pyspatialml/rasterstats.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.22.0/pyspatialml/transformers.py` & `pyspatialml-0.22.1/pyspatialml/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         # get values of closest training points to new data
         neighbor_vals = np.array([self.y_[i] for i in neighbor_ids])
 
         # mask neighbor values with zero distances
         mask = neighbor_dist.mask
 
         if mask.all() == False:
-            mask = np.zeros(neighbor_dist.shape, dtype=np.bool)
+            mask = np.zeros(neighbor_dist.shape, dtype=bool)
             mask[:] = False
 
         if neighbor_vals.ndim == 2:
             neighbor_vals = np.ma.masked_array(neighbor_vals, mask)
         else:
             n_outputs = neighbor_vals.shape[2]
             mask = np.repeat(mask[:, :, np.newaxis], n_outputs, axis=2)
```

### Comparing `pyspatialml-0.22.0/pyspatialml/vector.py` & `pyspatialml-0.22.1/pyspatialml/vector.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from scipy.cluster.hierarchy import cut_tree, linkage
 from shapely.geometry import Point
 
 
 def filter_points(gdf, min_dist=0, remove="first"):
     """Filter points in geodataframe using a minimum distance buffer.
 
-    Args
-    ----
+    Parameters
+    ----------
     gdf : Geopandas GeoDataFrame
         Containing point geometries.
 
     min_dist : int or float, optional (default=0)
         Minimum distance by which to filter out closely spaced points.
 
     remove : str, optional (default='first')
@@ -39,16 +39,16 @@
     return gdf
 
 
 def get_random_point_in_polygon(poly):
     """Generates random shapely Point geometry objects within a single
     shapely Polygon object.
 
-    Args
-    ----
+    Parameters
+    ----------
     poly : Shapely Polygon object
 
     Returns
     -------
     p : Shapely Point object
     """
```

### Comparing `pyspatialml-0.22.0/PKG-INFO` & `pyspatialml-0.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspatialml
-Version: 0.22.0
+Version: 0.22.1
 Summary: Machine learning classification and regression modelling for spatial raster data.
 Home-page: https://stevenpawley.github.io/Pyspatialml/
 License: GPL-3.0-or-later
 Author: Steven Pawley
 Author-email: dr.stevenpawley@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

