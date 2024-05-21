# Comparing `tmp/geocif-0.1.27.tar.gz` & `tmp/geocif-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.27.tar", last modified: Fri May 17 00:28:41 2024, max compression
+gzip compressed data, was "geocif-0.1.28.tar", last modified: Tue May 21 22:11:57 2024, max compression
```

## Comparing `geocif-0.1.27.tar` & `geocif-0.1.28.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.907815 geocif-0.1.27/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.27/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.27/MANIFEST.in
--rw-rw-rw-   0        0        0     1586 2024-05-17 00:28:41.903523 geocif-0.1.27/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.27/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.288003 geocif-0.1.27/geocif/
--rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.27/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.410964 geocif-0.1.27/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.27/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.27/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.27/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.27/geocif/agmet/utils.py
--rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.27/geocif/analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.539350 geocif-0.1.27/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.27/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.27/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.27/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.27/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.27/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.27/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.27/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.602148 geocif-0.1.27/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.27/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.27/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.27/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    42209 2024-05-16 14:18:55.000000 geocif-0.1.27/geocif/geocif.py
--rw-rw-rw-   0        0        0     6633 2024-05-12 15:40:15.000000 geocif-0.1.27/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.27/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.827261 geocif-0.1.27/geocif/ml/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.27/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    12360 2024-05-14 02:40:35.000000 geocif-0.1.27/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.27/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    12671 2024-05-12 03:53:54.000000 geocif-0.1.27/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     8953 2024-05-15 14:01:01.000000 geocif-0.1.27/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.27/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.27/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.27/geocif/ml/output.py
--rw-rw-rw-   0        0        0     8286 2024-05-12 14:57:40.000000 geocif-0.1.27/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     8393 2024-05-13 20:11:22.000000 geocif-0.1.27/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9433 2024-05-16 16:45:11.000000 geocif-0.1.27/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.27/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.27/geocif/ml/xai.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.857837 geocif-0.1.27/geocif/playground/
--rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.27/geocif/playground/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.27/geocif/playground/automl.py
--rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.27/geocif/playground/misc.py
--rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.27/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.870078 geocif-0.1.27/geocif/viz/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.27/geocif/viz/__init__.py
--rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.27/geocif/viz/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.346553 geocif-0.1.27/geocif.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-17 00:28:36.000000 geocif-0.1.27/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1107 2024-05-17 00:28:39.000000 geocif-0.1.27/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 00:28:36.000000 geocif-0.1.27/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.27/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-17 00:28:36.000000 geocif-0.1.27/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.27/requirements.txt
--rw-rw-rw-   0        0        0      415 2024-05-17 00:28:41.920358 geocif-0.1.27/setup.cfg
--rw-rw-rw-   0        0        0     1617 2024-05-17 00:28:02.000000 geocif-0.1.27/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.898825 geocif-0.1.27/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.27/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.342620 geocif-0.1.28/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.28/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.28/MANIFEST.in
+-rw-rw-rw-   0        0        0     1586 2024-05-21 22:11:57.341416 geocif-0.1.28/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.28/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.093252 geocif-0.1.28/geocif/
+-rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.28/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.177120 geocif-0.1.28/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.28/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.28/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.28/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.28/geocif/agmet/utils.py
+-rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.28/geocif/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.193507 geocif-0.1.28/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.28/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.28/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.28/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.28/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.28/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.28/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.28/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.202149 geocif-0.1.28/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.28/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.28/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.28/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    42243 2024-05-17 16:05:26.000000 geocif-0.1.28/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6651 2024-05-21 22:11:34.000000 geocif-0.1.28/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.28/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.326779 geocif-0.1.28/geocif/ml/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.28/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    12360 2024-05-14 02:40:35.000000 geocif-0.1.28/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.28/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    12671 2024-05-12 03:53:54.000000 geocif-0.1.28/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     8953 2024-05-15 14:01:01.000000 geocif-0.1.28/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.28/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.28/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.28/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     8286 2024-05-12 14:57:40.000000 geocif-0.1.28/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     8393 2024-05-13 20:11:22.000000 geocif-0.1.28/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9433 2024-05-16 16:45:11.000000 geocif-0.1.28/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.28/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.28/geocif/ml/xai.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.333285 geocif-0.1.28/geocif/playground/
+-rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.28/geocif/playground/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.28/geocif/playground/automl.py
+-rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.28/geocif/playground/misc.py
+-rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.28/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.337458 geocif-0.1.28/geocif/viz/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.28/geocif/viz/__init__.py
+-rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.28/geocif/viz/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.164425 geocif-0.1.28/geocif.egg-info/
+-rw-rw-rw-   0        0        0     1586 2024-05-21 22:11:55.000000 geocif-0.1.28/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1107 2024-05-21 22:11:56.000000 geocif-0.1.28/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 22:11:55.000000 geocif-0.1.28/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.28/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-21 22:11:55.000000 geocif-0.1.28/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.28/requirements.txt
+-rw-rw-rw-   0        0        0      415 2024-05-21 22:11:57.350364 geocif-0.1.28/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2024-05-21 22:11:52.000000 geocif-0.1.28/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:57.339423 geocif-0.1.28/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.28/tests/test_geocif.py
```

### Comparing `geocif-0.1.27/LICENSE` & `geocif-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/PKG-INFO` & `geocif-0.1.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.27
+Version: 0.1.28
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.27/README.md` & `geocif-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/agmet/geoagmet.py` & `geocif-0.1.28/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/agmet/plot.py` & `geocif-0.1.28/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/agmet/utils.py` & `geocif-0.1.28/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/analysis.py` & `geocif-0.1.28/geocif/analysis.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/backup/features.py` & `geocif-0.1.28/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/backup/geo.py` & `geocif-0.1.28/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/backup/geocif.py` & `geocif-0.1.28/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/backup/metadata.py` & `geocif-0.1.28/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/cei/definitions.py` & `geocif-0.1.28/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/cei/indices.py` & `geocif-0.1.28/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/geocif.py` & `geocif-0.1.28/geocif/geocif.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,16 @@
         """
         ====================================================================
                                 Variables, Paths
         ====================================================================
         """
         # If ML model is run for individual region or cluster, then Region_ID is the same for each region
         # or cluster and therefore redundant for the ML model
