# Comparing `tmp/mumaxxr-0.0.8.tar.gz` & `tmp/mumaxxr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mumaxxr-0.0.8.tar", last modified: Tue Mar 12 11:34:15 2024, max compression
+gzip compressed data, was "mumaxxr-0.0.9.tar", last modified: Tue Mar 12 12:26:49 2024, max compression
```

## Comparing `mumaxxr-0.0.8.tar` & `mumaxxr-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 11:34:15.956005 mumaxxr-0.0.8/
--rw-rw-rw-   0        0        0     1091 2024-03-12 10:31:35.000000 mumaxxr-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3731 2024-03-12 11:34:15.954002 mumaxxr-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3186 2024-03-12 11:26:50.000000 mumaxxr-0.0.8/README.rst
--rw-rw-rw-   0        0        0      705 2024-03-12 11:28:02.000000 mumaxxr-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 11:34:15.957005 mumaxxr-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-12 11:34:15.886405 mumaxxr-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-12 11:34:15.916687 mumaxxr-0.0.8/src/mumaxXR/
--rw-rw-rw-   0        0        0    27777 2024-03-12 11:29:49.000000 mumaxxr-0.0.8/src/mumaxXR/OvfEngine.py
--rw-rw-rw-   0        0        0       92 2024-03-12 10:31:35.000000 mumaxxr-0.0.8/src/mumaxXR/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 11:34:15.952697 mumaxxr-0.0.8/src/mumaxxr.egg-info/
--rw-rw-rw-   0        0        0     3731 2024-03-12 11:34:15.000000 mumaxxr-0.0.8/src/mumaxxr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-03-12 11:34:15.000000 mumaxxr-0.0.8/src/mumaxxr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 11:34:15.000000 mumaxxr-0.0.8/src/mumaxxr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-12 11:34:15.000000 mumaxxr-0.0.8/src/mumaxxr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-12 12:26:49.786566 mumaxxr-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-03-12 10:31:35.000000 mumaxxr-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3730 2024-03-12 12:26:49.784561 mumaxxr-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3185 2024-03-12 12:24:17.000000 mumaxxr-0.0.9/README.rst
+-rw-rw-rw-   0        0        0      705 2024-03-12 12:24:30.000000 mumaxxr-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-12 12:26:49.786566 mumaxxr-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-12 12:26:49.717250 mumaxxr-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-12 12:26:49.746162 mumaxxr-0.0.9/src/mumaxXR/
+-rw-rw-rw-   0        0        0    27777 2024-03-12 11:29:49.000000 mumaxxr-0.0.9/src/mumaxXR/OvfEngine.py
+-rw-rw-rw-   0        0        0       92 2024-03-12 10:31:35.000000 mumaxxr-0.0.9/src/mumaxXR/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-12 12:26:49.782564 mumaxxr-0.0.9/src/mumaxxr.egg-info/
+-rw-rw-rw-   0        0        0     3730 2024-03-12 12:26:49.000000 mumaxxr-0.0.9/src/mumaxxr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-03-12 12:26:49.000000 mumaxxr-0.0.9/src/mumaxxr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-12 12:26:49.000000 mumaxxr-0.0.9/src/mumaxxr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-03-12 12:26:49.000000 mumaxxr-0.0.9/src/mumaxxr.egg-info/top_level.txt
```

### Comparing `mumaxxr-0.0.8/LICENSE` & `mumaxxr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mumaxxr-0.0.8/PKG-INFO` & `mumaxxr-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumaxxr
-Version: 0.0.8
+Version: 0.0.9
 Summary: xarray engine to load ovf files from mumax simulations into xarray
 Author-email: Tim Vogel <tim.vogel@physik.uni-kl.de>
 Project-URL: Homepage, https://github.com/timvgl/mumaxXR/
 Project-URL: Issues, https://github.com/timvgl/mumaxXR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,13 +39,13 @@
 
     dataset = xr.open_dataset(example_mumax_output_dir_0, chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_1, path_to_example_mumax_output_dir_2], sweepName='name_of_changed_parameter', sweepParam=[value_0_of_parameter, value_1_of_parameter, value_2_of_parameter])
 
 For ND concatenation pass a list of names to sweepNames and a list of tuples to sweepParams
 
 .. code-block:: python
 
-    dataset = xr.open_dataset(example_mumax_output_dir_1', chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_2, path_to_example_mumax_output_dir_3, path_to_example_mumax_output_dir_4], sweepName=['name_of_changed_parameter_1', 'name_of_changed_parameter_2'], sweepParam=[(value_1_1_of_parameter, value_2_1_of_parameter), (value_1_2_of_parameter, value_2_1_of_parameter), (value_1_1_of_parameter, value_2_2_of_parameter), (value_1_2_of_parameter, value_2_2_of_parameter)])
+    dataset = xr.open_dataset(example_mumax_output_dir_1, chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_2, path_to_example_mumax_output_dir_3, path_to_example_mumax_output_dir_4], sweepName=['name_of_changed_parameter_1', 'name_of_changed_parameter_2'], sweepParam=[(value_1_1_of_parameter, value_2_1_of_parameter), (value_1_2_of_parameter, value_2_1_of_parameter), (value_1_1_of_parameter, value_2_2_of_parameter), (value_1_2_of_parameter, value_2_2_of_parameter)])
 
 If you want the ovf-files to be deleted after reading, set removeOvfFiles=True. This only works, if the ovf-files don't have to be accessed multiple times.
 If you want to use ovf-files periodically, set useEachNthOvfFile=N. N has to be larger than one. Otherwise it is ignored. Using this flag, only each nth ovf file is used for the dataset.
 
