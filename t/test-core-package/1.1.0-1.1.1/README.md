# Comparing `tmp/test_core_package-1.1.0.tar.gz` & `tmp/test_core_package-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-1.1.0.tar", last modified: Tue May 14 07:33:02 2024, max compression
+gzip compressed data, was "test_core_package-1.1.1.tar", last modified: Tue May 21 13:18:14 2024, max compression
```

## Comparing `test_core_package-1.1.0.tar` & `test_core_package-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.464499 test_core_package-1.1.0/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.1.0/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-14 07:33:02.458488 test_core_package-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.239672 test_core_package-1.1.0/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-1.1.0/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.262216 test_core_package-1.1.0/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-1.1.0/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4307 2024-05-13 08:57:22.000000 test_core_package-1.1.0/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     9288 2024-05-14 07:31:50.000000 test_core_package-1.1.0/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1581 2024-05-14 07:17:02.000000 test_core_package-1.1.0/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.269766 test_core_package-1.1.0/qa_qc_check/model/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-1.1.0/qa_qc_check/model/__init__.py
--rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-1.1.0/qa_qc_check/model/metadata_model.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.277895 test_core_package-1.1.0/qa_qc_check/validator/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-1.1.0/qa_qc_check/validator/__init__.py
--rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-1.1.0/qa_qc_check/validator/meta_data_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.282566 test_core_package-1.1.0/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.320562 test_core_package-1.1.0/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.351300 test_core_package-1.1.0/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.399792 test_core_package-1.1.0/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-1.1.0/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-14 07:33:02.464499 test_core_package-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-14 07:32:54.000000 test_core_package-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:33:02.458488 test_core_package-1.1.0/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-14 07:33:02.000000 test_core_package-1.1.0/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-14 07:33:02.000000 test_core_package-1.1.0/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:33:02.000000 test_core_package-1.1.0/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-14 07:33:02.000000 test_core_package-1.1.0/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-14 07:33:02.000000 test_core_package-1.1.0/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.822685 test_core_package-1.1.1/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.1.1/LICENCE.txt
+-rw-rw-rw-   0        0        0      965 2024-05-21 13:18:14.818372 test_core_package-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.518630 test_core_package-1.1.1/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-1.1.1/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.529588 test_core_package-1.1.1/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-1.1.1/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-1.1.1/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4110 2024-05-21 12:03:24.000000 test_core_package-1.1.1/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9272 2024-05-21 12:04:23.000000 test_core_package-1.1.1/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-14 07:17:02.000000 test_core_package-1.1.1/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.537784 test_core_package-1.1.1/qa_qc_check/model/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-1.1.1/qa_qc_check/model/__init__.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-1.1.1/qa_qc_check/model/metadata_model.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.543417 test_core_package-1.1.1/qa_qc_check/validator/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-1.1.1/qa_qc_check/validator/__init__.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-1.1.1/qa_qc_check/validator/meta_data_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.547383 test_core_package-1.1.1/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.1/satelite/__init__.py
+-rw-rw-rw-   0        0        0     1011 2024-05-17 11:24:27.000000 test_core_package-1.1.1/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.550367 test_core_package-1.1.1/satelite/core/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/core/__init__.py
+-rw-rw-rw-   0        0        0     2552 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/core/downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.560046 test_core_package-1.1.1/satelite/gdal/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/gdal/__init__.py
+-rw-rw-rw-   0        0        0     2620 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/gdal/gdal_commands.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.560860 test_core_package-1.1.1/satelite/models/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/models/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/models/s2_enum.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.567014 test_core_package-1.1.1/satelite/raster/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/raster/__init__.py
+-rw-rw-rw-   0        0        0     9161 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/raster/raster.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.597599 test_core_package-1.1.1/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      457 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.601695 test_core_package-1.1.1/satelite/sentinel2/band_stack/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/band_stack/__init__.py
+-rw-rw-rw-   0        0        0     2903 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-rw-rw-   0        0        0     2488 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-1.1.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3248 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.605726 test_core_package-1.1.1/satelite/sentinel2/indices/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/indices/__init__.py
+-rw-rw-rw-   0        0        0     4320 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/indices/general_indices.py
+-rw-rw-rw-   0        0        0     2534 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/mosaic_same_bands.py
+-rw-rw-rw-   0        0        0     1548 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/path_row_from_shp.py
+-rw-rw-rw-   0        0        0     3337 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/s2_l1c_urls.py
+-rw-rw-rw-   0        0        0     2992 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/sentinel2/s2_l2a_urls.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.613606 test_core_package-1.1.1/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.1/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0     1038 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.722356 test_core_package-1.1.1/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.1/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1366 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0      334 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-rw-rw-   0        0        0      906 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-rw-rw-   0        0        0      931 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-rw-rw-   0        0        0     1594 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/tests/sentinel2/test_validate.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.725877 test_core_package-1.1.1/satelite/validators/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/validators/__init__.py
+-rw-rw-rw-   0        0        0     2446 2024-05-14 07:37:16.000000 test_core_package-1.1.1/satelite/validators/check_shape_of_rid.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:18:14.825858 test_core_package-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2024-05-21 12:21:52.000000 test_core_package-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:18:14.816992 test_core_package-1.1.1/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      965 2024-05-21 13:18:14.000000 test_core_package-1.1.1/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1844 2024-05-21 13:18:14.000000 test_core_package-1.1.1/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:18:14.000000 test_core_package-1.1.1/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      362 2024-05-21 13:18:14.000000 test_core_package-1.1.1/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-21 13:18:14.000000 test_core_package-1.1.1/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-1.1.0/qa_qc_check/controller/meta_data.py` & `test_core_package-1.1.1/qa_qc_check/controller/meta_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-from os import environ, getenv
+import os
 from urllib.parse import urlparse
 
 import boto3
 from botocore.exceptions import ClientError
 from osgeo import gdal
 
 from qa_qc_check.model.metadata_model import MetadataModel
 
 gdal.UseExceptions()
