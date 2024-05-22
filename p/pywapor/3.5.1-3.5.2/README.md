# Comparing `tmp/pywapor-3.5.1.tar.gz` & `tmp/pywapor-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywapor-3.5.1.tar", last modified: Wed Mar 27 15:41:53 2024, max compression
+gzip compressed data, was "pywapor-3.5.2.tar", last modified: Wed May 22 14:00:32 2024, max compression
```

## Comparing `pywapor-3.5.1.tar` & `pywapor-3.5.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.427584 pywapor-3.5.1/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2024-03-27 14:46:37.000000 pywapor-3.5.1/LICENSE
--rw-r--r--   0 hmcoerver   (501) staff       (20)      518 2024-03-27 14:46:37.000000 pywapor-3.5.1/MANIFEST.in
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-03-27 15:41:53.427336 pywapor-3.5.1/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13150 2024-03-27 14:46:52.000000 pywapor-3.5.1/README.md
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.409808 pywapor-3.5.1/pywapor/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      432 2024-03-27 14:46:52.000000 pywapor-3.5.1/pywapor/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.410885 pywapor-3.5.1/pywapor/collect/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15485 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/accounts.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10593 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/downloader.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.417815 pywapor-3.5.1/pywapor/collect/product/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5782 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/CHIRPS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8398 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/COPERNICUS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8540 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/ERA5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9011 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/GEOS5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1084450 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/GLO30.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1085475 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/GLO90.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/GLOBCOVER.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    39183 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/LANDSAT.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/MERRA2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/MODIS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/MODIS_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)    21329 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/SENTINEL2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7765 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/SENTINEL3.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7379 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/SRTM.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/SRTM30_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8376 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/STATICS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11418 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/TERRA.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    26281 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/VIIRSL1.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      370 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/product/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.418736 pywapor-3.5.1/pywapor/collect/protocol/
--rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9316 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/cds.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     4705 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/cog.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12151 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/copernicus_odata.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9959 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/crawler.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    19421 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/opendap.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/collect/protocol/projections.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.419823 pywapor-3.5.1/pywapor/configs/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16723 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/WaPOR2_level_1.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17024 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/WaPOR2_level_2.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    20735 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/WaPOR2_level_3.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    19718 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/WaPOR3_level_2.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    19620 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/WaPOR3_level_3.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    28403 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/all_in.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    19239 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/configs/nrt.json
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.421133 pywapor-3.5.1/pywapor/enhancers/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1597 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/apply_enhancers.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2773 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/dem.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.421758 pywapor-3.5.1/pywapor/enhancers/dms/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/dms/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/dms/pyDMS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/dms/pyDMS_utils.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16289 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/dms/thermal_sharpener.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/gap_fill.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/lulc.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/other.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/pressure.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.422433 pywapor-3.5.1/pywapor/enhancers/smooth/
--rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/smooth/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/smooth/archive.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/smooth/core.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/smooth/plotters.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13855 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/smooth/whittaker.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/temperature.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/enhancers/wind.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16310 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.424609 pywapor-3.5.1/pywapor/et_look_v2_v3/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/biomass.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/clear_sky_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/constants.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/evapotranspiration.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/leaf.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/meteo.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/neutral.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/resistance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6885 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/roughness.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/soil_moisture.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/solar_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/stress.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    24188 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/et_look_v2_v3/unstable.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.426562 pywapor-3.5.1/pywapor/general/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      304 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9590 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/aligner.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/bitmasks.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13267 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/compositer.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2746 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/curvilinear.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/lazifier.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32054 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/levels.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15505 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/log_indenter.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2241 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/logger.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2373 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/performance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/pre_defaults.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15740 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/processing_functions.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12558 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/reproject.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/units.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/general/variables.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    24221 2024-03-27 15:37:07.000000 pywapor-3.5.1/pywapor/main.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/post_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7259 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/pre_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6973 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/pre_se_root.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12004 2024-03-27 14:46:37.000000 pywapor-3.5.1/pywapor/se_root.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-27 15:41:53.426941 pywapor-3.5.1/pywapor.egg-info/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-03-27 15:41:53.000000 pywapor-3.5.1/pywapor.egg-info/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3160 2024-03-27 15:41:53.000000 pywapor-3.5.1/pywapor.egg-info/SOURCES.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2024-03-27 15:41:53.000000 pywapor-3.5.1/pywapor.egg-info/dependency_links.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)      203 2024-03-27 15:41:53.000000 pywapor-3.5.1/pywapor.egg-info/requires.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2024-03-27 15:41:53.000000 pywapor-3.5.1/pywapor.egg-info/top_level.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2024-03-27 15:41:53.427630 pywapor-3.5.1/setup.cfg
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1354 2024-03-27 14:46:52.000000 pywapor-3.5.1/setup.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.784295 pywapor-3.5.2/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2024-03-27 14:46:37.000000 pywapor-3.5.2/LICENSE
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      518 2024-03-27 14:46:37.000000 pywapor-3.5.2/MANIFEST.in
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-05-22 14:00:32.784088 pywapor-3.5.2/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13150 2024-03-27 14:46:52.000000 pywapor-3.5.2/README.md
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.743734 pywapor-3.5.2/pywapor/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      432 2024-05-20 13:50:40.000000 pywapor-3.5.2/pywapor/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.744791 pywapor-3.5.2/pywapor/collect/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15485 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/accounts.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10593 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/downloader.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.771397 pywapor-3.5.2/pywapor/collect/product/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5782 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/CHIRPS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8398 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/COPERNICUS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8540 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/ERA5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9011 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GEOS5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1084450 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GLO30.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1085475 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GLO90.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GLOBCOVER.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    39183 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/LANDSAT.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/MERRA2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/MODIS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/MODIS_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    21329 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SENTINEL2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7765 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SENTINEL3.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7379 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SRTM.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SRTM30_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8376 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/STATICS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11418 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/TERRA.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    26513 2024-05-20 12:31:05.000000 pywapor-3.5.2/pywapor/collect/product/VIIRSL1.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      370 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.772387 pywapor-3.5.2/pywapor/collect/protocol/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9316 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/cds.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     4705 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/cog.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12151 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/copernicus_odata.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9959 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/crawler.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    19421 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/opendap.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/projections.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.774043 pywapor-3.5.2/pywapor/configs/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17059 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR2_level_1.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17360 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR2_level_2.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    21071 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR2_level_3.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20940 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR3_level_2.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20842 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR3_level_3.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    30166 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/all_in.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20467 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/nrt.json
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.775307 pywapor-3.5.2/pywapor/enhancers/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1597 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/apply_enhancers.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2773 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dem.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.776437 pywapor-3.5.2/pywapor/enhancers/dms/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/pyDMS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/pyDMS_utils.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16289 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/thermal_sharpener.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/gap_fill.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/lulc.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/other.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/pressure.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.777132 pywapor-3.5.2/pywapor/enhancers/smooth/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/archive.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/core.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/plotters.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13855 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/whittaker.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/temperature.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/wind.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16310 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.780768 pywapor-3.5.2/pywapor/et_look_v2_v3/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/biomass.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/clear_sky_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/constants.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/evapotranspiration.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/leaf.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/meteo.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/neutral.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/resistance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6885 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/roughness.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/soil_moisture.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/solar_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/stress.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    24188 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/unstable.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.783288 pywapor-3.5.2/pywapor/general/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      304 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9590 2024-05-22 13:55:32.000000 pywapor-3.5.2/pywapor/general/aligner.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/bitmasks.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13267 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/compositer.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2746 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/curvilinear.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/lazifier.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32054 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/levels.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15505 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/log_indenter.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2241 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/logger.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2373 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/performance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/pre_defaults.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15740 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/processing_functions.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12558 2024-05-22 13:49:43.000000 pywapor-3.5.2/pywapor/general/reproject.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/units.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/variables.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    24332 2024-05-22 13:49:37.000000 pywapor-3.5.2/pywapor/main.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/post_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7259 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/pre_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6973 2024-05-22 13:55:50.000000 pywapor-3.5.2/pywapor/pre_se_root.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12004 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/se_root.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.783809 pywapor-3.5.2/pywapor.egg-info/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3160 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/SOURCES.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/dependency_links.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      203 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/requires.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/top_level.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2024-05-22 14:00:32.784350 pywapor-3.5.2/setup.cfg
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1354 2024-05-20 13:50:31.000000 pywapor-3.5.2/setup.py
```

### Comparing `pywapor-3.5.1/LICENSE` & `pywapor-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/MANIFEST.in` & `pywapor-3.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/PKG-INFO` & `pywapor-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywapor
-Version: 3.5.1
+Version: 3.5.2
 Home-page: https://www.fao.org/aquastat/py-wapor/
 Author: FAO
 Author-email: bert.coerver@fao.org
 License: Apache
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pywapor-3.5.1/README.md` & `pywapor-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/accounts.py` & `pywapor-3.5.2/pywapor/collect/accounts.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/downloader.py` & `pywapor-3.5.2/pywapor/collect/downloader.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/CHIRPS.py` & `pywapor-3.5.2/pywapor/collect/product/CHIRPS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/COPERNICUS.py` & `pywapor-3.5.2/pywapor/collect/product/COPERNICUS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/ERA5.py` & `pywapor-3.5.2/pywapor/collect/product/ERA5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/GEOS5.py` & `pywapor-3.5.2/pywapor/collect/product/GEOS5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/GLO30.txt` & `pywapor-3.5.2/pywapor/collect/product/GLO30.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/GLO90.txt` & `pywapor-3.5.2/pywapor/collect/product/GLO90.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/GLOBCOVER.py` & `pywapor-3.5.2/pywapor/collect/product/GLOBCOVER.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/LANDSAT.py` & `pywapor-3.5.2/pywapor/collect/product/LANDSAT.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/MERRA2.py` & `pywapor-3.5.2/pywapor/collect/product/MERRA2.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/MODIS.py` & `pywapor-3.5.2/pywapor/collect/product/MODIS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/MODIS_tiles.geojson` & `pywapor-3.5.2/pywapor/collect/product/MODIS_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/SENTINEL2.py` & `pywapor-3.5.2/pywapor/collect/product/SENTINEL2.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/SENTINEL3.py` & `pywapor-3.5.2/pywapor/collect/product/SENTINEL3.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/SRTM.py` & `pywapor-3.5.2/pywapor/collect/product/SRTM.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/SRTM30_tiles.geojson` & `pywapor-3.5.2/pywapor/collect/product/SRTM30_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/STATICS.py` & `pywapor-3.5.2/pywapor/collect/product/STATICS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/TERRA.py` & `pywapor-3.5.2/pywapor/collect/product/TERRA.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/product/VIIRSL1.py` & `pywapor-3.5.2/pywapor/collect/product/VIIRSL1.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,14 +473,21 @@
             geoloc = geoloc_.assign_coords(coords)
             geoloc = geoloc.where(
                         (geoloc.longitude < lonlim[1]) &
                         (geoloc.longitude > lonlim[0]) &
                         (geoloc.latitude > latlim[0]) &
                         (geoloc.latitude < latlim[1]), drop = True
                         )
