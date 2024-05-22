# Comparing `tmp/geo_roughness_tool-0.2.3.tar.gz` & `tmp/geo_roughness_tool-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.2.3.tar", last modified: Wed May 22 00:10:26 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.2.4.tar", last modified: Wed May 22 00:15:12 2024, max compression
```

## Comparing `geo_roughness_tool-0.2.3.tar` & `geo_roughness_tool-0.2.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.984018 geo_roughness_tool-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.988018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.988018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png
--rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:10:06.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:26.992018 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 00:10:26.000000 geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.178133 geo_roughness_tool-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.178133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/preview_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.2.3/LICENSE` & `geo_roughness_tool-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/PKG-INFO` & `geo_roughness_tool-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.2.3/README.md` & `geo_roughness_tool-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/setup.py` & `geo_roughness_tool-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.2.3',
+    version='0.2.4',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/header_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.2.3/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 src/geo_roughness_tool/gui/analyze_and_optimize.py
 src/geo_roughness_tool/gui/defaults.py
 src/geo_roughness_tool/gui/footer_frame.py
 src/geo_roughness_tool/gui/header_frame.py
 src/geo_roughness_tool/gui/parameter_input.py
 src/geo_roughness_tool/gui/path_frame.py
 src/geo_roughness_tool/gui/preview_image.py
-src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png
-src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png
+src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
+src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
 src/geo_roughness_tool/tests/__init__.py
 src/geo_roughness_tool/tests/test_application_driver.py
```