-gdal.SetConfigOption("AWS_DEFAULT_REGION", "ap-south-1")
-gdal.SetConfigOption(
-    "AWS_SECRET_ACCESS_KEY", "O532YGW4+gYA3Y+NhXiI5w6+MjNdyasgdbpE4490"
-)
-gdal.SetConfigOption("AWS_ACCESS_KEY_ID", "AKIAVMZ7IZCPHXL6UY4G")
-gdal.SetConfigOption("AWS_REQUEST_PAYER", "REQUESTER")
-
-environ["AWS_ACCESS_KEY_ID"] = "AKIAVMZ7IZCPHXL6UY4G"
-environ["AWS_SECRET_ACCESS_KEY"] = "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"
-environ["AWS_DEFAULT_REGION"] = "ap-south-1"
-environ["AWS_REQUEST_PAYER"] = "REQUESTER"
+gdal.SetConfigOption("AWS_DEFAULT_REGION", os.environ["AWS_DEFAULT_REGION_NEW"])
+gdal.SetConfigOption("AWS_SECRET_ACCESS_KEY", os.environ["AWS_SECRET_ACCESS_KEY_NEW"])
+gdal.SetConfigOption("AWS_ACCESS_KEY_ID", os.environ["AWS_ACCESS_KEY_ID_NEW"])
+gdal.SetConfigOption("AWS_REQUEST_PAYER", os.environ["AWS_REQUEST_PAYER_NEW"])
 
 
 class MetaData:
     def __init__(self, file: str):
         self.file = file
 
     def main(self) -> MetadataModel:
```

### Comparing `test_core_package-1.1.0/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-1.1.1/qa_qc_check/controller/meta_data_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import json
 import logging
 import os
 from dataclasses import asdict
-from typing import Dict
+
+from dotenv import load_dotenv
 
 from qa_qc_check.controller.meta_data import MetaData
 from qa_qc_check.controller.qa_qc import QaQc
 from qa_qc_check.model.metadata_model import MetadataModel, QaQcModel
 
 logger = logging.getLogger()
 
+load_dotenv()
+
 
 class MetadataExtractor:
 
     def __init__(self, file: str, check_type: str):
         """Initializing MetadataExtractor
 
         Args:
@@ -212,15 +214,14 @@
             logging.info("started computing metadata")
             computed_values = self._entry_values_computer(metadata)
             logging.info("started qaqc")
             qa_qc = QaQc(self.checks_json)
             checks = qa_qc.main(computed_values, self.product, self.check_type)
             logging.info("qaqc done")
             metadata.metadata_check = checks["metadata_check"]
-            print(metadata)
             return {
                 "statusCode": 200,
                 "body": {
                     "message": "metadata extraction successful",
                     "metadata": asdict(metadata),
                 },
             }
```

### Comparing `test_core_package-1.1.0/qa_qc_check/controller/qa_qc.py` & `test_core_package-1.1.1/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.0/qa_qc_check/model/metadata_model.py` & `test_core_package-1.1.1/qa_qc_check/model/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.0/qa_qc_check/validator/meta_data_validator.py` & `test_core_package-1.1.1/qa_qc_check/validator/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.0/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-1.1.1/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
         pd.DataFrame]:
         """
         Fetching features list using tile ids
         :param tile_list:
         :return: list
         """
         api_df_list = []
-        for tileId in tile_list:
+        for tile_id in tile_list:
             url = (
                 f'https://catalogue.dataspace.copernicus.eu/resto/api/collections/Sentinel2/search.json?cloudCover=[{self.cloud_cover_perc}]'
                 f'&startDate={self.start_date}T00:00:00Z&completionDate={self.end_date}T23:59:59Z&'
                 f'productType={self.METADATA[self.processing_level]["producttype"]}&'
-                f'processingLevel={self.METADATA[self.processing_level]["processinglevel"]}&tileId={tileId}&maxRecords=1000')
+                f'processingLevel={self.METADATA[self.processing_level]["processinglevel"]}&tileId={tile_id}&maxRecords=1000')
             response = requests.get(url)
             json = response.json()
             df = pd.DataFrame.from_dict(json["features"])
             # Extract specific keys from the 'metadata' column
             df["productIdentifier"] = df["properties"].apply(
                 lambda x: x.get("productIdentifier")
             )
```

### Comparing `test_core_package-1.1.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-1.1.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.0/satelite/sentinel2/get_tiles.py` & `test_core_package-1.1.1/satelite/sentinel2/get_tiles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from os import environ
 
 import fiona
 from fiona.session import AWSSession
 from sqlalchemy import text
 
-from satelite.config import Session
+from satelite.config import DBSession
 
 
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
-        self.session = Session.create()
+        self.db = DBSession.create()
 
     def fetch_tile_from_db(self, sql_query, geom_):
-        result = self.session.execute(sql_query,
-                                      {"geojson_geometry": str(geom_)})
+        """
+            Fetch tile from database
+        :param sql_query:
+        :param geom_:
+        :return:
+        """
+
+        result = self.db.execute(sql_query,
+                                 {"geojson_geometry": str(geom_)})
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
         """
         tile_list = set()
