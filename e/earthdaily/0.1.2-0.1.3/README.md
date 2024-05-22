# Comparing `tmp/earthdaily-0.1.2.tar.gz` & `tmp/earthdaily-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthdaily-0.1.2.tar", last modified: Wed May 15 16:11:08 2024, max compression
+gzip compressed data, was "earthdaily-0.1.3.tar", last modified: Wed May 22 16:03:32 2024, max compression
```

## Comparing `earthdaily-0.1.2.tar` & `earthdaily-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 16:11:07.000000 earthdaily-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-15 16:11:08.526383 earthdaily-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-15 16:11:07.000000 earthdaily-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/accessor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/accessor/whittaker/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/accessor/whittaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/accessor/whittaker/_pywapor_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/data/pivot.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/data/pivot_corumba.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/earthdatastore/
--rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/_scales_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/_zonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/custom_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/geometry_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/harmonizer/
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/mask/
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/mask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:11:08.526383 earthdaily-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-15 16:11:07.000000 earthdaily-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.236873 earthdaily-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-22 16:03:31.000000 earthdaily-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-22 16:03:32.236873 earthdaily-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-22 16:03:31.000000 earthdaily-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.232873 earthdaily-0.1.3/earthdaily/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.232873 earthdaily-0.1.3/earthdaily/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/accessor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.232873 earthdaily-0.1.3/earthdaily/accessor/whittaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/accessor/whittaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/accessor/whittaker/_pywapor_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.232873 earthdaily-0.1.3/earthdaily/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.232873 earthdaily-0.1.3/earthdaily/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/datasets/data/pivot.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/datasets/data/pivot_corumba.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.236873 earthdaily-0.1.3/earthdaily/earthdatastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    37591 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/_scales_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.236873 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/_zonal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.236873 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33897 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/custom_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/geometry_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.236873 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/harmonizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.236873 earthdaily-0.1.3/earthdaily/earthdatastore/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-22 16:03:31.000000 earthdaily-0.1.3/earthdaily/earthdatastore/mask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:03:32.232873 earthdaily-0.1.3/earthdaily.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-22 16:03:32.000000 earthdaily-0.1.3/earthdaily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-22 16:03:32.000000 earthdaily-0.1.3/earthdaily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:03:32.000000 earthdaily-0.1.3/earthdaily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:03:32.000000 earthdaily-0.1.3/earthdaily.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 16:03:32.000000 earthdaily-0.1.3/earthdaily.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 16:03:32.000000 earthdaily-0.1.3/earthdaily.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:03:32.236873 earthdaily-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-22 16:03:31.000000 earthdaily-0.1.3/setup.py
```

### Comparing `earthdaily-0.1.2/LICENSE` & `earthdaily-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/PKG-INFO` & `earthdaily-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.1.2
+Version: 0.1.3
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_rvgjz_m1_/tmpz3v1lq0k_TarContainer/0/2", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.1.2 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.3 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.1.2/README.md` & `earthdaily-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/accessor/__init__.py` & `earthdaily-0.1.3/earthdaily/accessor/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/accessor/whittaker/__init__.py` & `earthdaily-0.1.3/earthdaily/accessor/whittaker/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/accessor/whittaker/_pywapor_core.py` & `earthdaily-0.1.3/earthdaily/accessor/whittaker/_pywapor_core.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/datasets/__init__.py` & `earthdaily-0.1.3/earthdaily/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/datasets/data/pivot.geojson` & `earthdaily-0.1.3/earthdaily/datasets/data/pivot.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/datasets/data/pivot_corumba.geojson` & `earthdaily-0.1.3/earthdaily/datasets/data/pivot_corumba.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/__init__.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,15 @@
     def datacube(
         self,
         collections: str | list,
         datetime=None,
         assets: None | list | dict = None,
         intersects: (gpd.GeoDataFrame | str | dict) = None,
         bbox=None,
-        mask_with: (None | str) = None,
+        mask_with: (None | str | list) = None,
         mask_statistics: bool | int = False,
         clear_cover: (int | float) = None,
         prefer_alternate: (str | bool) = "download",
         search_kwargs: dict = {},
         add_default_scale_factor: bool = True,
         common_band_names=True,
         cross_calibration_collection: (None | str) = None,
@@ -583,16 +583,17 @@
               ``2017-06-10T00:00:00Z/2017-06-11T23:59:59Z``
         assets : None | list | dict, optional
             DESCRIPTION. The default is None.
         intersects : (gpd.GeoDataFrame, str(wkt), dict(json)), optional
             DESCRIPTION. The default is None.
         bbox : TYPE, optional
             DESCRIPTION. The default is None.
-        mask_with : (None, str), optional
-            "native" mask, or "ag_cloud_mask".
+        mask_with : (None, str, list), optional
+            "native" mask, or "ag_cloud_mask", or ["ag_cloud_mask","native"],
+            and so if ag_cloud_mask is not available, will switch to native.
             The default is None.
         mask_statistics : bool | int, optional
             DESCRIPTION. The default is False.
         clear_cover : (int, float), optional
             Percent of clear data above a field (from 0 to 100).
             The default is None.
         prefer_alternate : (str, False), optional
@@ -630,31 +631,34 @@
             raise NotImplementedError(
                 "You must set `groupby_date=None` to have properties per item."
             )
 
         if isinstance(collections, str):
             collections = [collections]
 
+        if intersects is not None:
+            intersects = cube_utils.GeometryManager(intersects).to_geopandas()
+            self.intersects = intersects
+
         if mask_with:
             if mask_with not in mask._available_masks:
-                raise ValueError(
-                    f"Specified mask '{mask_with}' is not available. Currently available masks provider are : {mask._available_masks}"
+                logging.log(
+                    level=logging.INFO,
+                    msg=f"Specified mask '{mask_with}' is not available. Currently available masks provider are : {mask._available_masks}",
                 )
+
             if mask_with == "ag_cloud_mask":
                 search_kwargs = self._update_search_kwargs_for_ag_cloud_mask(
                     search_kwargs, collections[0]
                 )
             else:
                 mask_with = mask._native_mask_def_mapping.get(collections[0], None)
                 if isinstance(assets, list):
                     assets.append(mask_with)
 
-        if intersects is not None:
-            intersects = cube_utils.GeometryManager(intersects).to_geopandas()
-            self.intersects = intersects
         items = self.search(
             collections=collections,
             bbox=bbox,
             intersects=intersects,
             datetime=datetime,
             prefer_alternate=prefer_alternate,
             add_default_scale_factor=add_default_scale_factor,
```

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/_scales_collections.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/_scales_collections.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/__init__.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,37 @@
 import rioxarray
 from functools import wraps
 import json
 
 __all__ = ["GeometryManager", "rioxarray", "zonal_stats", "zonal_stats_numpy"]
 
 
+def _datacube_masks(method, *args, **kwargs):
+    @wraps(method)
+    def _impl(self, *args, **kwargs):
+        mask_with = kwargs.get("mask_with", None)
+        if isinstance(mask_with, list) and len(mask_with) > 1:
+            kwargs.pop("mask_with")
+            for mask in mask_with:
+                try:
+                    datacube = method(self, mask_with=mask, *args, **kwargs)
+                    break
+                except Warning:
+                    # if warning about no items for ag_cloud_mask for example
+                    continue
+        else:
+            datacube = method(self, *args, **kwargs)
+        return datacube
+
+    return _impl
+
+
 def _datacubes(method):
     @wraps(method)
+    @_datacube_masks
     def _impl(self, *args, **kwargs):
         collections = kwargs.get("collections", args[0] if len(args) > 0 else None)
         if isinstance(collections, list) and len(collections) > 1:
             if "collections" in kwargs.keys():
                 kwargs.pop("collections")
             else:
                 args = args[1:]
```

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/_zonal.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/_zonal.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6617424242424242%*

 * *Differences: {"'ecostress-eco-l2t-lste-002'": "[OrderedDict([('browse', 'browse'), ('metadata', 'metadata'), "*

 * *                                 "('002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_QC', "*

 * *                                 "'002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_QC'), "*

 * *                                 "('002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_071 […]*

```diff
@@ -131,14 +131,28 @@
             "t": "t",
             "tcwv": "tcwv",
             "tp": "tp",
             "u": "u",
             "v": "v"
         }
     ],
+    "ecostress-eco-l2t-lste-002": [
+        {
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_EmisWB": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_EmisWB",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_LST": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_LST",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_LST_err": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_LST_err",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_QC": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_QC",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_cloud": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_cloud",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_height": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_height",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_view_zenith": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_view_zenith",
+            "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_water": "002/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01/ECOv002_L2T_LSTE_33232_015_18KYE_20240516T193004_0711_01_water",
+            "browse": "browse",
+            "metadata": "metadata"
+        }
+    ],
     "eda-albedo-map": [
         {
             "albedo-map": "albedo-map"
         }
     ],
     "eda-analysis-ready-mosaic": [
         {
@@ -180,14 +194,64 @@
         }
     ],
     "edagro-analytics-field-borders-layer": [
         {
             "data": "data"
         }
     ],
+    "esa-worldcover-landcover-2020-v100": [
+        {
+            "ESA_WORLDCOVER_10M_MAP": "ESA_WORLDCOVER_10M_MAP"
+        }
+    ],
+    "esa-worldcover-landcover-2021-v200": [
+        {
+            "ESA_WORLDCOVER_10M_MAP": "ESA_WORLDCOVER_10M_MAP"
+        }
+    ],
+    "esa-worldcover-s1-vvvhratio-2020-v100": [
+        {
+            "s1_vvvhratio_2020": "s1_vvvhratio_2020"
+        }
+    ],
+    "esa-worldcover-s1-vvvhratio-2021-v200": [
+        {
+            "s1_vvvhratio_2021": "s1_vvvhratio_2021"
+        }
+    ],
+    "esa-worldcover-s2-nvdi-2020-v100": [
+        {
+            "s2_ndvi_2020": "s2_ndvi_2020"
+        }
+    ],
+    "esa-worldcover-s2-nvdi-2021-v200": [
+        {
+            "s2_ndvi_2021": "s2_ndvi_2021"
+        }
+    ],
+    "esa-worldcover-s2-rgbnir-2020-v100": [
+        {
+            "s2_rgbnir_2020": "s2_rgbnir_2020"
+        }
+    ],
+    "esa-worldcover-s2-rgbnir-2021-v200": [
+        {
+            "s2_rgbnir_2021": "s2_rgbnir_2021"
+        }
+    ],
+    "esa-worldcover-s2-swir-2020-v100": [
+        {
+            "s2_swir_2020": "s2_swir_2020"
+        }
+    ],
+    "esa-worldcover-s2-swir-2021-v200": [
+        {
+            "s2_swir_2021": "s2_swir_2021"
+        }
+    ],
     "gaofen-1-l2a-cog-edagro": [
         {
             "blue": "blue",
             "green": "green",
             "nir": "nir",
             "raster": "raster",
             "red": "red"
@@ -210,14 +274,15 @@
     "gaofen-6-l2a-cog-edagro-ag-cloud-mask": [
         {
             "agriculture-cloud-mask": "agriculture-cloud-mask"
         }
     ],
     "goes": [
         {
+            "OR_ABI-L2-ACMF-M6_G18_s20241430900220_e20241430909528_c20241430910280.nc": "OR_ABI-L2-ACMF-M6_G18_s20241430900220_e20241430909528_c20241430910280.nc",
             "OR_ABI-L2-AODF-M6_G16_s20233490810206_e20233490819514_c20233490820523.nc": "OR_ABI-L2-AODF-M6_G16_s20233490810206_e20233490819514_c20233490820523.nc"
         }
     ],
     "himawari-l1b": [
         {
             "HS_H09_20231215_0550_B01_FLDK_R10_S0110.DAT.bz2": "HS_H09_20231215_0550_B01_FLDK_R10_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B02_FLDK_R10_S0110.DAT.bz2": "HS_H09_20231215_0550_B02_FLDK_R10_S0110.DAT.bz2",
@@ -230,15 +295,31 @@
             "HS_H09_20231215_0550_B09_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B09_FLDK_R20_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B10_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B10_FLDK_R20_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B11_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B11_FLDK_R20_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B12_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B12_FLDK_R20_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B13_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B13_FLDK_R20_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B14_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B14_FLDK_R20_S0110.DAT.bz2",
             "HS_H09_20231215_0550_B15_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B15_FLDK_R20_S0110.DAT.bz2",
-            "HS_H09_20231215_0550_B16_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B16_FLDK_R20_S0110.DAT.bz2"
+            "HS_H09_20231215_0550_B16_FLDK_R20_S0110.DAT.bz2": "HS_H09_20231215_0550_B16_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B01_FLDK_R10_S0110.DAT.bz2": "HS_H09_20240522_0550_B01_FLDK_R10_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B02_FLDK_R10_S0110.DAT.bz2": "HS_H09_20240522_0550_B02_FLDK_R10_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B03_FLDK_R05_S0110.DAT.bz2": "HS_H09_20240522_0550_B03_FLDK_R05_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B04_FLDK_R10_S0110.DAT.bz2": "HS_H09_20240522_0550_B04_FLDK_R10_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B05_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B05_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B06_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B06_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B07_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B07_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B08_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B08_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B09_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B09_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B10_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B10_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B11_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B11_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B12_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B12_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B13_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B13_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B14_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B14_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B15_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B15_FLDK_R20_S0110.DAT.bz2",
+            "HS_H09_20240522_0550_B16_FLDK_R20_S0110.DAT.bz2": "HS_H09_20240522_0550_B16_FLDK_R20_S0110.DAT.bz2"
         }
     ],
     "himawari-l2-cloud": [
         {
             "AHI-CHGT_v1r0_h08_s202212130450206_e202212130450540_c202212130508561.nc": "AHI-CHGT_v1r0_h08_s202212130450206_e202212130450540_c202212130508561.nc",
             "AHI-CMSK_v1r0_h08_s202212130450206_e202212130450540_c202212130508561.nc": "AHI-CMSK_v1r0_h08_s202212130450206_e202212130450540_c202212130508561.nc",
             "AHI-CPHS_v1r0_h08_s202212130450206_e202212130450540_c202212130508561.nc": "AHI-CPHS_v1r0_h08_s202212130450206_e202212130450540_c202212130508561.nc"
@@ -357,14 +438,20 @@
         }
     ],
     "landsat-l2-cog-ag-cloud-mask": [
         {
             "agriculture-cloud-mask": "agriculture-cloud-mask"
         }
     ],
+    "lulc-classification-map": [
+        {
+            "lulc-classification-map": "lulc-classification-map",
+            "thumbnail": "thumbnail"
+        }
+    ],
     "modis-43A4-061": [
         {
             "BRDF_Albedo_Band_Mandatory_Quality_Band1": "BRDF_Albedo_Band_Mandatory_Quality_Band1",
             "BRDF_Albedo_Band_Mandatory_Quality_Band2": "BRDF_Albedo_Band_Mandatory_Quality_Band2",
             "BRDF_Albedo_Band_Mandatory_Quality_Band3": "BRDF_Albedo_Band_Mandatory_Quality_Band3",
             "BRDF_Albedo_Band_Mandatory_Quality_Band4": "BRDF_Albedo_Band_Mandatory_Quality_Band4",
             "BRDF_Albedo_Band_Mandatory_Quality_Band5": "BRDF_Albedo_Band_Mandatory_Quality_Band5",
@@ -409,21 +496,77 @@
     "modis-mod07-l2-061": [
         {
             "data": "data",
             "metadata": "metadata",
             "opendap": "opendap"
         }
     ],
+    "modis-mod11-l2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
+    "modis-mod11a2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
+    "modis-mod21-l2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
+    "modis-mod21a2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
     "modis-mod35-l2-061": [
         {
             "data": "data",
             "metadata": "metadata",
             "opendap": "opendap"
         }
     ],
+    "modis-myd11-l2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
+    "modis-myd11a2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
+    "modis-myd21-l2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
+    "modis-myd21a2-061": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata"
+        }
+    ],
     "modis-myd35-l2-061": [
         {
             "data": "data",
             "metadata": "metadata",
             "opendap": "opendap"
         }
     ],
@@ -448,14 +591,21 @@
     "msg-seviri-cloud-mask": [
         {
             "Metadata": "Metadata",
             "Metadata in JSON format": "Metadata in JSON format",
             "Product download": "Product download"
         }
     ],
+    "nst-observer-catalog": [
+        {
+            "browse": "browse",
+            "cloud_mask": "cloud_mask",
+            "thumbnail": "thumbnail"
+        }
+    ],
     "resourcesat-2-l2a-cog-edagro": [
         {
             "green": "green",
             "nir": "nir",
             "raster": "raster",
             "red": "red"
         }
@@ -482,14 +632,15 @@
             "preview/icons/logo.png": "preview/icons/logo.png",
             "preview/map-overlay.kml": "preview/map-overlay.kml",
             "preview/product-preview.html": "preview/product-preview.html",
             "preview/quick-look.png": "preview/quick-look.png",
             "preview/thumbnail.png": "preview/thumbnail.png",
             "productInfo.json": "productInfo.json",
             "report-20231206T225118.pdf": "report-20231206T225118.pdf",
+            "report-20240521T170707.pdf": "report-20240521T170707.pdf",
             "support/s1-level-1-calibration.xsd": "support/s1-level-1-calibration.xsd",
             "support/s1-level-1-measurement.xsd": "support/s1-level-1-measurement.xsd",
             "support/s1-level-1-noise.xsd": "support/s1-level-1-noise.xsd",
             "support/s1-level-1-product.xsd": "support/s1-level-1-product.xsd",
             "support/s1-level-1-quicklook.xsd": "support/s1-level-1-quicklook.xsd",
             "support/s1-level-1-rfi.xsd": "support/s1-level-1-rfi.xsd",
             "support/s1-map-overlay.xsd": "support/s1-map-overlay.xsd",
@@ -638,15 +789,16 @@
     "sentinel-2-l2a-cog-ag-cloud-mask-geosys-private": [
         {
             "agriculture-cloud-mask": "agriculture-cloud-mask"
         }
     ],
     "sentinel-2-methane-product": [
         {
-            "colourized_geotiff": "colourized_geotiff"
+            "colourized_geotiff": "colourized_geotiff",
+            "thumbnail": "thumbnail"
         }
     ],
     "venus-l2a": [
         {
             "atmospheric_biophysical_parameters": "atmospheric_biophysical_parameters",
             "blue": "image_file_SRE_B3",
             "coastal": "image_file_SRE_B2",
@@ -690,9 +842,73 @@
             "stac_json": "stac_json",
             "thumbnail": "thumbnail",
             "useful_image": "useful_image",
             "useful_image_data": "useful_image_data",
             "viewing_data": "viewing_data",
             "yellow": "image_file_SRE_B5"
         }
+    ],
+    "viirs-vj121-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vj121a1d-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vj121a1n-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vj121a2-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vnp21-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vnp21a1d-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vnp21a1n-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
+    ],
+    "viirs-vnp21a2-002": [
+        {
+            "browse": "browse",
+            "data": "data",
+            "metadata": "metadata",
+            "opendap": "opendap"
+        }
     ]
 }
```

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/custom_reducers.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/custom_reducers.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/geometry_manager.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/geometry_manager.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/preprocessing.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/cube_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily/earthdatastore/mask/__init__.py` & `earthdaily-0.1.3/earthdaily/earthdatastore/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/earthdaily.egg-info/PKG-INFO` & `earthdaily-0.1.3/earthdaily.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.1.2
+Version: 0.1.3
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_rvgjz_m1_/tmpz3v1lq0k_TarContainer/0/35", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.1.2 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.3 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.1.2/earthdaily.egg-info/SOURCES.txt` & `earthdaily-0.1.3/earthdaily.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.2/setup.py` & `earthdaily-0.1.3/setup.py`

 * *Files identical despite different names*

