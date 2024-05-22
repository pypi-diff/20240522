# Comparing `tmp/landusemix-0.0.3.tar.gz` & `tmp/landusemix-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landusemix-0.0.3.tar", last modified: Sat May 18 00:30:01 2024, max compression
+gzip compressed data, was "landusemix-0.0.4.tar", last modified: Wed May 22 01:52:39 2024, max compression
```

## Comparing `landusemix-0.0.3.tar` & `landusemix-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 00:29:54.000000 landusemix-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-18 00:30:01.245154 landusemix-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-18 00:29:54.000000 landusemix-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/landusemix/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-18 00:29:54.000000 landusemix-0.0.3/landusemix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 00:29:54.000000 landusemix-0.0.3/landusemix/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-18 00:29:54.000000 landusemix-0.0.3/landusemix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/landusemix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:30:01.245154 landusemix-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-18 00:29:54.000000 landusemix-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 00:29:54.000000 landusemix-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-18 00:29:54.000000 landusemix-0.0.3/tests/test_landusemix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 01:52:36.000000 landusemix-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 01:52:39.173718 landusemix-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 01:52:36.000000 landusemix-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/landusemix/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 01:52:36.000000 landusemix-0.0.4/landusemix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 01:52:36.000000 landusemix-0.0.4/landusemix/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 01:52:36.000000 landusemix-0.0.4/landusemix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/landusemix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 01:52:39.000000 landusemix-0.0.4/landusemix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:52:39.173718 landusemix-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 01:52:36.000000 landusemix-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:39.173718 landusemix-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:52:36.000000 landusemix-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 01:52:36.000000 landusemix-0.0.4/tests/test_landusemix.py
```

### Comparing `landusemix-0.0.3/LICENSE` & `landusemix-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.3/PKG-INFO` & `landusemix-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: geopandas
-Requires-Dist: shapely
-Requires-Dist: folium
 
 
 # Land Use Mix Python Package
 
 ## Overview
 
 The `landusemix` package provides tools for calculating land use mix indices. These indices can be used to measure the diversity and concentration of land use areas, which is valuable for GIS researchers and urban planners.
@@ -70,14 +68,59 @@
 print(f"Entropy Index: {entropy}")
 
 # Calculate the Herfindahl-Hirschman Index (HHI)
 hhi = mix_indices.herfindahl_hirschman_index()
 print(f"Herfindahl-Hirschman Index: {hhi}")
 ```
 
+You can also load data from various formats including GeoJSON, Shapefile, and CSV.
+
+#### Example: Loading GeoJSON Data
+
+```python
+geojson_data = load_geojson('path_to_your_file.geojson')
+```
+
+#### Example: Loading Shapefile Data
+
+```python
+shapefile_data = load_shapefile('path_to_your_file.shp')
+```
+
+#### Example: Loading CSV Data
+
+```python
+csv_data = load_csv('path_to_your_file.csv')
+```
+
+### Using Sample Data
+
+The package includes sample data files for testing and demonstration purposes.
+
+#### Example: Loading Sample GeoJSON Data
+
+```python
+sample_geojson = load_sample_geojson()
+print(sample_geojson)
+```
+
+#### Example: Loading Sample Shapefile Data
+
+```python
+sample_shapefile = load_sample_shapefile()
+print(sample_shapefile)
+```
+
+#### Example: Loading Sample CSV Data
+
+```python
+sample_csv = load_sample_csv()
+print(sample_csv)
+```
+
 ## Indices Description
 
 - **Entropy Index**: 
 
 The entropy index (ENT) is a measure of diversity in land use types within a given area. It is calculated using the following formula:
 
 $$ \mathrm{ENT}=-\frac{\left[\sum_{i=1}^k P^i \ln \left(P^i\right)\right]}{\ln (k)} $$
```

### Comparing `landusemix-0.0.3/landusemix/utils.py` & `landusemix-0.0.4/landusemix/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 
 import json
 import pandas as pd
 import geopandas as gpd
 import os
 
