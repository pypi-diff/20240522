# Comparing `tmp/geo_roughness_tool-0.1.1.tar.gz` & `tmp/geo_roughness_tool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.1.1.tar", last modified: Tue May 21 21:09:48 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.1.2.tar", last modified: Tue May 21 22:50:09 2024, max compression
```

## Comparing `geo_roughness_tool-0.1.1.tar` & `geo_roughness_tool-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.745254 geo_roughness_tool-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-21 21:09:48.745254 geo_roughness_tool-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:09:48.745254 geo_roughness_tool-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.737254 geo_roughness_tool-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.737254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.139984 geo_roughness_tool-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.139984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.1.1/LICENSE` & `geo_roughness_tool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/PKG-INFO` & `geo_roughness_tool-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
-Author-email: your-email@example.com
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
 Keywords: GIS,GeoTIFF,DEM,surface roughness,geographic information systems
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -22,18 +21,20 @@
 License-File: LICENSE
 Requires-Dist: customtkinter>=5.2.2
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: Pillow>=10.3.0
 Requires-Dist: rasterio>=1.3.10
 Requires-Dist: setuptools>=69.5.1
-Requires-Dist: geo_roughness_tool~=0.0.1
 Requires-Dist: Markdown~=3.6
 Requires-Dist: tkinterhtml~=0.7
 
+![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
+
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
 
 - **GeoTIFF Support**: Load and process DEM data directly from GeoTIFF files.
@@ -76,15 +77,15 @@
 python3 --version
 pip3 --version
 ```
 
 #### 3. Install GeoRoughness Tool
 Install the package via pip:
 ```bash
-pip3 install dem-roughness-calculator
+pip3 install geo-roughness-tool
 ```
 
 ## Usage
 
 ### GUI Application
 
 To launch the GUI, simply run the following command in your terminal:
```

### Comparing `geo_roughness_tool-0.1.1/README.md` & `geo_roughness_tool-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
+
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
 
 - **GeoTIFF Support**: Load and process DEM data directly from GeoTIFF files.
@@ -44,15 +47,15 @@
 python3 --version
 pip3 --version
 ```
 
 #### 3. Install GeoRoughness Tool
 Install the package via pip:
 ```bash
-pip3 install dem-roughness-calculator
+pip3 install geo-roughness-tool
 ```
 
 ## Usage
 
 ### GUI Application
 
 To launch the GUI, simply run the following command in your terminal:
```

### Comparing `geo_roughness_tool-0.1.1/setup.py` & `geo_roughness_tool-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
-    author_email='your-email@example.com',  # Replace with your email
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
     long_description_content_type='text/markdown',
     install_requires=read_requirements('requirements.txt'),  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
     entry_points={
         'console_scripts': [
```

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/header_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
-Author-email: your-email@example.com
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
 Keywords: GIS,GeoTIFF,DEM,surface roughness,geographic information systems
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -22,18 +21,20 @@
 License-File: LICENSE
 Requires-Dist: customtkinter>=5.2.2
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: Pillow>=10.3.0
 Requires-Dist: rasterio>=1.3.10
 Requires-Dist: setuptools>=69.5.1
-Requires-Dist: geo_roughness_tool~=0.0.1
 Requires-Dist: Markdown~=3.6
 Requires-Dist: tkinterhtml~=0.7
 
+![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
+![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
+
 # GeoRoughness Tool
 
 The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
 
 - **GeoTIFF Support**: Load and process DEM data directly from GeoTIFF files.
@@ -76,15 +77,15 @@
 python3 --version
 pip3 --version
 ```
 
 #### 3. Install GeoRoughness Tool
 Install the package via pip:
 ```bash
-pip3 install dem-roughness-calculator
+pip3 install geo-roughness-tool
 ```
 
 ## Usage
 
 ### GUI Application
 
 To launch the GUI, simply run the following command in your terminal:
```

### Comparing `geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

