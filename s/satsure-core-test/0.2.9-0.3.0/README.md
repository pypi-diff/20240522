# Comparing `tmp/satsure-core-test-0.2.9.tar.gz` & `tmp/satsure-core-test-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.2.9.tar", last modified: Mon May 20 14:04:19 2024, max compression
+gzip compressed data, was "satsure-core-test-0.3.0.tar", last modified: Wed May 22 06:43:33 2024, max compression
```

## Comparing `satsure-core-test-0.2.9.tar` & `satsure-core-test-0.3.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.045443 satsure-core-test-0.2.9/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.2.9/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-20 14:04:19.045261 satsure-core-test-0.2.9/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.2.9/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.033589 satsure-core-test-0.2.9/satsure_core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:33:06.000000 satsure-core-test-0.2.9/satsure_core/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.033806 satsure-core-test-0.2.9/satsure_core/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.034735 satsure-core-test-0.2.9/satsure_core/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-19 09:35:17.000000 satsure-core-test-0.2.9/satsure_core/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6366 2024-05-19 09:39:40.000000 satsure-core-test-0.2.9/satsure_core/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.035273 satsure-core-test-0.2.9/satsure_core/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       69 2024-05-19 09:35:17.000000 satsure-core-test-0.2.9/satsure_core/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5986 2024-05-19 10:00:10.000000 satsure-core-test-0.2.9/satsure_core/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.035805 satsure-core-test-0.2.9/satsure_core/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.036185 satsure-core-test-0.2.9/satsure_core/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.038491 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-19 09:57:43.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.039056 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2839 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-19 09:57:43.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3768 2024-05-20 07:41:47.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.039500 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3981 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2559 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.039810 satsure-core-test-0.2.9/satsure_core/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.040647 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:33:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      671 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      431 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_get_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      711 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_reproject.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.041711 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:33:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_mask_cloud.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_merge.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_offset_file.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_resample_file.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.044016 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      884 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-19 09:57:43.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.044351 satsure-core-test-0.2.9/satsure_core/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-19 09:39:40.000000 satsure-core-test-0.2.9/satsure_core/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.045051 satsure-core-test-0.2.9/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2724 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-20 14:04:19.045563 satsure-core-test-0.2.9/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      533 2024-05-20 14:03:47.000000 satsure-core-test-0.2.9/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.067850 satsure-core-test-0.3.0/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.0/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-22 06:43:33.067655 satsure-core-test-0.3.0/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.0/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.054073 satsure-core-test-0.3.0/satsure_core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.054273 satsure-core-test-0.3.0/satsure_core/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.055054 satsure-core-test-0.3.0/satsure_core/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.0/satsure_core/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.055475 satsure-core-test-0.3.0/satsure_core/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       69 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5986 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.056032 satsure-core-test-0.3.0/satsure_core/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.056322 satsure-core-test-0.3.0/satsure_core/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.0/satsure_core/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.061205 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.061693 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3217 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.062139 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.062444 satsure-core-test-0.3.0/satsure_core/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.063295 satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      671 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      431 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/test_get_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      711 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/test_reproject.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.064348 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_mask_cloud.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_merge.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_offset_file.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_resample_file.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.066245 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      884 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.066719 satsure-core-test-0.3.0/satsure_core/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.0/satsure_core/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:43:33.067434 satsure-core-test-0.3.0/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-22 06:43:32.000000 satsure-core-test-0.3.0/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2724 2024-05-22 06:43:32.000000 satsure-core-test-0.3.0/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-22 06:43:32.000000 satsure-core-test-0.3.0/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-22 06:43:32.000000 satsure-core-test-0.3.0/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-22 06:43:32.000000 satsure-core-test-0.3.0/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-22 06:43:33.067896 satsure-core-test-0.3.0/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-22 06:43:30.000000 satsure-core-test-0.3.0/setup.py
```

### Comparing `satsure-core-test-0.2.9/PKG-INFO` & `satsure-core-test-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.9
+Version: 0.3.0
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/config.py` & `satsure-core-test-0.3.0/satsure_core/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/core/downloader.py` & `satsure-core-test-0.3.0/satsure_core/satelite/core/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         :return:
         """
         request = self.retry_request(retries)
         response = request.get(source)
         if response.status_code == 200:
             with open(destination, 'wb') as f:
                 f.write(response.content)
+            print("download done for", source, destination)
+
             return True
 
         return False
 
     @staticmethod
     def validate_fields(tile_code: str, from_date: str,
                         download_path: PosixPath,
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/core/uploader.py` & `satsure-core-test-0.3.0/satsure_core/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.3.0/satsure_core/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/raster/raster.py` & `satsure-core-test-0.3.0/satsure_core/satelite/raster/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     :param cloud_mask_bands:
     :param cloud_mask_threshold:
     :param target_value:
     :param level:
     :return:
     """
     if len(cloud_mask_bands) != len(cloud_mask_threshold):