+
 def read_json(filepath):
     """Read a JSON file and return a Python dictionary."""
     with open(filepath, 'r') as f:
         data = json.load(f)
     return data
 
+
 def convert_dataframe_to_dict(dataframe):
     """Convert a DataFrame to a Python dictionary."""
     return dataframe.to_dict()
 
+
 def load_geojson(filepath):
     """Load a GeoJSON file into a GeoDataFrame."""
     return gpd.read_file(filepath)
 
+
 def load_shapefile(filepath):
     """Load a Shapefile into a GeoDataFrame."""
     return gpd.read_file(filepath)
 
+
 def load_csv(filepath):
     """Load a CSV file into a DataFrame."""
     return pd.read_csv(filepath)
 
+
 def load_sample_geojson():
     """Load the included sample GeoJSON file."""
-    sample_path = os.path.join(os.path.dirname(__file__), 'data', 'sample.geojson')
+    sample_path = os.path.join(os.path.dirname(
+        __file__), 'data', 'geojson', 'multiple.geojson')
     return load_geojson(sample_path)
 
+
 def load_sample_shapefile():
     """Load the included sample Shapefile."""
-    sample_path = os.path.join(os.path.dirname(__file__), 'data', 'sample.shp')
+    sample_path = os.path.join(os.path.dirname(
+        __file__), 'data', 'shapefiles', 'multiple', 'multiple.shp')
     return load_shapefile(sample_path)
 
+
 def load_sample_csv():
     """Load the included sample CSV file."""
     sample_path = os.path.join(os.path.dirname(__file__), 'data', 'sample.csv')
     return load_csv(sample_path)
```

### Comparing `landusemix-0.0.3/landusemix.egg-info/PKG-INFO` & `landusemix-0.0.4/landusemix.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: geopandas
-Requires-Dist: shapely
-Requires-Dist: folium
 
 
 # Land Use Mix Python Package
 
 ## Overview
 
 The `landusemix` package provides tools for calculating land use mix indices. These indices can be used to measure the diversity and concentration of land use areas, which is valuable for GIS researchers and urban planners.
@@ -70,14 +68,59 @@
 print(f"Entropy Index: {entropy}")
 
 # Calculate the Herfindahl-Hirschman Index (HHI)
 hhi = mix_indices.herfindahl_hirschman_index()
 print(f"Herfindahl-Hirschman Index: {hhi}")
 ```
 
+You can also load data from various formats including GeoJSON, Shapefile, and CSV.
+
+#### Example: Loading GeoJSON Data
+
+```python
+geojson_data = load_geojson('path_to_your_file.geojson')
+```
+
+#### Example: Loading Shapefile Data
+
+```python
+shapefile_data = load_shapefile('path_to_your_file.shp')
+```
+
+#### Example: Loading CSV Data
+
+```python
+csv_data = load_csv('path_to_your_file.csv')
+```
+
+### Using Sample Data
+
+The package includes sample data files for testing and demonstration purposes.
+
+#### Example: Loading Sample GeoJSON Data
+
+```python
+sample_geojson = load_sample_geojson()
+print(sample_geojson)
+```
+
+#### Example: Loading Sample Shapefile Data
+
+```python
+sample_shapefile = load_sample_shapefile()
+print(sample_shapefile)
+```
+
+#### Example: Loading Sample CSV Data
+
+```python
+sample_csv = load_sample_csv()
+print(sample_csv)
+```
+
 ## Indices Description
 
 - **Entropy Index**: 
 
 The entropy index (ENT) is a measure of diversity in land use types within a given area. It is calculated using the following formula:
 
 $$ \mathrm{ENT}=-\frac{\left[\sum_{i=1}^k P^i \ln \left(P^i\right)\right]}{\ln (k)} $$
```

### Comparing `landusemix-0.0.3/setup.py` & `landusemix-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="landusemix",
-    version="0.0.3",
+    version="0.0.4",
     author="Mehmet Ali Akyol",
     author_email="akyol.mehmet@metu.edu.tr",
     description="A package for calculating land use mix indices",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/makyol/landusemix",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pandas',
         'geopandas',
-        'shapely',
-        'folium',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