-        if self.cluster_strategy in ["individual", "auto_detect"]:
-            self.cat_features.remove("Region_ID")
+        #if self.cluster_strategy in ["individual", "auto_detect"]:
+        #    self.cat_features.remove("Region_ID")
 
         self.fixed_columns: list = [
             "Country",
             "Region",
             "Crop",
             "Area",
             "Season",
@@ -421,14 +421,15 @@
         ]:
             if col not in df.columns:
                 df.loc[:, col] = np.NaN
 
         # Create an index based on following columns
         index_columns = [
             "Model",
+            "Cluster Strategy"
             "Country",
             "Region",
             "Crop",
             "Harvest Year",
             "Stage Name",
         ]
         df.index = df.apply(
@@ -713,14 +714,15 @@
         os.makedirs(dir_output, exist_ok=True)
         df.to_csv(
             dir_output / f"{self.country}_{self.crop}_{self.forecast_season}.csv",
             index=False,
         )
 
         # cat_features should be converted to category type
+
         df[self.cat_features] = df[self.cat_features].astype("category")
 
         """  Heatmap of correlation of various features with yield at each time step"""
         # For each time step, determine the number of occurences of each feature
         # when it is most correlated with the target for a region
         # Use this to plot a heatmap showing which features are most correlated
         # with yield at each time step
```

### Comparing `geocif-0.1.27/geocif/indices_runner.py` & `geocif-0.1.28/geocif/indices_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,29 +151,29 @@
                 filename,
                 admin_zone,
                 category,
                 year,
                 "ndvi",
                 True,
             )
-            for year in range(2001, ar.utcnow().year + 1)
+            for year in range(2023, ar.utcnow().year + 1)
             for status, path, filename, admin_zone, category in combinations
         ]
 
         # Only keep those entries in combinations where the third elemt is
         # mozambique, south_africa, angola or dem_people's_rep_of_korea
         # This is done to test the code for these countries
-        # combinations = [i for i in combinations if "angola" in i[2] or
-        #                 "lesotho" in i[2] or
+        combinations = [i for i in combinations if "angola_maize" in i[3] or
+                       "lesotho_maize" in i[3] or
         #                 "namibia" in i[2] or
         #                 "united_republic_of_tanzania" in i[2] or
-        #                 "zambia" in i[2] or
-        #                 "zimbabwe" in i[2] or
+                         "zambia_maize" in i[3] or
+                         "zimbabwe_maize" in i[3] or
         #                 "south_africa" in i[2] or
-        #                 "mozambique" in i[2] or
+                      "mozambique_maize" in i[3]]
         #                 "malawi" in i[2]]
 
         if self.do_parallel:
             num_cpu = int(cpu_count() * 0.6)
             with Pool(num_cpu) as p:
                 for i, _ in enumerate(p.imap_unordered(indices.process, combinations)):
                     pass
@@ -197,15 +197,15 @@
     Returns:
 
     """
     """ Check dictionary keys to have no spaces"""
     indices.validate_index_definitions()
 
     for method in [
-        "monthly_r",  # "dekad_r"  # "dekad_r"
+        "biweekly_r",  # "dekad_r"  # "dekad_r"
     ]:  # , "full_season", "phenological_stages", "fraction_season"]:
         obj = cei_runner(path_config_files)
         obj.main(method)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `geocif-0.1.27/geocif/logger.py` & `geocif-0.1.28/geocif/logger.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/correlations.py` & `geocif-0.1.28/geocif/ml/correlations.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/embedding.py` & `geocif-0.1.28/geocif/ml/embedding.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/feature_engineering.py` & `geocif-0.1.28/geocif/ml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/feature_selection.py` & `geocif-0.1.28/geocif/ml/feature_selection.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/outliers.py` & `geocif-0.1.28/geocif/ml/outliers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/outlook.py` & `geocif-0.1.28/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/output.py` & `geocif-0.1.28/geocif/ml/output.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/stages.py` & `geocif-0.1.28/geocif/ml/stages.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/stats.py` & `geocif-0.1.28/geocif/ml/stats.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/trainers.py` & `geocif-0.1.28/geocif/ml/trainers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/trend.py` & `geocif-0.1.28/geocif/ml/trend.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/ml/xai.py` & `geocif-0.1.28/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/playground/misc.py` & `geocif-0.1.28/geocif/playground/misc.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/utils.py` & `geocif-0.1.28/geocif/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif/viz/plot.py` & `geocif-0.1.28/geocif/viz/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/geocif.egg-info/PKG-INFO` & `geocif-0.1.28/geocif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.27
+Version: 0.1.28
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.27/geocif.egg-info/SOURCES.txt` & `geocif-0.1.28/geocif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.27/setup.py` & `geocif-0.1.28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="geocif",
     name="geocif",
     packages=find_packages(include=["geocif", "geocif.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://ritviksahajpal.github.io/yield_forecasting/",
-    version="0.1.27",
+    version="0.1.28",
     zip_safe=False,
 )
```

