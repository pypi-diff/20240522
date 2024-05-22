# Comparing `tmp/geo_roughness_tool-0.2.2.tar.gz` & `tmp/geo_roughness_tool-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.2.2.tar", last modified: Tue May 21 23:55:56 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.2.3.tar", last modified: Wed May 22 00:10:26 2024, max compression
```

## Comparing `geo_roughness_tool-0.2.2.tar` & `geo_roughness_tool-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.520017 geo_roughness_tool-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.524017 geo_roughness_tool-0.2.2/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.524017 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/src/geo_roughness_tool/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png
--rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 23:55:48.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:55:56.528018 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-21 23:55:56.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-21 23:55:56.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:55:56.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 23:55:56.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 23:55:56.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 23:55:56.000000 geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.984018 geo_roughness_tool-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.988018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.988018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.2.2/LICENSE` & `geo_roughness_tool-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/PKG-INFO` & `geo_roughness_tool-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
@@ -24,15 +24,15 @@
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: Pillow>=10.3.0
 Requires-Dist: rasterio>=1.3.10
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: Markdown~=3.6
 Requires-Dist: tkinterhtml~=0.7
 
-![GeoRoughness_Banner_dark.png](../blob/master.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
```

### Comparing `geo_roughness_tool-0.2.2/README.md` & `geo_roughness_tool-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![GeoRoughness_Banner_dark.png](../blob/master.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
```

### Comparing `geo_roughness_tool-0.2.2/setup.py` & `geo_roughness_tool-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/header_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
-import os
 import webbrowser
 from typing import Any
 from PIL import Image
 import customtkinter as ctk
 from .defaults import DEFAULTS
+import os
 
 # Set up logging
 logger = logging.getLogger(__name__)
 
+
 class HeaderFrame(ctk.CTkFrame):
     """
     A class used to create the header frame of the GUI.
 
     Attributes
     ----------
     main_gui : Any
```

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
@@ -24,15 +24,15 @@
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: Pillow>=10.3.0
 Requires-Dist: rasterio>=1.3.10
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: Markdown~=3.6
 Requires-Dist: tkinterhtml~=0.7
 
-![GeoRoughness_Banner_dark.png](../blob/master.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
```

### Comparing `geo_roughness_tool-0.2.2/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

