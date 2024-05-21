# Comparing `tmp/geo_roughness_tool-0.1.2.tar.gz` & `tmp/geo_roughness_tool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.1.2.tar", last modified: Tue May 21 22:50:09 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.2.0.tar", last modified: Tue May 21 23:28:40 2024, max compression
```

## Comparing `geo_roughness_tool-0.1.2.tar` & `geo_roughness_tool-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.139984 geo_roughness_tool-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.139984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 22:49:59.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:50:09.143984 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 22:50:09.000000 geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.418595 geo_roughness_tool-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.418595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 23:28:27.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:28:40.422595 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 23:28:40.000000 geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.1.2/LICENSE` & `geo_roughness_tool-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/PKG-INFO` & `geo_roughness_tool-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.1.2
+Version: 0.2.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.1.2/README.md` & `geo_roughness_tool-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/setup.py` & `geo_roughness_tool-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.1.2',
+    version='0.2.0',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/header_frame.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/path_frame.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,105 @@
-import logging
-from typing import Any
+import abc
+import os
+import tkinter as tk
+from tkinter import filedialog
 
 import customtkinter as ctk
 
 from .defaults import DEFAULTS
 
-# Set up logging
-logger = logging.getLogger(__name__)
 
-
-class HeaderFrame(ctk.CTkFrame):
-    """
-    A class used to create the header frame of the GUI.
-
-    Attributes
-    ----------
-    main_gui : Any
-        The main GUI object.
-    title_label : ctk.CTkLabel
-        The label that displays the title.
-    description_label : ctk.CTkLabel
-        The label that displays the description.
-    """
-    def __init__(self, parent: ctk.CTk, main_gui: Any, **kwargs: Any):
-        """
-        Constructs all the necessary attributes for the HeaderFrame object.
-
-        Parameters
-        ----------
-            parent : ctk.CTk
-                The parent widget.
-            main_gui : Any
-                The main GUI object.
-            **kwargs : Any
-                Additional keyword arguments.
-        """
+class PathFrame(ctk.CTkFrame):
+    def __init__(self, parent, main_gui, **kwargs):
         super().__init__(parent, **kwargs)
-        logger.info("Initializing HeaderFrame")
+
         self.main_gui = main_gui
 
-        # Configure the grid
+        # Make the GUI responsive
         self.grid_columnconfigure(0, weight=1)
-        self.grid_columnconfigure(1, weight=0)
-        self.grid_rowconfigure([0, 1], weight=1)
+        self.grid_rowconfigure(0, weight=1)
+        self.grid_rowconfigure(1, weight=1)
 
-        # Create the title label
-        self.title_label = (
-            ctk.CTkLabel(self,
-                         text="GeoRoughness Tool",
-                         font=self.main_gui.fonts['h1']))
-        self.title_label.grid(row=0,
-                              column=0,
-                              padx=DEFAULTS.PADX,
-                              pady=(DEFAULTS.PADY, 0),
-                              sticky="w")
-        logger.info("Title label created")
-
-        # Create the description label
-        self.description_label = (
-            ctk.CTkLabel(self,
-                         text="Program to calculate and categorize surface Roughness.",
-                         font=self.main_gui.fonts['body']))
-        self.description_label.grid(row=1,
-                                    column=0,
-                                    padx=DEFAULTS.PADX,
-                                    pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
-                                    sticky="w")
-        logger.info("Description label created")
-
-        # Create the toggle button
-        self.toggle_button = ctk.CTkButton(self, text="Show Advanced", command=self.toggle_advanced_options)
-        self.toggle_button.grid(row=0,
-                                column=1,
-                                padx=(DEFAULTS.PADX, DEFAULTS.PADY * 2),
-                                pady=(DEFAULTS.PADY, 0),
-                                sticky="e")
-        logger.info("Toggle button created")
-
-    def toggle_advanced_options(self):
-        self.main_gui.toggle_advanced_options()
-        if self.main_gui.show_advanced_options:
-            self.toggle_button.configure(text="Hide Advanced")
+        self.input_path_field = InputPathField(self, main_gui, "Input Path")
+        self.input_path_field.grid(row=0,
+                                   column=0,
+                                   padx=DEFAULTS.PADX,
+                                   pady=(DEFAULTS.PADY* 0.5, DEFAULTS.PADY * 0.5),
+                                   sticky="nsew")
+
+        self.output_dir_field = OutputDirField(self, main_gui, "Output Directory (Optional)")
+        self.output_dir_field.grid(row=1,
+                                   column=0,
+                                   padx=DEFAULTS.PADX,
+                                   pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
+                                   sticky="nsew")
+        self.output_dir_field.grid_remove()  # Initially hide the output directory field
+
+    def toggle_advanced_options(self, show):
+        if show:
+            self.output_dir_field.grid()
         else:
-            self.toggle_button.configure(text="Show Advanced")
+            self.output_dir_field.grid_remove()
+
+    def get_parameters(self):
+        return {
+            "input_path": self.input_path_field.get(),
+            "output_dir": self.output_dir_field.get() or None
+        }
+
+
+
+class PathField(ctk.CTkFrame, abc.ABC):
+    def __init__(self, parent, main_gui, name, **kwargs):
+        super().__init__(parent, **kwargs)
+        self.main_gui = main_gui
+        self.grid_columnconfigure(0, weight=1)
+
+        self.name_label = ctk.CTkLabel(self, text=name, font=self.main_gui.fonts['h3'])
+        self.name_label.grid(row=0,
+                             column=0,
+                             padx=DEFAULTS.PADX,
+                             pady=(DEFAULTS.PADY, DEFAULTS.PADY * 0.5),
+                             sticky="w")
+
+        self.entry = ctk.CTkEntry(self)
+        self.entry.grid(row=1,
+                        column=0,
+                        padx=(DEFAULTS.PADX, DEFAULTS.PADX * 0.5),
+                        pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
+                        sticky="ew")
+
+        self.browse_button = ctk.CTkButton(self, text="Browse", command=self.browse)
+        self.browse_button.grid(row=1,
+                                column=1,
+                                padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX),
+                                pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY))
 
+    @abc.abstractmethod
+    def browse(self):
+        pass
+
+    def get(self):
+        return self.entry.get()
+
+    def validate(self):
+        path = self.get()
+        if not os.path.exists(path):
+            print("Invalid path")
+            return False
+        return True
+
+
+class InputPathField(PathField):
+    def browse(self):
+        file_path = filedialog.askopenfilename()
+        if file_path:
+            self.entry.delete(0, tk.END)
+            self.entry.insert(0, file_path)
+
+
+class OutputDirField(PathField):
+    def browse(self):
+        dir_path = filedialog.askdirectory()
+        if dir_path:
+            self.entry.delete(0, tk.END)
+            self.entry.insert(0, dir_path)
```

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.1.2
+Version: 0.2.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.1.2/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.2.0/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

