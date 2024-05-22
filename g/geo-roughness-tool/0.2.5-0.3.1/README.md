# Comparing `tmp/geo_roughness_tool-0.2.5.tar.gz` & `tmp/geo_roughness_tool-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.2.5.tar", last modified: Wed May 22 00:20:37 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.3.1.tar", last modified: Wed May 22 07:45:13 2024, max compression
```

## Comparing `geo_roughness_tool-0.2.5.tar` & `geo_roughness_tool-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.488464 geo_roughness_tool-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:20:37.488464 geo_roughness_tool-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:20:37.488464 geo_roughness_tool-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.480464 geo_roughness_tool-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.480464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/preview_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
--rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.666103 geo_roughness_tool-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 07:45:13.666103 geo_roughness_tool-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:45:13.666103 geo_roughness_tool-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.658103 geo_roughness_tool-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.658103 geo_roughness_tool-0.3.1/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.662103 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.662103 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/preview_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.666103 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/app_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/app_icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.666103 geo_roughness_tool-0.3.1/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 07:45:05.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:45:13.666103 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 07:45:13.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-22 07:45:13.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:45:13.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 07:45:13.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 07:45:13.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 07:45:13.000000 geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.2.5/LICENSE` & `geo_roughness_tool-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/PKG-INFO` & `geo_roughness_tool-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.5
+Version: 0.3.1
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.2.5/README.md` & `geo_roughness_tool-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/setup.py` & `geo_roughness_tool-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.2.5',
+    version='0.3.1',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/header_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         # Create the help button
         self.help_button = ctk.CTkButton(self, text="Help", command=self.open_help)
         self.help_button.grid(row=0, column=1, padx=(DEFAULTS.PADX, DEFAULTS.PADX * 2), pady=(DEFAULTS.PADY, DEFAULTS.PADY * 0.5), sticky="e")
         logger.info("Help button created")
 
         # Create the toggle button
         self.toggle_button = ctk.CTkButton(self, text="Show Advanced", command=self.toggle_advanced_options)
-        self.toggle_button.grid(row=1, column=1, padx=(DEFAULTS.PADX, DEFAULTS.PADX * 2), pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5), sticky="e")
+        self.toggle_button.grid(row=1, column=1, padx=(DEFAULTS.PADX, DEFAULTS.PADX * 2), pady=(DEFAULTS.PADY * 0.5, 0), sticky="e")
         logger.info("Toggle button created")
 
         # Bind the resize event to update the image size
         self.bind("<Configure>", self.on_resize)
 
         # Initial image setup
         self.update_banner_image()
```

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/gui_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 Author: Lukas Batschelet
 Date: 14.05.2024
 -----------
 This module contains the main GUI class for the Surface Roughness Calculator application.
 """
 
 import logging
+import os
 import tkinter as tk
+import platform
 from tkinter import messagebox, filedialog
 
 import customtkinter as ctk
 import rasterio
-from PIL import Image
+from PIL import Image, ImageTk
 from customtkinter import CTkScrollableFrame
 
 from .classes.application_driver import ApplicationDriver
 from .classes.processing_parameters import ProcessingParameters
 from .classes.threshold_optimizer import ThresholdOptimizer
 from .gui.defaults import DEFAULTS
 from .gui.footer_frame import FooterFrame
@@ -47,14 +49,23 @@
             "h3": ctk.CTkFont(size=14, weight="bold"),
             "body": ctk.CTkFont(size=13),
             "small": ctk.CTkFont(size=10),
             "tiny": ctk.CTkFont(size=8),
             "monospace": ctk.CTkFont(family="Courier New", size=12)
         }
 
+        # Set window icon
+        script_dir = os.path.dirname(__file__)
+        if platform.system() == "Windows":
+            self.iconbitmap(os.path.join(script_dir, "gui/resources", "app_icon_dark.ico"))
+        else:
+            light_icon_path = os.path.join(script_dir, "gui/resources", "app_icon_light.png")
+            dark_icon_path = os.path.join(script_dir, "gui/resources", "app_icon_dark.png")
+            self.set_icon(light_icon_path, dark_icon_path)
+
         # Get screen width and height
         screen_width = int(0.65 * self.winfo_screenwidth())
         screen_height = int(0.7 * self.winfo_screenheight())
 
         # Set window size to screen size
         self.geometry(f"{screen_width}x{screen_height}")
 
@@ -89,14 +100,36 @@
                                 sticky="nsew")
 
         self.footer_frame = FooterFrame(self.scrolled_frame, self)
         self.footer_frame.grid(row=4,
                                column=0,
                                sticky="nsew")
 
+    def set_icon(self, light_icon_path, dark_icon_path):
+        if self.get_appearance_mode() == "Dark":
+            icon_image = Image.open(dark_icon_path)
+        else:
+            icon_image = Image.open(light_icon_path)
+
+        icon_photo = ImageTk.PhotoImage(icon_image)
+        self.iconphoto(True, icon_photo)
+
+    def bind_theme_change_event(self):
+        def on_theme_change(event):
+            if platform.system() != "Windows":
+                self.set_icon(
+                    os.path.join(os.path.dirname(__file__), "resources", "app_icon_light.png"),
+                    os.path.join(os.path.dirname(__file__), "resources", "app_icon_dark.png")
+                )
+
+        self.bind('<<ThemeChanged>>', on_theme_change)
+
+    def get_appearance_mode(self):
+        return ctk.get_appearance_mode()
+
     def toggle_advanced_options(self):
         self.show_advanced_options = not self.show_advanced_options
         self.parameter_frame.toggle_advanced_options(self.show_advanced_options)
         self.path_frame.toggle_advanced_options(self.show_advanced_options)
 
     def start_processing(self) -> None:
         """
```

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.5
+Version: 0.3.1
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.3.1/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 src/geo_roughness_tool/gui/footer_frame.py
 src/geo_roughness_tool/gui/header_frame.py
 src/geo_roughness_tool/gui/parameter_input.py
 src/geo_roughness_tool/gui/path_frame.py
 src/geo_roughness_tool/gui/preview_image.py
 src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
 src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
+src/geo_roughness_tool/gui/resources/app_icon_dark.ico
+src/geo_roughness_tool/gui/resources/app_icon_dark.png
+src/geo_roughness_tool/gui/resources/app_icon_light.png
 src/geo_roughness_tool/tests/__init__.py
 src/geo_roughness_tool/tests/test_application_driver.py
```

