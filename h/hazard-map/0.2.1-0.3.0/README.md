# Comparing `tmp/hazard_map-0.2.1.tar.gz` & `tmp/hazard_map-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazard_map-0.2.1.tar", max compression
+gzip compressed data, was "hazard_map-0.3.0.tar", max compression
```

## Comparing `hazard_map-0.2.1.tar` & `hazard_map-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2523 2024-05-02 10:55:17.115293 hazard_map-0.2.1/hazard_map/__init__.py
--rw-r--r--   0        0        0    16039 2024-05-02 10:55:17.115293 hazard_map-0.2.1/hazard_map/hazard_map.py
--rw-r--r--   0        0        0      835 2024-05-02 10:55:17.115293 hazard_map-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2798 2024-05-02 10:55:17.116293 hazard_map-0.2.1/readme.md
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hazard_map-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3889 2024-05-22 11:59:47.602604 hazard_map-0.3.0/hazard_map/__init__.py
+-rw-r--r--   0        0        0    25295 2024-05-22 11:59:47.602604 hazard_map-0.3.0/hazard_map/hazard_map.py
+-rw-r--r--   0        0        0      835 2024-05-22 11:59:47.603604 hazard_map-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2798 2024-05-22 11:59:47.603604 hazard_map-0.3.0/readme.md
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hazard_map-0.3.0/PKG-INFO
```

### Comparing `hazard_map-0.2.1/hazard_map/__init__.py` & `hazard_map-0.3.0/hazard_map/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,65 @@
 import argparse
 import os
 
 from termcolor import colored
 
 
 def main():
-    from hazard_map.hazard_map import HazardMap, Sheet
+    from hazard_map.hazard_map import HazardMap, Kind, ListSheet, MappingSheet
 
     arguments = parse_arguments()
 
     print(f"Welcome to {colored('hazard-map', 'yellow')}!")
 
     print()
 
     print('The outputs of this script will be saved in the following directory:')
     print(f"\"{colored(arguments.output_directory, 'cyan')}\"")
 
     print()
 
     hazard_log = HazardMap(arguments.input_workbook)
 
+    hazard_log.read_lists(
+        {
+            Kind.HAZARD: ListSheet(
+                'HazardsREVISED',
+                'Revised_Hazard_ID',
+                'Hazard_Name',
+                'Description',
+                ['Category', 'Sub Category'],
+                None,
+                None,
+            ),
+            Kind.CAUSE: ListSheet(
+                'CausesREVISED',
+                'Revised_Cause_ID',
+                'Cause_Name',
+                'Description',
+                ['Category', 'Sub Category'],
+                None,
+                None,
+            ),
+            Kind.CONTROL: ListSheet(
+                'ControlsREVISED',
+                'Revised_Control_ID',
+                'Control_Name',
+                'Control Description',
+                ['Category', 'Sub Category'],
+                'Default Control Strength',
+                'Control Type',
+            ),
+        }
+    )
+
     hazard_log.extract_sheet_mappings(
         [
-            Sheet('HazardCause Mapping', (0, 0), (1, 1), (2, 2), False),
-            Sheet('CauseControl Mapping', (0, 0), (1, 1), (2, 2), False),
+            MappingSheet('HazardCause Mapping', (0, 0), (1, 1), (2, 2), False),
+            MappingSheet('CauseControl Mapping', (0, 0), (1, 1), (2, 2), False),
         ],
         arguments.mapping_regex,
     )
     print(
         'Mappings were successfully extracted from the workbook '
         f"\"{colored(os.path.basename(arguments.input_workbook), 'cyan')}\"!"
     )
@@ -36,24 +68,33 @@
 
     print(hazard_log.report_kind_counts())
     disconnected_report = hazard_log.report_disconnected_nodes()
     if disconnected_report:
         print()
         print(disconnected_report)
 
+    control_relevance_report = hazard_log.review_relevance(
+        Kind.CONTROL, arguments.relevance_report_lines
+    )
+    if control_relevance_report:
+        print()
+        print(control_relevance_report)
+
     print()
 
     hazard_log.write_to_file(
         arguments.output_directory,
         arguments.output_json,
     )
 
     hazard_log.draw_graph()
     hazard_log.save_drawing(arguments.output_directory, arguments.plot_dpi)
 
+    print()
+
 
 def parse_arguments():
     """Uses the argparse library to create a command-line interface for the script."""
     parser = argparse.ArgumentParser(
         prog='hazard-map',
         description='Build and analyze a network model of hazards, causes, and controls',
     )
@@ -85,14 +126,22 @@
         '--mapping-regex',
         help='Set a custom regex for identifying mapping pairs',
         default='',
         type=str,
     )
 
     parser.add_argument(
+        '-r',
+        '--relevance-report-lines',
+        help='Choose the number of lines in the relevance reports',
+        default=10,
+        type=int,
+    )
+
+    parser.add_argument(
         '-d',
         '--plot-dpi',
         help='Set a custom DPI (quality) for the plot output',
         default=None,
         type=int,
     )
```

### Comparing `hazard_map-0.2.1/pyproject.toml` & `hazard_map-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hazard-map"
-version = "0.2.1"
+version = "0.3.0"
 description = "Build and analyze a network model of hazards, causes, and controls"
 authors = ["Thom Cameron <thomcm@proton.me>"]
 readme = "readme.md"
 license = "license.txt"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `hazard_map-0.2.1/readme.md` & `hazard_map-0.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `hazard_map-0.2.1/PKG-INFO` & `hazard_map-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazard-map
-Version: 0.2.1
+Version: 0.3.0
 Summary: Build and analyze a network model of hazards, causes, and controls
 License: license.txt
 Author: Thom Cameron
 Author-email: thomcm@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

