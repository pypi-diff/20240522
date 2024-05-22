# Comparing `tmp/scigee-0.0.8.tar.gz` & `tmp/scigee-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scigee-0.0.8.tar", last modified: Sat Aug 14 10:16:36 2021, max compression
+gzip compressed data, was "scigee-0.0.9.tar", last modified: Wed Sep  8 07:30:37 2021, max compression
```

## Comparing `scigee-0.0.8.tar` & `scigee-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/
--rw-rw-rw-   0        0        0       66 2020-06-26 09:14:35.000000 scigee-0.0.8/.gitattributes
--rw-rw-rw-   0        0        0      189 2021-02-07 14:35:32.000000 scigee-0.0.8/.gitignore
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    14497 2020-06-26 12:15:10.000000 scigee-0.0.8/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-rw-rw-   0        0        0      392 2021-08-14 10:16:36.000000 scigee-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       11 2020-06-26 09:14:35.000000 scigee-0.0.8/README.md
--rw-rw-rw-   0        0        0    14497 2020-07-14 09:50:33.000000 scigee-0.0.8/example.ipynb
--rw-rw-rw-   0        0        0    20478 2021-06-04 16:01:13.000000 scigee-0.0.8/module_test.ipynb
--rw-rw-rw-   0        0        0     1254 2020-04-29 16:45:08.000000 scigee-0.0.8/publish.py
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee/
--rw-rw-rw-   0        0        0      317 2021-06-04 15:27:28.000000 scigee-0.0.8/scigee/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee/__pycache__/
--rw-rw-rw-   0        0        0      450 2021-06-04 15:27:36.000000 scigee-0.0.8/scigee/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     3885 2020-06-26 10:23:13.000000 scigee-0.0.8/scigee/__pycache__/canvas.cpython-37.pyc
--rw-rw-rw-   0        0        0    13117 2021-06-04 15:57:13.000000 scigee-0.0.8/scigee/__pycache__/chart.cpython-37.pyc
--rw-rw-rw-   0        0        0     7564 2020-06-26 12:14:36.000000 scigee-0.0.8/scigee/__pycache__/geeface.cpython-37.pyc
--rw-rw-rw-   0        0        0    12938 2021-06-04 16:00:35.000000 scigee-0.0.8/scigee/__pycache__/geeface_lite.cpython-37.pyc
--rw-rw-rw-   0        0        0     5505 2020-06-26 12:00:19.000000 scigee-0.0.8/scigee/__pycache__/utilize.cpython-37.pyc
--rw-rw-rw-   0        0        0     4982 2020-05-04 14:23:59.000000 scigee-0.0.8/scigee/canvas.py
--rw-rw-rw-   0        0        0    18735 2021-06-04 15:55:30.000000 scigee-0.0.8/scigee/chart.py
--rw-rw-rw-   0        0        0     7555 2020-06-26 12:13:41.000000 scigee-0.0.8/scigee/geeface.py
--rw-rw-rw-   0        0        0    24258 2021-08-14 10:16:08.000000 scigee-0.0.8/scigee/geeface_lite.py
--rw-rw-rw-   0        0        0      138 2021-06-04 16:04:53.000000 scigee-0.0.8/scigee/requirements.txt
--rw-rw-rw-   0        0        0     6940 2020-06-26 11:59:57.000000 scigee-0.0.8/scigee/utilize.py
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee-history-versions/
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/
--rw-rw-rw-   0        0        0      205 2020-06-26 10:22:44.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/__pycache__/
--rw-rw-rw-   0        0        0      339 2020-06-26 10:23:08.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     3885 2020-06-26 10:23:13.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/__pycache__/canvas.cpython-37.pyc
--rw-rw-rw-   0        0        0     7564 2020-06-26 12:14:36.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/__pycache__/geeface.cpython-37.pyc
--rw-rw-rw-   0        0        0     5505 2020-06-26 12:00:19.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/__pycache__/utilize.cpython-37.pyc
--rw-rw-rw-   0        0        0     4982 2020-05-04 14:23:59.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/canvas.py
--rw-rw-rw-   0        0        0     7555 2020-06-26 12:13:41.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/geeface.py
--rw-rw-rw-   0        0        0     6940 2020-06-26 11:59:57.000000 scigee-0.0.8/scigee-history-versions/scigee-0.0.2/utilize.py
-drwxrwxrwx   0        0        0        0 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee.egg-info/
--rw-rw-rw-   0        0        0      392 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-08-14 10:16:36.000000 scigee-0.0.8/scigee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-14 10:16:36.000000 scigee-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1138 2021-08-14 10:16:20.000000 scigee-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-08 07:30:37.591591 scigee-0.0.9/
+-rw-rw-rw-   0        0        0      392 2021-09-08 07:30:37.591591 scigee-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2021-09-07 07:32:27.000000 scigee-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-09-08 07:30:37.561413 scigee-0.0.9/scigee/
+-rw-rw-rw-   0        0        0      317 2021-09-07 07:32:27.000000 scigee-0.0.9/scigee/__init__.py
+-rw-rw-rw-   0        0        0     4982 2021-09-07 07:32:27.000000 scigee-0.0.9/scigee/canvas.py
+-rw-rw-rw-   0        0        0    18735 2021-09-07 07:32:27.000000 scigee-0.0.9/scigee/chart.py
+-rw-rw-rw-   0        0        0     7555 2021-09-07 07:32:27.000000 scigee-0.0.9/scigee/geeface.py
+-rw-rw-rw-   0        0        0    28216 2021-09-08 07:29:30.000000 scigee-0.0.9/scigee/geeface_lite.py
+-rw-rw-rw-   0        0        0     6940 2021-09-07 07:32:27.000000 scigee-0.0.9/scigee/utilize.py
+drwxrwxrwx   0        0        0        0 2021-09-08 07:30:37.591591 scigee-0.0.9/scigee.egg-info/
+-rw-rw-rw-   0        0        0      392 2021-09-08 07:30:37.000000 scigee-0.0.9/scigee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2021-09-08 07:30:37.000000 scigee-0.0.9/scigee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-08 07:30:37.000000 scigee-0.0.9/scigee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2021-09-08 07:30:37.000000 scigee-0.0.9/scigee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-09-08 07:30:37.000000 scigee-0.0.9/scigee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-09-08 07:30:37.591591 scigee-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2021-09-08 07:30:23.000000 scigee-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scigee-0.0.8/scigee/canvas.py` & `scigee-0.0.9/scigee/canvas.py`

 * *Files identical despite different names*

### Comparing `scigee-0.0.8/scigee/chart.py` & `scigee-0.0.9/scigee/chart.py`

 * *Files identical despite different names*

### Comparing `scigee-0.0.8/scigee/geeface.py` & `scigee-0.0.9/scigee/geeface.py`

 * *Files identical despite different names*

### Comparing `scigee-0.0.8/scigee/geeface_lite.py` & `scigee-0.0.9/scigee/geeface_lite.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,57 +231,141 @@
     plt.show()
 
 class DataInfo:
     def __init__(self):
       pass
     # --------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def s5p_o3(): # start from 2018-09-08
