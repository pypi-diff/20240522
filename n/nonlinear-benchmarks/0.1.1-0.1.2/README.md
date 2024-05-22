# Comparing `tmp/nonlinear_benchmarks-0.1.1.tar.gz` & `tmp/nonlinear_benchmarks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonlinear_benchmarks-0.1.1.tar", last modified: Tue May 14 14:16:08 2024, max compression
+gzip compressed data, was "nonlinear_benchmarks-0.1.2.tar", last modified: Wed May 22 09:37:36 2024, max compression
```

## Comparing `nonlinear_benchmarks-0.1.1.tar` & `nonlinear_benchmarks-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 14:16:08.002000 nonlinear_benchmarks-0.1.1/
--rw-rw-rw-   0        0        0     1505 2023-10-17 14:32:40.000000 nonlinear_benchmarks-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6483 2024-05-14 14:16:07.953000 nonlinear_benchmarks-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5595 2024-05-14 14:13:43.000000 nonlinear_benchmarks-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 14:16:07.744000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/
--rw-rw-rw-   0        0        0      891 2024-05-01 15:03:51.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/__init__.py
--rw-rw-rw-   0        0        0    12326 2024-05-13 12:24:40.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/benchmarks.py
--rw-rw-rw-   0        0        0     5637 2024-05-13 12:19:25.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/error_metrics.py
--rw-rw-rw-   0        0        0    12335 2024-05-01 15:29:12.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/not_splitted_benchmarks.py
--rw-rw-rw-   0        0        0     9218 2024-05-13 12:24:40.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/utilities.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:16:07.931000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/
--rw-rw-rw-   0        0        0     6483 2024-05-14 14:16:07.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2024-05-14 14:16:07.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 14:16:07.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-05-14 14:16:07.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-14 14:16:07.000000 nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      807 2024-05-14 14:16:08.000000 nonlinear_benchmarks-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-05-14 14:14:13.000000 nonlinear_benchmarks-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:37:36.620449 nonlinear_benchmarks-0.1.2/
+-rw-rw-rw-   0        0        0     1505 2023-10-17 14:32:40.000000 nonlinear_benchmarks-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6789 2024-05-22 09:37:36.619446 nonlinear_benchmarks-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5901 2024-05-22 09:34:09.000000 nonlinear_benchmarks-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 09:37:36.604472 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/
+-rw-rw-rw-   0        0        0      891 2024-05-01 15:03:51.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/__init__.py
+-rw-rw-rw-   0        0        0    13062 2024-05-22 09:13:51.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/benchmarks.py
+-rw-rw-rw-   0        0        0     5637 2024-05-13 12:19:30.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/error_metrics.py
+-rw-rw-rw-   0        0        0    12335 2024-05-01 15:29:12.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/not_splitted_benchmarks.py
+-rw-rw-rw-   0        0        0     9510 2024-05-22 09:21:46.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:37:36.618472 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/
+-rw-rw-rw-   0        0        0     6789 2024-05-22 09:37:36.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-05-22 09:37:36.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:37:36.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-22 09:37:36.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-22 09:37:36.000000 nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      807 2024-05-22 09:37:36.622448 nonlinear_benchmarks-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-05-22 09:36:51.000000 nonlinear_benchmarks-0.1.2/setup.py
```

### Comparing `nonlinear_benchmarks-0.1.1/LICENSE` & `nonlinear_benchmarks-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonlinear_benchmarks-0.1.1/PKG-INFO` & `nonlinear_benchmarks-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonlinear_benchmarks
-Version: 0.1.1
+Version: 0.1.2
 Summary: The official dataload for http://www.nonlinearbenchmark.org/
 Home-page: https://github.com/GerbenBeintema/nonlinear_benchmarks
 Author: Gerben Beintema
 Author-email: g.i.beintema@tue.nl
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/GerbenBeintema/nonlinear_benchmarks/issues
 Classifier: Programming Language :: Python :: 3
@@ -57,15 +57,16 @@
 
 When using the `WienerHammerBenchMark` (or any other benchmark function), you can customize the behavior with the following options:
 
  * `data_file_locations=True` : Returns the raw data file locations.
  * `train_test_split=False` : Retrieves the entire dataset without splitting.
  * `force_download=True` : Forces (re-)downloading of benchmark files.
  * `url=` : Allows manual override of the download link (contact maintainers if the default link is broken).
- * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g., `u.shape = (250,)` becomes `u.shape = (250, 1)`).
+ * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g. `u.shape = (250,)` becomes `u.shape = (250, 1)`).
+ * `always_return_tuples_of_datasets=True`: Even if there is only a single training or test set a list is still returned (i.e. adds `[train] if not isinstance(train,list) else train`)
 
 # Install
 
 ```
 pip install nonlinear-benchmarks
 ```
 
@@ -133,15 +134,15 @@
 multisine_train_val = train_val
 print(test[0].state_initialization_window_length) # = 50 (for all test sets)
 test_multisine, test_arrow_full, test_arrow_no_extrapolation = test
 ```
 
 Submission test RMSE template: [submission_examples/silverbox.py](submission_examples/silverbox.py)
 
-Note that the test arrow full and the test arrow no extrapolation have some overlap.
+Note that the `test_arrow_no_extrapolation` is a subset of the `test_arrow_full`.
 
 # Error Metrics
 
 We also provide error metrics in `nonlinear_benchmarks.error_metrics`.
 
 ```python
 from nonlinear_benchmarks.error_metrics import RMSE, NRMSE, R_squared, MAE, fit_index
@@ -166,7 +167,10 @@
 n = test.state_initialization_window_length
 
 # y_model = your model output using only test.u and test.y[:n]
 
 RMSE_result = RMSE(test.y[n:], y_model[n:]) #skip the first n
 print(RMSE_result) #report this number
 ```
+
+For example see the Silverbox submission template: [submission_examples/silverbox.py](submission_examples/silverbox.py)
+
```

### Comparing `nonlinear_benchmarks-0.1.1/README.md` & `nonlinear_benchmarks-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 When using the `WienerHammerBenchMark` (or any other benchmark function), you can customize the behavior with the following options:
 
  * `data_file_locations=True` : Returns the raw data file locations.
  * `train_test_split=False` : Retrieves the entire dataset without splitting.
  * `force_download=True` : Forces (re-)downloading of benchmark files.
  * `url=` : Allows manual override of the download link (contact maintainers if the default link is broken).
- * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g., `u.shape = (250,)` becomes `u.shape = (250, 1)`).
+ * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g. `u.shape = (250,)` becomes `u.shape = (250, 1)`).
+ * `always_return_tuples_of_datasets=True`: Even if there is only a single training or test set a list is still returned (i.e. adds `[train] if not isinstance(train,list) else train`)
 
 # Install
 
 ```
 pip install nonlinear-benchmarks
 ```
 
@@ -108,15 +109,15 @@
 multisine_train_val = train_val
 print(test[0].state_initialization_window_length) # = 50 (for all test sets)
 test_multisine, test_arrow_full, test_arrow_no_extrapolation = test
 ```
 
 Submission test RMSE template: [submission_examples/silverbox.py](submission_examples/silverbox.py)
 
-Note that the test arrow full and the test arrow no extrapolation have some overlap.
+Note that the `test_arrow_no_extrapolation` is a subset of the `test_arrow_full`.
 
 # Error Metrics
 
 We also provide error metrics in `nonlinear_benchmarks.error_metrics`.
 
 ```python
 from nonlinear_benchmarks.error_metrics import RMSE, NRMSE, R_squared, MAE, fit_index
@@ -141,7 +142,10 @@
 n = test.state_initialization_window_length
 
 # y_model = your model output using only test.u and test.y[:n]
 
 RMSE_result = RMSE(test.y[n:], y_model[n:]) #skip the first n
 print(RMSE_result) #report this number
 ```
+
+For example see the Silverbox submission template: [submission_examples/silverbox.py](submission_examples/silverbox.py)
+
```

### Comparing `nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/__init__.py` & `nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/benchmarks.py` & `nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/benchmarks.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from scipy.io import loadmat
 import tempfile
 import os.path
 from pathlib import Path
 from nonlinear_benchmarks.utilities import *
 import numpy as np
 