@@ -30,63 +37,64 @@
 
         for geom_ in geom_list:
             rows = self.fetch_tile_from_db(sql_query, geom_)
             for row in rows:
                 tile_list.add(row[0])
 
         tile_list = list(tile_list)
-        self.session.close()
+        self.db.close()
 
         return tile_list
 
     def get_tile_from_rids(self, rids: list, shape_path: str):
         """To get tiles from rids
         :param rids:
         :param shape_path:
         :return: list
         """
         master_tile_list = []
-        with fiona.Env(
-                session=AWSSession(
-                    aws_access_key_id=environ.get(
-                        "AWS_ACCESS_KEY_ID", None
-                    ),
-                    aws_secret_access_key=environ.get(
-                        "AWS_SECRET_ACCESS_KEY", None
-                    ),
-                    requester_pays=True,
-                    region_name=environ.get(
-                        "AWS_DEFAULT_REGION", None
-                    ),
-                )
-        ) as env:
-            for region_ in rids:
+
+        for region_ in rids:
+            with fiona.Env(
+                    session=AWSSession(
+                        aws_access_key_id=environ.get(
+                            "AWS_ACCESS_KEY_ID", None
+                        ),
+                        aws_secret_access_key=environ.get(
+                            "AWS_SECRET_ACCESS_KEY", None
+                        ),
+                        requester_pays=True,
+                        region_name=environ.get(
+                            "AWS_DEFAULT_REGION", None
+                        ),
+                    )
+            ) as env:
                 with fiona.open(
                         f"s3://satsure-immutables/{shape_path}/{region_}.shp"
                 ) as src:
                     bbox = src.bounds
 
                 sql_query = text(
                     """SELECT tile FROM tileids
                                     WHERE ST_Intersects(
                                         geometry,
                                         ST_MakeEnvelope(:minx, :miny, :maxx, :maxy, 4326) -- 4326 is the SRID, adjust if needed
                                     )
                                     """
                 )
-                result = self.session.execute(
+                result = self.db.execute(
                     sql_query,
                     {
                         "minx": bbox[0],
                         "miny": bbox[1],
                         "maxx": bbox[2],
                         "maxy": bbox[3],
                     },
                 )
                 rows = result.fetchall()
                 tile_list = set()
                 for row in rows:
                     tile_list.add(row[0])
                 master_tile_list.extend(tile_list)
 
-        self.session.close()
+        self.db.close()
         return master_tile_list
```

### Comparing `test_core_package-1.1.0/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-1.1.1/satelite/tests/sentinel2/test_get_tile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from satelite.sentinel2 import GetTiles
-from satelite.config import Session
+from satelite.config import DBSession
 
 
 class TestGetTiles:
 
     def test_get_tile_from_geom(self, monkeypatch):
         """testcase to get tile from geom"""
         geom = [{
@@ -27,14 +27,14 @@
             def mock_attribute():
                 pass
 
             mock_attribute.close = lambda: True
 
             return mock_attribute
 
-        monkeypatch.setattr(Session, "create", session_mock)
+        monkeypatch.setattr(DBSession, "create", session_mock)
         monkeypatch.setattr(GetTiles, "fetch_tile_from_db",
                             lambda x, y, z: [("gwfhg",), ("3basg",)])
 
         result = GetTiles().get_tile_from_geom(geom)
 
         assert len(result) == 2
```

### Comparing `test_core_package-1.1.0/setup.py` & `test_core_package-1.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
-    name="test_core_package",
-    version="1.1.0",
+    name="test-core-package",
+    version="1.1.1",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
@@ -24,12 +24,19 @@
         "jmespath==1.0.1",
         "multidict==6.0.5",
         "python-dateutil==2.9.0.post0",
         "s3transfer==0.10.1",
         "six==1.16.0",
         "urllib3==1.26.18",
         "yarl==1.9.4",
+        "awscli",
+        "gdal==3.6.2",
+        "google-cloud-storage",
+        "pyproj",
+        "rasterstats",
+        "rasterio",
+        "wget",
     ],
     package_data={
-        "test_core_package": ["qa_qc_check/*.json"],
+        "qa_qc_check": ["controller/*.json"],
     },
 )
```