-        collection = "COPERNICUS/S5P/NRTI/L3_O3" # "COPERNICUS/S5P/OFFL/L3_O3"
+    def s5p_o3(NTRI = True): # start from 2018-09-08
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_O3"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_O3"
         bands = [
                 "O3_column_number_density", "O3_column_number_density_amf", "O3_slant_column_number_density",
                 "O3_effective_temperature", "cloud_fraction", 
                 "sensor_azimuth_angle", "sensor_zenith_angle", "solar_azimuth_angle", "solar_zenith_angle"
         ]
         label_bands = [
                     "o3_vcd", "o3_amf", "o3_scd",
                     "o3_temperature", "s5p_cloud_fraction",
-                    "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_zai", "s5p_sun_zen"
+                    "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_azi", "s5p_sun_zen"
         ]
         scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
         return collection, bands, label_bands, scale
     # --------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def s5p_hcho(): # start from 2018-10-02
-        collection = "COPERNICUS/S5P/NRTI/L3_HCHO"
+    def s5p_hcho(NTRI = True): # start from 2018-10-02
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_HCHO"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_HCHO"
         bands = [
                 "tropospheric_HCHO_column_number_density", "tropospheric_HCHO_column_number_density_amf", "HCHO_slant_column_number_density",
                 "cloud_fraction",
                 "sensor_azimuth_angle", "sensor_zenith_angle", "solar_azimuth_angle", "solar_zenith_angle"
         ]
         label_bands = [
                     "hcho_vcd", "hcho_amf", "hcho_scd",
                     "s5p_cloud_fraction",
-                    "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_zai", "s5p_sun_zen"
+                    "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_azi", "s5p_sun_zen"
         ]
         scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
         return collection, bands, label_bands, scale
     # --------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def s5p_no2(): # start from 2018-07-10
