# Comparing `tmp/ElecPhys-0.0.56.tar.gz` & `tmp/elecphys-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElecPhys-0.0.56.tar", last modified: Mon Mar 11 13:30:27 2024, max compression
+gzip compressed data, was "elecphys-0.0.57.tar", last modified: Wed May 22 18:44:09 2024, max compression
```

## Comparing `ElecPhys-0.0.56.tar` & `elecphys-0.0.57.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:30:27.872513 ElecPhys-0.0.56/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:30:27.872513 ElecPhys-0.0.56/ElecPhys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-11 13:30:27.000000 ElecPhys-0.0.56/ElecPhys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-11 13:30:27.000000 ElecPhys-0.0.56/ElecPhys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:30:27.000000 ElecPhys-0.0.56/ElecPhys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-11 13:30:27.000000 ElecPhys-0.0.56/ElecPhys.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-11 13:30:27.000000 ElecPhys-0.0.56/ElecPhys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 13:30:27.000000 ElecPhys-0.0.56/ElecPhys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-11 13:30:27.872513 ElecPhys-0.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:30:27.872513 ElecPhys-0.0.56/elecphys/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/cfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/data_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/fourier_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43548 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:30:27.872513 ElecPhys-0.0.56/elecphys/matlab_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/matlab_scripts/convertRHD2Mat.m
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22133 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/elecphys/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 13:30:27.872513 ElecPhys-0.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-11 13:30:17.000000 ElecPhys-0.0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:44:09.075482 elecphys-0.0.57/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:44:09.075482 elecphys-0.0.57/ElecPhys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-22 18:44:09.000000 elecphys-0.0.57/ElecPhys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-22 18:44:09.000000 elecphys-0.0.57/ElecPhys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:44:09.000000 elecphys-0.0.57/ElecPhys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 18:44:09.000000 elecphys-0.0.57/ElecPhys.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 18:44:09.000000 elecphys-0.0.57/ElecPhys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 18:44:09.000000 elecphys-0.0.57/ElecPhys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 18:43:58.000000 elecphys-0.0.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 18:43:58.000000 elecphys-0.0.57/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-22 18:44:09.075482 elecphys-0.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-22 18:43:58.000000 elecphys-0.0.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:44:09.075482 elecphys-0.0.57/elecphys/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/cfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/data_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/fourier_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43548 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:44:09.075482 elecphys-0.0.57/elecphys/matlab_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/matlab_scripts/convertRHD2Mat.m
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22133 2024-05-22 18:43:58.000000 elecphys-0.0.57/elecphys/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 18:43:58.000000 elecphys-0.0.57/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:44:09.075482 elecphys-0.0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-22 18:43:58.000000 elecphys-0.0.57/setup.py
```

### Comparing `ElecPhys-0.0.56/ElecPhys.egg-info/PKG-INFO` & `elecphys-0.0.57/ElecPhys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElecPhys
-Version: 0.0.56
+Version: 0.0.57
 Summary: Electrophysiology data processing
 Home-page: https://github.com/AminAlam/ElecPhys
 Author: Amin Alam
 License: MIT
 Keywords: EEG,signal-processing,electrophysiology,data-analysis,data-visualization,data-conversion,data-preprocessing,data-loading,rhd,notch-filter,dft,stft,fourier-transform
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ElecPhys Version: 0.0.56 Summary: Electrophysiology
+Metadata-Version: 2.1 Name: ElecPhys Version: 0.0.57 Summary: Electrophysiology
 data processing Home-page: https://github.com/AminAlam/ElecPhys Author: Amin
 Alam License: MIT Keywords: EEG,signal-processing,electrophysiology,data-
 analysis,data-visualization,data-conversion,data-preprocessing,data-
 loading,rhd,notch-filter,dft,stft,fourier-transform Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: mat73 Requires-Dist: matplotlib Requires-Dist: scipy
 Requires-Dist: tqdm Requires-Dist: pandas
