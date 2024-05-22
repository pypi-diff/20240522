# Comparing `tmp/geo_roughness_tool-0.2.4.tar.gz` & `tmp/geo_roughness_tool-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.2.4.tar", last modified: Wed May 22 00:15:12 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.2.5.tar", last modified: Wed May 22 00:20:37 2024, max compression
```

## Comparing `geo_roughness_tool-0.2.4.tar` & `geo_roughness_tool-0.2.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.178133 geo_roughness_tool-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.178133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/preview_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
--rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.182133 geo_roughness_tool-0.2.4/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:14:57.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:15:12.186133 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 00:15:12.000000 geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.488464 geo_roughness_tool-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:20:37.488464 geo_roughness_tool-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:20:37.488464 geo_roughness_tool-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.480464 geo_roughness_tool-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.480464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 00:20:28.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/preview_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:20:29.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:20:37.484464 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 00:20:37.000000 geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.2.4/LICENSE` & `geo_roughness_tool-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/PKG-INFO` & `geo_roughness_tool-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.2.4/README.md` & `geo_roughness_tool-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/setup.py` & `geo_roughness_tool-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/header_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         # Load the original images
         script_dir = os.path.dirname(__file__)
         self.original_light_image = Image.open(os.path.join(script_dir, "resources", "GeoRoughness-Banner-lang-Light.png"))
         self.original_dark_image = Image.open(os.path.join(script_dir, "resources", "GeoRoughness-Banner-lang-dark.png"))
 
         # Create the banner label
         self.banner_label = ctk.CTkLabel(self, text="")
-        self.banner_label.grid(row=0, column=0, padx=DEFAULTS.PADX, pady=(DEFAULTS.PADY, 0), sticky="w")
+        self.banner_label.grid(row=0, column=0, padx=DEFAULTS.PADX, pady=(DEFAULTS.PADY, 0), sticky="nsw", rowspan=2)
         logger.info("Banner label created")
 
         # Create the help button
         self.help_button = ctk.CTkButton(self, text="Help", command=self.open_help)
         self.help_button.grid(row=0, column=1, padx=(DEFAULTS.PADX, DEFAULTS.PADX * 2), pady=(DEFAULTS.PADY, DEFAULTS.PADY * 0.5), sticky="e")
         logger.info("Help button created")
```

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.2.4/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.2.5/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

