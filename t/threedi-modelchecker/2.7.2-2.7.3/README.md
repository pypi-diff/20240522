# Comparing `tmp/threedi_modelchecker-2.7.2.tar.gz` & `tmp/threedi_modelchecker-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi_modelchecker-2.7.2.tar", last modified: Tue Apr 23 07:01:33 2024, max compression
+gzip compressed data, was "threedi_modelchecker-2.7.3.tar", last modified: Wed May 22 12:05:33 2024, max compression
```

## Comparing `threedi_modelchecker-2.7.2.tar` & `threedi_modelchecker-2.7.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.320778 threedi_modelchecker-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-23 07:01:33.320778 threedi_modelchecker-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:01:33.320778 threedi_modelchecker-2.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.304778 threedi_modelchecker-2.7.2/threedi_modelchecker/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.308778 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/geo_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    40348 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/other.py
--rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/checks/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)   116618 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.308778 threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/raster_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/raster_interface_gdal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/raster_interface_rasterio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.312778 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.312778 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  6242304 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/data/empty.gpkg
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    27178 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22499 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    30012 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_other.py
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-23 07:01:29.000000 threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_model_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:33.320778 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-23 07:01:33.000000 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-23 07:01:33.000000 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:01:33.000000 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 07:01:33.000000 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 07:01:33.000000 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 07:01:33.000000 threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.155342 threedi_modelchecker-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    25369 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-22 12:05:33.155342 threedi_modelchecker-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:05:33.155342 threedi_modelchecker-2.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.139342 threedi_modelchecker-2.7.3/threedi_modelchecker/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.143342 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24255 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/geo_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40348 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/checks/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116622 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.143342 threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/raster_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/raster_interface_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/raster_interface_rasterio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.143342 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.143342 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  6242304 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/data/empty.gpkg
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27178 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22499 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30012 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-22 12:05:29.000000 threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_model_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:05:33.151342 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-22 12:05:33.000000 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-22 12:05:33.000000 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:05:33.000000 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 12:05:33.000000 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 12:05:33.000000 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 12:05:33.000000 threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/top_level.txt
```

### Comparing `threedi_modelchecker-2.7.2/CHANGES.rst` & `threedi_modelchecker-2.7.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Changelog of threedi-modelchecker
 =================================
 
 
+2.7.3 (2024-05-22)
+------------------
+
+- Expand description of check 188.
+- Add missing spaces in error message for check 185.
+
+
 2.7.2 (2024-04-23)
 ------------------
 
 - Fix bug with check 183
 
 
 2.7.1 (2024-04-22)
 ------------------
 
 - Add info check 1406 to inform the user if a raster is not compressed.
 - Add check 799 to warn if raster friction pixels are < 1 while Chezy friction is selected
 - Change error message for check 1500
+- Fix check 183 which failed in the QGIS plugin
 
 
 2.7.0 (2024-03-12)
 ------------------
 
 - Support geopackage
 - Support changes in threedi-schema (0.220) needed for geopackage support
```

### Comparing `threedi_modelchecker-2.7.2/LICENSE` & `threedi_modelchecker-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/PKG-INFO` & `threedi_modelchecker-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.7.2
+Version: 2.7.3
 Summary: Checks validity of a 3Di schematisation
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-modelchecker
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `threedi_modelchecker-2.7.2/README.rst` & `threedi_modelchecker-2.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/pyproject.toml` & `threedi_modelchecker-2.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/base.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/base.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/cross_section_definitions.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/cross_section_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -622,14 +622,17 @@
                 continue
             if not self.min_valid(min(values)):
                 invalids.append(record)
             elif not self.max_valid(max(values)):
                 invalids.append(record)
         return invalids
 
+    def description(self):
+        return f"some values in {self.column_name} are {self.range_str}, which is not allowed for friction type(s) {self.friction_types}"
+
 
 class OpenIncreasingCrossSectionVariableCheck(CrossSectionBaseCheck):
     """
     Check if cross sections used with friction with conveyance
     are open and monotonically increasing in width
     """
```

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/factories.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/factories.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/geo_query.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/geo_query.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/other.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/other.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/raster.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/raster.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/checks/timeseries.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/checks/timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/config.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3044,19 +3044,19 @@
                 )
             )
             .filter(
                 models.CrossSectionDefinition.friction_values.is_not(None)
                 & models.CrossSectionLocation.friction_value.is_not(None)
             )
         ),
-        message=f"Both {models.CrossSectionDefinition.friction_values.table.name}.{models.CrossSectionDefinition.friction_values.name}"
-        f"and {models.CrossSectionLocation.friction_value.table.name}.{models.CrossSectionLocation.friction_value.name}"
+        message=f"Both {models.CrossSectionDefinition.friction_values.table.name}.{models.CrossSectionDefinition.friction_values.name} "
+        f"and {models.CrossSectionLocation.friction_value.table.name}.{models.CrossSectionLocation.friction_value.name} "
         f"are defined for conveyance friction. Only "
-        f"{models.CrossSectionDefinition.friction_values.table.name}.{models.CrossSectionDefinition.friction_values.name}"
-        f"will be used",
+        f"{models.CrossSectionDefinition.friction_values.table.name}.{models.CrossSectionDefinition.friction_values.name} "
+        f"will be used.",
     ),
 ]
 CHECKS += [
     OpenIncreasingCrossSectionVariableCheck(
         error_code=186,
         column=col,
     )
```

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/exporters.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/exporters.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/raster_interface.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/raster_interface.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/raster_interface_gdal.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/raster_interface_gdal.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/interfaces/raster_interface_rasterio.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/interfaces/raster_interface_rasterio.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/model_checks.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/scripts.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/conftest.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/data/empty.gpkg` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/data/empty.gpkg`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/factories.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_base.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_cross_section_definitions.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_factories.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_factories.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_other.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_other.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_raster.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_raster.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_checks_timeseries.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_checks_timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_exporters.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker/tests/test_model_checks.py` & `threedi_modelchecker-2.7.3/threedi_modelchecker/tests/test_model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/PKG-INFO` & `threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.7.2
+Version: 2.7.3
 Summary: Checks validity of a 3Di schematisation
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-modelchecker
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `threedi_modelchecker-2.7.2/threedi_modelchecker.egg-info/SOURCES.txt` & `threedi_modelchecker-2.7.3/threedi_modelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