-def EMPS(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
+def EMPS(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, \
+         url=None, atleast_2d=False, always_return_tuples_of_datasets=False):
     '''The Electro-Mechanical Positioning System is a standard configuration of a drive system for prismatic joint of robots or machine tools. The main source of nonlinearity is caused by friction effects that are present in the setup. Due to the presence of a pure integrator in the system, the measurements are obtained in a closed-loop setting.
 
     The provided data is described in this link. The provided Electro-Mechanical Positioning System datasets are available for download here. This zip-file contains the system description and available data sets .mat file format.
 
     Please refer to the Electro-Mechanical Positioning System as:
 
     A. Janot, M. Gautier and M. Brunot, Data Set and Reference Models of EMPS, 2019 Workshop on Nonlinear System Identification Benchmarks, Eindhoven, The Netherlands, April 10-12, 2019.
@@ -39,23 +40,27 @@
     datasets = []
     for name, file_name in [('train (DATA_EMPS)','DATA_EMPS.mat'),('test (DATA_EMPS_PULSES)','DATA_EMPS_PULSES.mat')]:
         matfile = loadmat(os.path.join(save_dir,file_name))
         q_cur, q_ref, t, vir = [matfile[a][:,0] for a in ['qm','qg','t','vir']] #qg is reference, either, q_ref is input or vir is input
         out_data = Input_output_data(u=vir, y=q_cur, sampling_time=t[1]-t[0], name=name)
         datasets.append(out_data)
 
+
+
+
     if train_test_split:
         train_val = datasets[0]
         test = datasets[1]
         test.state_initialization_window_length = 20
-        return atleast_2d_fun(train_val, test, apply=atleast_2d)
+        return always_return_tuples_of_datasets_fun(*atleast_2d_fun(train_val, test, apply=atleast_2d), apply=always_return_tuples_of_datasets)
     else:
         return atleast_2d_fun(datasets, apply=atleast_2d)
 
-def CED(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
+def CED(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, \
+        url=None, atleast_2d=False, always_return_tuples_of_datasets=False):
     '''The coupled electric drives consists of two electric motors that drive a pulley using a flexible belt. 
     The pulley is held by a spring, resulting in a lightly damped dynamic mode. The electric drives can
     be individually controlled allowing the tension and the speed of the belt to be simultaneously controlled. 
     The drive control is symmetric around zero, hence both clockwise and counter clockwise movement is possible.
     The focus is only on the speed control system. The angular speed of the pulley is measured as an output with
     a pulse counter and this sensor is insensitive to the sign of the velocity. The available data sets are short,
     which constitute a challenge when performing identification.
@@ -103,15 +108,16 @@
         test[1].name = 'test CED high input amplitude'
         test[0].state_initialization_window_length = 4
         test[1].state_initialization_window_length = 4
         return atleast_2d_fun(train_val, test, apply=atleast_2d)
     else:
         return atleast_2d_fun(datasets, apply=atleast_2d)
 
-def Cascaded_Tanks(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
+def Cascaded_Tanks(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, \
+    atleast_2d=False, always_return_tuples_of_datasets=False):
     #does not work anymore?
     # url = 'https://data.4tu.nl/file/d4810b78-6cdd-48fe-8950-9bd601e5f47f/3b697e42-01a4-4979-a370-813a456c36f5' if url is None else url
     url = 'https://drive.google.com/file/d/1HnQf_gu0g_UlggoBqy2s34l9YJiFdN01/view' if url is None else url
     download_size = 7520592
     save_dir = cashed_download(url, 'Cascaded_Tanks', zip_name='CascadedTanksFiles.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
     save_dir = os.path.join(save_dir,'CascadedTanksFiles')
 
@@ -123,41 +129,44 @@
     uEst, uVal, yEst, yVal, Ts = out['uEst'][:,0],out['uVal'][:,0],out['yEst'][:,0],out['yVal'][:,0],out['Ts'][0,0]
     datasets = [Input_output_data(u=uEst,y=yEst, sampling_time=Ts, name='train Cascaded_Tanks'),\
                 Input_output_data(u=uVal,y=yVal, sampling_time=Ts, name='test Cascaded_Tanks')]
     if train_test_split:
         train_val = datasets[0]
         test = datasets[1]
         test.state_initialization_window_length = 5
-        return atleast_2d_fun(train_val, test, apply=atleast_2d)
+        return always_return_tuples_of_datasets_fun(*atleast_2d_fun(train_val, test, apply=atleast_2d), apply=always_return_tuples_of_datasets)
     else:
         datasets[0].name, datasets[1].name = 'Cascaded_Tanks first dataset', 'Cascaded_Tanks second dataset'
         return atleast_2d_fun(datasets, apply=atleast_2d)
 
-def WienerHammerBenchMark(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
+def WienerHammerBenchMark(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, \
+    atleast_2d=False, always_return_tuples_of_datasets=False):
     url = 'http://www.ee.kth.se/~hjalmars/ifac_tc11_benchmarks/2009_wienerhammerstein/WienerHammerBenchMark.mat' if url is None else url
     download_size=1707601
     save_dir = cashed_download(url,'WienerHammerBenchMark',dir_placement=dir_placement,download_size=download_size,force_download=force_download,zipped=False)
 
     if data_file_locations:
         return os.path.join(save_dir,'WienerHammerBenchMark.mat')
 
     out = loadmat(os.path.join(save_dir,'WienerHammerBenchMark.mat'))
     u,y,fs = out['uBenchMark'][:,0], out['yBenchMark'][:,0], out['fs'][0,0]
     full_data = Input_output_data(u=u,y=y, sampling_time=1/fs, name='WH benchmark full')
     if train_test_split==False:
-        return atleast_2d_fun(full_data, apply=atleast_2d)
+        V = atleast_2d_fun(full_data, apply=atleast_2d)
+        return (V,) if always_return_tuples_of_datasets else V
     
     sys_data = full_data[5200:184000] 
     train, test = sys_data[:100000], sys_data[100000:]
     train.name = 'train WH'
     test.name = 'test WH'
     test.state_initialization_window_length = 50
-    return atleast_2d_fun(train, test, apply=atleast_2d)
+    return always_return_tuples_of_datasets_fun(*atleast_2d_fun(train, test, apply=atleast_2d), apply=always_return_tuples_of_datasets)
 
-def Silverbox(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
+def Silverbox(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, \
+    atleast_2d=False, always_return_tuples_of_datasets=False):
     '''The Silverbox system can be seen as an electronic implementation of the Duffing oscillator. It is build as a 
     2nd order linear time-invariant system with a 3rd degree polynomial static nonlinearity around it in feedback. 
     This type of dynamics are, for instance, often encountered in mechanical systems.
 
     The provided data is part of a previously published ECC paper available online. A technical note describing the 
     Silverbox benchmark can be found here. All the provided data (.mat file format) on the Silverbox system is available
     for download here. This .zip file contains the Silverbox dataset as specified in the benchmark document (V1 is the
@@ -200,11 +209,13 @@
         multisine_train_val.name = 'train SB multisine'
         test_multisine.name = 'test SB multisine'
         for v in [test_multisine, test_arrow_full, test_arrow_no_extrapolation]:
             v.state_initialization_window_length = 50
 
         from collections import namedtuple
         # m = namedtuple('Silverbox_data_splits', ['test_multisine', 'test_arrow_full', 'test_arrow_no_extrapolation'])
+        multisine_train_val = (multisine_train_val,) if always_return_tuples_of_datasets else multisine_train_val
         return atleast_2d_fun(multisine_train_val, (test_multisine, test_arrow_full, test_arrow_no_extrapolation), apply=atleast_2d)
     else:
+        data2 = (data2,) if always_return_tuples_of_datasets else data2
         return atleast_2d_fun(data2, apply=atleast_2d)
```

### Comparing `nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/error_metrics.py` & `nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/error_metrics.py`

 * *Files identical despite different names*

### Comparing `nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/not_splitted_benchmarks.py` & `nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/not_splitted_benchmarks.py`

 * *Files identical despite different names*

### Comparing `nonlinear_benchmarks-0.1.1/nonlinear_benchmarks/utilities.py` & `nonlinear_benchmarks-0.1.2/nonlinear_benchmarks/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,418 +160,436 @@
 000009f0: 7475 726e 2064 6174 610d 0a20 2020 2069  turn data..    i
 00000a00: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
 00000a10: 612c 2049 6e70 7574 5f6f 7574 7075 745f  a, Input_output_
 00000a20: 6461 7461 293a 0d0a 2020 2020 2020 2020  data):..        
 00000a30: 7265 7475 726e 2064 6174 612e 6174 6c65  return data.atle
 00000a40: 6173 745f 3264 2829 0d0a 2020 2020 656c  ast_2d()..    el
 00000a50: 7365 3a0d 0a20 2020 2020 2020 2072 6574  se:..        ret
-00000a60: 7572 6e20 5b61 746c 6561 7374 5f32 645f  urn [atleast_2d_
-00000a70: 6675 6e28 642c 2061 7070 6c79 3d61 7070  fun(d, apply=app
-00000a80: 6c79 2920 666f 7220 6420 696e 2064 6174  ly) for d in dat
-00000a90: 615d 0d0a 0d0a 0d0a 6465 6620 6765 745f  a]......def get_
-00000aa0: 746d 705f 6265 6e63 686d 6172 6b5f 6469  tmp_benchmark_di
-00000ab0: 7265 6374 6f72 7928 293a 0d0a 2020 2020  rectory():..    
-00000ac0: 2727 2741 2075 7469 6c69 7479 2066 756e  '''A utility fun
-00000ad0: 6374 696f 6e20 7768 6963 6820 6765 7473  ction which gets
-00000ae0: 2074 6865 2075 7469 6c69 7479 2064 6972   the utility dir
-00000af0: 6563 746f 7269 6573 2066 6f72 2065 6163  ectories for eac
-00000b00: 6820 4f53 0d0a 0d0a 2020 2020 4974 2063  h OS....    It c
-00000b10: 7265 6174 6573 2061 2077 6f72 6b69 6e67  reates a working
-00000b20: 2064 6972 6563 746f 7279 2063 616c 6c65   directory calle
-00000b30: 6420 6e6f 6e6c 696e 6561 725f 6265 6e63  d nonlinear_benc
-00000b40: 686d 6172 6b73 200d 0a0d 0a20 2020 2020  hmarks ....     
-00000b50: 2020 2069 6e20 4c4f 4341 4c41 5050 4441     in LOCALAPPDA
-00000b60: 5441 2066 6f72 2077 696e 646f 7773 0d0a  TA for windows..
-00000b70: 0d0a 2020 2020 2020 2020 696e 207e 2f2e  ..        in ~/.
-00000b80: 6e6f 6e6c 696e 6561 725f 6265 6e63 686d  nonlinear_benchm
-00000b90: 6172 6b73 2f20 666f 7220 756e 6978 206c  arks/ for unix l
-00000ba0: 696b 650d 0a0d 0a20 2020 2020 2020 2069  ike....        i
-00000bb0: 6e20 7e2f 4c69 6272 6172 792f 4170 706c  n ~/Library/Appl
-00000bc0: 6963 6174 696f 6e20 5375 7070 6f72 742f  ication Support/
-00000bd0: 6e6f 6e6c 696e 6561 725f 6265 6e63 686d  nonlinear_benchm
-00000be0: 6172 6b73 2f20 666f 7220 6461 7277 696e  arks/ for darwin
-00000bf0: 0d0a 0d0a 2020 2020 6974 2063 7265 6174  ....    it creat
-00000c00: 6573 2074 776f 2064 6972 6563 746f 7269  es two directori
-00000c10: 6573 2069 6e73 6964 6520 6f66 2074 6865  es inside of the
-00000c20: 206e 6f6e 6c69 6e65 6172 5f62 656e 6368   nonlinear_bench
-00000c30: 6d61 726b 7320 6469 7265 6374 6f72 790d  marks directory.
-00000c40: 0a0d 0a20 2020 2020 2020 2064 6174 615f  ...        data_
-00000c50: 7365 7473 203a 2063 6163 6865 206c 6f63  sets : cache loc
-00000c60: 6174 696f 6e20 6f66 2074 6865 2064 6f77  ation of the dow
-00000c70: 6e6c 6f61 6465 6420 6461 7461 2073 6574  nloaded data set
-00000c80: 730d 0a0d 0a20 2020 2020 2020 2063 6865  s....        che
-00000c90: 636b 706f 696e 7473 203a 2075 7365 6420  ckpoints : used 
-00000ca0: 6475 7269 6e67 2074 7261 696e 696e 6720  during training 
-00000cb0: 6f66 2074 6f72 6368 206d 6f64 656c 730d  of torch models.
-00000cc0: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
-00000cd0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00000ce0: 2064 6963 7428 6261 7365 3d62 6173 655f   dict(base=base_
-00000cf0: 6469 722c 2064 6174 615f 7365 7473 3d64  dir, data_sets=d
-00000d00: 6174 615f 7365 7473 5f64 6972 2c20 6368  ata_sets_dir, ch
-00000d10: 6563 6b70 6f69 6e74 733d 6368 6563 6b70  eckpoints=checkp
-00000d20: 6f69 6e74 735f 6469 7229 0d0a 2020 2020  oints_dir)..    
-00000d30: 2727 270d 0a0d 0a20 2020 2064 6566 206d  '''....    def m
-00000d40: 6b64 6972 2864 6972 6563 746f 7279 293a  kdir(directory):
-00000d50: 0d0a 2020 2020 2020 2020 6966 206f 732e  ..        if os.
-00000d60: 7061 7468 2e69 7364 6972 2864 6972 6563  path.isdir(direc
-00000d70: 746f 7279 2920 6973 2046 616c 7365 3a0d  tory) is False:.
-00000d80: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-00000d90: 6d6b 6469 7228 6469 7265 6374 6f72 7929  mkdir(directory)
-00000da0: 0d0a 0d0a 2020 2020 6672 6f6d 2073 7973  ....    from sys
-00000db0: 2069 6d70 6f72 7420 706c 6174 666f 726d   import platform
-00000dc0: 0d0a 2020 2020 6966 2070 6c61 7466 6f72  ..    if platfor
-00000dd0: 6d20 3d3d 2022 6461 7277 696e 223a 2023  m == "darwin": #
-00000de0: 6e6f 7420 7465 7374 6564 2062 7574 2068  not tested but h
-00000df0: 6572 6520 6974 2067 6f65 730d 0a20 2020  ere it goes..   
-00000e00: 2020 2020 2062 6173 655f 6469 7220 3d20       base_dir = 
-00000e10: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
-00000e20: 6572 2827 7e2f 4c69 6272 6172 792f 4170  er('~/Library/Ap
-00000e30: 706c 6963 6174 696f 6e20 5375 7070 6f72  plication Suppor
-00000e40: 742f 6e6f 6e6c 696e 6561 725f 6265 6e63  t/nonlinear_benc
-00000e50: 686d 6172 6b73 2f27 290d 0a20 2020 2065  hmarks/')..    e
-00000e60: 6c69 6620 706c 6174 666f 726d 203d 3d20  lif platform == 
-00000e70: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
-00000e80: 2020 6261 7365 5f64 6972 203d 206f 732e    base_dir = os.
-00000e90: 7061 7468 2e6a 6f69 6e28 6f73 2e67 6574  path.join(os.get
-00000ea0: 656e 7628 274c 4f43 414c 4150 5044 4154  env('LOCALAPPDAT
-00000eb0: 4127 292c 276e 6f6e 6c69 6e65 6172 5f62  A'),'nonlinear_b
-00000ec0: 656e 6368 6d61 726b 732f 2729 0d0a 2020  enchmarks/')..  
-00000ed0: 2020 656c 7365 3a20 2375 6e69 7820 6c69    else: #unix li
-00000ee0: 6b65 2c20 6d69 6768 7420 6265 2070 726f  ke, might be pro
-00000ef0: 626c 656d 6174 6963 2066 6f72 2073 6f6d  blematic for som
-00000f00: 6520 7765 6972 6420 6f70 6572 6174 696e  e weird operatin
-00000f10: 6720 7379 7374 656d 732e 0d0a 2020 2020  g systems...    
-00000f20: 2020 2020 6261 7365 5f64 6972 203d 206f      base_dir = o
-00000f30: 732e 7061 7468 2e65 7870 616e 6475 7365  s.path.expanduse
-00000f40: 7228 277e 2f2e 6e6f 6e6c 696e 6561 725f  r('~/.nonlinear_
-00000f50: 6265 6e63 686d 6172 6b73 2f27 2923 5061  benchmarks/')#Pa
-00000f60: 7468 2827 7e2f 2e6e 6f6e 6c69 6e65 6172  th('~/.nonlinear
-00000f70: 5f62 656e 6368 6d61 726b 732f 2729 0d0a  _benchmarks/')..
-00000f80: 2020 2020 6d6b 6469 7228 6261 7365 5f64      mkdir(base_d
-00000f90: 6972 290d 0a20 2020 2072 6574 7572 6e20  ir)..    return 
-00000fa0: 6261 7365 5f64 6972 0d0a 0d0a 6465 6620  base_dir....def 
-00000fb0: 636c 6561 725f 6361 6368 6528 293a 0d0a  clear_cache():..
-00000fc0: 2020 2020 2727 2744 656c 6574 6520 616c      '''Delete al
-00000fd0: 6c20 6361 6368 6564 2064 6f77 6e6c 6f61  l cached downloa
-00000fe0: 6473 2727 270d 0a20 2020 200d 0a20 2020  ds'''..    ..   
-00000ff0: 2074 656d 705f 6469 7220 3d20 6765 745f   temp_dir = get_
-00001000: 746d 705f 6265 6e63 686d 6172 6b5f 6469  tmp_benchmark_di
-00001010: 7265 6374 6f72 7928 290d 0a20 2020 2066  rectory()..    f
-00001020: 6f72 206c 2069 6e20 5b27 454d 5053 272c  or l in ['EMPS',
-00001030: 2743 4544 272c 2746 3136 272c 2757 6965  'CED','F16','Wie
-00001040: 6e48 616d 6d65 7227 2c27 426f 7563 5765  nHammer','BoucWe
-00001050: 6e27 2c27 5061 7257 4846 272c 2757 6965  n','ParWHF','Wie
-00001060: 6e65 7248 616d 6d65 7242 656e 6368 4d61  nerHammerBenchMa
-00001070: 726b 272c 2753 696c 7665 7262 6f78 272c  rk','Silverbox',
-00001080: 2743 6173 6361 6465 645f 5461 6e6b 7327  'Cascaded_Tanks'
-00001090: 5d3a 0d0a 2020 2020 2020 2020 7472 793a  ]:..        try:
-000010a0: 0d0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
-000010b0: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
-000010c0: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
-000010d0: 722c 6c29 290d 0a20 2020 2020 2020 2065  r,l))..        e
-000010e0: 7863 6570 7420 4669 6c65 4e6f 7446 6f75  xcept FileNotFou
-000010f0: 6e64 4572 726f 723a 0d0a 2020 2020 2020  ndError:..      
-00001100: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-00001110: 7472 793a 0d0a 2020 2020 2020 2020 7368  try:..        sh
-00001120: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
-00001130: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
-00001140: 722c 2744 6149 5379 5f64 6174 6127 2929  r,'DaISy_data'))
-00001150: 0d0a 2020 2020 6578 6365 7074 2046 696c  ..    except Fil
-00001160: 654e 6f74 466f 756e 6445 7272 6f72 3a0d  eNotFoundError:.
-00001170: 0a20 2020 2020 2020 2070 6173 730d 0a0d  .        pass...
-00001180: 0a0d 0a63 6c61 7373 204d 7950 726f 6772  ...class MyProgr
-00001190: 6573 7342 6172 2829 3a0d 0a20 2020 2064  essBar():..    d
-000011a0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000011b0: 2c64 6f77 6e6c 6f61 645f 7369 7a65 293a  ,download_size):
-000011c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-000011d0: 6261 7220 3d20 4e6f 6e65 0d0a 2020 2020  bar = None..    
-000011e0: 2020 2020 7365 6c66 2e64 6f77 6e6c 6f61      self.downloa
-000011f0: 645f 7369 7a65 203d 2064 6f77 6e6c 6f61  d_size = downloa
-00001200: 645f 7369 7a65 0d0a 0d0a 2020 2020 6465  d_size....    de
-00001210: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
-00001220: 2062 6c6f 636b 5f6e 756d 2c20 626c 6f63   block_num, bloc
-00001230: 6b5f 7369 7a65 2c20 746f 7461 6c5f 7369  k_size, total_si
-00001240: 7a65 293a 0d0a 2020 2020 2020 2020 746f  ze):..        to
-00001250: 7461 6c5f 7369 7a65 203d 2073 656c 662e  tal_size = self.
-00001260: 646f 776e 6c6f 6164 5f73 697a 650d 0a20  download_size.. 
-00001270: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00001280: 6c66 2e70 6261 723a 0d0a 2020 2020 2020  lf.pbar:..      
-00001290: 2020 2020 2020 7365 6c66 2e70 6261 723d        self.pbar=
-000012a0: 7072 6f67 7265 7373 6261 722e 5072 6f67  progressbar.Prog
-000012b0: 7265 7373 4261 7228 6d61 7876 616c 3d74  ressBar(maxval=t
-000012c0: 6f74 616c 5f73 697a 6529 0d0a 2020 2020  otal_size)..    
-000012d0: 2020 2020 2020 2020 7365 6c66 2e70 6261          self.pba
-000012e0: 722e 7374 6172 7428 290d 0a0d 0a20 2020  r.start()....   
-000012f0: 2020 2020 2064 6f77 6e6c 6f61 6465 6420       downloaded 
-00001300: 3d20 626c 6f63 6b5f 6e75 6d20 2a20 626c  = block_num * bl
-00001310: 6f63 6b5f 7369 7a65 0d0a 2020 2020 2020  ock_size..      
-00001320: 2020 6966 2064 6f77 6e6c 6f61 6465 6420    if downloaded 
-00001330: 3c20 746f 7461 6c5f 7369 7a65 3a0d 0a20  < total_size:.. 
-00001340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001350: 7062 6172 2e75 7064 6174 6528 646f 776e  pbar.update(down
-00001360: 6c6f 6164 6564 290d 0a20 2020 2020 2020  loaded)..       
-00001370: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001380: 2020 2020 7365 6c66 2e70 6261 722e 6669      self.pbar.fi
-00001390: 6e69 7368 2829 0d0a 0d0a 0d0a 6465 6620  nish()......def 
-000013a0: 6361 7368 6564 5f64 6f77 6e6c 6f61 6428  cashed_download(
-000013b0: 7572 6c2c 6e61 6d65 5f64 6972 2c7a 6970  url,name_dir,zip
-000013c0: 5f6e 616d 653d 4e6f 6e65 2c64 6972 5f70  _name=None,dir_p
-000013d0: 6c61 6365 6d65 6e74 3d4e 6f6e 652c 646f  lacement=None,do
-000013e0: 776e 6c6f 6164 5f73 697a 653d 4e6f 6e65  wnload_size=None
-000013f0: 2c66 6f72 6365 5f64 6f77 6e6c 6f61 643d  ,force_download=
-00001400: 4661 6c73 652c 7a69 7070 6564 3d54 7275  False,zipped=Tru
-00001410: 6529 3a0d 0a20 2020 2027 2727 7572 6c20  e):..    '''url 
-00001420: 6973 2074 6865 2066 696c 6520 746f 2062  is the file to b
-00001430: 6520 646f 776e 6c6f 6164 6564 0d0a 2020  e downloaded..  
-00001440: 2020 6e61 6d65 5f64 6972 2069 7320 7468    name_dir is th
-00001450: 6520 6469 7265 6374 6f72 7920 6e61 6d65  e directory name
-00001460: 2077 6865 7265 2074 6865 2066 696c 6520   where the file 
-00001470: 616e 6420 7468 6520 636f 6e74 656e 7473  and the contents
-00001480: 206f 6620 7468 6520 6669 6c65 2077 696c   of the file wil
-00001490: 6c20 6265 2073 6176 6564 0d0a 2020 2020  l be saved..    
-000014a0: 6469 725f 706c 6163 656d 656e 7420 6973  dir_placement is
-000014b0: 2061 6e20 6f70 7469 6f6e 616c 2061 7267   an optional arg
-000014c0: 756d 656e 7420 7468 6174 2067 6976 6573  ument that gives
-000014d0: 2074 6865 206c 6f63 6174 696f 6e20 6f66   the location of
-000014e0: 2074 6865 2064 6f77 6e6c 6f61 6465 6420   the downloaded 
-000014f0: 6669 6c65 200d 0a20 2020 2069 6620 6974  file ..    if it
-00001500: 2069 7320 6e6f 6e65 2069 7420 7769 6c6c   is none it will
-00001510: 2064 6f77 6e6c 6f61 6420 746f 2074 6865   download to the
-00001520: 2074 656d 7020 6469 720d 0a20 2020 2069   temp dir..    i
-00001530: 6620 6469 725f 6e61 6d65 2069 7320 4e6f  f dir_name is No
-00001540: 6e65 2069 7420 7769 6c6c 2062 6520 7361  ne it will be sa
-00001550: 7665 6420 696e 2074 6865 2074 656d 7020  ved in the temp 
-00001560: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
-00001570: 2073 7973 7465 6d27 2727 0d0a 0d0a 2020   system'''....  
-00001580: 2020 2366 696e 6469 6e67 2f6d 616b 696e    #finding/makin
-00001590: 6720 6469 7265 6374 6f72 6965 730d 0a20  g directories.. 
-000015a0: 2020 2069 6620 6469 725f 706c 6163 656d     if dir_placem
-000015b0: 656e 7420 6973 204e 6f6e 653a 0d0a 2020  ent is None:..  
-000015c0: 2020 2020 2020 7020 3d20 6765 745f 746d        p = get_tm
-000015d0: 705f 6265 6e63 686d 6172 6b5f 6469 7265  p_benchmark_dire
-000015e0: 6374 6f72 7928 2920 2375 7365 2074 656d  ctory() #use tem
-000015f0: 7020 6469 720d 0a20 2020 2065 6c73 653a  p dir..    else:
-00001600: 0d0a 2020 2020 2020 2020 7020 3d20 5061  ..        p = Pa
-00001610: 7468 2864 6972 5f70 6c61 6365 6d65 6e74  th(dir_placement
-00001620: 2920 2375 7365 2067 6976 656e 2064 6972  ) #use given dir
-00001630: 0d0a 2020 2020 7361 7665 5f64 6972 203d  ..    save_dir =
-00001640: 206f 732e 7061 7468 2e6a 6f69 6e28 702c   os.path.join(p,
-00001650: 5061 7468 286e 616d 655f 6469 7229 290d  Path(name_dir)).
-00001660: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
-00001670: 6973 6469 7228 7361 7665 5f64 6972 2920  isdir(save_dir) 
-00001680: 6973 2046 616c 7365 3a0d 0a20 2020 2020  is False:..     
-00001690: 2020 206f 732e 6d6b 6469 7228 7361 7665     os.mkdir(save
-000016a0: 5f64 6972 290d 0a20 2020 2066 696c 655f  _dir)..    file_
-000016b0: 6e61 6d65 203d 2075 726c 2e73 706c 6974  name = url.split
-000016c0: 2827 2f27 295b 2d31 5d20 6966 207a 6970  ('/')[-1] if zip
-000016d0: 5f6e 616d 653d 3d4e 6f6e 6520 656c 7365  _name==None else
-000016e0: 207a 6970 5f6e 616d 650d 0a20 2020 2073   zip_name..    s
-000016f0: 6176 655f 6c6f 6320 3d20 6f73 2e70 6174  ave_loc = os.pat
-00001700: 682e 6a6f 696e 2873 6176 655f 6469 722c  h.join(save_dir,
-00001710: 6669 6c65 5f6e 616d 6529 200d 0a0d 0a20  file_name) .... 
-00001720: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
-00001730: 6669 6c65 2873 6176 655f 6c6f 6329 2061  file(save_loc) a
-00001740: 6e64 206e 6f74 2066 6f72 6365 5f64 6f77  nd not force_dow
-00001750: 6e6c 6f61 643a 0d0a 2020 2020 2020 2020  nload:..        
-00001760: 7265 7475 726e 2073 6176 655f 6469 720d  return save_dir.
-00001770: 0a0d 0a20 2020 2069 6620 666f 7263 655f  ...    if force_
-00001780: 646f 776e 6c6f 6164 3a0d 0a20 2020 2020  download:..     
-00001790: 2020 2070 7269 6e74 2866 2728 7265 2d29     print(f'(re-)
-000017a0: 646f 776e 6c6f 6164 696e 6720 6461 7461  downloading data
-000017b0: 7365 7420 6672 6f6d 207b 7572 6c7d 205c  set from {url} \
-000017c0: 6e20 696e 207b 7361 7665 5f6c 6f63 7d27  n in {save_loc}'
-000017d0: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
-000017e0: 2020 2020 2020 7072 696e 7428 6627 6461        print(f'da
-000017f0: 7461 7365 7420 6e6f 7420 666f 756e 6420  taset not found 
-00001800: 646f 776e 6c6f 6164 696e 6720 6672 6f6d  downloading from
-00001810: 207b 7572 6c7d 205c 6e20 696e 207b 7361   {url} \n in {sa
-00001820: 7665 5f6c 6f63 7d27 290d 0a0d 0a20 2020  ve_loc}')....   
-00001830: 2069 6620 2764 7269 7665 2e67 6f6f 676c   if 'drive.googl
-00001840: 6527 2069 6e20 7572 6c3a 0d0a 2020 2020  e' in url:..    
-00001850: 2020 2020 646f 776e 6c6f 6164 5f66 696c      download_fil
-00001860: 655f 6672 6f6d 5f67 6f6f 676c 655f 6472  e_from_google_dr
-00001870: 6976 6528 7572 6c2c 2073 6176 655f 6c6f  ive(url, save_lo
-00001880: 6329 0d0a 2020 2020 656c 7365 3a0d 0a20  c)..    else:.. 
-00001890: 2020 2020 2020 2066 726f 6d20 6874 7470         from http
-000018a0: 2e63 6c69 656e 7420 696d 706f 7274 2049  .client import I
-000018b0: 6e63 6f6d 706c 6574 6552 6561 640d 0a20  ncompleteRead.. 
-000018c0: 2020 2020 2020 2074 7269 6573 203d 2030         tries = 0
-000018d0: 0d0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-000018e0: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
-000018f0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00001900: 2020 2020 2020 2020 2069 6620 646f 776e           if down
-00001910: 6c6f 6164 5f73 697a 6520 6973 204e 6f6e  load_size is Non
-00001920: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001930: 2020 2020 2020 2020 7572 6c6c 6962 2e72          urllib.r
-00001940: 6571 7565 7374 2e75 726c 7265 7472 6965  equest.urlretrie
-00001950: 7665 2875 726c 2c20 7361 7665 5f6c 6f63  ve(url, save_loc
-00001960: 2923 204d 7950 726f 6772 6573 7342 6172  )# MyProgressBar
-00001970: 2829 2069 7320 6120 7374 6561 6d20 736f  () is a steam so
-00001980: 206e 6f20 6c65 6e67 7468 2069 7320 6769   no length is gi
-00001990: 7665 6e0d 0a20 2020 2020 2020 2020 2020  ven..           
-000019a0: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000019d0: 2020 2020 2020 2020 2020 2075 726c 6c69             urlli
-000019e0: 622e 7265 7175 6573 742e 7572 6c72 6574  b.request.urlret
-000019f0: 7269 6576 6528 7572 6c2c 2073 6176 655f  rieve(url, save_
-00001a00: 6c6f 632c 204d 7950 726f 6772 6573 7342  loc, MyProgressB
-00001a10: 6172 2864 6f77 6e6c 6f61 645f 7369 7a65  ar(download_size
-00001a20: 3d69 6e74 2864 6f77 6e6c 6f61 645f 7369  =int(download_si
-00001a30: 7a65 2929 290d 0a20 2020 2020 2020 2020  ze)))..         
-00001a40: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00001a50: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00001a60: 6365 7074 2049 6e63 6f6d 706c 6574 6552  cept IncompleteR
-00001a70: 6561 643a 0d0a 2020 2020 2020 2020 2020  ead:..          
-00001a80: 2020 2020 2020 7472 6965 7320 2b3d 2031        tries += 1
-00001a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001aa0: 2020 7072 696e 7428 2749 6e63 6f6d 706c    print('Incompl
-00001ab0: 6574 6552 6561 6420 646f 776e 6c6f 6164  eteRead download
-00001ac0: 2066 6169 6c65 642c 2072 652d 646f 776e   failed, re-down
-00001ad0: 6c6f 6164 696e 6720 6669 6c65 2729 0d0a  loading file')..
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 646f 776e 6c6f 6164 5f73 697a 6520 3d20  download_size = 
-00001b00: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
-00001b10: 2020 2020 2020 6966 2074 7269 6573 3d3d        if tries==
-00001b20: 353a 0d0a 2020 2020 2020 2020 2020 2020  5:..            
-00001b30: 2020 2020 2020 2020 6173 7365 7274 2046          assert F
-00001b40: 616c 7365 2c20 2744 6f77 6e6c 6f61 6420  alse, 'Download 
-00001b50: 4661 696c 2035 2074 696d 6573 2065 7869  Fail 5 times exi
-00001b60: 7469 6e67 2e27 0d0a 0d0a 0d0a 2020 2020  ting.'......    
-00001b70: 6966 206e 6f74 207a 6970 7065 643a 2072  if not zipped: r
-00001b80: 6574 7572 6e20 7361 7665 5f64 6972 0d0a  eturn save_dir..
-00001b90: 2020 2020 7072 696e 7428 2765 7874 7261      print('extra
-00001ba0: 6374 696e 6720 6669 6c65 2e2e 2e27 290d  cting file...').
-00001bb0: 0a20 2020 2070 7269 6e74 2866 277b 7361  .    print(f'{sa
-00001bc0: 7665 5f6c 6f63 3d7d 2729 0d0a 2020 2020  ve_loc=}')..    
-00001bd0: 656e 6469 6e67 203d 2066 696c 655f 6e61  ending = file_na
-00001be0: 6d65 2e73 706c 6974 2827 2e27 295b 2d31  me.split('.')[-1
-00001bf0: 5d0d 0a20 2020 2069 6620 656e 6469 6e67  ]..    if ending
-00001c00: 3d3d 2767 7a27 3a0d 0a20 2020 2020 2020  =='gz':..       
-00001c10: 2069 6d70 6f72 7420 7368 7574 696c 0d0a   import shutil..
-00001c20: 2020 2020 2020 2020 696d 706f 7274 2067          import g
-00001c30: 7a69 700d 0a20 2020 2020 2020 2077 6974  zip..        wit
-00001c40: 6820 6f70 656e 286f 732e 7061 7468 2e6a  h open(os.path.j
-00001c50: 6f69 6e28 7361 7665 5f64 6972 2c66 696c  oin(save_dir,fil
-00001c60: 655f 6e61 6d65 5b3a 2d33 5d29 2c20 2777  e_name[:-3]), 'w
-00001c70: 6227 2920 6173 2066 5f6f 7574 3a0d 0a20  b') as f_out:.. 
-00001c80: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00001c90: 677a 6970 2e6f 7065 6e28 7361 7665 5f6c  gzip.open(save_l
-00001ca0: 6f63 2c20 2772 6227 2920 6173 2066 5f69  oc, 'rb') as f_i
-00001cb0: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-00001cc0: 2020 2020 7368 7574 696c 2e63 6f70 7966      shutil.copyf
-00001cd0: 696c 656f 626a 2866 5f69 6e2c 2066 5f6f  ileobj(f_in, f_o
-00001ce0: 7574 290d 0a20 2020 2065 6c69 6620 656e  ut)..    elif en
-00001cf0: 6469 6e67 3d3d 277a 6970 273a 0d0a 2020  ding=='zip':..  
-00001d00: 2020 2020 2020 6672 6f6d 207a 6970 6669        from zipfi
-00001d10: 6c65 2069 6d70 6f72 7420 5a69 7046 696c  le import ZipFil
-00001d20: 6520 6173 2046 696c 650d 0a20 2020 2020  e as File..     
-00001d30: 2020 2077 6974 6820 4669 6c65 2873 6176     with File(sav
-00001d40: 655f 6c6f 6329 2061 7320 4f62 6a3a 0d0a  e_loc) as Obj:..
-00001d50: 2020 2020 2020 2020 2020 2020 4f62 6a2e              Obj.
-00001d60: 6578 7472 6163 7461 6c6c 2873 6176 655f  extractall(save_
-00001d70: 6469 7229 0d0a 2020 2020 656c 6966 2065  dir)..    elif e
-00001d80: 6e64 696e 673d 3d27 7261 7227 3a0d 0a20  nding=='rar':.. 
-00001d90: 2020 2020 2020 2066 726f 6d20 7261 7266         from rarf
-00001da0: 696c 6520 696d 706f 7274 2052 6172 4669  ile import RarFi
-00001db0: 6c65 2061 7320 4669 6c65 0d0a 2020 2020  le as File..    
-00001dc0: 2020 2020 7769 7468 2046 696c 6528 7361      with File(sa
-00001dd0: 7665 5f6c 6f63 2920 6173 204f 626a 3a0d  ve_loc) as Obj:.
-00001de0: 0a20 2020 2020 2020 2020 2020 204f 626a  .            Obj
-00001df0: 2e65 7874 7261 6374 616c 6c28 7361 7665  .extractall(save
-00001e00: 5f64 6972 290d 0a20 2020 2065 6c73 653a  _dir)..    else:
-00001e10: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00001e20: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00001e30: 726f 7228 6627 6669 6c65 207b 6669 6c65  ror(f'file {file
-00001e40: 5f6e 616d 657d 2074 7970 6520 6e6f 7420  _name} type not 
-00001e50: 696d 706c 656d 656e 7465 6427 290d 0a20  implemented').. 
-00001e60: 2020 2072 6574 7572 6e20 7361 7665 5f64     return save_d
-00001e70: 6972 0d0a 0d0a 0d0a 6465 6620 646f 776e  ir......def down
-00001e80: 6c6f 6164 5f66 696c 655f 6672 6f6d 5f67  load_file_from_g
-00001e90: 6f6f 676c 655f 6472 6976 6528 7572 6c2c  oogle_drive(url,
-00001ea0: 2064 6573 7469 6e61 7469 6f6e 293a 0d0a   destination):..
-00001eb0: 2020 2020 6964 203d 2075 726c 2e73 706c      id = url.spl
-00001ec0: 6974 2827 2f27 295b 2d32 5d0d 0a20 2020  it('/')[-2]..   
-00001ed0: 2055 524c 203d 2022 6874 7470 733a 2f2f   URL = "https://
-00001ee0: 646f 6373 2e67 6f6f 676c 652e 636f 6d2f  docs.google.com/
-00001ef0: 7563 3f65 7870 6f72 743d 646f 776e 6c6f  uc?export=downlo
-00001f00: 6164 220d 0a0d 0a20 2020 2073 6573 7369  ad"....    sessi
-00001f10: 6f6e 203d 2072 6571 7565 7374 732e 5365  on = requests.Se
-00001f20: 7373 696f 6e28 290d 0a0d 0a20 2020 2072  ssion()....    r
-00001f30: 6573 706f 6e73 6520 3d20 7365 7373 696f  esponse = sessio
-00001f40: 6e2e 6765 7428 5552 4c2c 2070 6172 616d  n.get(URL, param
-00001f50: 7320 3d20 7b20 2769 6427 203a 2069 6420  s = { 'id' : id 
-00001f60: 7d2c 2073 7472 6561 6d20 3d20 5472 7565  }, stream = True
-00001f70: 290d 0a20 2020 2074 6f6b 656e 203d 2067  )..    token = g
-00001f80: 6574 5f63 6f6e 6669 726d 5f74 6f6b 656e  et_confirm_token
-00001f90: 2872 6573 706f 6e73 6529 0d0a 0d0a 2020  (response)....  
-00001fa0: 2020 6966 2074 6f6b 656e 3a0d 0a20 2020    if token:..   
-00001fb0: 2020 2020 2070 6172 616d 7320 3d20 7b20       params = { 
-00001fc0: 2769 6427 203a 2069 642c 2027 636f 6e66  'id' : id, 'conf
-00001fd0: 6972 6d27 203a 2074 6f6b 656e 207d 0d0a  irm' : token }..
-00001fe0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00001ff0: 203d 2073 6573 7369 6f6e 2e67 6574 2855   = session.get(U
-00002000: 524c 2c20 7061 7261 6d73 203d 2070 6172  RL, params = par
-00002010: 616d 732c 2073 7472 6561 6d20 3d20 5472  ams, stream = Tr
-00002020: 7565 290d 0a0d 0a20 2020 2073 6176 655f  ue)....    save_
-00002030: 7265 7370 6f6e 7365 5f63 6f6e 7465 6e74  response_content
-00002040: 2872 6573 706f 6e73 652c 2064 6573 7469  (response, desti
-00002050: 6e61 7469 6f6e 2920 2020 200d 0a0d 0a64  nation)    ....d
-00002060: 6566 2067 6574 5f63 6f6e 6669 726d 5f74  ef get_confirm_t
-00002070: 6f6b 656e 2872 6573 706f 6e73 6529 3a0d  oken(response):.
-00002080: 0a20 2020 2066 6f72 206b 6579 2c20 7661  .    for key, va
-00002090: 6c75 6520 696e 2072 6573 706f 6e73 652e  lue in response.
-000020a0: 636f 6f6b 6965 732e 6974 656d 7328 293a  cookies.items():
-000020b0: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
-000020c0: 2e73 7461 7274 7377 6974 6828 2764 6f77  .startswith('dow
-000020d0: 6e6c 6f61 645f 7761 726e 696e 6727 293a  nload_warning'):
-000020e0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000020f0: 7475 726e 2076 616c 7565 0d0a 0d0a 2020  turn value....  
-00002100: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
-00002110: 0a64 6566 2073 6176 655f 7265 7370 6f6e  .def save_respon
-00002120: 7365 5f63 6f6e 7465 6e74 2872 6573 706f  se_content(respo
-00002130: 6e73 652c 2064 6573 7469 6e61 7469 6f6e  nse, destination
-00002140: 293a 0d0a 2020 2020 4348 554e 4b5f 5349  ):..    CHUNK_SI
-00002150: 5a45 203d 2033 3237 3638 0d0a 0d0a 2020  ZE = 32768....  
-00002160: 2020 7769 7468 206f 7065 6e28 6465 7374    with open(dest
-00002170: 696e 6174 696f 6e2c 2022 7762 2229 2061  ination, "wb") a
-00002180: 7320 663a 0d0a 2020 2020 2020 2020 666f  s f:..        fo
-00002190: 7220 6368 756e 6b20 696e 2072 6573 706f  r chunk in respo
-000021a0: 6e73 652e 6974 6572 5f63 6f6e 7465 6e74  nse.iter_content
-000021b0: 2843 4855 4e4b 5f53 495a 4529 3a0d 0a20  (CHUNK_SIZE):.. 
-000021c0: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
-000021d0: 756e 6b3a 2023 2066 696c 7465 7220 6f75  unk: # filter ou
-000021e0: 7420 6b65 6570 2d61 6c69 7665 206e 6577  t keep-alive new
-000021f0: 2063 6875 6e6b 730d 0a20 2020 2020 2020   chunks..       
-00002200: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00002210: 2863 6875 6e6b 290d 0a0d 0a23 2069 6620  (chunk)....# if 
-00002220: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
-00002230: 6169 6e5f 5f27 3a0d 0a23 2020 2020 2069  ain__':..#     i
-00002240: 6d70 6f72 7420 6e6f 6e6c 696e 6561 725f  mport nonlinear_
-00002250: 6265 6e63 686d 6172 6b73 0d0a 2320 2020  benchmarks..#   
-00002260: 2020 752c 7920 3d20 6e6f 6e6c 696e 6561    u,y = nonlinea
-00002270: 725f 6265 6e63 686d 6172 6b73 2e43 4544  r_benchmarks.CED
-00002280: 2873 706c 6974 5f64 6174 613d 4661 6c73  (split_data=Fals
-00002290: 6529 0d0a 2320 2020 2020 7379 735f 6461  e)..#     sys_da
-000022a0: 7461 2e70 6c6f 7428 7368 6f77 3d54 7275  ta.plot(show=Tru
-000022b0: 6529 0d0a 0d0a 2020 2020 2320 6669 6c65  e)....    # file
-000022c0: 6e61 6d65 203d 2027 2e2f 6669 6c65 2e7a  name = './file.z
-000022d0: 6970 270d 0a20 2020 2023 2075 726c 203d  ip'..    # url =
-000022e0: 2027 6874 7470 3a2f 2f77 7777 2e6e 6f6e   'http://www.non
-000022f0: 6c69 6e65 6172 6265 6e63 686d 6172 6b2e  linearbenchmark.
-00002300: 6f72 672f 4649 4c45 532f 4245 4e43 484d  org/FILES/BENCHM
-00002310: 4152 4b53 2f45 4d50 532f 454d 5053 2e7a  ARKS/EMPS/EMPS.z
-00002320: 6970 270d 0a20 2020 2023 2075 726c 6c69  ip'..    # urlli
-00002330: 622e 7265 7175 6573 742e 7572 6c72 6574  b.request.urlret
-00002340: 7269 6576 6528 7572 6c2c 2066 696c 656e  rieve(url, filen
-00002350: 616d 6529 0d0a 0d0a 2020 2020 2320 7265  ame)....    # re
-00002360: 7370 203d 2075 726c 6c69 622e 7265 7175  sp = urllib.requ
-00002370: 6573 742e 7572 6c6f 7065 6e28 7572 6c29  est.urlopen(url)
-00002380: 0d0a 2020 2020 2320 7265 7370 4874 6d6c  ..    # respHtml
-00002390: 203d 2072 6573 702e 7265 6164 2829 0d0a   = resp.read()..
-000023a0: 2020 2020 2320 6269 6e66 696c 6520 3d20      # binfile = 
-000023b0: 6f70 656e 2866 696c 656e 616d 652c 2022  open(filename, "
-000023c0: 7762 2229 0d0a 2020 2020 2320 6269 6e66  wb")..    # binf
-000023d0: 696c 652e 7772 6974 6528 7265 7370 4874  ile.write(respHt
-000023e0: 6d6c 290d 0a20 2020 2023 2062 696e 6669  ml)..    # binfi
-000023f0: 6c65 2e63 6c6f 7365 2829 0d0a 0d0a 2020  le.close()....  
-00002400: 2020                                       
+00000a60: 7572 6e20 7475 706c 6528 6174 6c65 6173  urn tuple(atleas
+00000a70: 745f 3264 5f66 756e 2864 2c20 6170 706c  t_2d_fun(d, appl
+00000a80: 793d 6170 706c 7929 2066 6f72 2064 2069  y=apply) for d i
+00000a90: 6e20 6461 7461 290d 0a0d 0a0d 0a64 6566  n data)......def
+00000aa0: 2061 6c77 6179 735f 7265 7475 726e 5f74   always_return_t
+00000ab0: 7570 6c65 735f 6f66 5f64 6174 6173 6574  uples_of_dataset
+00000ac0: 735f 6675 6e28 7472 6169 6e2c 2074 6573  s_fun(train, tes
+00000ad0: 742c 2061 7070 6c79 3d46 616c 7365 293a  t, apply=False):
+00000ae0: 0d0a 2020 2020 6966 2061 7070 6c79 3d3d  ..    if apply==
+00000af0: 4661 6c73 653a 0d0a 2020 2020 2020 2020  False:..        
+00000b00: 7265 7475 726e 2074 7261 696e 2c20 7465  return train, te
+00000b10: 7374 0d0a 2020 2020 7472 6169 6e20 3d20  st..    train = 
+00000b20: 2874 7261 696e 2c29 2069 6620 6e6f 7420  (train,) if not 
+00000b30: 6973 696e 7374 616e 6365 2874 7261 696e  isinstance(train
+00000b40: 2c20 286c 6973 742c 7475 706c 6529 2920  , (list,tuple)) 
+00000b50: 656c 7365 2074 7261 696e 0d0a 2020 2020  else train..    
+00000b60: 7465 7374 203d 2028 7465 7374 2c29 2069  test = (test,) i
+00000b70: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00000b80: 2874 6573 742c 2028 6c69 7374 2c74 7570  (test, (list,tup
+00000b90: 6c65 2929 2065 6c73 6520 7465 7374 0d0a  le)) else test..
+00000ba0: 2020 2020 7265 7475 726e 2074 7261 696e      return train
+00000bb0: 2c20 7465 7374 0d0a 0d0a 0d0a 6465 6620  , test......def 
+00000bc0: 6765 745f 746d 705f 6265 6e63 686d 6172  get_tmp_benchmar
+00000bd0: 6b5f 6469 7265 6374 6f72 7928 293a 0d0a  k_directory():..
+00000be0: 2020 2020 2727 2741 2075 7469 6c69 7479      '''A utility
+00000bf0: 2066 756e 6374 696f 6e20 7768 6963 6820   function which 
+00000c00: 6765 7473 2074 6865 2075 7469 6c69 7479  gets the utility
+00000c10: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
+00000c20: 2065 6163 6820 4f53 0d0a 0d0a 2020 2020   each OS....    
+00000c30: 4974 2063 7265 6174 6573 2061 2077 6f72  It creates a wor
+00000c40: 6b69 6e67 2064 6972 6563 746f 7279 2063  king directory c
+00000c50: 616c 6c65 6420 6e6f 6e6c 696e 6561 725f  alled nonlinear_
+00000c60: 6265 6e63 686d 6172 6b73 200d 0a0d 0a20  benchmarks .... 
+00000c70: 2020 2020 2020 2069 6e20 4c4f 4341 4c41         in LOCALA
+00000c80: 5050 4441 5441 2066 6f72 2077 696e 646f  PPDATA for windo
+00000c90: 7773 0d0a 0d0a 2020 2020 2020 2020 696e  ws....        in
+00000ca0: 207e 2f2e 6e6f 6e6c 696e 6561 725f 6265   ~/.nonlinear_be
+00000cb0: 6e63 686d 6172 6b73 2f20 666f 7220 756e  nchmarks/ for un
+00000cc0: 6978 206c 696b 650d 0a0d 0a20 2020 2020  ix like....     
+00000cd0: 2020 2069 6e20 7e2f 4c69 6272 6172 792f     in ~/Library/
+00000ce0: 4170 706c 6963 6174 696f 6e20 5375 7070  Application Supp
+00000cf0: 6f72 742f 6e6f 6e6c 696e 6561 725f 6265  ort/nonlinear_be
+00000d00: 6e63 686d 6172 6b73 2f20 666f 7220 6461  nchmarks/ for da
+00000d10: 7277 696e 0d0a 0d0a 2020 2020 6974 2063  rwin....    it c
+00000d20: 7265 6174 6573 2074 776f 2064 6972 6563  reates two direc
+00000d30: 746f 7269 6573 2069 6e73 6964 6520 6f66  tories inside of
+00000d40: 2074 6865 206e 6f6e 6c69 6e65 6172 5f62   the nonlinear_b
+00000d50: 656e 6368 6d61 726b 7320 6469 7265 6374  enchmarks direct
+00000d60: 6f72 790d 0a0d 0a20 2020 2020 2020 2064  ory....        d
+00000d70: 6174 615f 7365 7473 203a 2063 6163 6865  ata_sets : cache
+00000d80: 206c 6f63 6174 696f 6e20 6f66 2074 6865   location of the
+00000d90: 2064 6f77 6e6c 6f61 6465 6420 6461 7461   downloaded data
+00000da0: 2073 6574 730d 0a0d 0a20 2020 2020 2020   sets....       
+00000db0: 2063 6865 636b 706f 696e 7473 203a 2075   checkpoints : u
+00000dc0: 7365 6420 6475 7269 6e67 2074 7261 696e  sed during train
+00000dd0: 696e 6720 6f66 2074 6f72 6368 206d 6f64  ing of torch mod
+00000de0: 656c 730d 0a0d 0a20 2020 2052 6574 7572  els....    Retur
+00000df0: 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d  ns..    -------.
+00000e00: 0a20 2020 2064 6963 7428 6261 7365 3d62  .    dict(base=b
+00000e10: 6173 655f 6469 722c 2064 6174 615f 7365  ase_dir, data_se
+00000e20: 7473 3d64 6174 615f 7365 7473 5f64 6972  ts=data_sets_dir
+00000e30: 2c20 6368 6563 6b70 6f69 6e74 733d 6368  , checkpoints=ch
+00000e40: 6563 6b70 6f69 6e74 735f 6469 7229 0d0a  eckpoints_dir)..
+00000e50: 2020 2020 2727 270d 0a0d 0a20 2020 2064      '''....    d
+00000e60: 6566 206d 6b64 6972 2864 6972 6563 746f  ef mkdir(directo
+00000e70: 7279 293a 0d0a 2020 2020 2020 2020 6966  ry):..        if
+00000e80: 206f 732e 7061 7468 2e69 7364 6972 2864   os.path.isdir(d
+00000e90: 6972 6563 746f 7279 2920 6973 2046 616c  irectory) is Fal
+00000ea0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000eb0: 206f 732e 6d6b 6469 7228 6469 7265 6374   os.mkdir(direct
+00000ec0: 6f72 7929 0d0a 0d0a 2020 2020 6672 6f6d  ory)....    from
+00000ed0: 2073 7973 2069 6d70 6f72 7420 706c 6174   sys import plat
+00000ee0: 666f 726d 0d0a 2020 2020 6966 2070 6c61  form..    if pla
+00000ef0: 7466 6f72 6d20 3d3d 2022 6461 7277 696e  tform == "darwin
+00000f00: 223a 2023 6e6f 7420 7465 7374 6564 2062  ": #not tested b
+00000f10: 7574 2068 6572 6520 6974 2067 6f65 730d  ut here it goes.
+00000f20: 0a20 2020 2020 2020 2062 6173 655f 6469  .        base_di
+00000f30: 7220 3d20 6f73 2e70 6174 682e 6578 7061  r = os.path.expa
+00000f40: 6e64 7573 6572 2827 7e2f 4c69 6272 6172  nduser('~/Librar
+00000f50: 792f 4170 706c 6963 6174 696f 6e20 5375  y/Application Su
+00000f60: 7070 6f72 742f 6e6f 6e6c 696e 6561 725f  pport/nonlinear_
+00000f70: 6265 6e63 686d 6172 6b73 2f27 290d 0a20  benchmarks/').. 
+00000f80: 2020 2065 6c69 6620 706c 6174 666f 726d     elif platform
+00000f90: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
+00000fa0: 2020 2020 2020 6261 7365 5f64 6972 203d        base_dir =
+00000fb0: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+00000fc0: 2e67 6574 656e 7628 274c 4f43 414c 4150  .getenv('LOCALAP
+00000fd0: 5044 4154 4127 292c 276e 6f6e 6c69 6e65  PDATA'),'nonline
+00000fe0: 6172 5f62 656e 6368 6d61 726b 732f 2729  ar_benchmarks/')
+00000ff0: 0d0a 2020 2020 656c 7365 3a20 2375 6e69  ..    else: #uni
+00001000: 7820 6c69 6b65 2c20 6d69 6768 7420 6265  x like, might be
+00001010: 2070 726f 626c 656d 6174 6963 2066 6f72   problematic for
+00001020: 2073 6f6d 6520 7765 6972 6420 6f70 6572   some weird oper
+00001030: 6174 696e 6720 7379 7374 656d 732e 0d0a  ating systems...
+00001040: 2020 2020 2020 2020 6261 7365 5f64 6972          base_dir
+00001050: 203d 206f 732e 7061 7468 2e65 7870 616e   = os.path.expan
+00001060: 6475 7365 7228 277e 2f2e 6e6f 6e6c 696e  duser('~/.nonlin
+00001070: 6561 725f 6265 6e63 686d 6172 6b73 2f27  ear_benchmarks/'
+00001080: 2923 5061 7468 2827 7e2f 2e6e 6f6e 6c69  )#Path('~/.nonli
+00001090: 6e65 6172 5f62 656e 6368 6d61 726b 732f  near_benchmarks/
+000010a0: 2729 0d0a 2020 2020 6d6b 6469 7228 6261  ')..    mkdir(ba
+000010b0: 7365 5f64 6972 290d 0a20 2020 2072 6574  se_dir)..    ret
+000010c0: 7572 6e20 6261 7365 5f64 6972 0d0a 0d0a  urn base_dir....
+000010d0: 6465 6620 636c 6561 725f 6361 6368 6528  def clear_cache(
+000010e0: 293a 0d0a 2020 2020 2727 2744 656c 6574  ):..    '''Delet
+000010f0: 6520 616c 6c20 6361 6368 6564 2064 6f77  e all cached dow
+00001100: 6e6c 6f61 6473 2727 270d 0a20 2020 200d  nloads'''..    .
+00001110: 0a20 2020 2074 656d 705f 6469 7220 3d20  .    temp_dir = 
+00001120: 6765 745f 746d 705f 6265 6e63 686d 6172  get_tmp_benchmar
+00001130: 6b5f 6469 7265 6374 6f72 7928 290d 0a20  k_directory().. 
+00001140: 2020 2066 6f72 206c 2069 6e20 5b27 454d     for l in ['EM
+00001150: 5053 272c 2743 4544 272c 2746 3136 272c  PS','CED','F16',
+00001160: 2757 6965 6e48 616d 6d65 7227 2c27 426f  'WienHammer','Bo
+00001170: 7563 5765 6e27 2c27 5061 7257 4846 272c  ucWen','ParWHF',
+00001180: 2757 6965 6e65 7248 616d 6d65 7242 656e  'WienerHammerBen
+00001190: 6368 4d61 726b 272c 2753 696c 7665 7262  chMark','Silverb
+000011a0: 6f78 272c 2743 6173 6361 6465 645f 5461  ox','Cascaded_Ta
+000011b0: 6e6b 7327 5d3a 0d0a 2020 2020 2020 2020  nks']:..        
+000011c0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000011d0: 2020 7368 7574 696c 2e72 6d74 7265 6528    shutil.rmtree(
+000011e0: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
+000011f0: 705f 6469 722c 6c29 290d 0a20 2020 2020  p_dir,l))..     
+00001200: 2020 2065 7863 6570 7420 4669 6c65 4e6f     except FileNo
+00001210: 7446 6f75 6e64 4572 726f 723a 0d0a 2020  tFoundError:..  
+00001220: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00001230: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00001240: 2020 7368 7574 696c 2e72 6d74 7265 6528    shutil.rmtree(
+00001250: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
+00001260: 705f 6469 722c 2744 6149 5379 5f64 6174  p_dir,'DaISy_dat
+00001270: 6127 2929 0d0a 2020 2020 6578 6365 7074  a'))..    except
+00001280: 2046 696c 654e 6f74 466f 756e 6445 7272   FileNotFoundErr
+00001290: 6f72 3a0d 0a20 2020 2020 2020 2070 6173  or:..        pas
+000012a0: 730d 0a0d 0a0d 0a63 6c61 7373 204d 7950  s......class MyP
+000012b0: 726f 6772 6573 7342 6172 2829 3a0d 0a20  rogressBar():.. 
+000012c0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000012d0: 7365 6c66 2c64 6f77 6e6c 6f61 645f 7369  self,download_si
+000012e0: 7a65 293a 0d0a 2020 2020 2020 2020 7365  ze):..        se
+000012f0: 6c66 2e70 6261 7220 3d20 4e6f 6e65 0d0a  lf.pbar = None..
+00001300: 2020 2020 2020 2020 7365 6c66 2e64 6f77          self.dow
+00001310: 6e6c 6f61 645f 7369 7a65 203d 2064 6f77  nload_size = dow
+00001320: 6e6c 6f61 645f 7369 7a65 0d0a 0d0a 2020  nload_size....  
+00001330: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+00001340: 656c 662c 2062 6c6f 636b 5f6e 756d 2c20  elf, block_num, 
+00001350: 626c 6f63 6b5f 7369 7a65 2c20 746f 7461  block_size, tota
+00001360: 6c5f 7369 7a65 293a 0d0a 2020 2020 2020  l_size):..      
+00001370: 2020 746f 7461 6c5f 7369 7a65 203d 2073    total_size = s
+00001380: 656c 662e 646f 776e 6c6f 6164 5f73 697a  elf.download_siz
+00001390: 650d 0a20 2020 2020 2020 2069 6620 6e6f  e..        if no
+000013a0: 7420 7365 6c66 2e70 6261 723a 0d0a 2020  t self.pbar:..  
+000013b0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000013c0: 6261 723d 7072 6f67 7265 7373 6261 722e  bar=progressbar.
+000013d0: 5072 6f67 7265 7373 4261 7228 6d61 7876  ProgressBar(maxv
+000013e0: 616c 3d74 6f74 616c 5f73 697a 6529 0d0a  al=total_size)..
+000013f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001400: 2e70 6261 722e 7374 6172 7428 290d 0a0d  .pbar.start()...
+00001410: 0a20 2020 2020 2020 2064 6f77 6e6c 6f61  .        downloa
+00001420: 6465 6420 3d20 626c 6f63 6b5f 6e75 6d20  ded = block_num 
+00001430: 2a20 626c 6f63 6b5f 7369 7a65 0d0a 2020  * block_size..  
+00001440: 2020 2020 2020 6966 2064 6f77 6e6c 6f61        if downloa
+00001450: 6465 6420 3c20 746f 7461 6c5f 7369 7a65  ded < total_size
+00001460: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00001470: 656c 662e 7062 6172 2e75 7064 6174 6528  elf.pbar.update(
+00001480: 646f 776e 6c6f 6164 6564 290d 0a20 2020  downloaded)..   
+00001490: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000014a0: 2020 2020 2020 2020 7365 6c66 2e70 6261          self.pba
+000014b0: 722e 6669 6e69 7368 2829 0d0a 0d0a 0d0a  r.finish()......
+000014c0: 6465 6620 6361 7368 6564 5f64 6f77 6e6c  def cashed_downl
+000014d0: 6f61 6428 7572 6c2c 6e61 6d65 5f64 6972  oad(url,name_dir
+000014e0: 2c7a 6970 5f6e 616d 653d 4e6f 6e65 2c64  ,zip_name=None,d
+000014f0: 6972 5f70 6c61 6365 6d65 6e74 3d4e 6f6e  ir_placement=Non
+00001500: 652c 646f 776e 6c6f 6164 5f73 697a 653d  e,download_size=
+00001510: 4e6f 6e65 2c66 6f72 6365 5f64 6f77 6e6c  None,force_downl
+00001520: 6f61 643d 4661 6c73 652c 7a69 7070 6564  oad=False,zipped
+00001530: 3d54 7275 6529 3a0d 0a20 2020 2027 2727  =True):..    '''
+00001540: 7572 6c20 6973 2074 6865 2066 696c 6520  url is the file 
+00001550: 746f 2062 6520 646f 776e 6c6f 6164 6564  to be downloaded
+00001560: 0d0a 2020 2020 6e61 6d65 5f64 6972 2069  ..    name_dir i
+00001570: 7320 7468 6520 6469 7265 6374 6f72 7920  s the directory 
+00001580: 6e61 6d65 2077 6865 7265 2074 6865 2066  name where the f
+00001590: 696c 6520 616e 6420 7468 6520 636f 6e74  ile and the cont
+000015a0: 656e 7473 206f 6620 7468 6520 6669 6c65  ents of the file
+000015b0: 2077 696c 6c20 6265 2073 6176 6564 0d0a   will be saved..
+000015c0: 2020 2020 6469 725f 706c 6163 656d 656e      dir_placemen
+000015d0: 7420 6973 2061 6e20 6f70 7469 6f6e 616c  t is an optional
+000015e0: 2061 7267 756d 656e 7420 7468 6174 2067   argument that g
+000015f0: 6976 6573 2074 6865 206c 6f63 6174 696f  ives the locatio
+00001600: 6e20 6f66 2074 6865 2064 6f77 6e6c 6f61  n of the downloa
+00001610: 6465 6420 6669 6c65 200d 0a20 2020 2069  ded file ..    i
+00001620: 6620 6974 2069 7320 6e6f 6e65 2069 7420  f it is none it 
+00001630: 7769 6c6c 2064 6f77 6e6c 6f61 6420 746f  will download to
+00001640: 2074 6865 2074 656d 7020 6469 720d 0a20   the temp dir.. 
+00001650: 2020 2069 6620 6469 725f 6e61 6d65 2069     if dir_name i
+00001660: 7320 4e6f 6e65 2069 7420 7769 6c6c 2062  s None it will b
+00001670: 6520 7361 7665 6420 696e 2074 6865 2074  e saved in the t
+00001680: 656d 7020 6469 7265 6374 6f72 7920 6f66  emp directory of
+00001690: 2074 6865 2073 7973 7465 6d27 2727 0d0a   the system'''..
+000016a0: 0d0a 2020 2020 2366 696e 6469 6e67 2f6d  ..    #finding/m
+000016b0: 616b 696e 6720 6469 7265 6374 6f72 6965  aking directorie
+000016c0: 730d 0a20 2020 2069 6620 6469 725f 706c  s..    if dir_pl
+000016d0: 6163 656d 656e 7420 6973 204e 6f6e 653a  acement is None:
+000016e0: 0d0a 2020 2020 2020 2020 7020 3d20 6765  ..        p = ge
+000016f0: 745f 746d 705f 6265 6e63 686d 6172 6b5f  t_tmp_benchmark_
+00001700: 6469 7265 6374 6f72 7928 2920 2375 7365  directory() #use
+00001710: 2074 656d 7020 6469 720d 0a20 2020 2065   temp dir..    e
+00001720: 6c73 653a 0d0a 2020 2020 2020 2020 7020  lse:..        p 
+00001730: 3d20 5061 7468 2864 6972 5f70 6c61 6365  = Path(dir_place
+00001740: 6d65 6e74 2920 2375 7365 2067 6976 656e  ment) #use given
+00001750: 2064 6972 0d0a 2020 2020 7361 7665 5f64   dir..    save_d
+00001760: 6972 203d 206f 732e 7061 7468 2e6a 6f69  ir = os.path.joi
+00001770: 6e28 702c 5061 7468 286e 616d 655f 6469  n(p,Path(name_di
+00001780: 7229 290d 0a20 2020 2069 6620 6f73 2e70  r))..    if os.p
+00001790: 6174 682e 6973 6469 7228 7361 7665 5f64  ath.isdir(save_d
+000017a0: 6972 2920 6973 2046 616c 7365 3a0d 0a20  ir) is False:.. 
+000017b0: 2020 2020 2020 206f 732e 6d6b 6469 7228         os.mkdir(
+000017c0: 7361 7665 5f64 6972 290d 0a20 2020 2066  save_dir)..    f
+000017d0: 696c 655f 6e61 6d65 203d 2075 726c 2e73  ile_name = url.s
+000017e0: 706c 6974 2827 2f27 295b 2d31 5d20 6966  plit('/')[-1] if
+000017f0: 207a 6970 5f6e 616d 653d 3d4e 6f6e 6520   zip_name==None 
+00001800: 656c 7365 207a 6970 5f6e 616d 650d 0a20  else zip_name.. 
+00001810: 2020 2073 6176 655f 6c6f 6320 3d20 6f73     save_loc = os
+00001820: 2e70 6174 682e 6a6f 696e 2873 6176 655f  .path.join(save_
+00001830: 6469 722c 6669 6c65 5f6e 616d 6529 200d  dir,file_name) .
+00001840: 0a0d 0a20 2020 2069 6620 6f73 2e70 6174  ...    if os.pat
+00001850: 682e 6973 6669 6c65 2873 6176 655f 6c6f  h.isfile(save_lo
+00001860: 6329 2061 6e64 206e 6f74 2066 6f72 6365  c) and not force
+00001870: 5f64 6f77 6e6c 6f61 643a 0d0a 2020 2020  _download:..    
+00001880: 2020 2020 7265 7475 726e 2073 6176 655f      return save_
+00001890: 6469 720d 0a0d 0a20 2020 2069 6620 666f  dir....    if fo
+000018a0: 7263 655f 646f 776e 6c6f 6164 3a0d 0a20  rce_download:.. 
+000018b0: 2020 2020 2020 2070 7269 6e74 2866 2728         print(f'(
+000018c0: 7265 2d29 646f 776e 6c6f 6164 696e 6720  re-)downloading 
+000018d0: 6461 7461 7365 7420 6672 6f6d 207b 7572  dataset from {ur
+000018e0: 6c7d 205c 6e20 696e 207b 7361 7665 5f6c  l} \n in {save_l
+000018f0: 6f63 7d27 290d 0a20 2020 2065 6c73 653a  oc}')..    else:
+00001900: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00001910: 6627 6461 7461 7365 7420 6e6f 7420 666f  f'dataset not fo
+00001920: 756e 6420 646f 776e 6c6f 6164 696e 6720  und downloading 
+00001930: 6672 6f6d 207b 7572 6c7d 205c 6e20 696e  from {url} \n in
+00001940: 207b 7361 7665 5f6c 6f63 7d27 290d 0a0d   {save_loc}')...
+00001950: 0a20 2020 2069 6620 2764 7269 7665 2e67  .    if 'drive.g
+00001960: 6f6f 676c 6527 2069 6e20 7572 6c3a 0d0a  oogle' in url:..
+00001970: 2020 2020 2020 2020 646f 776e 6c6f 6164          download
+00001980: 5f66 696c 655f 6672 6f6d 5f67 6f6f 676c  _file_from_googl
+00001990: 655f 6472 6976 6528 7572 6c2c 2073 6176  e_drive(url, sav
+000019a0: 655f 6c6f 6329 0d0a 2020 2020 656c 7365  e_loc)..    else
+000019b0: 3a0d 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+000019c0: 6874 7470 2e63 6c69 656e 7420 696d 706f  http.client impo
+000019d0: 7274 2049 6e63 6f6d 706c 6574 6552 6561  rt IncompleteRea
+000019e0: 640d 0a20 2020 2020 2020 2074 7269 6573  d..        tries
+000019f0: 203d 2030 0d0a 2020 2020 2020 2020 7768   = 0..        wh
+00001a00: 696c 6520 5472 7565 3a0d 0a20 2020 2020  ile True:..     
+00001a10: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00001a20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001a30: 646f 776e 6c6f 6164 5f73 697a 6520 6973  download_size is
+00001a40: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00001a50: 2020 2020 2020 2020 2020 2020 7572 6c6c              urll
+00001a60: 6962 2e72 6571 7565 7374 2e75 726c 7265  ib.request.urlre
+00001a70: 7472 6965 7665 2875 726c 2c20 7361 7665  trieve(url, save
+00001a80: 5f6c 6f63 2923 204d 7950 726f 6772 6573  _loc)# MyProgres
+00001a90: 7342 6172 2829 2069 7320 6120 7374 6561  sBar() is a stea
+00001aa0: 6d20 736f 206e 6f20 6c65 6e67 7468 2069  m so no length i
+00001ab0: 7320 6769 7665 6e0d 0a20 2020 2020 2020  s given..       
+00001ac0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00001ad0: 616b 0d0a 2020 2020 2020 2020 2020 2020  ak..            
+00001ae0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00001b00: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
+00001b10: 6c72 6574 7269 6576 6528 7572 6c2c 2073  lretrieve(url, s
+00001b20: 6176 655f 6c6f 632c 204d 7950 726f 6772  ave_loc, MyProgr
+00001b30: 6573 7342 6172 2864 6f77 6e6c 6f61 645f  essBar(download_
+00001b40: 7369 7a65 3d69 6e74 2864 6f77 6e6c 6f61  size=int(downloa
+00001b50: 645f 7369 7a65 2929 290d 0a20 2020 2020  d_size)))..     
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00001b70: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
+00001b80: 2020 6578 6365 7074 2049 6e63 6f6d 706c    except Incompl
+00001b90: 6574 6552 6561 643a 0d0a 2020 2020 2020  eteRead:..      
+00001ba0: 2020 2020 2020 2020 2020 7472 6965 7320            tries 
+00001bb0: 2b3d 2031 0d0a 2020 2020 2020 2020 2020  += 1..          
+00001bc0: 2020 2020 2020 7072 696e 7428 2749 6e63        print('Inc
+00001bd0: 6f6d 706c 6574 6552 6561 6420 646f 776e  ompleteRead down
+00001be0: 6c6f 6164 2066 6169 6c65 642c 2072 652d  load failed, re-
+00001bf0: 646f 776e 6c6f 6164 696e 6720 6669 6c65  downloading file
+00001c00: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00001c10: 2020 2020 646f 776e 6c6f 6164 5f73 697a      download_siz
+00001c20: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
+00001c30: 2020 2020 2020 2020 2020 6966 2074 7269            if tri
+00001c40: 6573 3d3d 353a 0d0a 2020 2020 2020 2020  es==5:..        
+00001c50: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00001c60: 7274 2046 616c 7365 2c20 2744 6f77 6e6c  rt False, 'Downl
+00001c70: 6f61 6420 4661 696c 2035 2074 696d 6573  oad Fail 5 times
+00001c80: 2065 7869 7469 6e67 2e27 0d0a 0d0a 0d0a   exiting.'......
+00001c90: 2020 2020 6966 206e 6f74 207a 6970 7065      if not zippe
+00001ca0: 643a 2072 6574 7572 6e20 7361 7665 5f64  d: return save_d
+00001cb0: 6972 0d0a 2020 2020 7072 696e 7428 2765  ir..    print('e
+00001cc0: 7874 7261 6374 696e 6720 6669 6c65 2e2e  xtracting file..
+00001cd0: 2e27 290d 0a20 2020 2070 7269 6e74 2866  .')..    print(f
+00001ce0: 277b 7361 7665 5f6c 6f63 3d7d 2729 0d0a  '{save_loc=}')..
+00001cf0: 2020 2020 656e 6469 6e67 203d 2066 696c      ending = fil
+00001d00: 655f 6e61 6d65 2e73 706c 6974 2827 2e27  e_name.split('.'
+00001d10: 295b 2d31 5d0d 0a20 2020 2069 6620 656e  )[-1]..    if en
+00001d20: 6469 6e67 3d3d 2767 7a27 3a0d 0a20 2020  ding=='gz':..   
+00001d30: 2020 2020 2069 6d70 6f72 7420 7368 7574       import shut
+00001d40: 696c 0d0a 2020 2020 2020 2020 696d 706f  il..        impo
+00001d50: 7274 2067 7a69 700d 0a20 2020 2020 2020  rt gzip..       
+00001d60: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
+00001d70: 7468 2e6a 6f69 6e28 7361 7665 5f64 6972  th.join(save_dir
+00001d80: 2c66 696c 655f 6e61 6d65 5b3a 2d33 5d29  ,file_name[:-3])
+00001d90: 2c20 2777 6227 2920 6173 2066 5f6f 7574  , 'wb') as f_out
+00001da0: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
+00001db0: 6974 6820 677a 6970 2e6f 7065 6e28 7361  ith gzip.open(sa
+00001dc0: 7665 5f6c 6f63 2c20 2772 6227 2920 6173  ve_loc, 'rb') as
+00001dd0: 2066 5f69 6e3a 0d0a 2020 2020 2020 2020   f_in:..        
+00001de0: 2020 2020 2020 2020 7368 7574 696c 2e63          shutil.c
+00001df0: 6f70 7966 696c 656f 626a 2866 5f69 6e2c  opyfileobj(f_in,
+00001e00: 2066 5f6f 7574 290d 0a20 2020 2065 6c69   f_out)..    eli
+00001e10: 6620 656e 6469 6e67 3d3d 277a 6970 273a  f ending=='zip':
+00001e20: 0d0a 2020 2020 2020 2020 6672 6f6d 207a  ..        from z
+00001e30: 6970 6669 6c65 2069 6d70 6f72 7420 5a69  ipfile import Zi
+00001e40: 7046 696c 6520 6173 2046 696c 650d 0a20  pFile as File.. 
+00001e50: 2020 2020 2020 2077 6974 6820 4669 6c65         with File
+00001e60: 2873 6176 655f 6c6f 6329 2061 7320 4f62  (save_loc) as Ob
+00001e70: 6a3a 0d0a 2020 2020 2020 2020 2020 2020  j:..            
+00001e80: 4f62 6a2e 6578 7472 6163 7461 6c6c 2873  Obj.extractall(s
+00001e90: 6176 655f 6469 7229 0d0a 2020 2020 656c  ave_dir)..    el
+00001ea0: 6966 2065 6e64 696e 673d 3d27 7261 7227  if ending=='rar'
+00001eb0: 3a0d 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+00001ec0: 7261 7266 696c 6520 696d 706f 7274 2052  rarfile import R
+00001ed0: 6172 4669 6c65 2061 7320 4669 6c65 0d0a  arFile as File..
+00001ee0: 2020 2020 2020 2020 7769 7468 2046 696c          with Fil
+00001ef0: 6528 7361 7665 5f6c 6f63 2920 6173 204f  e(save_loc) as O
+00001f00: 626a 3a0d 0a20 2020 2020 2020 2020 2020  bj:..           
+00001f10: 204f 626a 2e65 7874 7261 6374 616c 6c28   Obj.extractall(
+00001f20: 7361 7665 5f64 6972 290d 0a20 2020 2065  save_dir)..    e
+00001f30: 6c73 653a 0d0a 2020 2020 2020 2020 7261  lse:..        ra
+00001f40: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00001f50: 6564 4572 726f 7228 6627 6669 6c65 207b  edError(f'file {
+00001f60: 6669 6c65 5f6e 616d 657d 2074 7970 6520  file_name} type 
+00001f70: 6e6f 7420 696d 706c 656d 656e 7465 6427  not implemented'
+00001f80: 290d 0a20 2020 2072 6574 7572 6e20 7361  )..    return sa
+00001f90: 7665 5f64 6972 0d0a 0d0a 0d0a 6465 6620  ve_dir......def 
+00001fa0: 646f 776e 6c6f 6164 5f66 696c 655f 6672  download_file_fr
+00001fb0: 6f6d 5f67 6f6f 676c 655f 6472 6976 6528  om_google_drive(
+00001fc0: 7572 6c2c 2064 6573 7469 6e61 7469 6f6e  url, destination
+00001fd0: 293a 0d0a 2020 2020 6964 203d 2075 726c  ):..    id = url
+00001fe0: 2e73 706c 6974 2827 2f27 295b 2d32 5d0d  .split('/')[-2].
+00001ff0: 0a20 2020 2055 524c 203d 2022 6874 7470  .    URL = "http
+00002000: 733a 2f2f 646f 6373 2e67 6f6f 676c 652e  s://docs.google.
+00002010: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
+00002020: 776e 6c6f 6164 220d 0a0d 0a20 2020 2073  wnload"....    s
+00002030: 6573 7369 6f6e 203d 2072 6571 7565 7374  ession = request
+00002040: 732e 5365 7373 696f 6e28 290d 0a0d 0a20  s.Session().... 
+00002050: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00002060: 7373 696f 6e2e 6765 7428 5552 4c2c 2070  ssion.get(URL, p
+00002070: 6172 616d 7320 3d20 7b20 2769 6427 203a  arams = { 'id' :
+00002080: 2069 6420 7d2c 2073 7472 6561 6d20 3d20   id }, stream = 
+00002090: 5472 7565 290d 0a20 2020 2074 6f6b 656e  True)..    token
+000020a0: 203d 2067 6574 5f63 6f6e 6669 726d 5f74   = get_confirm_t
+000020b0: 6f6b 656e 2872 6573 706f 6e73 6529 0d0a  oken(response)..
+000020c0: 0d0a 2020 2020 6966 2074 6f6b 656e 3a0d  ..    if token:.
+000020d0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+000020e0: 3d20 7b20 2769 6427 203a 2069 642c 2027  = { 'id' : id, '
+000020f0: 636f 6e66 6972 6d27 203a 2074 6f6b 656e  confirm' : token
+00002100: 207d 0d0a 2020 2020 2020 2020 7265 7370   }..        resp
+00002110: 6f6e 7365 203d 2073 6573 7369 6f6e 2e67  onse = session.g
+00002120: 6574 2855 524c 2c20 7061 7261 6d73 203d  et(URL, params =
+00002130: 2070 6172 616d 732c 2073 7472 6561 6d20   params, stream 
+00002140: 3d20 5472 7565 290d 0a0d 0a20 2020 2073  = True)....    s
+00002150: 6176 655f 7265 7370 6f6e 7365 5f63 6f6e  ave_response_con
+00002160: 7465 6e74 2872 6573 706f 6e73 652c 2064  tent(response, d
+00002170: 6573 7469 6e61 7469 6f6e 2920 2020 200d  estination)    .
+00002180: 0a0d 0a64 6566 2067 6574 5f63 6f6e 6669  ...def get_confi
+00002190: 726d 5f74 6f6b 656e 2872 6573 706f 6e73  rm_token(respons
+000021a0: 6529 3a0d 0a20 2020 2066 6f72 206b 6579  e):..    for key
+000021b0: 2c20 7661 6c75 6520 696e 2072 6573 706f  , value in respo
+000021c0: 6e73 652e 636f 6f6b 6965 732e 6974 656d  nse.cookies.item
+000021d0: 7328 293a 0d0a 2020 2020 2020 2020 6966  s():..        if
+000021e0: 206b 6579 2e73 7461 7274 7377 6974 6828   key.startswith(
+000021f0: 2764 6f77 6e6c 6f61 645f 7761 726e 696e  'download_warnin
+00002200: 6727 293a 0d0a 2020 2020 2020 2020 2020  g'):..          
+00002210: 2020 7265 7475 726e 2076 616c 7565 0d0a    return value..
+00002220: 0d0a 2020 2020 7265 7475 726e 204e 6f6e  ..    return Non
+00002230: 650d 0a0d 0a64 6566 2073 6176 655f 7265  e....def save_re
+00002240: 7370 6f6e 7365 5f63 6f6e 7465 6e74 2872  sponse_content(r
+00002250: 6573 706f 6e73 652c 2064 6573 7469 6e61  esponse, destina
+00002260: 7469 6f6e 293a 0d0a 2020 2020 4348 554e  tion):..    CHUN
+00002270: 4b5f 5349 5a45 203d 2033 3237 3638 0d0a  K_SIZE = 32768..
+00002280: 0d0a 2020 2020 7769 7468 206f 7065 6e28  ..    with open(
+00002290: 6465 7374 696e 6174 696f 6e2c 2022 7762  destination, "wb
+000022a0: 2229 2061 7320 663a 0d0a 2020 2020 2020  ") as f:..      
+000022b0: 2020 666f 7220 6368 756e 6b20 696e 2072    for chunk in r
+000022c0: 6573 706f 6e73 652e 6974 6572 5f63 6f6e  esponse.iter_con
+000022d0: 7465 6e74 2843 4855 4e4b 5f53 495a 4529  tent(CHUNK_SIZE)
+000022e0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+000022f0: 6620 6368 756e 6b3a 2023 2066 696c 7465  f chunk: # filte
+00002300: 7220 6f75 7420 6b65 6570 2d61 6c69 7665  r out keep-alive
+00002310: 206e 6577 2063 6875 6e6b 730d 0a20 2020   new chunks..   
+00002320: 2020 2020 2020 2020 2020 2020 2066 2e77               f.w
+00002330: 7269 7465 2863 6875 6e6b 290d 0a0d 0a23  rite(chunk)....#
+00002340: 2069 6620 5f5f 6e61 6d65 5f5f 203d 3d20   if __name__ == 
+00002350: 275f 5f6d 6169 6e5f 5f27 3a0d 0a23 2020  '__main__':..#  
+00002360: 2020 2069 6d70 6f72 7420 6e6f 6e6c 696e     import nonlin
+00002370: 6561 725f 6265 6e63 686d 6172 6b73 0d0a  ear_benchmarks..
+00002380: 2320 2020 2020 752c 7920 3d20 6e6f 6e6c  #     u,y = nonl
+00002390: 696e 6561 725f 6265 6e63 686d 6172 6b73  inear_benchmarks
+000023a0: 2e43 4544 2873 706c 6974 5f64 6174 613d  .CED(split_data=
+000023b0: 4661 6c73 6529 0d0a 2320 2020 2020 7379  False)..#     sy
+000023c0: 735f 6461 7461 2e70 6c6f 7428 7368 6f77  s_data.plot(show
+000023d0: 3d54 7275 6529 0d0a 0d0a 2020 2020 2320  =True)....    # 
+000023e0: 6669 6c65 6e61 6d65 203d 2027 2e2f 6669  filename = './fi
+000023f0: 6c65 2e7a 6970 270d 0a20 2020 2023 2075  le.zip'..    # u
+00002400: 726c 203d 2027 6874 7470 3a2f 2f77 7777  rl = 'http://www
+00002410: 2e6e 6f6e 6c69 6e65 6172 6265 6e63 686d  .nonlinearbenchm
+00002420: 6172 6b2e 6f72 672f 4649 4c45 532f 4245  ark.org/FILES/BE
+00002430: 4e43 484d 4152 4b53 2f45 4d50 532f 454d  NCHMARKS/EMPS/EM
+00002440: 5053 2e7a 6970 270d 0a20 2020 2023 2075  PS.zip'..    # u
+00002450: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
+00002460: 6c72 6574 7269 6576 6528 7572 6c2c 2066  lretrieve(url, f
+00002470: 696c 656e 616d 6529 0d0a 0d0a 2020 2020  ilename)....    
+00002480: 2320 7265 7370 203d 2075 726c 6c69 622e  # resp = urllib.
+00002490: 7265 7175 6573 742e 7572 6c6f 7065 6e28  request.urlopen(
+000024a0: 7572 6c29 0d0a 2020 2020 2320 7265 7370  url)..    # resp
+000024b0: 4874 6d6c 203d 2072 6573 702e 7265 6164  Html = resp.read
+000024c0: 2829 0d0a 2020 2020 2320 6269 6e66 696c  ()..    # binfil
+000024d0: 6520 3d20 6f70 656e 2866 696c 656e 616d  e = open(filenam
+000024e0: 652c 2022 7762 2229 0d0a 2020 2020 2320  e, "wb")..    # 
+000024f0: 6269 6e66 696c 652e 7772 6974 6528 7265  binfile.write(re
+00002500: 7370 4874 6d6c 290d 0a20 2020 2023 2062  spHtml)..    # b
+00002510: 696e 6669 6c65 2e63 6c6f 7365 2829 0d0a  infile.close()..
+00002520: 0d0a 2020 2020                           ..
```

### Comparing `nonlinear_benchmarks-0.1.1/nonlinear_benchmarks.egg-info/PKG-INFO` & `nonlinear_benchmarks-0.1.2/nonlinear_benchmarks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonlinear_benchmarks
-Version: 0.1.1
+Version: 0.1.2
 Summary: The official dataload for http://www.nonlinearbenchmark.org/
 Home-page: https://github.com/GerbenBeintema/nonlinear_benchmarks
 Author: Gerben Beintema
 Author-email: g.i.beintema@tue.nl
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/GerbenBeintema/nonlinear_benchmarks/issues
 Classifier: Programming Language :: Python :: 3
@@ -57,15 +57,16 @@
 
 When using the `WienerHammerBenchMark` (or any other benchmark function), you can customize the behavior with the following options:
 
  * `data_file_locations=True` : Returns the raw data file locations.
  * `train_test_split=False` : Retrieves the entire dataset without splitting.
  * `force_download=True` : Forces (re-)downloading of benchmark files.
  * `url=` : Allows manual override of the download link (contact maintainers if the default link is broken).
- * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g., `u.shape = (250,)` becomes `u.shape = (250, 1)`).
+ * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g. `u.shape = (250,)` becomes `u.shape = (250, 1)`).
+ * `always_return_tuples_of_datasets=True`: Even if there is only a single training or test set a list is still returned (i.e. adds `[train] if not isinstance(train,list) else train`)
 
 # Install
 
 ```
 pip install nonlinear-benchmarks
 ```
 
@@ -133,15 +134,15 @@
 multisine_train_val = train_val
 print(test[0].state_initialization_window_length) # = 50 (for all test sets)
 test_multisine, test_arrow_full, test_arrow_no_extrapolation = test
 ```
 
 Submission test RMSE template: [submission_examples/silverbox.py](submission_examples/silverbox.py)
 
-Note that the test arrow full and the test arrow no extrapolation have some overlap.
+Note that the `test_arrow_no_extrapolation` is a subset of the `test_arrow_full`.
 
 # Error Metrics
 
 We also provide error metrics in `nonlinear_benchmarks.error_metrics`.
 
 ```python
 from nonlinear_benchmarks.error_metrics import RMSE, NRMSE, R_squared, MAE, fit_index
@@ -166,7 +167,10 @@
 n = test.state_initialization_window_length
 
 # y_model = your model output using only test.u and test.y[:n]
 
 RMSE_result = RMSE(test.y[n:], y_model[n:]) #skip the first n
 print(RMSE_result) #report this number
 ```
+
+For example see the Silverbox submission template: [submission_examples/silverbox.py](submission_examples/silverbox.py)
+
```

### Comparing `nonlinear_benchmarks-0.1.1/setup.cfg` & `nonlinear_benchmarks-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f6e 6c69 6e65 6172 5f62 656e   = nonlinear_ben
 00000020: 6368 6d61 726b 730d 0a76 6572 7369 6f6e  chmarks..version
-00000030: 203d 2030 2e31 2e31 0d0a 6175 7468 6f72   = 0.1.1..author
+00000030: 203d 2030 2e31 2e32 0d0a 6175 7468 6f72   = 0.1.2..author
 00000040: 203d 2047 6572 6265 6e20 4265 696e 7465   = Gerben Beinte
 00000050: 6d61 0d0a 6175 7468 6f72 5f65 6d61 696c  ma..author_email
 00000060: 203d 2067 2e69 2e62 6569 6e74 656d 6140   = g.i.beintema@
 00000070: 7475 652e 6e6c 0d0a 6465 7363 7269 7074  tue.nl..descript
 00000080: 696f 6e20 3d20 5468 6520 6f66 6669 6369  ion = The offici
 00000090: 616c 2064 6174 616c 6f61 6420 666f 7220  al dataload for 
 000000a0: 6874 7470 3a2f 2f77 7777 2e6e 6f6e 6c69  http://www.nonli
```

### Comparing `nonlinear_benchmarks-0.1.1/setup.py` & `nonlinear_benchmarks-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 'scipy',
 'requests',
 'rarfile']
 
 packages = [a for a in find_namespace_packages(where='.') if a[:6]=='nonlinear_benchmarks']
 
 setup(name = 'nonlinear_benchmarks',
-      version = '0.1.1',
+      version = '0.1.2',
       description = 'The official dataload for http://www.nonlinearbenchmark.org/',
       author = 'Gerben Beintema',
       author_email = 'g.i.beintema@tue.nl',
       license = 'BSD 3-Clause License',
       python_requires = '>=3.6',
       packages=packages,
       install_requires = install_requires,
```

