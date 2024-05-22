# Comparing `tmp/dwd_global_radiation-1.0.0rc5.tar.gz` & `tmp/dwd_global_radiation-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.0.0rc5.tar", last modified: Tue May 21 11:01:52 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.0.0rc6.tar", last modified: Wed May 22 14:32:56 2024, max compression
```

## Comparing `dwd_global_radiation-1.0.0rc5.tar` & `dwd_global_radiation-1.0.0rc6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-21 11:01:52.151512 dwd_global_radiation-1.0.0rc5/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc5/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-21 11:01:52.151512 dwd_global_radiation-1.0.0rc5/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc5/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-21 11:01:52.147512 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    23928 2024-05-17 10:30:25.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-21 11:01:52.147512 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-21 11:01:52.151512 dwd_global_radiation-1.0.0rc5/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc5/setup.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc6/LICENSE
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc6/README.md
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-22 14:32:56.431814 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/__init__.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    24231 2024-05-22 14:22:24.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/utils.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/setup.cfg
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-22 14:23:30.000000 dwd_global_radiation-1.0.0rc6/setup.py
```

### Comparing `dwd_global_radiation-1.0.0rc5/LICENSE` & `dwd_global_radiation-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc5/PKG-INFO` & `dwd_global_radiation-1.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.0.0rc5/README.md` & `dwd_global_radiation-1.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc5/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.0.0rc6/dwd_global_radiation/global_radiation.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,21 @@
         # Check for unique location name
         if any(loc.name == name for loc in self.locations):
             raise ValueError(f"A location with the name '{name}' already exists.")
 
         # If all checks pass, create and add the new location
         location = Location(latitude, longitude, name)
         self.locations.append(location)
+    def remove_location(self, name):
+        """Removes a location by its name."""
+        for i, location in enumerate(self.locations):
+            if location.name == name:
+                del self.locations[i]
+                return
+        raise ValueError(f"Location with name '{name}' not found")
 
     def _get_grid_data(self, all_grid_global_rad_data):
 
         ndlats = all_grid_global_rad_data.variables["lat"][:].filled()
         ndlons = all_grid_global_rad_data.variables["lon"][:].filled()
         long_grid, lat_grid = np.meshgrid(ndlons, ndlats)
         coordinates = np.dstack((lat_grid, long_grid)).reshape(-1, 2)
```

### Comparing `dwd_global_radiation-1.0.0rc5/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.0.0rc6/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.0.0rc5/setup.py` & `dwd_global_radiation-1.0.0rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.0.0rc5',
+    version='1.0.0rc6',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
```