+
+            if np.prod(list(geoloc.sizes.values())) == 0:
+                cleanup += [nc03_file]
+                log.info(f"--> Found 0 pixels inside AOI, skipping scene.").sub()
+                log.sub()
+                continue
+
             domain_375 = {k.replace("_375", ""): [adj(geoloc[k].min(), "even_down"), adj(geoloc[k].max(), "odd_up")] for k in geoloc.coords if "_375" in k}
             domain_750 = {k.replace("_750", ""): [int(geoloc[k].min()), int(geoloc[k].max())] for k in geoloc.coords if "_750" in k}
             log.info(f"--> Found {np.prod([v[1] - v[0] + 1 for v in domain_375.values()]):,} pixels inside AOI.").sub()
 
             geoloc_ds = geoloc_.isel({k: slice(v[0], v[1]+1) for k, v in domain_375.items()})
             lats_file_ds = save_ds(geoloc_ds[["latitude"]], os.path.join(folder, nc03_parts[-1].replace(".nc", "_lat.nc")), label = "Saving latitudes.")
             lats_file = lats_file_ds.encoding["source"]
```

### Comparing `pywapor-3.5.1/pywapor/collect/protocol/cds.py` & `pywapor-3.5.2/pywapor/collect/protocol/cds.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/protocol/cog.py` & `pywapor-3.5.2/pywapor/collect/protocol/cog.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/protocol/copernicus_odata.py` & `pywapor-3.5.2/pywapor/collect/protocol/copernicus_odata.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/protocol/crawler.py` & `pywapor-3.5.2/pywapor/collect/protocol/crawler.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/protocol/opendap.py` & `pywapor-3.5.2/pywapor/collect/protocol/opendap.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/collect/protocol/projections.py` & `pywapor-3.5.2/pywapor/collect/protocol/projections.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/configs/WaPOR2_level_1.json` & `pywapor-3.5.2/pywapor/configs/WaPOR2_level_1.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9769225063131313%*

 * *Differences: {"'et_look'": "{'ndvi': {'products': {0: {'product_name': 'MYD13Q1.061', 'is_example': False}, 1: "*

 * *              "{'product_name': 'MOD13Q1.061', 'is_example': True}}, 'temporal_interp': 'linear'}, "*

 * *              "'r0': {'temporal_interp': 'linear'}, 'se_root': {'products': {0: {'source': "*

 * *              "'FILE:{folder}{sep}se_root_out*.nc'}}, 'temporal_interp': 'linear'}, 'p': "*

 * *              "{'temporal_interp': 'linear'}, 'z': {'temporal_interp': 'linear'}, 'ra': "*

 * *              "{'temporal_interp': 'l […]*

```diff
@@ -7,85 +7,85 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.MODIS.mask_qa"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "MOD13Q1.061",
+                    "is_example": false,
+                    "product_name": "MYD13Q1.061",
                     "source": "MODIS"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.MODIS.mask_qa"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "MYD13Q1.061",
+                    "is_example": true,
+                    "product_name": "MOD13Q1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -95,15 +95,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -113,29 +113,29 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -161,85 +161,85 @@
                     ],
                     "is_example": false,
                     "product_name": "MCD43A3.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "M2T1NXRAD.5.12.4",
                     "source": "MERRA2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rs_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -249,15 +249,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -275,15 +275,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -301,127 +301,127 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "30M",
                     "source": "SRTM"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_obst_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_oro": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "land_mask": {
             "composite_type": "mean",
             "products": [
@@ -429,15 +429,15 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lst": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -463,85 +463,85 @@
                     ],
                     "is_example": false,
                     "product_name": "MOD11A1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.MODIS.mask_qa"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "MOD13Q1.061",
+                    "is_example": false,
+                    "product_name": "MYD13Q1.061",
                     "source": "MODIS"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.MODIS.mask_qa"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "MYD13Q1.061",
+                    "is_example": true,
+                    "product_name": "MOD13Q1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -551,15 +551,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -569,29 +569,29 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -617,85 +617,85 @@
                     ],
                     "is_example": false,
                     "product_name": "MCD43A3.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "M2T1NXRAD.5.12.4",
                     "source": "MERRA2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rs_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -705,15 +705,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -731,15 +731,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -757,141 +757,141 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "30M",
                     "source": "SRTM"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_obst_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_oro": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "lst": {
             "products": [
                 {
@@ -918,42 +918,42 @@
                     ],
                     "is_example": false,
                     "product_name": "MOD11A1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.MODIS.mask_qa"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "MOD13Q1.061",
+                    "is_example": false,
+                    "product_name": "MYD13Q1.061",
                     "source": "MODIS"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.MODIS.mask_qa"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "MYD13Q1.061",
+                    "is_example": true,
+                    "product_name": "MOD13Q1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -962,15 +962,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -979,28 +979,28 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1009,54 +1009,54 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": []
@@ -1074,28 +1074,28 @@
             "value": [
                 "GEOS5.inst3_2d_asm_Nx"
             ]
         },
         "optical": {
             "type": "set",
             "value": [
-                "MODIS.MOD13Q1.061",
-                "MODIS.MYD13Q1.061"
+                "MODIS.MYD13Q1.061",
+                "MODIS.MOD13Q1.061"
             ]
         },
         "precipitation": {
             "type": "set",
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "MERRA2.M2T1NXRAD.5.12.4"
             ]
```

### Comparing `pywapor-3.5.1/pywapor/configs/WaPOR2_level_2.json` & `pywapor-3.5.2/pywapor/configs/WaPOR2_level_2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782068602693602%*

 * *Differences: {"'et_look'": "{'ndvi': {'temporal_interp': 'linear'}, 'r0': {'temporal_interp': 'linear'}, "*

 * *              "'se_root': {'products': {0: {'source': 'FILE:{folder}{sep}se_root_out*.nc'}}, "*

 * *              "'temporal_interp': 'linear'}, 'p': {'temporal_interp': 'linear'}, 'z': "*

 * *              "{'temporal_interp': 'linear'}, 'ra': {'temporal_interp': 'linear'}, 'u2m': "*

 * *              "{'temporal_interp': 'linear'}, 'v2m': {'temporal_interp': 'linear'}, 'p_air': "*

 * *              "{'temporal_interp': 'linear'}, 'p […]*

```diff
@@ -7,43 +7,43 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -68,29 +68,29 @@
                     ],
                     "is_example": true,
                     "product_name": "urn:eop:VITO:PROBAV_S5_TOC_100M_COG_V2",
                     "source": "TERRA"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -100,15 +100,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -118,29 +118,29 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -170,85 +170,85 @@
                     ],
                     "is_example": true,
                     "product_name": "urn:eop:VITO:PROBAV_S5_TOC_100M_COG_V2",
                     "source": "TERRA"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "M2T1NXRAD.5.12.4",
                     "source": "MERRA2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rs_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -258,15 +258,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -284,15 +284,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -310,127 +310,127 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "30M",
                     "source": "SRTM"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_obst_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_oro": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "land_mask": {
             "composite_type": "mean",
             "products": [
@@ -438,15 +438,15 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lst": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -472,43 +472,43 @@
                     ],
                     "is_example": false,
                     "product_name": "MOD11A1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -533,29 +533,29 @@
                     ],
                     "is_example": true,
                     "product_name": "urn:eop:VITO:PROBAV_S5_TOC_100M_COG_V2",
                     "source": "TERRA"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -565,15 +565,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -583,29 +583,29 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -635,85 +635,85 @@
                     ],
                     "is_example": true,
                     "product_name": "urn:eop:VITO:PROBAV_S5_TOC_100M_COG_V2",
                     "source": "TERRA"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "M2T1NXRAD.5.12.4",
                     "source": "MERRA2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rs_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -723,15 +723,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -749,15 +749,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -775,141 +775,141 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "30M",
                     "source": "SRTM"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_obst_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_oro": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "lst": {
             "products": [
                 {
@@ -936,15 +936,15 @@
                     ],
                     "is_example": false,
                     "product_name": "MOD11A1.061",
                     "source": "MODIS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -968,15 +968,15 @@
                     ],
                     "is_example": true,
                     "product_name": "urn:eop:VITO:PROBAV_S5_TOC_100M_COG_V2",
                     "source": "TERRA"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -985,15 +985,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1002,28 +1002,28 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1032,54 +1032,54 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": []
@@ -1109,15 +1109,15 @@
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "MERRA2.M2T1NXRAD.5.12.4"
             ]
```

### Comparing `pywapor-3.5.1/pywapor/configs/WaPOR2_level_3.json` & `pywapor-3.5.2/pywapor/configs/WaPOR2_level_3.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758296550575196%*

 * *Differences: {"'et_look'": "{'ndvi': {'products': {0: {'product_name': 'LC08_SR', 'is_example': True}, 1: "*

 * *              "{'product_name': 'LC09_SR'}, 2: {'product_name': 'LT05_SR', 'is_example': False}, "*

 * *              "3: {'product_name': 'LE07_SR'}}, 'temporal_interp': 'linear'}, 'r0': {'products': "*

 * *              "{0: {'product_name': 'LC08_SR', 'enhancers': {0: {'keywords': {'product_name': "*

 * *              "'LC08_SR'}}}, 'is_example': True}, 1: {'product_name': 'LC09_SR', 'enhancers': {0: "*

 * *              "{'keywor […]*

```diff
@@ -7,117 +7,117 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
+                    "is_example": true,
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "LC08_SR",
+                    "is_example": false,
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -127,15 +127,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -145,187 +145,187 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC09_SR"
+                                "product_name": "LC08_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
+                    "is_example": true,
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LE07_SR"
+                                "product_name": "LC09_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC08_SR"
+                                "product_name": "LT05_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "LC08_SR",
+                    "is_example": false,
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LT05_SR"
+                                "product_name": "LE07_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "M2T1NXRAD.5.12.4",
                     "source": "MERRA2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rs_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -335,15 +335,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -361,15 +361,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -387,127 +387,127 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "30M",
                     "source": "SRTM"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_obst_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_oro": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "land_mask": {
             "composite_type": "mean",
             "products": [
@@ -515,15 +515,15 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lst": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -531,161 +531,161 @@
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_ST",
+                    "product_name": "LC08_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_ST",
+                    "product_name": "LT05_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC09_ST",
+                    "product_name": "LE07_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_ST",
+                    "product_name": "LC09_ST",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
+                    "is_example": true,
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "LC08_SR",
+                    "is_example": false,
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -695,15 +695,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -713,187 +713,187 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC09_SR"
+                                "product_name": "LC08_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
+                    "is_example": true,
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LE07_SR"
+                                "product_name": "LC09_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC08_SR"
+                                "product_name": "LT05_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "LC08_SR",
+                    "is_example": false,
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LT05_SR"
+                                "product_name": "LE07_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "M2T1NXRAD.5.12.4",
                     "source": "MERRA2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rs_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -903,15 +903,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -929,15 +929,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -955,141 +955,141 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "30M",
                     "source": "SRTM"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_obst_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z_oro": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR2",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "lst": {
             "products": [
                 {
@@ -1098,118 +1098,118 @@
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_ST",
+                    "product_name": "LC08_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_ST",
+                    "product_name": "LT05_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC09_ST",
+                    "product_name": "LE07_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_ST",
+                    "product_name": "LC09_ST",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
+                    "is_example": true,
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "LC08_SR",
+                    "is_example": false,
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1218,15 +1218,15 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1235,28 +1235,28 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "qv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1265,54 +1265,54 @@
                     ],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "inst3_2d_asm_Nx",
                     "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": []
@@ -1330,30 +1330,30 @@
             "value": [
                 "GEOS5.inst3_2d_asm_Nx"
             ]
         },
         "optical": {
             "type": "set",
             "value": [
-                "LANDSAT.LC09_SR",
-                "LANDSAT.LE07_SR",
                 "LANDSAT.LC08_SR",
-                "LANDSAT.LT05_SR"
+                "LANDSAT.LC09_SR",
+                "LANDSAT.LT05_SR",
+                "LANDSAT.LE07_SR"
             ]
         },
         "precipitation": {
             "type": "set",
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "MERRA2.M2T1NXRAD.5.12.4"
             ]
@@ -1363,15 +1363,15 @@
             "value": [
                 "STATICS.WaPOR2"
             ]
         },
         "thermal": {
             "type": "set",
             "value": [
-                "LANDSAT.LE07_ST",
                 "LANDSAT.LC08_ST",
-                "LANDSAT.LC09_ST",
-                "LANDSAT.LT05_ST"
+                "LANDSAT.LT05_ST",
+                "LANDSAT.LE07_ST",
+                "LANDSAT.LC09_ST"
             ]
         }
     }
 }
```

### Comparing `pywapor-3.5.1/pywapor/configs/WaPOR3_level_2.json` & `pywapor-3.5.2/pywapor/configs/WaPOR3_level_2.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9732501298264906%*

 * *Differences: {"'et_look'": "{'ndvi': {'temporal_interp': {replace: OrderedDict([('lmbdas', 1000.0), ('method', "*

 * *              "'whittaker')])}}, 'r0': {'temporal_interp': {replace: OrderedDict([('lmbdas', "*

 * *              "1000.0), ('method', 'whittaker')])}}, 'se_root': {'products': {0: {'source': "*

 * *              "'FILE:{folder}{sep}se_root_out*.nc'}}, 'temporal_interp': 'linear'}, 'p': "*

 * *              "{'temporal_interp': 'linear'}, 'z': {'temporal_interp': 'linear'}, 'ra': "*

 * *              "{'temporal_interp': 'linear […]*

```diff
@@ -7,29 +7,29 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -42,29 +42,32 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -74,15 +77,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -92,15 +95,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -113,15 +116,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -131,57 +137,57 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -191,15 +197,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -217,15 +223,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -243,29 +249,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_dew": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -275,29 +281,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -310,43 +316,43 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO90",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -361,15 +367,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -388,15 +397,19 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
@@ -408,43 +421,46 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -467,15 +483,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -488,15 +507,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -506,15 +528,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -527,29 +552,32 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -559,15 +587,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -577,15 +605,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -598,15 +626,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -619,15 +650,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -637,57 +671,57 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -697,15 +731,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -723,15 +757,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -749,29 +783,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_dew": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -781,29 +815,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -816,15 +850,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -834,15 +868,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -852,15 +886,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -873,57 +907,60 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO90",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -938,15 +975,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -964,15 +1004,19 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
@@ -984,15 +1028,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1015,15 +1062,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1035,15 +1085,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1053,15 +1106,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1074,15 +1130,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1091,15 +1150,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1108,15 +1167,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1129,15 +1188,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1146,15 +1208,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_dew": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1163,15 +1225,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1183,15 +1245,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1204,40 +1266,53 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R60m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": [
                 "bt"
             ]
         },
         "_EXAMPLE_": "SENTINEL2.S2MSI2A_R60m",
-        "_WHITTAKER_": {},
+        "_WHITTAKER_": {
+            "SENTINEL2.S2MSI2A_R60m": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "VIIRSL1.VNP02IMG": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            }
+        },
         "elevation": {
             "type": "set",
             "value": [
                 "COPERNICUS.GLO90"
             ]
         },
         "meteorological": {
@@ -1257,15 +1332,15 @@
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "ERA5.sis-agrometeorological-indicators"
             ]
```

### Comparing `pywapor-3.5.1/pywapor/configs/WaPOR3_level_3.json` & `pywapor-3.5.2/pywapor/configs/nrt.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9010495902468982%*

 * *Differences: {"'et_look'": "{'ndvi': {'temporal_interp': {replace: OrderedDict([('lmbdas', 1000.0), ('method', "*

 * *              "'whittaker')])}}, 'r0': {'temporal_interp': {replace: OrderedDict([('lmbdas', "*

 * *              "1000.0), ('method', 'whittaker')])}}, 'se_root': {'products': {0: {'source': "*

 * *              "'FILE:{folder}{sep}se_root_out*.nc'}}, 'temporal_interp': 'linear'}, 'p': "*

 * *              "{'temporal_interp': 'linear'}, 'z': {'temporal_interp': 'linear'}, 'ra': "*

 * *              "{'temporal_interp': 'linear […]*

```diff
@@ -7,29 +7,29 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -42,65 +42,82 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
+                }
+            ],
+            "spatial_interp": "bilinear",
+            "temporal_interp": "linear",
+            "variable_enhancers": []
+        },
+        "qv": {
+            "composite_type": "mean",
+            "products": [
+                {
+                    "enhancers": [],
+                    "is_example": false,
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -113,15 +130,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -131,75 +151,75 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -212,20 +232,20 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_max"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -238,115 +258,112 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_min"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "t_dew": {
+        "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
-                    "enhancers": [
-                        {
-                            "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
-                        }
-                    ],
+                    "enhancers": [],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "WaPOR3",
+                    "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "t_opt": {
+        "u2m": {
             "composite_type": "mean",
             "products": [
                 {
-                    "enhancers": [],
+                    "enhancers": [
+                        {
+                            "func": "pywapor.enhancers.wind.adjust_wind_height"
+                        }
+                    ],
                     "is_example": false,
-                    "product_name": "WaPOR3",
-                    "source": "STATICS"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "u": {
+        "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.enhancers.wind.windspeed"
-                        },
-                        {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO30",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -361,15 +378,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -388,15 +408,19 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
@@ -408,43 +432,46 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -467,15 +494,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -488,15 +518,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -506,15 +539,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -527,65 +563,68 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -595,15 +634,32 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "variable_enhancers": []
+        },
+        "qv": {
+            "composite_type": "mean",
+            "products": [
+                {
+                    "enhancers": [],
+                    "is_example": false,
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
+                }
+            ],
+            "spatial_interp": "bilinear",
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -616,15 +672,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -634,75 +693,75 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -715,20 +774,20 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_max"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -741,123 +800,84 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_min"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
-            "variable_enhancers": []
-        },
-        "t_dew": {
-            "composite_type": "mean",
-            "products": [
-                {
-                    "enhancers": [
-                        {
-                            "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
-                        }
-                    ],
-                    "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
-                }
-            ],
-            "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
-            "variable_enhancers": []
-        },
-        "u": {
-            "composite_type": "mean",
-            "products": [
-                {
-                    "enhancers": [
-                        {
-                            "func": "pywapor.enhancers.wind.windspeed"
-                        },
-                        {
-                            "func": "pywapor.enhancers.wind.adjust_wind_height"
-                        }
-                    ],
-                    "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
-                }
-            ],
-            "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -870,57 +890,60 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO30",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -935,15 +958,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -961,15 +987,19 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
@@ -981,15 +1011,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1012,15 +1045,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1032,15 +1068,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1050,15 +1089,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1071,49 +1113,52 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1123,69 +1168,82 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "variable_enhancers": []
+        },
+        "qv": {
+            "products": [
+                {
+                    "enhancers": [],
+                    "is_example": false,
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
+                }
+            ],
+            "spatial_interp": "bilinear",
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "t_dew": {
+        "u2m": {
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
+                            "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "u": {
+        "v2m": {
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.enhancers.wind.windspeed"
-                        },
-                        {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1198,50 +1256,63 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
-                    "product_name": "reanalysis-era5-single-levels",
-                    "source": "ERA5"
+                    "product_name": "tavg1_2d_slv_Nx",
+                    "source": "GEOS5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": [
                 "bt"
             ]
         },
         "_EXAMPLE_": "SENTINEL2.S2MSI2A_R20m",
-        "_WHITTAKER_": {},
+        "_WHITTAKER_": {
+            "SENTINEL2.S2MSI2A_R20m": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "VIIRSL1.VNP02IMG": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            }
+        },
         "elevation": {
             "type": "set",
             "value": [
                 "COPERNICUS.GLO30"
             ]
         },
         "meteorological": {
             "type": "set",
             "value": [
-                "ERA5.reanalysis-era5-single-levels"
+                "GEOS5.tavg1_2d_slv_Nx"
             ]
         },
         "optical": {
             "type": "set",
             "value": [
                 "SENTINEL2.S2MSI2A_R20m"
             ]
@@ -1251,15 +1322,15 @@
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "ERA5.sis-agrometeorological-indicators"
             ]
```

### Comparing `pywapor-3.5.1/pywapor/configs/all_in.json` & `pywapor-3.5.2/pywapor/configs/all_in.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9706255601494858%*

 * *Differences: {"'et_look'": "{'ndvi': {'products': {insert: [(0, OrderedDict([('source', 'LANDSAT'), "*

 * *              "('product_name', 'LC08_SR'), ('enhancers', [OrderedDict([('func', "*

 * *              "'pywapor.collect.product.LANDSAT.calc_normalized_difference')]), "*

 * *              "OrderedDict([('func', 'pywapor.enhancers.gap_fill.gap_fill')])]), ('is_example', "*

 * *              "False)]))], delete: [3]}, 'temporal_interp': {replace: OrderedDict([('lmbdas', "*

 * *              "1000.0), ('method', 'whittaker')])}}, 'r0': {'pro […]*

```diff
@@ -7,84 +7,84 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.SENTINEL2.calc_normalized_difference"
+                            "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
+                            "func": "pywapor.collect.product.SENTINEL2.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
@@ -94,29 +94,32 @@
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -126,15 +129,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -144,91 +147,91 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.SENTINEL2.calc_r0"
-                        },
-                        {
-                            "func": "pywapor.enhancers.gap_fill.gap_fill"
-                        }
-                    ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
-                },
-                {
-                    "enhancers": [
-                        {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC09_SR"
+                                "product_name": "LC08_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC09_SR",
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
+                            "func": "pywapor.collect.product.SENTINEL2.calc_r0"
+                        },
+                        {
+                            "func": "pywapor.enhancers.gap_fill.gap_fill"
+                        }
+                    ],
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
+                },
+                {
+                    "enhancers": [
+                        {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LT05_SR"
+                                "product_name": "LC09_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC08_SR"
+                                "product_name": "LT05_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
@@ -245,15 +248,18 @@
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -263,57 +269,57 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -323,15 +329,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -349,15 +355,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -375,29 +381,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_dew": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -407,29 +413,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -442,43 +448,43 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO30",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -493,15 +499,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -520,75 +529,81 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "lst": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -596,59 +611,62 @@
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_ST",
+                    "product_name": "LT05_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_ST",
+                    "product_name": "LC09_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC09_ST",
+                    "product_name": "LC08_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_ST",
+                    "product_name": "LE07_ST",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
@@ -656,29 +674,29 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -701,70 +719,73 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.SENTINEL2.calc_normalized_difference"
+                            "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
+                            "func": "pywapor.collect.product.SENTINEL2.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
@@ -774,73 +795,79 @@
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -853,29 +880,32 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -885,15 +915,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -903,15 +933,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -921,91 +951,94 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.SENTINEL2.calc_r0"
-                        },
-                        {
-                            "func": "pywapor.enhancers.gap_fill.gap_fill"
-                        }
-                    ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
-                },
-                {
-                    "enhancers": [
-                        {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC09_SR"
+                                "product_name": "LC08_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC09_SR",
+                    "product_name": "LC08_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
+                            "func": "pywapor.collect.product.SENTINEL2.calc_r0"
+                        },
+                        {
+                            "func": "pywapor.enhancers.gap_fill.gap_fill"
+                        }
+                    ],
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
+                },
+                {
+                    "enhancers": [
+                        {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LT05_SR"
+                                "product_name": "LC09_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
                                 "value": []
                             },
                             "func": "pywapor.collect.product.LANDSAT.calc_r0",
                             "keywords": {
-                                "product_name": "LC08_SR"
+                                "product_name": "LT05_SR"
                             }
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "args": {
                                 "type": "tuple",
@@ -1022,15 +1055,18 @@
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1040,57 +1076,57 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1100,15 +1136,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -1126,15 +1162,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -1152,29 +1188,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_dew": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1184,29 +1220,29 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1219,15 +1255,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1237,15 +1273,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1255,15 +1291,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1276,57 +1312,60 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO30",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -1341,15 +1380,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1367,134 +1409,143 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "lst": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LE07_ST",
+                    "product_name": "LT05_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_ST",
+                    "product_name": "LC09_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC09_ST",
+                    "product_name": "LC08_ST",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.mask_uncertainty"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_ST",
+                    "product_name": "LE07_ST",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
@@ -1519,69 +1570,72 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.SENTINEL2.calc_normalized_difference"
+                            "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
+                            "func": "pywapor.collect.product.SENTINEL2.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.collect.product.LANDSAT.calc_normalized_difference"
                         },
@@ -1591,73 +1645,79 @@
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": true,
-                    "product_name": "S2MSI2A_R20m",
-                    "source": "SENTINEL2"
+                    "is_example": false,
+                    "product_name": "LC08_SR",
+                    "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
-                    "is_example": false,
-                    "product_name": "LC09_SR",
-                    "source": "LANDSAT"
+                    "is_example": true,
+                    "product_name": "S2MSI2A_R20m",
+                    "source": "SENTINEL2"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LT05_SR",
+                    "product_name": "LC09_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "LC08_SR",
+                    "product_name": "LT05_SR",
                     "source": "LANDSAT"
                 },
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.gap_fill.gap_fill"
                         }
                     ],
                     "is_example": false,
                     "product_name": "LE07_SR",
                     "source": "LANDSAT"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1670,15 +1730,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1687,15 +1750,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1704,15 +1767,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1722,15 +1785,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1739,15 +1805,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_dew": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1756,15 +1822,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1776,15 +1842,15 @@
                     ],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1797,41 +1863,85 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "reanalysis-era5-single-levels",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": [
-                "bt",
-                "lst"
+                "lst",
+                "bt"
             ]
         },
         "_EXAMPLE_": "SENTINEL2.S2MSI2A_R20m",
-        "_WHITTAKER_": {},
+        "_WHITTAKER_": {
+            "LANDSAT.LC08_SR": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LC08_ST": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LC09_SR": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LC09_ST": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LE07_SR": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LE07_ST": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LT05_SR": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "LANDSAT.LT05_ST": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "SENTINEL2.S2MSI2A_R20m": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "VIIRSL1.VNP02IMG": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            }
+        },
         "elevation": {
             "type": "set",
             "value": [
                 "COPERNICUS.GLO30"
             ]
         },
         "meteorological": {
@@ -1839,31 +1949,31 @@
             "value": [
                 "ERA5.reanalysis-era5-single-levels"
             ]
         },
         "optical": {
             "type": "set",
             "value": [
-                "LANDSAT.LC08_SR",
-                "LANDSAT.LE07_SR",
                 "SENTINEL2.S2MSI2A_R20m",
                 "LANDSAT.LC09_SR",
+                "LANDSAT.LE07_SR",
+                "LANDSAT.LC08_SR",
                 "LANDSAT.LT05_SR"
             ]
         },
         "precipitation": {
             "type": "set",
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "ERA5.sis-agrometeorological-indicators"
             ]
```

### Comparing `pywapor-3.5.1/pywapor/configs/nrt.json` & `pywapor-3.5.2/pywapor/configs/WaPOR3_level_3.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9010495902468982%*

 * *Differences: {"'et_look'": "{'ndvi': {'temporal_interp': {replace: OrderedDict([('lmbdas', 1000.0), ('method', "*

 * *              "'whittaker')])}}, 'r0': {'temporal_interp': {replace: OrderedDict([('lmbdas', "*

 * *              "1000.0), ('method', 'whittaker')])}}, 'se_root': {'products': {0: {'source': "*

 * *              "'FILE:{folder}{sep}se_root_out*.nc'}}, 'temporal_interp': 'linear'}, 'p': "*

 * *              "{'temporal_interp': 'linear'}, 'z': {'temporal_interp': 'linear'}, 'ra': "*

 * *              "{'temporal_interp': 'linear […]*

```diff
@@ -7,29 +7,29 @@
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -42,79 +42,68 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
-                }
-            ],
-            "spatial_interp": "bilinear",
-            "temporal_interp": [],
-            "variable_enhancers": []
-        },
-        "qv": {
-            "composite_type": "mean",
-            "products": [
-                {
-                    "enhancers": [],
-                    "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -127,15 +116,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -145,75 +137,75 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -226,20 +218,20 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_max"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -252,112 +244,115 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_min"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "t_opt": {
+        "t_dew": {
             "composite_type": "mean",
             "products": [
                 {
-                    "enhancers": [],
+                    "enhancers": [
+                        {
+                            "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
+                        }
+                    ],
                     "is_example": false,
-                    "product_name": "WaPOR3",
-                    "source": "STATICS"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "u2m": {
+        "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
-                    "enhancers": [
-                        {
-                            "func": "pywapor.enhancers.wind.adjust_wind_height"
-                        }
-                    ],
+                    "enhancers": [],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "WaPOR3",
+                    "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "v2m": {
+        "u": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
+                            "func": "pywapor.enhancers.wind.windspeed"
+                        },
+                        {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO30",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "full": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -372,15 +367,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -399,15 +397,19 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
@@ -419,43 +421,46 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "lw_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "lw_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -478,15 +483,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -499,15 +507,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -517,15 +528,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -538,65 +552,68 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "P05",
                     "source": "CHIRPS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -606,29 +623,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
-            "variable_enhancers": []
-        },
-        "qv": {
-            "composite_type": "mean",
-            "products": [
-                {
-                    "enhancers": [],
-                    "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
-                }
-            ],
-            "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "r0": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -641,15 +647,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ra": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -659,75 +668,75 @@
                     ],
                     "is_example": false,
                     "product_name": "sis-agrometeorological-indicators",
                     "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_offset": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "rn_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "se_root": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "from_file",
-                    "source": "FILE:{folder}{sep}se_root_out*.nc.from_file"
+                    "source": "FILE:{folder}{sep}se_root_out*.nc"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_max": {
             "composite_type": "max",
             "products": [
                 {
                     "enhancers": [
@@ -740,20 +749,20 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_max"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_air_min": {
             "composite_type": "min",
             "products": [
                 {
                     "enhancers": [
@@ -766,84 +775,123 @@
                             "keywords": {
                                 "in_var": "t_air",
                                 "out_var": "t_air_min"
                             }
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_amp": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
+            "variable_enhancers": []
+        },
+        "t_dew": {
+            "composite_type": "mean",
+            "products": [
+                {
+                    "enhancers": [
+                        {
+                            "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
+                        }
+                    ],
+                    "is_example": false,
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
+                }
+            ],
+            "spatial_interp": "bilinear",
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "t_opt": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
+            "variable_enhancers": []
+        },
+        "u": {
+            "composite_type": "mean",
+            "products": [
+                {
+                    "enhancers": [
+                        {
+                            "func": "pywapor.enhancers.wind.windspeed"
+                        },
+                        {
+                            "func": "pywapor.enhancers.wind.adjust_wind_height"
+                        }
+                    ],
+                    "is_example": false,
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
+                }
+            ],
+            "spatial_interp": "bilinear",
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "u2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "v2m": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -856,57 +904,60 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "vpd_slope": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "WaPOR3",
                     "source": "STATICS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "wv": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "z": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
                     "product_name": "GLO30",
                     "source": "COPERNICUS"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "se_root": {
         "bsi": {
             "composite_type": "mean",
             "products": [
@@ -921,15 +972,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "bt": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -947,15 +1001,19 @@
                     ],
                     "is_example": false,
                     "product_name": "VNP02IMG",
                     "source": "VIIRSL1"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": [
                 "pywapor.enhancers.dms.thermal_sharpener.sharpen"
             ]
         },
         "green": {
             "composite_type": "mean",
             "products": [
@@ -967,15 +1025,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "mndwi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -998,15 +1059,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "ndvi": {
             "products": [
                 {
                     "enhancers": [
                         {
@@ -1018,15 +1082,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nir": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1036,15 +1103,18 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "nmdi": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1057,49 +1127,52 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "p_air": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "p_air_0": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.pressure.pa_to_kpa"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "psri": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1109,79 +1182,72 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
-            "variable_enhancers": []
-        },
-        "qv": {
-            "products": [
-                {
-                    "enhancers": [],
-                    "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
-                }
-            ],
-            "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "t_air": {
             "products": [
                 {
                     "enhancers": [
                         {
                             "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "u2m": {
+        "t_dew": {
             "products": [
                 {
                     "enhancers": [
                         {
-                            "func": "pywapor.enhancers.wind.adjust_wind_height"
+                            "func": "pywapor.enhancers.temperature.kelvin_to_celsius"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
-        "v2m": {
+        "u": {
             "products": [
                 {
                     "enhancers": [
                         {
+                            "func": "pywapor.enhancers.wind.windspeed"
+                        },
+                        {
                             "func": "pywapor.enhancers.wind.adjust_wind_height"
                         }
                     ],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         },
         "vari_red_edge": {
             "composite_type": "mean",
             "products": [
                 {
                     "enhancers": [
@@ -1194,50 +1260,63 @@
                     ],
                     "is_example": true,
                     "product_name": "S2MSI2A_R20m",
                     "source": "SENTINEL2"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
             "variable_enhancers": []
         },
         "wv": {
             "products": [
                 {
                     "enhancers": [],
                     "is_example": false,
-                    "product_name": "tavg1_2d_slv_Nx",
-                    "source": "GEOS5"
+                    "product_name": "reanalysis-era5-single-levels",
+                    "source": "ERA5"
                 }
             ],
             "spatial_interp": "bilinear",
-            "temporal_interp": [],
+            "temporal_interp": "linear",
             "variable_enhancers": []
         }
     },
     "summary": {
         "_ENHANCE_": {
             "type": "set",
             "value": [
                 "bt"
             ]
         },
         "_EXAMPLE_": "SENTINEL2.S2MSI2A_R20m",
-        "_WHITTAKER_": {},
+        "_WHITTAKER_": {
+            "SENTINEL2.S2MSI2A_R20m": {
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            },
+            "VIIRSL1.VNP02IMG": {
+                "a": 0.85,
+                "lmbdas": 1000.0,
+                "method": "whittaker"
+            }
+        },
         "elevation": {
             "type": "set",
             "value": [
                 "COPERNICUS.GLO30"
             ]
         },
         "meteorological": {
             "type": "set",
             "value": [
-                "GEOS5.tavg1_2d_slv_Nx"
+                "ERA5.reanalysis-era5-single-levels"
             ]
         },
         "optical": {
             "type": "set",
             "value": [
                 "SENTINEL2.S2MSI2A_R20m"
             ]
@@ -1247,15 +1326,15 @@
             "value": [
                 "CHIRPS.P05"
             ]
         },
         "soil moisture": {
             "type": "set",
             "value": [
-                "FILE:{folder}{sep}se_root_out*.nc.from_file.from_file"
+                "FILE:{folder}{sep}se_root_out*.nc.from_file"
             ]
         },
         "solar radiation": {
             "type": "set",
             "value": [
                 "ERA5.sis-agrometeorological-indicators"
             ]
```

### Comparing `pywapor-3.5.1/pywapor/enhancers/apply_enhancers.py` & `pywapor-3.5.2/pywapor/enhancers/apply_enhancers.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/dem.py` & `pywapor-3.5.2/pywapor/enhancers/dem.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/dms/pyDMS.py` & `pywapor-3.5.2/pywapor/enhancers/dms/pyDMS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/dms/pyDMS_utils.py` & `pywapor-3.5.2/pywapor/enhancers/dms/pyDMS_utils.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/dms/thermal_sharpener.py` & `pywapor-3.5.2/pywapor/enhancers/dms/thermal_sharpener.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/gap_fill.py` & `pywapor-3.5.2/pywapor/enhancers/gap_fill.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/lulc.py` & `pywapor-3.5.2/pywapor/enhancers/lulc.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/other.py` & `pywapor-3.5.2/pywapor/enhancers/other.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/smooth/archive.py` & `pywapor-3.5.2/pywapor/enhancers/smooth/archive.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/smooth/core.py` & `pywapor-3.5.2/pywapor/enhancers/smooth/core.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/smooth/plotters.py` & `pywapor-3.5.2/pywapor/enhancers/smooth/plotters.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/smooth/whittaker.py` & `pywapor-3.5.2/pywapor/enhancers/smooth/whittaker.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/temperature.py` & `pywapor-3.5.2/pywapor/enhancers/temperature.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/enhancers/wind.py` & `pywapor-3.5.2/pywapor/enhancers/wind.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look.py` & `pywapor-3.5.2/pywapor/et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/__init__.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/biomass.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/biomass.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/clear_sky_radiation.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/constants.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/constants.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/evapotranspiration.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/leaf.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/leaf.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/meteo.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/meteo.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/neutral.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/neutral.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/radiation.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/resistance.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/resistance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/roughness.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/roughness.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/soil_moisture.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/solar_radiation.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/stress.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/stress.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/et_look_v2_v3/unstable.py` & `pywapor-3.5.2/pywapor/et_look_v2_v3/unstable.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/aligner.py` & `pywapor-3.5.2/pywapor/general/aligner.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/bitmasks.py` & `pywapor-3.5.2/pywapor/general/bitmasks.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/compositer.py` & `pywapor-3.5.2/pywapor/general/compositer.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/curvilinear.py` & `pywapor-3.5.2/pywapor/general/curvilinear.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/lazifier.py` & `pywapor-3.5.2/pywapor/general/lazifier.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/levels.py` & `pywapor-3.5.2/pywapor/general/levels.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/log_indenter.py` & `pywapor-3.5.2/pywapor/general/log_indenter.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/logger.py` & `pywapor-3.5.2/pywapor/general/logger.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/performance.py` & `pywapor-3.5.2/pywapor/general/performance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/pre_defaults.py` & `pywapor-3.5.2/pywapor/general/pre_defaults.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/processing_functions.py` & `pywapor-3.5.2/pywapor/general/processing_functions.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/reproject.py` & `pywapor-3.5.2/pywapor/general/reproject.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/units.py` & `pywapor-3.5.2/pywapor/general/units.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/general/variables.py` & `pywapor-3.5.2/pywapor/general/variables.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/main.py` & `pywapor-3.5.2/pywapor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         log.sub().info("--> Configuration loaded.")
         return config
     
     @classmethod
     def from_summary(cls, summary):
         log.info(f"--> Creating configuration from summary.").add()
         example_product = summary.pop('_EXAMPLE_', '')
-        temporal_interp = summary.pop('_TEMP_INTERP_', {})
+        temporal_interp = summary.pop('_WHITTAKER_', {})
         enhance = summary.pop('_ENHANCE_', {})
 
         full = dict()
 
         unique_enhancers = set([item for row in list(enhance.values()) for item in row])
         extra_vars = list()
         for enhancer in unique_enhancers:
@@ -240,15 +240,18 @@
 
                             products += [{
                                 "source": cls.source_func(prod), 
                                 "product_name": cls.pname_func(prod), 
                                 "enhancers": enhancers,
                                 "is_example": prod == example_product,
                                 }]
-                        t_interps += [temporal_interp.get(prod, [])]
+                            
+                        x = temporal_interp.get(prod, None)
+                        if not isinstance(x, type(None)):
+                            t_interps += [x]
                     
                     if len(products) == 0:
                         continue
 
                     if len(t_interps) == 0:
                         temporal_interp_ = "linear"
                     elif len(t_interps) == 1:
@@ -612,15 +615,15 @@
         'elevation': {'COPERNICUS.GLO30'},
         'meteorological': {'GEOS5.tavg1_2d_slv_Nx'},
         'optical': {'SENTINEL2.S2MSI2A_R20m'},
         'precipitation': {'CHIRPS.P05'},
         'solar radiation': {'ERA5.sis-agrometeorological-indicators'},
         'statics': {'STATICS.WaPOR3'},
         'thermal': {'VIIRSL1.VNP02IMG'},
-        'soil moisture': {'FILE:{folder}{sep}se_root_out*.nc.from_file'},
+        'soil moisture': {'FILE:{folder}{sep}se_root_out*.nc'},
 
         # Define which product to reproject the other products to.
         '_EXAMPLE_': 'SENTINEL2.S2MSI2A_R20m', 
 
         # Define any special functions to apply to a specific variable.
         '_ENHANCE_': {"bt": ["pywapor.enhancers.dms.thermal_sharpener.sharpen"],},
```

### Comparing `pywapor-3.5.1/pywapor/post_et_look.py` & `pywapor-3.5.2/pywapor/post_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/pre_et_look.py` & `pywapor-3.5.2/pywapor/pre_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/pre_se_root.py` & `pywapor-3.5.2/pywapor/pre_se_root.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor/se_root.py` & `pywapor-3.5.2/pywapor/se_root.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/pywapor.egg-info/PKG-INFO` & `pywapor-3.5.2/pywapor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywapor
-Version: 3.5.1
+Version: 3.5.2
 Home-page: https://www.fao.org/aquastat/py-wapor/
 Author: FAO
 Author-email: bert.coerver@fao.org
 License: Apache
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pywapor-3.5.1/pywapor.egg-info/SOURCES.txt` & `pywapor-3.5.2/pywapor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.1/setup.py` & `pywapor-3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pywapor',
-    version = '3.5.1',
+    version = '3.5.2',
     url = 'https://www.fao.org/aquastat/py-wapor/',
     author = "FAO",
     author_email = "bert.coerver@fao.org",
     license = "Apache",
     packages = find_packages(include = ['pywapor', 'pywapor.*']),
     include_package_data=True,
     python_requires='>=3.7',
```