-        return False
+        raise ValueError("cloud_mask_threshold and cloud_mask_bands count is not same")
 
     output = Path(output_folder) / output_name
     Path(output_folder).mkdir(exist_ok=True, parents=True)
 
     img_A = rio.open(cloud_mask_bands[0])
     img_B = rio.open(cloud_mask_bands[1])
     img_C = rio.open(input_file)
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,7 +68,9 @@
                     output_crs=None,
                     output_pixel_size=(10, 10),
                     creation_option="COMPRESS=LZW",
                 )
                 if create_jpeg and fcc_path:
                     create_jpeg_image(fcc_path,
                                       bands_position=rgb_bands_position)
+
+        print("Create FCC process done")
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/get_tiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,56 +9,40 @@
 
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
         self.db = DBSession.create()
 
-    def fetch_tile_from_db(self, sql_query, geom_list):
+    def fetch_tile_from_db(self, sql_query, geom_):
         """
             Fetch tile from database
         :param sql_query:
         :param geom_:
         :return:
         """
 
-        result = self.db.execute(
-            sql_query,
-            {
-                "minx": geom_list['minx'][0],
-                "miny": geom_list['miny'][0],
-                "maxx": geom_list['maxx'][0],
-                "maxy": geom_list['maxy'][0],
-            },
-        )
+        result = self.db.execute(sql_query,
+                                 {"geojson_geometry": str(geom_)})
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
         """
         tile_list = set()
-        # print(geometry,geojson_geometry)
         sql_query = text(
             f"""SELECT tile FROM tileids WHERE ST_Intersects( geometry,
-                                            ST_GeomFromText(:geojson_geometry)) """
-        )
-        sql_query = text(
-            """
-                            SELECT tile FROM tileids
-                            WHERE ST_Intersects(
-                                geometry,
-                                ST_MakeEnvelope(:minx, :miny, :maxx, :maxy, 4326) -- 4326 is the SRID, adjust if needed
-                            )
-                            """
+                                            ST_GeomFromGeoJSON(:geojson_geometry)) """
         )
 
-        rows = self.fetch_tile_from_db(sql_query, geom_list)
-        for row in rows:
-            tile_list.add(row[0])
+        for geom_ in geom_list:
+            rows = self.fetch_tile_from_db(sql_query, geom_)
+            for row in rows:
+                tile_list.add(row[0])
 
         tile_list = list(tile_list)
         self.db.close()
 
         return tile_list
 
     def get_tile_from_rids(self, rids: list, shape_path: str):
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/indices/general_indices.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,7 +93,9 @@
                 index_path,
                 cloud_mask_output_folder,
                 output_name=f"{date}_{unique_tile}_IS1{band_combination_id}02{file_version}.tif",
                 cloud_mask_bands=cloud_mask_bands_path,
                 cloud_mask_threshold=cloud_mask_threshold,
                 level=self.level
             )
+
+        print("Normalized process is done")
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,27 @@
                     continue
                 files.sort()
                 date = files[0].stem.split(file_name_delimiter)[
                            date_identifier_position][:8]
                 creation_option = None
                 if input_file_format == "tif":
                     creation_option = "COMPRESS=LZW"
+                output_file_name = f"{date}_{unique_tile}_{band}.{input_file_format}"
                 merge(
                     files,
                     output_folder=str(self.output_folder),
-                    output_name=f"{date}_{unique_tile}_{band}.{input_file_format}",
+                    output_name=output_file_name,
                     output_nodata_value=0,
                     keep_separate=False,
                     output_format=None,
                     output_datatype=None,
                     output_crs=None,
                     output_pixel_size=(10, 10),
                     creation_option=creation_option
                 )
 
+                print("Output file name", output_file_name)
                 for file in files:
-                    if file.name == f"{date}_{unique_tile}_{band}.{input_file_format}":
+                    if file.name == output_file_name:
                         continue
+                    print("Deleting duplicate files", file.name)
                     file.unlink()
```

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.3.0/satsure_core/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/conftest.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_reproject.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/gdal/test_reproject.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_mask_cloud.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_mask_cloud.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_merge.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_merge.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_normalised_difference_index.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_normalised_difference_index.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_offset_file.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_offset_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_resample_file.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/raster/test_resample_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.3.0/satsure_core/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.3.0/satsure_core/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.9/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.3.0/satsure_core_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.9
+Version: 0.3.0
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.2.9/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.3.0/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