```

### Comparing `ElecPhys-0.0.56/ElecPhys.egg-info/SOURCES.txt` & `elecphys-0.0.57/ElecPhys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/LICENSE` & `elecphys-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/PKG-INFO` & `elecphys-0.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElecPhys
-Version: 0.0.56
+Version: 0.0.57
 Summary: Electrophysiology data processing
 Home-page: https://github.com/AminAlam/ElecPhys
 Author: Amin Alam
 License: MIT
 Keywords: EEG,signal-processing,electrophysiology,data-analysis,data-visualization,data-conversion,data-preprocessing,data-loading,rhd,notch-filter,dft,stft,fourier-transform
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ElecPhys Version: 0.0.56 Summary: Electrophysiology
+Metadata-Version: 2.1 Name: ElecPhys Version: 0.0.57 Summary: Electrophysiology
 data processing Home-page: https://github.com/AminAlam/ElecPhys Author: Amin
 Alam License: MIT Keywords: EEG,signal-processing,electrophysiology,data-
 analysis,data-visualization,data-conversion,data-preprocessing,data-
 loading,rhd,notch-filter,dft,stft,fourier-transform Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: mat73 Requires-Dist: matplotlib Requires-Dist: scipy
 Requires-Dist: tqdm Requires-Dist: pandas
```

### Comparing `ElecPhys-0.0.56/README.md` & `elecphys-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/cfc.py` & `elecphys-0.0.57/elecphys/cfc.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/conversion.py` & `elecphys-0.0.57/elecphys/conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,21 @@
     if notch_filter_freq != 0 and notch_filter_freq != 50 and notch_filter_freq != 60:
         raise ValueError(
             'Notch filter frequency must be 0 (no filtering), 50 (Hz), or 60 (Hz)')
 
     mat_file_contents = mat73.loadmat(mat_file)
     data = mat_file_contents['data']
     fs = mat_file_contents['fs']
+    
+    # if fs is not an integer and cannot be converted to integer, raise error
+    if not isinstance(fs, int):
+        try:
+            fs = int(fs)
+        except ValueError:
+            raise ValueError('Sampling frequency must be an integer')
 
     for ch_num in tqdm(range(data.shape[0])):
         ch_name = f'Ch{ch_num+1}'
         if notch_filter_freq == 0:
             data_filtered = data[ch_num, :]
         else:
             data_filtered = preprocessing.apply_notch(
```

### Comparing `ElecPhys-0.0.56/elecphys/data_io.py` & `elecphys-0.0.57/elecphys/data_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
         channels_map: list
             list of channel indices corresponding to the order of channels in data_all
     """
     files_list = os.listdir(npz_folder)
     for file_name in files_list:
         if not file_name.endswith('.npz'):
             files_list.remove(file_name)
+    if len(files_list) == 0:
+        raise ValueError(f'No NPZ files found in {npz_folder}')
     files_list = utils.sort_file_names(files_list)
     all_channels_in_folder = list(range(1, len(files_list) + 1))
     channels_list = utils.convert_string_to_list(channels_list)
     if channels_list is None:
         channels_list = all_channels_in_folder
     ignore_channels = utils.convert_string_to_list(ignore_channels)
     if ignore_channels is None:
```

### Comparing `ElecPhys-0.0.56/elecphys/dimensionality_reduction.py` & `elecphys-0.0.57/elecphys/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/fourier_analysis.py` & `elecphys-0.0.57/elecphys/fourier_analysis.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/handlers.py` & `elecphys-0.0.57/elecphys/handlers.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/main.py` & `elecphys-0.0.57/elecphys/main.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/matlab_scripts/convertRHD2Mat.m` & `elecphys-0.0.57/elecphys/matlab_scripts/convertRHD2Mat.m`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/preprocessing.py` & `elecphys-0.0.57/elecphys/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/utils.py` & `elecphys-0.0.57/elecphys/utils.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/elecphys/visualization.py` & `elecphys-0.0.57/elecphys/visualization.py`

 * *Files identical despite different names*

### Comparing `ElecPhys-0.0.56/setup.py` & `elecphys-0.0.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         with open(readme_path) as r:
             description = "\n" + r.read()
         return description
     return MINIMAL_DESCRIPTION
 
 setup(
     name="ElecPhys",
-    version="0.0.56",
+    version="0.0.57",
     author='Amin Alam',
     description='Electrophysiology data processing',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     install_requires=get_requires(),
     python_requires='>=3.8',
     license='MIT',
```