-Of course the wavetype option and the mumax directory concatenation can be used simultaniously.
+Of course the wavetype option and the mumax directory concatenation can be used simultaneously.
```

### Comparing `mumaxxr-0.0.8/README.rst` & `mumaxxr-0.0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 
     dataset = xr.open_dataset(example_mumax_output_dir_0, chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_1, path_to_example_mumax_output_dir_2], sweepName='name_of_changed_parameter', sweepParam=[value_0_of_parameter, value_1_of_parameter, value_2_of_parameter])
 
 For ND concatenation pass a list of names to sweepNames and a list of tuples to sweepParams
 
 .. code-block:: python
 
-    dataset = xr.open_dataset(example_mumax_output_dir_1', chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_2, path_to_example_mumax_output_dir_3, path_to_example_mumax_output_dir_4], sweepName=['name_of_changed_parameter_1', 'name_of_changed_parameter_2'], sweepParam=[(value_1_1_of_parameter, value_2_1_of_parameter), (value_1_2_of_parameter, value_2_1_of_parameter), (value_1_1_of_parameter, value_2_2_of_parameter), (value_1_2_of_parameter, value_2_2_of_parameter)])
+    dataset = xr.open_dataset(example_mumax_output_dir_1, chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_2, path_to_example_mumax_output_dir_3, path_to_example_mumax_output_dir_4], sweepName=['name_of_changed_parameter_1', 'name_of_changed_parameter_2'], sweepParam=[(value_1_1_of_parameter, value_2_1_of_parameter), (value_1_2_of_parameter, value_2_1_of_parameter), (value_1_1_of_parameter, value_2_2_of_parameter), (value_1_2_of_parameter, value_2_2_of_parameter)])
 
 If you want the ovf-files to be deleted after reading, set removeOvfFiles=True. This only works, if the ovf-files don't have to be accessed multiple times.
 If you want to use ovf-files periodically, set useEachNthOvfFile=N. N has to be larger than one. Otherwise it is ignored. Using this flag, only each nth ovf file is used for the dataset.
 
-Of course the wavetype option and the mumax directory concatenation can be used simultaniously.
+Of course the wavetype option and the mumax directory concatenation can be used simultaneously.
```

### Comparing `mumaxxr-0.0.8/pyproject.toml` & `mumaxxr-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "numpy>=1.24.4", "xarray>=2023.1.0", "dask>=2023.5.0", "forbiddenfruit>=0.1.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mumaxxr"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Tim Vogel", email="tim.vogel@physik.uni-kl.de" },
 ]
 description = "xarray engine to load ovf files from mumax simulations into xarray"
 readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mumaxxr-0.0.8/src/mumaxXR/OvfEngine.py` & `mumaxxr-0.0.9/src/mumaxXR/OvfEngine.py`

 * *Files identical despite different names*

### Comparing `mumaxxr-0.0.8/src/mumaxxr.egg-info/PKG-INFO` & `mumaxxr-0.0.9/src/mumaxxr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumaxxr
-Version: 0.0.8
+Version: 0.0.9
 Summary: xarray engine to load ovf files from mumax simulations into xarray
 Author-email: Tim Vogel <tim.vogel@physik.uni-kl.de>
 Project-URL: Homepage, https://github.com/timvgl/mumaxXR/
 Project-URL: Issues, https://github.com/timvgl/mumaxXR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,13 +39,13 @@
 
     dataset = xr.open_dataset(example_mumax_output_dir_0, chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_1, path_to_example_mumax_output_dir_2], sweepName='name_of_changed_parameter', sweepParam=[value_0_of_parameter, value_1_of_parameter, value_2_of_parameter])
 
 For ND concatenation pass a list of names to sweepNames and a list of tuples to sweepParams
 
 .. code-block:: python
 
-    dataset = xr.open_dataset(example_mumax_output_dir_1', chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_2, path_to_example_mumax_output_dir_3, path_to_example_mumax_output_dir_4], sweepName=['name_of_changed_parameter_1', 'name_of_changed_parameter_2'], sweepParam=[(value_1_1_of_parameter, value_2_1_of_parameter), (value_1_2_of_parameter, value_2_1_of_parameter), (value_1_1_of_parameter, value_2_2_of_parameter), (value_1_2_of_parameter, value_2_2_of_parameter)])
+    dataset = xr.open_dataset(example_mumax_output_dir_1, chunks='auto', engine=OvfEngine, dirListToConcat=[path_to_example_mumax_output_dir_2, path_to_example_mumax_output_dir_3, path_to_example_mumax_output_dir_4], sweepName=['name_of_changed_parameter_1', 'name_of_changed_parameter_2'], sweepParam=[(value_1_1_of_parameter, value_2_1_of_parameter), (value_1_2_of_parameter, value_2_1_of_parameter), (value_1_1_of_parameter, value_2_2_of_parameter), (value_1_2_of_parameter, value_2_2_of_parameter)])
 
 If you want the ovf-files to be deleted after reading, set removeOvfFiles=True. This only works, if the ovf-files don't have to be accessed multiple times.
 If you want to use ovf-files periodically, set useEachNthOvfFile=N. N has to be larger than one. Otherwise it is ignored. Using this flag, only each nth ovf file is used for the dataset.
 
-Of course the wavetype option and the mumax directory concatenation can be used simultaniously.
+Of course the wavetype option and the mumax directory concatenation can be used simultaneously.
```