-        collection = "COPERNICUS/S5P/NRTI/L3_NO2"
+    def s5p_no2(NTRI = True): # start from 2018-07-10
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_NO2"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_NO2"
         bands = [
                 "NO2_column_number_density", "tropospheric_NO2_column_number_density", "stratospheric_NO2_column_number_density",
                 "NO2_slant_column_number_density", "tropopause_pressure", "absorbing_aerosol_index", "cloud_fraction",
                 "sensor_altitude", "sensor_azimuth_angle", "sensor_zenith_angle", "solar_azimuth_angle", "solar_zenith_angle"
         ]
         label_bands = [
                     "no2_total_vcd", "no2_vcd", "no2_strato_vcd", "no2_scd",
                     "tropopause_pressure", "absorbing_aerosol_index", "s5p_cloud_fraction",
-                    "sp5_sen_alt", "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_zai", "s5p_sun_zen"
+                    "sp5_sen_alt", "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_azi", "s5p_sun_zen"
+        ]
+        scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
+        return collection, bands, label_bands, scale
+    # --------------------------------------------------------------------------------------------------------------
+    @staticmethod
+    def s5p_co(NTRI = True): # start from 2018-06-28
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_CO"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_CO"
+        bands = [
+                "CO_column_number_density", "H2O_column_number_density", "cloud_height",
+                "sensor_altitude", "sensor_azimuth_angle", "sensor_zenith_angle", "solar_azimuth_angle", "solar_zenith_angle"
+        ]
+        label_bands = [
+                    "co_vcd", "h2o_vcd", "cloud_height",
+                    "sp5_sen_alt", "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_azi", "s5p_sun_zen"
+        ]
+        scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
+        return collection, bands, label_bands, scale
+    # --------------------------------------------------------------------------------------------------------------
+    @staticmethod
+    def s5p_so2(NTRI = True): # start from 2018-07-10
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_SO2"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_SO2"
+        bands = [
+                "SO2_column_number_density", "SO2_column_number_density_amf", "SO2_slant_column_number_density",
+                "absorbing_aerosol_index", "cloud_fraction",
+                "sensor_azimuth_angle", "sensor_zenith_angle", "solar_azimuth_angle", "solar_zenith_angle",
+                "SO2_column_number_density_15km"
+        ]
+        label_bands = [
+                    "so2_vcd", "so2_amf", "hcho_scd",
+                    "s5p_aai", "s5p_cloud_fraction",
+                    "s5p_sen_azi", "s5p_sen_zen", "s5p_sun_azi", "s5p_sun_zen",
+                    "so2_vcd_15km"
+        ]
+        scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
+        return collection, bands, label_bands, scale
+    # --------------------------------------------------------------------------------------------------------------
+    @staticmethod
+    def s5p_ch4(NTRI = True): # start from 2019-02-08
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_CH4"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_CH4"
+        bands = [
+            "CH4_column_volume_mixing_ratio_dry_air", 
+            "aerosol_height", "aerosol_optical_depth",
+            "sensor_azimuth_angle", "sensor_zenith_angle",
+            "solar_azimuth_angle", "solar_zenith_angle"
+        ]
+        label_bands = [
+                    "xch4", "aerosol_height", "aod", 
+                    "s5p_sen_azi", "s5p_sen_zen", 
+                    "s5p_sun_azi", "s5p_sun_zen"
+        ]
+        scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
+        return collection, bands, label_bands, scale
+    # --------------------------------------------------------------------------------------------------------------
+    @staticmethod
+    def s5p_aai(NTRI = True): # start from 2018-07-04
+        if NTRI:
+            collection = "COPERNICUS/S5P/NRTI/L3_AER_AI"
+        else:
+            collection = "COPERNICUS/S5P/OFFL/L3_AER_AI"
+        bands = [
+            "absorbing_aerosol_index", "sensor_altitude", "sensor_azimuth_angle", "sensor_zenith_angle",
+            "solar_azimuth_angle", "solar_zenith_angle"
+        ]
+        label_bands = [
+                    "aai", "sp5_sen_alt", "s5p_sen_azi", "s5p_sen_zen", 
+                    "s5p_sun_azi", "s5p_sun_zen"
         ]
         scale = 0.01 * 100 * 1000 # 0.01 arc degree -> meters
         return collection, bands, label_bands, scale
     # --------------------------------------------------------------------------------------------------------------
     @staticmethod
     def modis_reflectance():
         collection = "MODIS/006/MCD43A4" # 1-Day
```

### Comparing `scigee-0.0.8/scigee/utilize.py` & `scigee-0.0.9/scigee/utilize.py`

 * *Files identical despite different names*

### Comparing `scigee-0.0.8/setup.py` & `scigee-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
 	name = "scigee",
-	version = "0.0.8",
+	version = "0.0.9",
 	keywords = ("easy geo warpper", "atmospheric data","satellite data", "flux"),
 	description = "For faster proccessing geofile",
 	long_description = "Read/write and process rs/gis related data, especially atmospheric rs data.",
 	license = "MIT Licence",
 
 	url="https://github.com/soonyenju/scigee",
 	author = "Songyan Zhu",
```

