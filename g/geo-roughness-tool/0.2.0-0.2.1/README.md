# Comparing `tmp/geo_roughness_tool-0.2.0.tar.gz` & `tmp/geo_roughness_tool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.2.0.tar", last modified: Tue May 21 23:28:40 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.2.1.tar", last modified: Tue May 21 23:53:27 2024, max compression
```

## Comparing `geo_roughness_tool-0.2.0.tar` & `geo_roughness_tool-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.418595 geo_roughness_tool-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.418595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.971317 geo_roughness_tool-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.975317 geo_roughness_tool-0.2.1/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.975317 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/src/geo_roughness_tool/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 23:53:19.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:53:27.979317 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-21 23:53:27.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-21 23:53:27.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:53:27.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 23:53:27.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 23:53:27.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 23:53:27.000000 geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.2.0/LICENSE` & `geo_roughness_tool-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/PKG-INFO` & `geo_roughness_tool-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.0
+Version: 0.2.1
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
 
-![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_dark.png](../blob/master.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
```

### Comparing `geo_roughness_tool-0.2.0/README.md` & `geo_roughness_tool-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_dark.png](../blob/master.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
```

### Comparing `geo_roughness_tool-0.2.0/setup.py` & `geo_roughness_tool-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
     long_description_content_type='text/markdown',
     install_requires=read_requirements('requirements.txt'),  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
+    include_package_data=True,  # Include package data specified in MANIFEST.in
     entry_points={
         'console_scripts': [
             'georough=geo_roughness_tool.main:main',
             'dingsbums=geo_roughness_tool.main:main',
             'giraffe=geo_roughness_tool.main:main',
         ]
     },
```

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/header_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,21 +49,23 @@
         self.current_size = (0, 0)
 
         # Configure the grid
         self.grid_columnconfigure(0, weight=1)
         self.grid_columnconfigure(1, weight=0)
         self.grid_rowconfigure([0,1], weight=1)
 
+
         # Load the original images
-        self.original_dark_image = Image.open("src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png")
-        self.original_light_image = Image.open("src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png")
+        script_dir = os.path.dirname(__file__)
+        self.original_light_image = Image.open(os.path.join(script_dir, "resources", "GeoRoughness-Banner-lang-Light.png"))
+        self.original_dark_image = Image.open(os.path.join(script_dir, "resources", "GeoRoughness-Banner-lang-dark.png"))
 
         # Create the banner label
         self.banner_label = ctk.CTkLabel(self, text="")
-        self.banner_label.grid(row=0, column=0, padx=DEFAULTS.PADX, pady=(DEFAULTS.PADY, DEFAULTS.PADY * 0.5), sticky="w", rowspan=2)
+        self.banner_label.grid(row=0, column=0, padx=DEFAULTS.PADX, pady=(DEFAULTS.PADY, 0), sticky="w")
         logger.info("Banner label created")
 
         # Create the help button
         self.help_button = ctk.CTkButton(self, text="Help", command=self.open_help)
         self.help_button.grid(row=0, column=1, padx=(DEFAULTS.PADX, DEFAULTS.PADX * 2), pady=(DEFAULTS.PADY, DEFAULTS.PADY * 0.5), sticky="e")
         logger.info("Help button created")
```

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.0
+Version: 0.2.1
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
 
-![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_dark.png](../blob/master.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
```

### Comparing `geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.2.1/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 src/geo_roughness_tool/__init__.py
 src/geo_roughness_tool/cli_main.py
 src/geo_roughness_tool/gui_main.py
 src/geo_roughness_tool/log_config.py
 src/geo_roughness_tool/main.py
@@ -22,9 +23,11 @@
 src/geo_roughness_tool/gui/analyze_and_optimize.py
 src/geo_roughness_tool/gui/defaults.py
 src/geo_roughness_tool/gui/footer_frame.py
 src/geo_roughness_tool/gui/header_frame.py
 src/geo_roughness_tool/gui/parameter_input.py
 src/geo_roughness_tool/gui/path_frame.py
 src/geo_roughness_tool/gui/preview_image.py
+src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-Light.png
+src/geo_roughness_tool/resources/GeoRoughness-Banner-lang-dark.png
 src/geo_roughness_tool/tests/__init__.py
 src/geo_roughness_tool/tests/test_application_driver.py
```

