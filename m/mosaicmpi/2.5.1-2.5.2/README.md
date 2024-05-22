# Comparing `tmp/mosaicmpi-2.5.1.tar.gz` & `tmp/mosaicmpi-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicmpi-2.5.1.tar", last modified: Fri May 17 21:42:30 2024, max compression
+gzip compressed data, was "mosaicmpi-2.5.2.tar", last modified: Wed May 22 04:00:13 2024, max compression
```

## Comparing `mosaicmpi-2.5.1.tar` & `mosaicmpi-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 21:42:30.551702 mosaicmpi-2.5.1/
--rw-rw-rw-   0        0        0     1090 2024-05-08 16:00:07.000000 mosaicmpi-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     4572 2024-05-17 21:42:30.551702 mosaicmpi-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3544 2024-05-17 21:19:13.000000 mosaicmpi-2.5.1/README.md
--rw-rw-rw-   0        0        0       86 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/pyproject.toml
--rw-rw-rw-   0        0        0     1002 2024-05-17 21:42:30.552713 mosaicmpi-2.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 21:42:30.504963 mosaicmpi-2.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 21:42:30.528383 mosaicmpi-2.5.1/src/mosaicmpi/
--rw-rw-rw-   0        0        0      550 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/__init__.py
--rw-rw-rw-   0        0        0    17785 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/biomart.py
--rw-rw-rw-   0        0        0    69264 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/cli.py
--rw-rw-rw-   0        0        0    36497 2024-05-15 15:02:29.000000 mosaicmpi-2.5.1/src/mosaicmpi/cnmf.py
--rw-rw-rw-   0        0        0    16074 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/colors.py
--rw-rw-rw-   0        0        0     3126 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/config.py
--rw-rw-rw-   0        0        0    63240 2024-05-17 21:40:12.000000 mosaicmpi-2.5.1/src/mosaicmpi/dataset.py
--rw-rw-rw-   0        0        0     3751 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/gprofiler.py
--rw-rw-rw-   0        0        0    23345 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/integration.py
--rw-rw-rw-   0        0        0     6613 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/nancorrmp.py
--rw-rw-rw-   0        0        0    53535 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/network.py
--rw-rw-rw-   0        0        0     9186 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/orphan.py
--rw-rw-rw-   0        0        0    79357 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/plots.py
--rw-rw-rw-   0        0        0     5798 2024-04-30 19:18:00.000000 mosaicmpi-2.5.1/src/mosaicmpi/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:42:30.550701 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/
--rw-rw-rw-   0        0        0     4572 2024-05-17 21:42:30.000000 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-05-17 21:42:30.000000 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 21:42:30.000000 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-17 21:42:30.000000 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      178 2024-05-17 21:42:30.000000 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 21:42:30.000000 mosaicmpi-2.5.1/src/mosaicmpi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 04:00:13.103981 mosaicmpi-2.5.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-08 16:00:07.000000 mosaicmpi-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0     4572 2024-05-22 04:00:13.103981 mosaicmpi-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3544 2024-05-21 17:53:03.000000 mosaicmpi-2.5.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1002 2024-05-22 04:00:13.104970 mosaicmpi-2.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 04:00:12.973069 mosaicmpi-2.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 04:00:13.081970 mosaicmpi-2.5.2/src/mosaicmpi/
+-rw-rw-rw-   0        0        0      550 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/__init__.py
+-rw-rw-rw-   0        0        0    17785 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/biomart.py
+-rw-rw-rw-   0        0        0    69264 2024-05-21 17:53:06.000000 mosaicmpi-2.5.2/src/mosaicmpi/cli.py
+-rw-rw-rw-   0        0        0    36497 2024-05-15 15:02:29.000000 mosaicmpi-2.5.2/src/mosaicmpi/cnmf.py
+-rw-rw-rw-   0        0        0    16074 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/colors.py
+-rw-rw-rw-   0        0        0     3126 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/config.py
+-rw-rw-rw-   0        0        0    64973 2024-05-21 18:23:56.000000 mosaicmpi-2.5.2/src/mosaicmpi/dataset.py
+-rw-rw-rw-   0        0        0     3751 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/gprofiler.py
+-rw-rw-rw-   0        0        0    23345 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/integration.py
+-rw-rw-rw-   0        0        0     6613 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/nancorrmp.py
+-rw-rw-rw-   0        0        0    53535 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/network.py
+-rw-rw-rw-   0        0        0     9186 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/orphan.py
+-rw-rw-rw-   0        0        0    79357 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/plots.py
+-rw-rw-rw-   0        0        0     5798 2024-04-30 19:18:00.000000 mosaicmpi-2.5.2/src/mosaicmpi/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 04:00:13.102930 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/
+-rw-rw-rw-   0        0        0     4572 2024-05-22 04:00:12.000000 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-05-22 04:00:12.000000 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 04:00:12.000000 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-22 04:00:12.000000 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      178 2024-05-22 04:00:12.000000 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 04:00:12.000000 mosaicmpi-2.5.2/src/mosaicmpi.egg-info/top_level.txt
```

### Comparing `mosaicmpi-2.5.1/LICENSE` & `mosaicmpi-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/PKG-INFO` & `mosaicmpi-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicmpi
-Version: 2.5.1
+Version: 2.5.2
 Summary: mosaicMPI: Mosaic Multi-resolution Program Integration
 Home-page: https://github.com/MorrissyLab/mosaicMPI
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/mosaicMPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 Requires-Dist: fastcluster
 Requires-Dist: tqdm
 
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
 # mosaicMPI: Mosaic Multi-resolution Program Integration
 
-![version badge](https://img.shields.io/badge/version-2.5.1-blue)
+![version badge](https://img.shields.io/badge/version-2.5.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
```

### Comparing `mosaicmpi-2.5.1/README.md` & `mosaicmpi-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
 # mosaicMPI: Mosaic Multi-resolution Program Integration
 
-![version badge](https://img.shields.io/badge/version-2.5.1-blue)
+![version badge](https://img.shields.io/badge/version-2.5.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
```

### Comparing `mosaicmpi-2.5.1/setup.cfg` & `mosaicmpi-2.5.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f73 6169 636d 7069 0d0a 7665   = mosaicmpi..ve
-00000020: 7273 696f 6e20 3d20 322e 352e 310d 0a61  rsion = 2.5.1..a
+00000020: 7273 696f 6e20 3d20 322e 352e 320d 0a61  rsion = 2.5.2..a
 00000030: 7574 686f 7220 3d20 5465 6420 5665 7268  uthor = Ted Verh
 00000040: 6579 0d0a 6175 7468 6f72 5f65 6d61 696c  ey..author_email
 00000050: 203d 2074 6276 6572 6865 7940 7563 616c   = tbverhey@ucal
 00000060: 6761 7279 2e63 610d 0a64 6573 6372 6970  gary.ca..descrip
 00000070: 7469 6f6e 203d 206d 6f73 6169 634d 5049  tion = mosaicMPI
 00000080: 3a20 4d6f 7361 6963 204d 756c 7469 2d72  : Mosaic Multi-r
 00000090: 6573 6f6c 7574 696f 6e20 5072 6f67 7261  esolution Progra
```

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/__init__.py` & `mosaicmpi-2.5.2/src/mosaicmpi/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/biomart.py` & `mosaicmpi-2.5.2/src/mosaicmpi/biomart.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/cli.py` & `mosaicmpi-2.5.2/src/mosaicmpi/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/cnmf.py` & `mosaicmpi-2.5.2/src/mosaicmpi/cnmf.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/colors.py` & `mosaicmpi-2.5.2/src/mosaicmpi/colors.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/config.py` & `mosaicmpi-2.5.2/src/mosaicmpi/config.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/dataset.py` & `mosaicmpi-2.5.2/src/mosaicmpi/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2741,1213 +2741,1321 @@
 0000ab40: 6422 5d5d 2e69 6e64 6578 0d0a 0d0a 2020  d"]].index....  
 0000ab50: 2020 2020 2020 2320 5375 6273 6574 206f        # Subset o
 0000ab60: 7574 2068 6967 682d 7661 7269 616e 6365  ut high-variance
 0000ab70: 2067 656e 6573 0d0a 2020 2020 2020 2020   genes..        
 0000ab80: 6e6f 726d 5f63 6f75 6e74 7320 3d20 7365  norm_counts = se
 0000ab90: 6c66 2e61 6461 7461 5b3a 2c20 6f76 6572  lf.adata[:, over
 0000aba0: 6469 7370 6572 7365 645f 6765 6e65 735d  dispersed_genes]
-0000abb0: 0d0a 2020 2020 2020 2020 2323 2053 6361  ..        ## Sca
-0000abc0: 6c65 2067 656e 6573 2074 6f20 756e 6974  le genes to unit
-0000abd0: 2076 6172 6961 6e63 650d 0a20 2020 2020   variance..     
-0000abe0: 2020 2069 6620 7370 2e69 7373 7061 7273     if sp.isspars
-0000abf0: 6528 7470 6d2e 5829 3a0d 0a20 2020 2020  e(tpm.X):..     
-0000ac00: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-0000ac10: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-0000ac20: 2822 416e 6e44 6174 6173 2077 6974 6820  ("AnnDatas with 
-0000ac30: 7370 6172 7365 206d 6174 7269 6365 7320  sparse matrices 
-0000ac40: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
-0000ac50: 6420 6279 206d 6f73 6169 634d 5049 2079  d by mosaicMPI y
-0000ac60: 6574 2e22 290d 0a20 2020 2020 2020 2020  et.")..         
-0000ac70: 2020 2023 2073 632e 7070 2e73 6361 6c65     # sc.pp.scale
-0000ac80: 286e 6f72 6d5f 636f 756e 7473 2c20 7a65  (norm_counts, ze
-0000ac90: 726f 5f63 656e 7465 723d 4661 6c73 6529  ro_center=False)
-0000aca0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000acb0: 6966 206e 702e 6973 6e61 6e28 6e6f 726d  if np.isnan(norm
-0000acc0: 5f63 6f75 6e74 732e 582e 6461 7461 292e  _counts.X.data).
-0000acd0: 7375 6d28 2920 3e20 303a 0d0a 2020 2020  sum() > 0:..    
-0000ace0: 2020 2020 2020 2020 2320 2020 2020 7261          #     ra
-0000acf0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-0000ad00: 4e61 4e73 2069 6e20 6e6f 726d 616c 697a  NaNs in normaliz
-0000ad10: 6564 2063 6f75 6e74 7320 6d61 7472 6978  ed counts matrix
-0000ad20: 2729 2020 2020 2020 2020 2020 2020 2020  ')              
-0000ad30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000ad40: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000ad50: 2020 2020 2020 6e6f 726d 5f63 6f75 6e74        norm_count
-0000ad60: 732e 5820 2f3d 206e 6f72 6d5f 636f 756e  s.X /= norm_coun
-0000ad70: 7473 2e58 2e73 7464 2861 7869 733d 302c  ts.X.std(axis=0,
-0000ad80: 2064 646f 663d 3129 0d0a 2020 2020 2020   ddof=1)..      
-0000ad90: 2020 2020 2020 6966 206e 702e 6973 6e61        if np.isna
-0000ada0: 6e28 6e6f 726d 5f63 6f75 6e74 732e 5829  n(norm_counts.X)
-0000adb0: 2e73 756d 2829 2e73 756d 2829 203e 2030  .sum().sum() > 0
-0000adc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000add0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000ade0: 726f 7228 274e 614e 7320 696e 206e 6f72  ror('NaNs in nor
-0000adf0: 6d61 6c69 7a65 6420 636f 756e 7473 206d  malized counts m
-0000ae00: 6174 7269 7827 2920 2020 2020 2020 2020  atrix')         
-0000ae10: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-0000ae20: 2020 2020 2020 2023 2320 5361 7665 2061         ## Save a
-0000ae30: 205c 6e2d 6465 6c69 6d69 7465 6420 6c69   \n-delimited li
-0000ae40: 7374 206f 6620 7468 6520 6869 6768 2d76  st of the high-v
-0000ae50: 6172 6961 6e63 6520 6765 6e65 7320 7573  ariance genes us
-0000ae60: 6564 2066 6f72 2066 6163 746f 7269 7a61  ed for factoriza
-0000ae70: 7469 6f6e 0d0a 2020 2020 2020 2020 6f70  tion..        op
-0000ae80: 656e 2863 6e6d 665f 6f62 6a2e 7061 7468  en(cnmf_obj.path
-0000ae90: 735b 276e 6d66 5f67 656e 6573 5f6c 6973  s['nmf_genes_lis
-0000aea0: 7427 5d2c 2027 7727 292e 7772 6974 6528  t'], 'w').write(
-0000aeb0: 275c 6e27 2e6a 6f69 6e28 6f76 6572 6469  '\n'.join(overdi
-0000aec0: 7370 6572 7365 645f 6765 6e65 7329 290d  spersed_genes)).
-0000aed0: 0a0d 0a20 2020 2020 2020 2069 6620 6e6f  ...        if no
-0000aee0: 726d 5f63 6f75 6e74 732e 582e 6474 7970  rm_counts.X.dtyp
-0000aef0: 6520 213d 206e 702e 666c 6f61 7436 343a  e != np.float64:
-0000af00: 0d0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
-0000af10: 726d 5f63 6f75 6e74 732e 5820 3d20 6e6f  rm_counts.X = no
-0000af20: 726d 5f63 6f75 6e74 732e 582e 6173 7479  rm_counts.X.asty
-0000af30: 7065 286e 702e 666c 6f61 7436 3429 0d0a  pe(np.float64)..
-0000af40: 0d0a 2020 2020 2020 2020 6e6f 726d 5f63  ..        norm_c
-0000af50: 6f75 6e74 732e 7772 6974 655f 6835 6164  ounts.write_h5ad
-0000af60: 2863 6e6d 665f 6f62 6a2e 7061 7468 735b  (cnmf_obj.paths[
-0000af70: 276e 6f72 6d61 6c69 7a65 645f 636f 756e  'normalized_coun
-0000af80: 7473 275d 290d 0a0d 0a20 2020 2020 2020  ts'])....       
-0000af90: 2023 2073 6176 6520 7061 7261 6d65 7465   # save paramete
-0000afa0: 7273 2066 6f72 2066 6163 746f 7269 7a61  rs for factoriza
-0000afb0: 7469 6f6e 2073 7465 700d 0a20 2020 2020  tion step..     
-0000afc0: 2020 2063 6e6d 665f 6f62 6a2e 7361 7665     cnmf_obj.save
-0000afd0: 5f6e 6d66 5f69 7465 725f 7061 7261 6d73  _nmf_iter_params
-0000afe0: 282a 636e 6d66 5f6f 626a 2e67 6574 5f6e  (*cnmf_obj.get_n
-0000aff0: 6d66 5f69 7465 725f 7061 7261 6d73 286b  mf_iter_params(k
-0000b000: 733d 6b76 616c 732c 206e 5f69 7465 723d  s=kvals, n_iter=
-0000b010: 6e5f 6974 6572 2c20 7261 6e64 6f6d 5f73  n_iter, random_s
-0000b020: 7461 7465 5f73 6565 643d 7365 6564 2c20  tate_seed=seed, 
-0000b030: 6265 7461 5f6c 6f73 733d 6265 7461 5f6c  beta_loss=beta_l
-0000b040: 6f73 7329 290d 0a0d 0a20 2020 2020 2020  oss))....       
-0000b050: 2023 2073 6176 6520 7061 7261 6d65 7465   # save paramete
-0000b060: 7273 2069 6e20 416e 6e44 6174 6120 6f62  rs in AnnData ob
-0000b070: 6a65 6374 0d0a 2020 2020 2020 2020 7365  ject..        se
-0000b080: 6c66 2e61 6461 7461 2e75 6e73 5b22 636e  lf.adata.uns["cn
-0000b090: 6d66 225d 203d 2063 6e6d 665f 6f62 6a2e  mf"] = cnmf_obj.
-0000b0a0: 6765 745f 6e6d 665f 6974 6572 5f70 6172  get_nmf_iter_par
-0000b0b0: 616d 7328 6b73 3d6b 7661 6c73 2c20 6e5f  ams(ks=kvals, n_
-0000b0c0: 6974 6572 3d6e 5f69 7465 722c 2072 616e  iter=n_iter, ran
-0000b0d0: 646f 6d5f 7374 6174 655f 7365 6564 3d73  dom_state_seed=s
-0000b0e0: 6565 642c 2062 6574 615f 6c6f 7373 3d62  eed, beta_loss=b
-0000b0f0: 6574 615f 6c6f 7373 295b 315d 2020 2320  eta_loss)[1]  # 
-0000b100: 6469 6374 206f 6620 636e 6d66 2070 6172  dict of cnmf par
-0000b110: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-0000b120: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-0000b130: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
-0000b140: 7928 6622 634e 4d46 2070 6172 616d 6574  y(f"cNMF paramet
-0000b150: 6572 7320 6164 6465 642e 2063 4e4d 4620  ers added. cNMF 
-0000b160: 696e 7075 7473 2069 6e69 7469 616c 697a  inputs initializ
-0000b170: 6564 2069 6e20 7b63 6e6d 665f 6f75 7470  ed in {cnmf_outp
-0000b180: 7574 5f64 6972 7d2f 7b63 6e6d 665f 6e61  ut_dir}/{cnmf_na
-0000b190: 6d65 7d22 290d 0a20 2020 2020 2020 2072  me}")..        r
-0000b1a0: 6574 7572 6e20 636e 6d66 5f6f 626a 0d0a  eturn cnmf_obj..
-0000b1b0: 2020 2020 0d0a 2020 2020 6465 6620 6164      ..    def ad
-0000b1c0: 645f 636e 6d66 5f72 6573 756c 7473 2873  d_cnmf_results(s
-0000b1d0: 656c 662c 2063 6e6d 665f 6f75 7470 7574  elf, cnmf_output
-0000b1e0: 5f64 6972 2c20 636e 6d66 5f6e 616d 652c  _dir, cnmf_name,
-0000b1f0: 206c 6f63 616c 5f64 656e 7369 7479 5f74   local_density_t
-0000b200: 6872 6573 686f 6c64 3a20 666c 6f61 7420  hreshold: float 
-0000b210: 3d20 4e6f 6e65 2c20 6c6f 6361 6c5f 6e65  = None, local_ne
-0000b220: 6967 6862 6f72 686f 6f64 5f73 697a 653a  ighborhood_size:
-0000b230: 2066 6c6f 6174 203d 204e 6f6e 6529 3a0d   float = None):.
-0000b240: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000b250: 2020 2020 2020 4166 7465 7220 6661 6374        After fact
-0000b260: 6f72 697a 6174 696f 6e2c 2061 6464 2063  orization, add c
-0000b270: 6f6d 706c 6574 6564 2063 4e4d 4620 7265  ompleted cNMF re
-0000b280: 7375 6c74 7320 696e 205b 636e 6d66 5f6f  sults in [cnmf_o
-0000b290: 7574 7075 745f 6469 725d 2f5b 636e 6d66  utput_dir]/[cnmf
-0000b2a0: 5f6e 616d 655d 2074 6f20 7468 6520 6461  _name] to the da
-0000b2b0: 7461 7365 7420 6f62 6a65 6374 2e0d 0a0d  taset object....
-0000b2c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000b2d0: 636e 6d66 5f6f 7574 7075 745f 6469 723a  cnmf_output_dir:
-0000b2e0: 204f 7574 7075 7420 6469 7265 6374 6f72   Output director
-0000b2f0: 7920 666f 7220 634e 4d46 2072 6573 756c  y for cNMF resul
-0000b300: 7473 0d0a 2020 2020 2020 2020 3a74 7970  ts..        :typ
-0000b310: 6520 636e 6d66 5f6f 7574 7075 745f 6469  e cnmf_output_di
-0000b320: 723a 2073 7472 0d0a 2020 2020 2020 2020  r: str..        
-0000b330: 3a70 6172 616d 2063 6e6d 665f 6e61 6d65  :param cnmf_name
-0000b340: 3a20 4e61 6d65 206f 6620 7468 6520 634e  : Name of the cN
-0000b350: 4d46 2072 6573 756c 7473 2e20 4669 6c65  MF results. File
-0000b360: 7320 7769 6c6c 2062 6520 6f75 7470 7574  s will be output
-0000b370: 2074 6f20 5b63 6e6d 665f 6f75 7470 7574   to [cnmf_output
-0000b380: 5f64 6972 5d2f 5b63 6e6d 665f 6e61 6d65  _dir]/[cnmf_name
-0000b390: 5d2f 0d0a 2020 2020 2020 2020 3a74 7970  ]/..        :typ
-0000b3a0: 6520 636e 6d66 5f6e 616d 653a 2073 7472  e cnmf_name: str
-0000b3b0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000b3c0: 206c 6f63 616c 5f64 656e 7369 7479 5f74   local_density_t
-0000b3d0: 6872 6573 686f 6c64 3a20 5468 7265 7368  hreshold: Thresh
-0000b3e0: 6f6c 6420 666f 7220 7468 6520 6c6f 6361  old for the loca
-0000b3f0: 6c20 6465 6e73 6974 7920 6669 6c74 6572  l density filter
-0000b400: 696e 6720 7072 696f 7220 746f 2047 4550  ing prior to GEP
-0000b410: 2063 6f6e 7365 6e73 7573 2e20 4163 6365   consensus. Acce
-0000b420: 7074 6162 6c65 2074 6872 6573 686f 6c64  ptable threshold
-0000b430: 7320 6172 6520 3e20 3020 616e 6420 3c3d  s are > 0 and <=
-0000b440: 2032 2028 322e 3020 6973 206e 6f20 6669   2 (2.0 is no fi
-0000b450: 6c74 6572 696e 6729 2e20 4465 6661 756c  ltering). Defaul
-0000b460: 7473 2074 6f20 4e6f 6e65 2e0d 0a20 2020  ts to None...   
-0000b470: 2020 2020 203a 7479 7065 206c 6f63 616c       :type local
-0000b480: 5f64 656e 7369 7479 5f74 6872 6573 686f  _density_thresho
-0000b490: 6c64 3a20 666c 6f61 742c 206f 7074 696f  ld: float, optio
-0000b4a0: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-0000b4b0: 7261 6d20 6c6f 6361 6c5f 6e65 6967 6862  ram local_neighb
-0000b4c0: 6f72 686f 6f64 5f73 697a 653a 2046 7261  orhood_size: Fra
-0000b4d0: 6374 696f 6e20 6f66 2074 6865 206e 756d  ction of the num
-0000b4e0: 6265 7220 6f66 2072 6570 6c69 6361 7465  ber of replicate
-0000b4f0: 7320 746f 2075 7365 2061 7320 6e65 6172  s to use as near
-0000b500: 6573 7420 6e65 6967 6862 6f72 7320 666f  est neighbors fo
-0000b510: 7220 6c6f 6361 6c20 6465 6e73 6974 7920  r local density 
-0000b520: 6669 6c74 6572 696e 672e 2044 6566 6175  filtering. Defau
-0000b530: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
-0000b540: 2020 2020 203a 7479 7065 206c 6f63 616c       :type local
-0000b550: 5f6e 6569 6768 626f 7268 6f6f 645f 7369  _neighborhood_si
-0000b560: 7a65 3a20 666c 6f61 742c 206f 7074 696f  ze: float, optio
-0000b570: 6e61 6c0d 0a20 2020 2020 2020 2022 2222  nal..        """
-0000b580: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0000b590: 6461 7461 2e75 6e73 5b22 636e 6d66 5f6e  data.uns["cnmf_n
-0000b5a0: 616d 6522 5d20 3d20 636e 6d66 5f6e 616d  ame"] = cnmf_nam
-0000b5b0: 650d 0a0d 0a20 2020 2020 2020 2023 2069  e....        # i
-0000b5c0: 6e66 6572 2066 726f 6d20 6669 6c65 6e61  nfer from filena
-0000b5d0: 6d65 7320 7768 6963 6820 6c6f 6361 6c20  mes which local 
-0000b5e0: 6465 6e73 6974 7920 7468 7265 7368 6f6c  density threshol
-0000b5f0: 6420 7761 7320 7573 6564 0d0a 2020 2020  d was used..    
-0000b600: 2020 2020 7365 6e73 6564 5f6c 6474 7320      sensed_ldts 
-0000b610: 3d20 7365 7428 290d 0a20 2020 2020 2020  = set()..       
-0000b620: 2066 6f72 2066 6e20 696e 2067 6c6f 6228   for fn in glob(
-0000b630: 6f73 2e70 6174 682e 6a6f 696e 2863 6e6d  os.path.join(cnm
-0000b640: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
-0000b650: 6d66 5f6e 616d 652c 2066 227b 636e 6d66  mf_name, f"{cnmf
-0000b660: 5f6e 616d 657d 2a2e 2a73 7065 6374 7261  _name}*.*spectra
-0000b670: 2a2e 6b5f 2a22 2929 3a0d 0a20 2020 2020  *.k_*")):..     
-0000b680: 2020 2020 2020 206c 6474 5f73 7472 203d         ldt_str =
-0000b690: 206f 732e 7061 7468 2e62 6173 656e 616d   os.path.basenam
-0000b6a0: 6528 666e 292e 7370 6c69 7428 222e 2229  e(fn).split(".")
-0000b6b0: 5b2d 335d 0d0a 2020 2020 2020 2020 2020  [-3]..          
-0000b6c0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-0000b6d0: 2020 2020 2020 2020 6c64 7420 3d20 666c          ldt = fl
-0000b6e0: 6f61 7428 6c64 745f 7374 722e 7265 706c  oat(ldt_str.repl
-0000b6f0: 6163 6528 2264 745f 222c 2022 2229 2e72  ace("dt_", "").r
-0000b700: 6570 6c61 6365 2822 5f22 2c20 222e 2229  eplace("_", ".")
-0000b710: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000b720: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-0000b730: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b740: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-0000b750: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000b760: 2020 2020 2020 2020 2020 2020 7365 6e73              sens
-0000b770: 6564 5f6c 6474 732e 6164 6428 286c 6474  ed_ldts.add((ldt
-0000b780: 5f73 7472 2c20 6c64 7429 290d 0a20 2020  _str, ldt))..   
-0000b790: 2020 2020 2069 6620 6c6f 6361 6c5f 6465       if local_de
-0000b7a0: 6e73 6974 795f 7468 7265 7368 6f6c 6420  nsity_threshold 
-0000b7b0: 6973 204e 6f6e 6520 616e 6420 6c65 6e28  is None and len(
-0000b7c0: 7365 6e73 6564 5f6c 6474 7329 203d 3d20  sensed_ldts) == 
-0000b7d0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-0000b7e0: 6c64 745f 7374 722c 206c 6474 203d 2073  ldt_str, ldt = s
-0000b7f0: 656e 7365 645f 6c64 7473 2e70 6f70 2829  ensed_ldts.pop()
-0000b800: 0d0a 2020 2020 2020 2020 656c 6966 206c  ..        elif l
-0000b810: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
-0000b820: 6573 686f 6c64 2069 6e20 286c 6474 5b31  eshold in (ldt[1
-0000b830: 5d20 666f 7220 6c64 7420 696e 2073 656e  ] for ldt in sen
-0000b840: 7365 645f 6c64 7473 293a 0d0a 2020 2020  sed_ldts):..    
-0000b850: 2020 2020 2020 2020 6c64 745f 7374 722c          ldt_str,
-0000b860: 206c 6474 203d 205b 286c 6474 5f73 7472   ldt = [(ldt_str
-0000b870: 2c20 6c64 7429 2066 6f72 206c 6474 5f73  , ldt) for ldt_s
-0000b880: 7472 2c20 6c64 7420 696e 2073 656e 7365  tr, ldt in sense
-0000b890: 645f 6c64 7473 2069 6620 6c64 7420 3d3d  d_ldts if ldt ==
-0000b8a0: 206c 6f63 616c 5f64 656e 7369 7479 5f74   local_density_t
-0000b8b0: 6872 6573 686f 6c64 5d2e 706f 7028 290d  hreshold].pop().
-0000b8c0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-0000b8d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000b8e0: 6520 5275 6e74 696d 6545 7272 6f72 2866  e RuntimeError(f
-0000b8f0: 226c 6f63 616c 5f64 656e 7369 7479 5f74  "local_density_t
-0000b900: 6872 6573 686f 6c64 206f 6620 7b6c 6f63  hreshold of {loc
-0000b910: 616c 5f64 656e 7369 7479 5f74 6872 6573  al_density_thres
-0000b920: 686f 6c64 7d20 646f 6573 206e 6f74 206d  hold} does not m
-0000b930: 6174 6368 2077 6861 7420 6973 2069 6e20  atch what is in 
-0000b940: 7468 6520 634e 4d46 2072 6573 756c 7420  the cNMF result 
-0000b950: 6469 7265 6374 6f72 793a 207b 7365 6e73  directory: {sens
-0000b960: 6564 5f6c 6474 737d 2229 0d0a 2020 2020  ed_ldts}")..    
-0000b970: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
-0000b980: 6e73 5b22 6c64 7422 5d20 3d20 6c64 740d  ns["ldt"] = ldt.
-0000b990: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-0000b9a0: 6174 612e 756e 735b 226c 6e73 225d 203d  ata.uns["lns"] =
-0000b9b0: 206c 6f63 616c 5f6e 6569 6768 626f 7268   local_neighborh
-0000b9c0: 6f6f 645f 7369 7a65 0d0a 2020 2020 2020  ood_size..      
-0000b9d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000b9e0: 2320 496d 706f 7274 2047 4550 730d 0a20  # Import GEPs.. 
-0000b9f0: 2020 2020 2020 2072 6573 756c 745f 7479         result_ty
-0000ba00: 7065 7320 3d20 7b0d 0a20 2020 2020 2020  pes = {..       
-0000ba10: 2020 2020 2022 6765 6e65 5f73 7065 6374       "gene_spect
-0000ba20: 7261 5f73 636f 7265 223a 2022 636e 6d66  ra_score": "cnmf
-0000ba30: 5f67 6570 5f73 636f 7265 222c 0d0a 2020  _gep_score",..  
-0000ba40: 2020 2020 2020 2020 2020 2267 656e 655f            "gene_
-0000ba50: 7370 6563 7472 615f 7470 6d22 3a20 2263  spectra_tpm": "c
-0000ba60: 6e6d 665f 6765 705f 7470 6d22 2c0d 0a20  nmf_gep_tpm",.. 
-0000ba70: 2020 2020 2020 2020 2020 2022 7370 6563             "spec
-0000ba80: 7472 6122 3a20 2263 6e6d 665f 6765 705f  tra": "cnmf_gep_
-0000ba90: 7261 7722 0d0a 2020 2020 2020 2020 2020  raw"..          
-0000baa0: 2020 7d0d 0a20 2020 2020 2020 2066 6f72    }..        for
-0000bab0: 206d 6174 6368 7374 722c 2072 6573 756c   matchstr, resul
-0000bac0: 745f 7479 7065 2069 6e20 7265 7375 6c74  t_type in result
-0000bad0: 5f74 7970 6573 2e69 7465 6d73 2829 3a0d  _types.items():.
-0000bae0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0000baf0: 6769 6e67 2e69 6e66 6f28 6622 496d 706f  ging.info(f"Impo
-0000bb00: 7274 696e 6720 4745 5073 3a20 7b6d 6174  rting GEPs: {mat
-0000bb10: 6368 7374 727d 2229 2020 0d0a 2020 2020  chstr}")  ..    
-0000bb20: 2020 2020 2020 2020 6d65 7461 5f77 203d          meta_w =
-0000bb30: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0000bb40: 2066 6f72 2066 6e20 696e 2067 6c6f 6228   for fn in glob(
-0000bb50: 6f73 2e70 6174 682e 6a6f 696e 2863 6e6d  os.path.join(cnm
-0000bb60: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
-0000bb70: 6d66 5f6e 616d 652c 2066 227b 636e 6d66  mf_name, f"{cnmf
-0000bb80: 5f6e 616d 657d 2a2e 7b6d 6174 6368 7374  _name}*.{matchst
-0000bb90: 727d 2e6b 5f2a 2e7b 6c64 745f 7374 727d  r}.k_*.{ldt_str}
-0000bba0: 2e2a 7478 7422 2929 3a0d 0a20 2020 2020  .*txt")):..     
-0000bbb0: 2020 2020 2020 2020 2020 206b 203d 2069             k = i
-0000bbc0: 6e74 286f 732e 7061 7468 2e62 6173 656e  nt(os.path.basen
-0000bbd0: 616d 6528 666e 292e 7265 6d6f 7665 7072  ame(fn).removepr
-0000bbe0: 6566 6978 2866 227b 636e 6d66 5f6e 616d  efix(f"{cnmf_nam
-0000bbf0: 657d 2e7b 6d61 7463 6873 7472 7d2e 2229  e}.{matchstr}.")
-0000bc00: 2e73 706c 6974 2822 2e22 295b 305d 2e72  .split(".")[0].r
-0000bc10: 6570 6c61 6365 2822 6b5f 222c 2022 2229  eplace("k_", "")
-0000bc20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000bc30: 2020 2077 203d 2070 642e 7265 6164 5f74     w = pd.read_t
-0000bc40: 6162 6c65 2866 6e2c 2069 6e64 6578 5f63  able(fn, index_c
-0000bc50: 6f6c 3d30 290d 0a20 2020 2020 2020 2020  ol=0)..         
-0000bc60: 2020 2020 2020 2077 2e69 6e64 6578 203d         w.index =
-0000bc70: 2073 7472 286b 2920 2b20 222e 2220 2b20   str(k) + "." + 
-0000bc80: 772e 696e 6465 782e 6173 7479 7065 2873  w.index.astype(s
-0000bc90: 7472 290d 0a20 2020 2020 2020 2020 2020  tr)..           
-0000bca0: 2020 2020 206d 6574 615f 772e 6170 7065       meta_w.appe
-0000bcb0: 6e64 2877 290d 0a20 2020 2020 2020 2020  nd(w)..         
-0000bcc0: 2020 206d 6574 615f 7720 3d20 7064 2e63     meta_w = pd.c
-0000bcd0: 6f6e 6361 7428 6d65 7461 5f77 2c20 6178  oncat(meta_w, ax
-0000bce0: 6973 3d30 292e 542e 7265 696e 6465 7828  is=0).T.reindex(
-0000bcf0: 7365 6c66 2e61 6461 7461 2e76 6172 2e69  self.adata.var.i
-0000bd00: 6e64 6578 292e 7265 6e61 6d65 5f61 7869  ndex).rename_axi
-0000bd10: 7328 5b22 6b2e 6765 7022 5d2c 2061 7869  s(["k.gep"], axi
-0000bd20: 733d 3129 0d0a 2020 2020 2020 2020 2020  s=1)..          
-0000bd30: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
-0000bd40: 6d5b 7265 7375 6c74 5f74 7970 655d 203d  m[result_type] =
-0000bd50: 206d 6574 615f 770d 0a0d 0a20 2020 2020   meta_w....     
-0000bd60: 2020 2023 2049 6d70 6f72 7420 5573 6167     # Import Usag
-0000bd70: 6573 0d0a 2020 2020 2020 2020 6c6f 6767  es..        logg
-0000bd80: 696e 672e 696e 666f 2866 2249 6d70 6f72  ing.info(f"Impor
-0000bd90: 7469 6e67 2055 7361 6765 7322 2920 200d  ting Usages")  .
-0000bda0: 0a20 2020 2020 2020 2075 7361 6765 203d  .        usage =
-0000bdb0: 205b 5d0d 0a20 2020 2020 2020 2066 6f72   []..        for
-0000bdc0: 2066 6e20 696e 2067 6c6f 6228 6f73 2e70   fn in glob(os.p
-0000bdd0: 6174 682e 6a6f 696e 2863 6e6d 665f 6f75  ath.join(cnmf_ou
-0000bde0: 7470 7574 5f64 6972 2c20 636e 6d66 5f6e  tput_dir, cnmf_n
-0000bdf0: 616d 652c 2066 227b 636e 6d66 5f6e 616d  ame, f"{cnmf_nam
-0000be00: 657d 2a2e 7573 6167 6573 2e6b 5f2a 2e7b  e}*.usages.k_*.{
-0000be10: 6c64 745f 7374 727d 2e2a 7478 7422 2929  ldt_str}.*txt"))
-0000be20: 3a0d 0a20 2020 2020 2020 2020 2020 206b  :..            k
-0000be30: 203d 2069 6e74 286f 732e 7061 7468 2e62   = int(os.path.b
-0000be40: 6173 656e 616d 6528 666e 292e 7265 6d6f  asename(fn).remo
-0000be50: 7665 7072 6566 6978 2866 227b 636e 6d66  veprefix(f"{cnmf
-0000be60: 5f6e 616d 657d 2e75 7361 6765 732e 2229  _name}.usages.")
-0000be70: 2e73 706c 6974 2822 2e22 295b 305d 2e72  .split(".")[0].r
-0000be80: 6570 6c61 6365 2822 6b5f 222c 2022 2229  eplace("k_", "")
-0000be90: 290d 0a20 2020 2020 2020 2020 2020 2068  )..            h
-0000bea0: 203d 2070 642e 7265 6164 5f74 6162 6c65   = pd.read_table
-0000beb0: 2866 6e2c 2069 6e64 6578 5f63 6f6c 3d30  (fn, index_col=0
-0000bec0: 290d 0a20 2020 2020 2020 2020 2020 2068  )..            h
-0000bed0: 2e63 6f6c 756d 6e73 203d 2073 7472 286b  .columns = str(k
-0000bee0: 2920 2b20 222e 2220 2b20 682e 636f 6c75  ) + "." + h.colu
-0000bef0: 6d6e 732e 6173 7479 7065 2873 7472 290d  mns.astype(str).
-0000bf00: 0a20 2020 2020 2020 2020 2020 2075 7361  .            usa
-0000bf10: 6765 2e61 7070 656e 6428 6829 0d0a 2020  ge.append(h)..  
-0000bf20: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-0000bf30: 2e6f 6273 6d5b 2263 6e6d 665f 7573 6167  .obsm["cnmf_usag
-0000bf40: 6522 5d20 3d20 7064 2e63 6f6e 6361 7428  e"] = pd.concat(
-0000bf50: 7573 6167 652c 2061 7869 733d 3129 2e73  usage, axis=1).s
-0000bf60: 6f72 745f 696e 6465 7828 6178 6973 3d31  ort_index(axis=1
-0000bf70: 292e 7265 6e61 6d65 5f61 7869 7328 5b22  ).rename_axis(["
-0000bf80: 6b2e 6765 7022 5d2c 2061 7869 733d 3129  k.gep"], axis=1)
-0000bf90: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0000bfa0: 2020 2020 2320 496d 706f 7274 2067 656e      # Import gen
-0000bfb0: 6520 6c69 7374 2075 7365 6420 666f 7220  e list used for 
-0000bfc0: 6661 6374 6f72 697a 6174 696f 6e0d 0a20  factorization.. 
-0000bfd0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-0000bfe0: 286f 732e 7061 7468 2e6a 6f69 6e28 636e  (os.path.join(cn
-0000bff0: 6d66 5f6f 7574 7075 745f 6469 722c 2063  mf_output_dir, c
-0000c000: 6e6d 665f 6e61 6d65 2c20 6622 7b63 6e6d  nmf_name, f"{cnm
-0000c010: 665f 6e61 6d65 7d2e 6f76 6572 6469 7370  f_name}.overdisp
-0000c020: 6572 7365 645f 6765 6e65 732e 7478 7422  ersed_genes.txt"
-0000c030: 2929 2061 7320 663a 0d0a 2020 2020 2020  )) as f:..      
-0000c040: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-0000c050: 2e75 6e73 5b22 6765 6e65 5f6c 6973 7422  .uns["gene_list"
-0000c060: 5d20 3d20 5b6c 696e 652e 7374 7269 7028  ] = [line.strip(
-0000c070: 2920 666f 7220 6c69 6e65 2069 6e20 662e  ) for line in f.
-0000c080: 7265 6164 6c69 6e65 7328 295d 0d0a 0d0a  readlines()]....
-0000c090: 2020 2020 2020 2020 2320 496d 706f 7274          # Import
-0000c0a0: 204b 2d73 656c 6563 7469 6f6e 2073 7461   K-selection sta
-0000c0b0: 7473 0d0a 2020 2020 2020 2020 6b76 616c  ts..        kval
-0000c0c0: 7320 3d20 7064 2e44 6174 6146 7261 6d65  s = pd.DataFrame
-0000c0d0: 282a 2a6e 702e 6c6f 6164 286f 732e 7061  (**np.load(os.pa
-0000c0e0: 7468 2e6a 6f69 6e28 636e 6d66 5f6f 7574  th.join(cnmf_out
-0000c0f0: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
-0000c100: 6d65 2c20 6622 7b63 6e6d 665f 6e61 6d65  me, f"{cnmf_name
-0000c110: 7d2e 6b5f 7365 6c65 6374 696f 6e5f 7374  }.k_selection_st
-0000c120: 6174 732e 6466 2e6e 707a 2229 2c20 616c  ats.df.npz"), al
-0000c130: 6c6f 775f 7069 636b 6c65 3d54 7275 6529  low_pickle=True)
-0000c140: 292e 7365 745f 696e 6465 7828 226b 2229  ).set_index("k")
-0000c150: 5b5b 2273 7461 6269 6c69 7479 222c 2022  [["stability", "
-0000c160: 7072 6564 6963 7469 6f6e 5f65 7272 6f72  prediction_error
-0000c170: 225d 5d0d 0a20 2020 2020 2020 206b 7661  "]]..        kva
-0000c180: 6c73 2e69 6e64 6578 203d 206b 7661 6c73  ls.index = kvals
-0000c190: 2e69 6e64 6578 2e61 7374 7970 6528 696e  .index.astype(in
-0000c1a0: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-0000c1b0: 2e61 6461 7461 2e75 6e73 5b22 6b76 616c  .adata.uns["kval
-0000c1c0: 7322 5d20 3d20 6b76 616c 730d 0a20 2020  s"] = kvals..   
-0000c1d0: 2020 2020 2073 656c 662e 6170 7065 6e64       self.append
-0000c1e0: 5f74 6f5f 6869 7374 6f72 7928 2263 4e4d  _to_history("cNM
-0000c1f0: 4620 7265 7375 6c74 7320 6164 6465 6420  F results added 
-0000c200: 6672 6f6d 206f 7574 7075 7420 6469 7265  from output dire
-0000c210: 6374 6f72 7920 7b63 6e6d 665f 6f75 7470  ctory {cnmf_outp
-0000c220: 7574 5f64 6972 7d2f 7b63 6e6d 665f 6e61  ut_dir}/{cnmf_na
-0000c230: 6d65 7d22 290d 0a0d 0a20 2020 2064 6566  me}")....    def
-0000c240: 2072 656d 6f76 655f 636e 6d66 5f72 6573   remove_cnmf_res
-0000c250: 756c 7473 2873 656c 6629 3a0d 0a20 2020  ults(self):..   
-0000c260: 2020 2020 2066 6f72 2072 6573 756c 745f       for result_
-0000c270: 7479 7065 2069 6e20 2822 636e 6d66 5f67  type in ("cnmf_g
-0000c280: 6570 5f73 636f 7265 222c 2022 636e 6d66  ep_score", "cnmf
-0000c290: 5f67 6570 5f74 706d 222c 2022 636e 6d66  _gep_tpm", "cnmf
-0000c2a0: 5f67 6570 5f72 6177 2229 3a0d 0a20 2020  _gep_raw"):..   
-0000c2b0: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-0000c2c0: 6174 612e 7661 726d 2e70 6f70 2872 6573  ata.varm.pop(res
-0000c2d0: 756c 745f 7479 7065 290d 0a20 2020 2020  ult_type)..     
-0000c2e0: 2020 2073 656c 662e 6164 6174 612e 6f62     self.adata.ob
-0000c2f0: 736d 2e70 6f70 2822 636e 6d66 5f75 7361  sm.pop("cnmf_usa
-0000c300: 6765 2229 0d0a 2020 2020 2020 2020 7365  ge")..        se
-0000c310: 6c66 2e61 6461 7461 2e75 6e73 2e70 6f70  lf.adata.uns.pop
-0000c320: 2822 6765 6e65 5f6c 6973 7422 290d 0a20  ("gene_list").. 
-0000c330: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-0000c340: 612e 756e 732e 706f 7028 226b 7661 6c73  a.uns.pop("kvals
-0000c350: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-0000c360: 2e61 7070 656e 645f 746f 5f68 6973 746f  .append_to_histo
-0000c370: 7279 2822 634e 4d46 2072 6573 756c 7473  ry("cNMF results
-0000c380: 2072 656d 6f76 6564 2e22 290d 0a0d 0a0d   removed.").....
-0000c390: 0a20 2020 2064 6566 2067 6574 5f75 7361  .    def get_usa
-0000c3a0: 6765 7328 7365 6c66 2c0d 0a20 2020 2020  ges(self,..     
-0000c3b0: 2020 2020 2020 2020 2020 2020 2020 6b3a                k:
-0000c3c0: 2055 6e69 6f6e 5b69 6e74 2c20 4974 6572   Union[int, Iter
-0000c3d0: 6162 6c65 5d20 3d20 4e6f 6e65 2c0d 0a20  able] = None,.. 
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 2020 6469 7363 7265 7469 7a65 3a20 626f    discretize: bo
-0000c400: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 6e6f 726d 616c 697a 653a 2062 6f6f 6c20  normalize: bool 
-0000c430: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-0000c440: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
-0000c450: 2070 642e 4461 7461 4672 616d 653a 0d0a   pd.DataFrame:..
-0000c460: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000c470: 2020 2020 2043 616c 6375 6c61 7465 2075       Calculate u
-0000c480: 7361 6765 206f 6620 6561 6368 2047 4550  sage of each GEP
-0000c490: 2069 6e20 6561 6368 2073 616d 706c 652f   in each sample/
-0000c4a0: 6f62 7365 7276 6174 696f 6e2e 0d0a 0d0a  observation.....
-0000c4b0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-0000c4c0: 3a20 4966 2061 6e20 696e 7465 6765 7220  : If an integer 
-0000c4d0: 6f72 206c 6973 7420 6f66 2069 6e74 6567  or list of integ
-0000c4e0: 6572 732c 2072 6574 7572 6e73 2075 7361  ers, returns usa
-0000c4f0: 6765 7320 6f6e 6c79 2066 6f72 2073 7065  ges only for spe
-0000c500: 6369 6669 6564 2072 616e 6b73 2e20 4f74  cified ranks. Ot
-0000c510: 6865 7277 6973 652c 2072 6574 7572 6e73  herwise, returns
-0000c520: 2075 7361 6765 206f 6620 616c 6c20 4745   usage of all GE
-0000c530: 5073 2061 6372 6f73 7320 7261 6e6b 732e  Ps across ranks.
-0000c540: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-0000c550: 650d 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-0000c560: 206b 3a20 696e 742c 206f 7074 696f 6e61   k: int, optiona
-0000c570: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-0000c580: 6d20 6469 7363 7265 7469 7a65 3a20 4469  m discretize: Di
-0000c590: 7363 7265 7469 7a65 7320 7468 6520 7573  scretizes the us
-0000c5a0: 6167 6520 6d61 7472 6978 2073 7563 6820  age matrix such 
-0000c5b0: 7468 6174 2066 6f72 2065 6163 6820 7661  that for each va
-0000c5c0: 6c75 6520 6f66 206b 2c20 6561 6368 2073  lue of k, each s
-0000c5d0: 616d 706c 6520 6861 7320 7573 6167 6520  ample has usage 
-0000c5e0: 6f66 206f 6e6c 7920 3120 4745 5020 2874  of only 1 GEP (t
-0000c5f0: 6865 206f 6e65 2077 6974 6820 7468 6520  he one with the 
-0000c600: 6d61 7869 6d75 6d20 7573 6167 6529 2e20  maximum usage). 
-0000c610: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
-0000c620: 650d 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-0000c630: 2064 6973 6372 6574 697a 653a 2062 6f6f   discretize: boo
-0000c640: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-0000c650: 2020 2020 203a 7061 7261 6d20 6e6f 726d       :param norm
-0000c660: 616c 697a 653a 204e 6f72 6d61 6c69 7a65  alize: Normalize
-0000c670: 2074 6865 2047 4550 2075 7361 6765 206d   the GEP usage m
-0000c680: 6174 7269 7820 7375 6368 2074 6861 7420  atrix such that 
-0000c690: 666f 7220 6561 6368 2076 616c 7565 206f  for each value o
-0000c6a0: 6620 6b2c 2075 7361 6765 206f 6620 616c  f k, usage of al
-0000c6b0: 6c20 4745 5073 2073 756d 7320 746f 2031  l GEPs sums to 1
-0000c6c0: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-0000c6d0: 6c73 650d 0a20 2020 2020 2020 203a 7479  lse..        :ty
-0000c6e0: 7065 206e 6f72 6d61 6c69 7a65 3a20 626f  pe normalize: bo
-0000c6f0: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
-0000c700: 2020 2020 2020 3a72 6574 7572 6e3a 206f        :return: o
-0000c710: 6273 6572 7661 7469 6f6e 20c3 9720 4745  bservation .. GE
-0000c720: 5020 6d61 7472 6978 0d0a 2020 2020 2020  P matrix..      
-0000c730: 2020 3a72 7479 7065 3a20 7064 2e44 6174    :rtype: pd.Dat
-0000c740: 6146 7261 6d65 0d0a 2020 2020 2020 2020  aFrame..        
-0000c750: 2222 220d 0a20 2020 2020 2020 2064 6620  """..        df 
-0000c760: 3d20 7365 6c66 2e61 6461 7461 2e6f 6273  = self.adata.obs
-0000c770: 6d5b 2263 6e6d 665f 7573 6167 6522 5d2e  m["cnmf_usage"].
-0000c780: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-0000c790: 6466 2e63 6f6c 756d 6e73 203d 2070 642e  df.columns = pd.
-0000c7a0: 4d75 6c74 6949 6e64 6578 2e66 726f 6d5f  MultiIndex.from_
-0000c7b0: 7475 706c 6573 2864 662e 636f 6c75 6d6e  tuples(df.column
-0000c7c0: 732e 7374 722e 7370 6c69 7428 222e 2229  s.str.split(".")
-0000c7d0: 2e74 6f5f 6c69 7374 2829 290d 0a20 2020  .to_list())..   
-0000c7e0: 2020 2020 2064 662e 636f 6c75 6d6e 7320       df.columns 
-0000c7f0: 3d20 6466 2e63 6f6c 756d 6e73 2e73 6574  = df.columns.set
-0000c800: 5f6c 6576 656c 7328 5b6c 2e61 7374 7970  _levels([l.astyp
-0000c810: 6528 2269 6e74 2229 2066 6f72 206c 2069  e("int") for l i
-0000c820: 6e20 6466 2e63 6f6c 756d 6e73 2e6c 6576  n df.columns.lev
-0000c830: 656c 735d 290d 0a20 2020 2020 2020 2069  els])..        i
-0000c840: 6620 6e6f 726d 616c 697a 653a 0d0a 2020  f normalize:..  
-0000c850: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
-0000c860: 697a 6564 203d 205b 5d0d 0a20 2020 2020  ized = []..     
-0000c870: 2020 2020 2020 2066 6f72 205f 2c20 7375         for _, su
-0000c880: 6264 6620 696e 2064 662e 542e 6772 6f75  bdf in df.T.grou
-0000c890: 7062 7928 6c65 7665 6c3d 3029 3a0d 0a20  pby(level=0):.. 
-0000c8a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000c8b0: 6f72 6d61 6c69 7a65 642e 6170 7065 6e64  ormalized.append
-0000c8c0: 2873 7562 6466 2e64 6976 2873 7562 6466  (subdf.div(subdf
-0000c8d0: 2e73 756d 2829 2929 0d0a 2020 2020 2020  .sum()))..      
-0000c8e0: 2020 2020 2020 6466 203d 2070 642e 636f        df = pd.co
-0000c8f0: 6e63 6174 286e 6f72 6d61 6c69 7a65 6429  ncat(normalized)
-0000c900: 2e54 0d0a 2020 2020 2020 2020 6966 2064  .T..        if d
-0000c910: 6973 6372 6574 697a 653a 0d0a 2020 2020  iscretize:..    
-0000c920: 2020 2020 2020 2020 6469 7363 7265 7469          discreti
-0000c930: 7a65 6420 3d20 5b5d 0d0a 2020 2020 2020  zed = []..      
-0000c940: 2020 2020 2020 666f 7220 5f2c 2073 7562        for _, sub
-0000c950: 6466 2069 6e20 6466 2e54 2e67 726f 7570  df in df.T.group
-0000c960: 6279 286c 6576 656c 3d30 293a 0d0a 2020  by(level=0):..  
-0000c970: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0000c980: 7363 7265 7469 7a65 642e 6170 7065 6e64  scretized.append
-0000c990: 2873 7562 6466 2e65 7128 7375 6264 662e  (subdf.eq(subdf.
-0000c9a0: 6d61 7828 2929 2e61 7374 7970 6528 696e  max()).astype(in
-0000c9b0: 7429 290d 0a20 2020 2020 2020 2020 2020  t))..           
-0000c9c0: 2064 6620 3d20 7064 2e63 6f6e 6361 7428   df = pd.concat(
-0000c9d0: 6469 7363 7265 7469 7a65 6429 2e54 2020  discretized).T  
-0000c9e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c9f0: 6966 206b 2069 7320 6e6f 7420 4e6f 6e65  if k is not None
-0000ca00: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-0000ca10: 6620 3d20 6466 2e6c 6f63 5b3a 2c20 6b5d  f = df.loc[:, k]
-0000ca20: 0d0a 2020 2020 2020 2020 6466 203d 2064  ..        df = d
-0000ca30: 662e 736f 7274 5f69 6e64 6578 2861 7869  f.sort_index(axi
-0000ca40: 733d 3129 2020 200d 0a20 2020 2020 2020  s=1)   ..       
-0000ca50: 2072 6574 7572 6e20 6466 0d0a 0d0a 2020   return df....  
-0000ca60: 2020 6465 6620 6765 745f 7072 6f67 7261    def get_progra
-0000ca70: 6d73 2873 656c 662c 0d0a 2020 2020 2020  ms(self,..      
-0000ca80: 2020 2020 2020 2020 2020 206b 3a20 556e             k: Un
-0000ca90: 696f 6e5b 696e 742c 2049 7465 7261 626c  ion[int, Iterabl
-0000caa0: 655d 203d 204e 6f6e 652c 0d0a 2020 2020  e] = None,..    
-0000cab0: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-0000cac0: 653d 2263 6e6d 665f 6765 705f 7363 6f72  e="cnmf_gep_scor
-0000cad0: 6522 0d0a 2020 2020 2020 2020 2020 2020  e"..            
-0000cae0: 2020 2020 2029 202d 3e20 7064 2e44 6174       ) -> pd.Dat
-0000caf0: 6146 7261 6d65 3a0d 0a20 2020 2020 2020  aFrame:..       
-0000cb00: 2022 2222 0d0a 2020 2020 2020 2020 4765   """..        Ge
-0000cb10: 7420 6665 6174 7572 6520 7363 6f72 6573  t feature scores
-0000cb20: 2066 6f72 2070 726f 6772 616d 732e 0d0a   for programs...
-0000cb30: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000cb40: 206b 3a20 4966 2061 6e20 696e 7465 6765   k: If an intege
-0000cb50: 7220 6f72 206c 6973 7420 6f66 2069 6e74  r or list of int
-0000cb60: 6567 6572 732c 2072 6574 7572 6e73 2047  egers, returns G
-0000cb70: 4550 7320 6f6e 6c79 2066 6f72 2073 7065  EPs only for spe
-0000cb80: 6369 6669 6564 2072 616e 6b73 2e20 4f74  cified ranks. Ot
-0000cb90: 6865 7277 6973 652c 2072 6574 7572 6e73  herwise, returns
-0000cba0: 2047 4550 7320 6672 6f6d 2061 6c6c 2072   GEPs from all r
-0000cbb0: 616e 6b73 2e20 4465 6661 756c 7473 2074  anks. Defaults t
-0000cbc0: 6f20 4e6f 6e65 0d0a 2020 2020 2020 2020  o None..        
-0000cbd0: 3a74 7970 6520 6b3a 2055 6e69 6f6e 5b69  :type k: Union[i
-0000cbe0: 6e74 2c20 4974 6572 6162 6c65 5d2c 206f  nt, Iterable], o
-0000cbf0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0000cc00: 203a 7061 7261 6d20 7479 7065 3a20 2263   :param type: "c
-0000cc10: 6e6d 665f 6765 705f 7363 6f72 6522 206f  nmf_gep_score" o
-0000cc20: 7220 2263 6e6d 665f 6765 705f 7470 6d22  r "cnmf_gep_tpm"
-0000cc30: 2c20 6465 6661 756c 7473 2074 6f20 2263  , defaults to "c
-0000cc40: 6e6d 665f 6765 705f 7363 6f72 6522 0d0a  nmf_gep_score"..
-0000cc50: 2020 2020 2020 2020 3a74 7970 6520 7479          :type ty
-0000cc60: 7065 3a20 7374 722c 206f 7074 696f 6e61  pe: str, optiona
-0000cc70: 6c0d 0a20 2020 2020 2020 203a 7265 7475  l..        :retu
-0000cc80: 726e 3a20 6665 6174 7572 6573 20c3 9720  rn: features .. 
-0000cc90: 4745 5020 6d61 7472 6978 0d0a 2020 2020  GEP matrix..    
-0000cca0: 2020 2020 3a72 7479 7065 3a20 7064 2e44      :rtype: pd.D
-0000ccb0: 6174 6146 7261 6d65 0d0a 2020 2020 2020  ataFrame..      
-0000ccc0: 2020 2222 220d 0a20 2020 2020 2020 2061    """..        a
-0000ccd0: 7373 6572 7420 7365 6c66 2e68 6173 5f63  ssert self.has_c
-0000cce0: 6e6d 665f 7265 7375 6c74 730d 0a20 2020  nmf_results..   
-0000ccf0: 2020 2020 2064 6620 3d20 7365 6c66 2e61       df = self.a
-0000cd00: 6461 7461 2e76 6172 6d5b 7479 7065 5d2e  data.varm[type].
-0000cd10: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-0000cd20: 6466 2e63 6f6c 756d 6e73 203d 2070 642e  df.columns = pd.
-0000cd30: 4d75 6c74 6949 6e64 6578 2e66 726f 6d5f  MultiIndex.from_
-0000cd40: 7475 706c 6573 2864 662e 636f 6c75 6d6e  tuples(df.column
-0000cd50: 732e 7374 722e 7370 6c69 7428 222e 2229  s.str.split(".")
-0000cd60: 2e74 6f5f 6c69 7374 2829 290d 0a20 2020  .to_list())..   
-0000cd70: 2020 2020 2064 662e 636f 6c75 6d6e 7320       df.columns 
-0000cd80: 3d20 6466 2e63 6f6c 756d 6e73 2e73 6574  = df.columns.set
-0000cd90: 5f6c 6576 656c 7328 5b6c 2e61 7374 7970  _levels([l.astyp
-0000cda0: 6528 2269 6e74 2229 2066 6f72 206c 2069  e("int") for l i
-0000cdb0: 6e20 6466 2e63 6f6c 756d 6e73 2e6c 6576  n df.columns.lev
-0000cdc0: 656c 735d 290d 0a20 2020 2020 2020 2069  els])..        i
-0000cdd0: 6620 6973 696e 7374 616e 6365 286b 2c20  f isinstance(k, 
-0000cde0: 2869 6e74 2c20 6e70 2e69 6e74 6567 6572  (int, np.integer
-0000cdf0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-0000ce00: 2064 6620 3d20 6466 2e6c 6f63 5b3a 2c20   df = df.loc[:, 
-0000ce10: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
-0000ce20: 6466 203d 2064 662e 7265 6e61 6d65 5f61  df = df.rename_a
-0000ce30: 7869 7328 636f 6c75 6d6e 733d 5b22 7072  xis(columns=["pr
-0000ce40: 6f67 7261 6d22 5d29 2e73 6f72 745f 696e  ogram"]).sort_in
-0000ce50: 6465 7828 6178 6973 3d31 290d 0a20 2020  dex(axis=1)..   
-0000ce60: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000ce70: 616e 6365 286b 2c20 4974 6572 6162 6c65  ance(k, Iterable
-0000ce80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000ce90: 6466 203d 2064 662e 6c6f 635b 3a2c 206b  df = df.loc[:, k
-0000cea0: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
-0000ceb0: 6620 3d20 6466 2e72 656e 616d 655f 6178  f = df.rename_ax
-0000cec0: 6973 2863 6f6c 756d 6e73 3d5b 226b 222c  is(columns=["k",
-0000ced0: 2022 7072 6f67 7261 6d22 5d29 2e73 6f72   "program"]).sor
-0000cee0: 745f 696e 6465 7828 6178 6973 3d31 290d  t_index(axis=1).
-0000cef0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cf00: 6466 0d0a 2020 2020 0d0a 2020 2020 6465  df..    ..    de
-0000cf10: 6620 6765 745f 6170 7072 6f78 696d 6174  f get_approximat
-0000cf20: 696f 6e28 7365 6c66 2c0d 0a20 2020 2020  ion(self,..     
-0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 2020 2020 206b 3a20 4f70 7469 6f6e 616c       k: Optional
-0000cf50: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0d 0a20  [int] = None,.. 
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 2020 2020 2020 2020 2070 726f 6772 616d           program
-0000cf80: 5f74 7970 653a 204c 6974 6572 616c 5b22  _type: Literal["
-0000cf90: 636e 6d66 5f67 6570 5f74 706d 222c 2022  cnmf_gep_tpm", "
-0000cfa0: 636e 6d66 5f67 6570 5f72 6177 225d 203d  cnmf_gep_raw"] =
-0000cfb0: 2022 636e 6d66 5f67 6570 5f74 706d 220d   "cnmf_gep_tpm".
-0000cfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cfd0: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
-0000cfe0: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
-0000cff0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000d000: 2222 2252 6574 7572 6e20 7468 6520 6170  """Return the ap
-0000d010: 7072 6f78 696d 6174 6564 2064 6174 6120  proximated data 
-0000d020: 6279 206d 756c 7469 706c 7969 6e67 2074  by multiplying t
-0000d030: 6865 2070 726f 6772 616d 7320 616e 6420  he programs and 
-0000d040: 7573 6167 6520 6d61 7472 6963 6573 2066  usage matrices f
-0000d050: 6f72 2061 2067 6976 656e 2072 616e 6b20  or a given rank 
-0000d060: 286b 292e 2044 6566 6175 6c74 7320 746f  (k). Defaults to
-0000d070: 2074 6865 2068 6967 6865 7374 2072 616e   the highest ran
-0000d080: 6b20 6176 6169 6c61 626c 652e 0d0a 0d0a  k available.....
-0000d090: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-0000d0a0: 3a20 7261 6e6b 2c20 6465 6661 756c 7473  : rank, defaults
-0000d0b0: 2074 6f20 4e6f 6e65 0d0a 2020 2020 2020   to None..      
-0000d0c0: 2020 3a74 7970 6520 6b3a 2069 6e74 2c20    :type k: int, 
-0000d0d0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-0000d0e0: 2020 3a72 6574 7572 6e3a 2041 7070 726f    :return: Appro
-0000d0f0: 7869 6d61 7469 6f6e 206f 6620 6461 7461  ximation of data
-0000d100: 7365 7420 6261 7365 6420 6f6e 2070 726f  set based on pro
-0000d110: 6772 616d 7320 616e 6420 7573 6167 6573  grams and usages
-0000d120: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-0000d130: 3a20 7064 2e44 6174 6146 7261 6d65 0d0a  : pd.DataFrame..
-0000d140: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000d150: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0000d160: 2e68 6173 5f63 6e6d 665f 7265 7375 6c74  .has_cnmf_result
-0000d170: 730d 0a20 2020 2020 2020 2069 6620 6b20  s..        if k 
-0000d180: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-0000d190: 2020 2020 2020 6b20 3d20 7365 6c66 2e61        k = self.a
-0000d1a0: 6461 7461 2e75 6e73 5b22 6b76 616c 7322  data.uns["kvals"
-0000d1b0: 5d2e 696e 6465 782e 6d61 7828 290d 0a20  ].index.max().. 
-0000d1c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d1d0: 2061 7070 726f 7869 6d61 7469 6f6e 203d   approximation =
-0000d1e0: 2028 7365 6c66 2e67 6574 5f75 7361 6765   (self.get_usage
-0000d1f0: 7328 6b3d 6b29 2020 4020 7365 6c66 2e67  s(k=k)  @ self.g
-0000d200: 6574 5f70 726f 6772 616d 7328 7479 7065  et_programs(type
-0000d210: 3d70 726f 6772 616d 5f74 7970 652c 206b  =program_type, k
-0000d220: 3d6b 292e 5429 0d0a 0d0a 2020 2020 2020  =k).T)....      
-0000d230: 2020 7265 7475 726e 2061 7070 726f 7869    return approxi
-0000d240: 6d61 7469 6f6e 0d0a 2020 2020 2020 2020  mation..        
-0000d250: 0d0a 2020 2020 6465 6620 6361 6c63 756c  ..    def calcul
-0000d260: 6174 655f 636e 6d66 5f70 7265 6469 6374  ate_cnmf_predict
-0000d270: 696f 6e5f 6572 726f 7228 7365 6c66 2c0d  ion_error(self,.
-0000d280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 2020 2020 6b3a 204f 7074 696f          k: Optio
-0000d2b0: 6e61 6c5b 556e 696f 6e5b 696e 742c 2049  nal[Union[int, I
-0000d2c0: 7465 7261 626c 655d 5d20 3d20 4e6f 6e65  terable]] = None
-0000d2d0: 2920 2d3e 2055 6e69 6f6e 5b66 6c6f 6174  ) -> Union[float
-0000d2e0: 2c20 7064 2e53 6572 6965 735d 3a0d 0a20  , pd.Series]:.. 
-0000d2f0: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-0000d300: 6174 6520 634e 4d46 2070 7265 6469 6374  ate cNMF predict
-0000d310: 696f 6e20 6572 726f 7220 7573 696e 6720  ion error using 
-0000d320: 7468 6520 6d65 7468 6f64 2069 6e20 7468  the method in th
-0000d330: 6520 6f72 6967 696e 616c 2063 4e4d 4620  e original cNMF 
-0000d340: 7061 636b 6167 652e 0d0a 0d0a 2020 2020  package.....    
-0000d350: 2020 2020 3a70 6172 616d 206b 3a20 5370      :param k: Sp
-0000d360: 6563 6966 7920 6f6e 6520 6f72 206d 6f72  ecify one or mor
-0000d370: 6520 6b20 7661 6c75 6573 2074 6f20 6361  e k values to ca
-0000d380: 6c63 756c 6174 6520 7072 6564 6963 7469  lculate predicti
-0000d390: 6f6e 2065 7272 6f72 2e20 5370 6563 6966  on error. Specif
-0000d3a0: 7920 4e6f 6e65 2074 6f20 6361 6c63 756c  y None to calcul
-0000d3b0: 6174 6520 666f 7220 616c 6c20 6176 6169  ate for all avai
-0000d3c0: 6c61 626c 6520 6b2e 2064 6566 6175 6c74  lable k. default
-0000d3d0: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
-0000d3e0: 2020 203a 7479 7065 206b 3a20 4f70 7469     :type k: Opti
-0000d3f0: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
-0000d400: 4974 6572 6162 6c65 5d5d 2c20 6f70 7469  Iterable]], opti
-0000d410: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-0000d420: 6169 7365 7320 5661 6c75 6545 7272 6f72  aises ValueError
-0000d430: 3a20 6966 2069 6e76 616c 6964 206b 2069  : if invalid k i
-0000d440: 7320 7370 6563 6966 6965 640d 0a20 2020  s specified..   
-0000d450: 2020 2020 203a 7265 7475 726e 3a20 7363       :return: sc
-0000d460: 616c 6172 206f 7220 7665 6374 6f72 0d0a  alar or vector..
-0000d470: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-0000d480: 5f74 7970 655f 0d0a 2020 2020 2020 2020  _type_..        
-0000d490: 2222 220d 0a0d 0a20 2020 2020 2020 2066  """....        f
-0000d4a0: 726f 6d20 736b 6c65 6172 6e2e 6465 636f  rom sklearn.deco
-0000d4b0: 6d70 6f73 6974 696f 6e20 696d 706f 7274  mposition import
-0000d4c0: 206e 6f6e 5f6e 6567 6174 6976 655f 6661   non_negative_fa
-0000d4d0: 6374 6f72 697a 6174 696f 6e0d 0a0d 0a0d  ctorization.....
-0000d4e0: 0a20 2020 2020 2020 2069 6620 6b20 6973  .        if k is
-0000d4f0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000d500: 2020 2020 6b76 616c 7320 3d20 7365 6c66      kvals = self
-0000d510: 2e61 6461 7461 2e75 6e73 5b22 6b76 616c  .adata.uns["kval
-0000d520: 7322 5d2e 696e 6465 780d 0a20 2020 2020  s"].index..     
-0000d530: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-0000d540: 6365 286b 2c20 4974 6572 6162 6c65 293a  ce(k, Iterable):
-0000d550: 0d0a 2020 2020 2020 2020 2020 2020 6b76  ..            kv
-0000d560: 616c 7320 3d20 6b0d 0a20 2020 2020 2020  als = k..       
-0000d570: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0000d580: 286b 2c20 2869 6e74 2c20 6e70 2e69 6e74  (k, (int, np.int
-0000d590: 6567 6572 2929 3a0d 0a20 2020 2020 2020  eger)):..       
-0000d5a0: 2020 2020 206b 7661 6c73 203d 205b 6b5d       kvals = [k]
-0000d5b0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0000d5c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000d5d0: 7365 2056 616c 7565 4572 726f 720d 0a20  se ValueError.. 
-0000d5e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d5f0: 206e 6f72 6d5f 636f 756e 7473 203d 2073   norm_counts = s
-0000d600: 656c 662e 6164 6174 612e 746f 5f64 6628  elf.adata.to_df(
-0000d610: 292e 6c6f 635b 3a2c 2073 656c 662e 6164  ).loc[:, self.ad
-0000d620: 6174 612e 7661 725b 2273 656c 6563 7465  ata.var["selecte
-0000d630: 6422 5d5d 0d0a 2020 2020 2020 2020 6e6f  d"]]..        no
-0000d640: 726d 5f63 6f75 6e74 7320 2f3d 206e 6f72  rm_counts /= nor
-0000d650: 6d5f 636f 756e 7473 2e73 7464 2861 7869  m_counts.std(axi
-0000d660: 733d 302c 2064 646f 663d 3129 0d0a 0d0a  s=0, ddof=1)....
-0000d670: 2020 2020 2020 2020 7072 6564 5f65 7272          pred_err
-0000d680: 6f72 203d 2070 642e 5365 7269 6573 2869  or = pd.Series(i
-0000d690: 6e64 6578 3d6b 7661 6c73 2c20 6e61 6d65  ndex=kvals, name
-0000d6a0: 3d22 634e 4d46 2070 7265 6469 6374 696f  ="cNMF predictio
-0000d6b0: 6e5f 6572 726f 7222 290d 0a20 2020 2020  n_error")..     
-0000d6c0: 2020 2066 6f72 206b 7661 6c20 696e 206b     for kval in k
-0000d6d0: 7661 6c73 3a0d 0a20 2020 2020 2020 2020  vals:..         
-0000d6e0: 2020 2023 206f 6274 6169 6e20 7265 636f     # obtain reco
-0000d6f0: 6e73 7472 7563 7465 6420 6e6f 726d 616c  nstructed normal
-0000d700: 697a 6564 2063 6f75 6e74 7320 6d61 7472  ized counts matr
-0000d710: 6978 2062 7920 7265 2d66 6974 7469 6e67  ix by re-fitting
-0000d720: 2075 7361 6765 2061 6e64 2063 6f6d 7075   usage and compu
-0000d730: 7469 6e67 2064 6f74 2070 726f 6475 6374  ting dot product
-0000d740: 3a20 7573 6167 652e 646f 7428 7370 6563  : usage.dot(spec
-0000d750: 7472 6129 0d0a 2020 2020 2020 2020 2020  tra)..          
-0000d760: 2020 6d65 6469 616e 5f73 7065 6374 7261    median_spectra
-0000d770: 203d 2073 656c 662e 6765 745f 7072 6f67   = self.get_prog
-0000d780: 7261 6d73 286b 3d6b 7661 6c2c 2074 7970  rams(k=kval, typ
-0000d790: 653d 2263 6e6d 665f 6765 705f 7261 7722  e="cnmf_gep_raw"
-0000d7a0: 292e 6472 6f70 6e61 2829 0d0a 2020 2020  ).dropna()..    
-0000d7b0: 2020 2020 2020 2020 7266 5f75 7361 6765          rf_usage
-0000d7c0: 732c 2072 665f 7370 6563 7472 612c 206e  s, rf_spectra, n
-0000d7d0: 6974 6572 203d 206e 6f6e 5f6e 6567 6174  iter = non_negat
-0000d7e0: 6976 655f 6661 6374 6f72 697a 6174 696f  ive_factorizatio
-0000d7f0: 6e28 583d 6e6f 726d 5f63 6f75 6e74 732e  n(X=norm_counts.
-0000d800: 7661 6c75 6573 2e61 7374 7970 6528 6e70  values.astype(np
-0000d810: 2e66 6c6f 6174 3634 292c 0d0a 2020 2020  .float64),..    
-0000d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abb0: 2e63 6f70 7928 2920 2023 2063 6f70 7920  .copy()  # copy 
+0000abc0: 746f 2070 7265 7665 6e74 206f 7665 7277  to prevent overw
+0000abd0: 7269 7465 0d0a 2020 2020 2020 2020 2323  rite..        ##
+0000abe0: 2053 6361 6c65 2067 656e 6573 2074 6f20   Scale genes to 
+0000abf0: 756e 6974 2076 6172 6961 6e63 650d 0a20  unit variance.. 
+0000ac00: 2020 2020 2020 2069 6620 7370 2e69 7373         if sp.iss
+0000ac10: 7061 7273 6528 7470 6d2e 5829 3a0d 0a20  parse(tpm.X):.. 
+0000ac20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000ac30: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+0000ac40: 7272 6f72 2822 416e 6e44 6174 6173 2077  rror("AnnDatas w
+0000ac50: 6974 6820 7370 6172 7365 206d 6174 7269  ith sparse matri
+0000ac60: 6365 7320 6172 6520 6e6f 7420 7375 7070  ces are not supp
+0000ac70: 6f72 7465 6420 6279 206d 6f73 6169 634d  orted by mosaicM
+0000ac80: 5049 2079 6574 2e22 290d 0a20 2020 2020  PI yet.")..     
+0000ac90: 2020 2020 2020 2023 2073 632e 7070 2e73         # sc.pp.s
+0000aca0: 6361 6c65 286e 6f72 6d5f 636f 756e 7473  cale(norm_counts
+0000acb0: 2c20 7a65 726f 5f63 656e 7465 723d 4661  , zero_center=Fa
+0000acc0: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+0000acd0: 2020 2320 6966 206e 702e 6973 6e61 6e28    # if np.isnan(
+0000ace0: 6e6f 726d 5f63 6f75 6e74 732e 582e 6461  norm_counts.X.da
+0000acf0: 7461 292e 7375 6d28 2920 3e20 303a 0d0a  ta).sum() > 0:..
+0000ad00: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0000ad10: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000ad20: 6f72 2827 4e61 4e73 2069 6e20 6e6f 726d  or('NaNs in norm
+0000ad30: 616c 697a 6564 2063 6f75 6e74 7320 6d61  alized counts ma
+0000ad40: 7472 6978 2729 2020 2020 2020 2020 2020  trix')          
+0000ad50: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000ad60: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000ad70: 2020 2020 2020 2020 2020 6e6f 726d 5f63            norm_c
+0000ad80: 6f75 6e74 732e 5820 2f3d 206e 6f72 6d5f  ounts.X /= norm_
+0000ad90: 636f 756e 7473 2e58 2e73 7464 2861 7869  counts.X.std(axi
+0000ada0: 733d 302c 2064 646f 663d 3129 0d0a 2020  s=0, ddof=1)..  
+0000adb0: 2020 2020 2020 2020 2020 6966 206e 702e            if np.
+0000adc0: 6973 6e61 6e28 6e6f 726d 5f63 6f75 6e74  isnan(norm_count
+0000add0: 732e 5829 2e73 756d 2829 2e73 756d 2829  s.X).sum().sum()
+0000ade0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+0000adf0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0000ae00: 7565 4572 726f 7228 274e 614e 7320 696e  ueError('NaNs in
+0000ae10: 206e 6f72 6d61 6c69 7a65 6420 636f 756e   normalized coun
+0000ae20: 7473 206d 6174 7269 7827 2920 2020 2020  ts matrix')     
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000ae40: 0a0d 0a20 2020 2020 2020 2023 2320 5361  ...        ## Sa
+0000ae50: 7665 2061 205c 6e2d 6465 6c69 6d69 7465  ve a \n-delimite
+0000ae60: 6420 6c69 7374 206f 6620 7468 6520 6869  d list of the hi
+0000ae70: 6768 2d76 6172 6961 6e63 6520 6765 6e65  gh-variance gene
+0000ae80: 7320 7573 6564 2066 6f72 2066 6163 746f  s used for facto
+0000ae90: 7269 7a61 7469 6f6e 0d0a 2020 2020 2020  rization..      
+0000aea0: 2020 6f70 656e 2863 6e6d 665f 6f62 6a2e    open(cnmf_obj.
+0000aeb0: 7061 7468 735b 276e 6d66 5f67 656e 6573  paths['nmf_genes
+0000aec0: 5f6c 6973 7427 5d2c 2027 7727 292e 7772  _list'], 'w').wr
+0000aed0: 6974 6528 275c 6e27 2e6a 6f69 6e28 6f76  ite('\n'.join(ov
+0000aee0: 6572 6469 7370 6572 7365 645f 6765 6e65  erdispersed_gene
+0000aef0: 7329 290d 0a0d 0a20 2020 2020 2020 2069  s))....        i
+0000af00: 6620 6e6f 726d 5f63 6f75 6e74 732e 582e  f norm_counts.X.
+0000af10: 6474 7970 6520 213d 206e 702e 666c 6f61  dtype != np.floa
+0000af20: 7436 343a 0d0a 2020 2020 2020 2020 2020  t64:..          
+0000af30: 2020 6e6f 726d 5f63 6f75 6e74 732e 5820    norm_counts.X 
+0000af40: 3d20 6e6f 726d 5f63 6f75 6e74 732e 582e  = norm_counts.X.
+0000af50: 6173 7479 7065 286e 702e 666c 6f61 7436  astype(np.float6
+0000af60: 3429 0d0a 0d0a 2020 2020 2020 2020 6e6f  4)....        no
+0000af70: 726d 5f63 6f75 6e74 732e 7772 6974 655f  rm_counts.write_
+0000af80: 6835 6164 2863 6e6d 665f 6f62 6a2e 7061  h5ad(cnmf_obj.pa
+0000af90: 7468 735b 276e 6f72 6d61 6c69 7a65 645f  ths['normalized_
+0000afa0: 636f 756e 7473 275d 290d 0a0d 0a20 2020  counts'])....   
+0000afb0: 2020 2020 2023 2073 6176 6520 7061 7261       # save para
+0000afc0: 6d65 7465 7273 2066 6f72 2066 6163 746f  meters for facto
+0000afd0: 7269 7a61 7469 6f6e 2073 7465 700d 0a20  rization step.. 
+0000afe0: 2020 2020 2020 2063 6e6d 665f 6f62 6a2e         cnmf_obj.
+0000aff0: 7361 7665 5f6e 6d66 5f69 7465 725f 7061  save_nmf_iter_pa
+0000b000: 7261 6d73 282a 636e 6d66 5f6f 626a 2e67  rams(*cnmf_obj.g
+0000b010: 6574 5f6e 6d66 5f69 7465 725f 7061 7261  et_nmf_iter_para
+0000b020: 6d73 286b 733d 6b76 616c 732c 206e 5f69  ms(ks=kvals, n_i
+0000b030: 7465 723d 6e5f 6974 6572 2c20 7261 6e64  ter=n_iter, rand
+0000b040: 6f6d 5f73 7461 7465 5f73 6565 643d 7365  om_state_seed=se
+0000b050: 6564 2c20 6265 7461 5f6c 6f73 733d 6265  ed, beta_loss=be
+0000b060: 7461 5f6c 6f73 7329 290d 0a0d 0a20 2020  ta_loss))....   
+0000b070: 2020 2020 2023 2073 6176 6520 7061 7261       # save para
+0000b080: 6d65 7465 7273 2069 6e20 416e 6e44 6174  meters in AnnDat
+0000b090: 6120 6f62 6a65 6374 0d0a 2020 2020 2020  a object..      
+0000b0a0: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
+0000b0b0: 5b22 636e 6d66 225d 203d 2063 6e6d 665f  ["cnmf"] = cnmf_
+0000b0c0: 6f62 6a2e 6765 745f 6e6d 665f 6974 6572  obj.get_nmf_iter
+0000b0d0: 5f70 6172 616d 7328 6b73 3d6b 7661 6c73  _params(ks=kvals
+0000b0e0: 2c20 6e5f 6974 6572 3d6e 5f69 7465 722c  , n_iter=n_iter,
+0000b0f0: 2072 616e 646f 6d5f 7374 6174 655f 7365   random_state_se
+0000b100: 6564 3d73 6565 642c 2062 6574 615f 6c6f  ed=seed, beta_lo
+0000b110: 7373 3d62 6574 615f 6c6f 7373 295b 315d  ss=beta_loss)[1]
+0000b120: 2020 2320 6469 6374 206f 6620 636e 6d66    # dict of cnmf
+0000b130: 2070 6172 616d 6574 6572 730d 0a20 2020   parameters..   
+0000b140: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+0000b150: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
+0000b160: 7374 6f72 7928 6622 634e 4d46 2070 6172  story(f"cNMF par
+0000b170: 616d 6574 6572 7320 6164 6465 642e 2063  ameters added. c
+0000b180: 4e4d 4620 696e 7075 7473 2069 6e69 7469  NMF inputs initi
+0000b190: 616c 697a 6564 2069 6e20 7b63 6e6d 665f  alized in {cnmf_
+0000b1a0: 6f75 7470 7574 5f64 6972 7d2f 7b63 6e6d  output_dir}/{cnm
+0000b1b0: 665f 6e61 6d65 7d22 290d 0a20 2020 2020  f_name}")..     
+0000b1c0: 2020 2072 6574 7572 6e20 636e 6d66 5f6f     return cnmf_o
+0000b1d0: 626a 0d0a 2020 2020 0d0a 2020 2020 6465  bj..    ..    de
+0000b1e0: 6620 6164 645f 636e 6d66 5f72 6573 756c  f add_cnmf_resul
+0000b1f0: 7473 2873 656c 662c 2063 6e6d 665f 6f75  ts(self, cnmf_ou
+0000b200: 7470 7574 5f64 6972 2c20 636e 6d66 5f6e  tput_dir, cnmf_n
+0000b210: 616d 652c 206c 6f63 616c 5f64 656e 7369  ame, local_densi
+0000b220: 7479 5f74 6872 6573 686f 6c64 3a20 666c  ty_threshold: fl
+0000b230: 6f61 7420 3d20 4e6f 6e65 2c20 6c6f 6361  oat = None, loca
+0000b240: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
+0000b250: 697a 653a 2066 6c6f 6174 203d 204e 6f6e  ize: float = Non
+0000b260: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+0000b270: 0d0a 2020 2020 2020 2020 4166 7465 7220  ..        After 
+0000b280: 6661 6374 6f72 697a 6174 696f 6e2c 2061  factorization, a
+0000b290: 6464 2063 6f6d 706c 6574 6564 2063 4e4d  dd completed cNM
+0000b2a0: 4620 7265 7375 6c74 7320 696e 205b 636e  F results in [cn
+0000b2b0: 6d66 5f6f 7574 7075 745f 6469 725d 2f5b  mf_output_dir]/[
+0000b2c0: 636e 6d66 5f6e 616d 655d 2074 6f20 7468  cnmf_name] to th
+0000b2d0: 6520 6461 7461 7365 7420 6f62 6a65 6374  e dataset object
+0000b2e0: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
+0000b2f0: 7261 6d20 636e 6d66 5f6f 7574 7075 745f  ram cnmf_output_
+0000b300: 6469 723a 204f 7574 7075 7420 6469 7265  dir: Output dire
+0000b310: 6374 6f72 7920 666f 7220 634e 4d46 2072  ctory for cNMF r
+0000b320: 6573 756c 7473 0d0a 2020 2020 2020 2020  esults..        
+0000b330: 3a74 7970 6520 636e 6d66 5f6f 7574 7075  :type cnmf_outpu
+0000b340: 745f 6469 723a 2073 7472 0d0a 2020 2020  t_dir: str..    
+0000b350: 2020 2020 3a70 6172 616d 2063 6e6d 665f      :param cnmf_
+0000b360: 6e61 6d65 3a20 4e61 6d65 206f 6620 7468  name: Name of th
+0000b370: 6520 634e 4d46 2072 6573 756c 7473 2e20  e cNMF results. 
+0000b380: 4669 6c65 7320 7769 6c6c 2062 6520 6f75  Files will be ou
+0000b390: 7470 7574 2074 6f20 5b63 6e6d 665f 6f75  tput to [cnmf_ou
+0000b3a0: 7470 7574 5f64 6972 5d2f 5b63 6e6d 665f  tput_dir]/[cnmf_
+0000b3b0: 6e61 6d65 5d2f 0d0a 2020 2020 2020 2020  name]/..        
+0000b3c0: 3a74 7970 6520 636e 6d66 5f6e 616d 653a  :type cnmf_name:
+0000b3d0: 2073 7472 0d0a 2020 2020 2020 2020 3a70   str..        :p
+0000b3e0: 6172 616d 206c 6f63 616c 5f64 656e 7369  aram local_densi
+0000b3f0: 7479 5f74 6872 6573 686f 6c64 3a20 5468  ty_threshold: Th
+0000b400: 7265 7368 6f6c 6420 666f 7220 7468 6520  reshold for the 
+0000b410: 6c6f 6361 6c20 6465 6e73 6974 7920 6669  local density fi
+0000b420: 6c74 6572 696e 6720 7072 696f 7220 746f  ltering prior to
+0000b430: 2047 4550 2063 6f6e 7365 6e73 7573 2e20   GEP consensus. 
+0000b440: 4163 6365 7074 6162 6c65 2074 6872 6573  Acceptable thres
+0000b450: 686f 6c64 7320 6172 6520 3e20 3020 616e  holds are > 0 an
+0000b460: 6420 3c3d 2032 2028 322e 3020 6973 206e  d <= 2 (2.0 is n
+0000b470: 6f20 6669 6c74 6572 696e 6729 2e20 4465  o filtering). De
+0000b480: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
+0000b490: 0a20 2020 2020 2020 203a 7479 7065 206c  .        :type l
+0000b4a0: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
+0000b4b0: 6573 686f 6c64 3a20 666c 6f61 742c 206f  eshold: float, o
+0000b4c0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000b4d0: 203a 7061 7261 6d20 6c6f 6361 6c5f 6e65   :param local_ne
+0000b4e0: 6967 6862 6f72 686f 6f64 5f73 697a 653a  ighborhood_size:
+0000b4f0: 2046 7261 6374 696f 6e20 6f66 2074 6865   Fraction of the
+0000b500: 206e 756d 6265 7220 6f66 2072 6570 6c69   number of repli
+0000b510: 6361 7465 7320 746f 2075 7365 2061 7320  cates to use as 
+0000b520: 6e65 6172 6573 7420 6e65 6967 6862 6f72  nearest neighbor
+0000b530: 7320 666f 7220 6c6f 6361 6c20 6465 6e73  s for local dens
+0000b540: 6974 7920 6669 6c74 6572 696e 672e 2044  ity filtering. D
+0000b550: 6566 6175 6c74 7320 746f 204e 6f6e 650d  efaults to None.
+0000b560: 0a20 2020 2020 2020 203a 7479 7065 206c  .        :type l
+0000b570: 6f63 616c 5f6e 6569 6768 626f 7268 6f6f  ocal_neighborhoo
+0000b580: 645f 7369 7a65 3a20 666c 6f61 742c 206f  d_size: float, o
+0000b590: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000b5a0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+0000b5b0: 6c66 2e61 6461 7461 2e75 6e73 5b22 636e  lf.adata.uns["cn
+0000b5c0: 6d66 5f6e 616d 6522 5d20 3d20 636e 6d66  mf_name"] = cnmf
+0000b5d0: 5f6e 616d 650d 0a0d 0a20 2020 2020 2020  _name....       
+0000b5e0: 2023 2069 6e66 6572 2066 726f 6d20 6669   # infer from fi
+0000b5f0: 6c65 6e61 6d65 7320 7768 6963 6820 6c6f  lenames which lo
+0000b600: 6361 6c20 6465 6e73 6974 7920 7468 7265  cal density thre
+0000b610: 7368 6f6c 6420 7761 7320 7573 6564 0d0a  shold was used..
+0000b620: 2020 2020 2020 2020 7365 6e73 6564 5f6c          sensed_l
+0000b630: 6474 7320 3d20 7365 7428 290d 0a20 2020  dts = set()..   
+0000b640: 2020 2020 2066 6f72 2066 6e20 696e 2067       for fn in g
+0000b650: 6c6f 6228 6f73 2e70 6174 682e 6a6f 696e  lob(os.path.join
+0000b660: 2863 6e6d 665f 6f75 7470 7574 5f64 6972  (cnmf_output_dir
+0000b670: 2c20 636e 6d66 5f6e 616d 652c 2066 227b  , cnmf_name, f"{
+0000b680: 636e 6d66 5f6e 616d 657d 2a2e 2a73 7065  cnmf_name}*.*spe
+0000b690: 6374 7261 2a2e 6b5f 2a22 2929 3a0d 0a20  ctra*.k_*")):.. 
+0000b6a0: 2020 2020 2020 2020 2020 206c 6474 5f73             ldt_s
+0000b6b0: 7472 203d 206f 732e 7061 7468 2e62 6173  tr = os.path.bas
+0000b6c0: 656e 616d 6528 666e 292e 7370 6c69 7428  ename(fn).split(
+0000b6d0: 222e 2229 5b2d 335d 0d0a 2020 2020 2020  ".")[-3]..      
+0000b6e0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+0000b6f0: 2020 2020 2020 2020 2020 2020 6c64 7420              ldt 
+0000b700: 3d20 666c 6f61 7428 6c64 745f 7374 722e  = float(ldt_str.
+0000b710: 7265 706c 6163 6528 2264 745f 222c 2022  replace("dt_", "
+0000b720: 2229 2e72 6570 6c61 6365 2822 5f22 2c20  ").replace("_", 
+0000b730: 222e 2229 290d 0a20 2020 2020 2020 2020  "."))..         
+0000b740: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
+0000b750: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+0000b760: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
+0000b770: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b790: 7365 6e73 6564 5f6c 6474 732e 6164 6428  sensed_ldts.add(
+0000b7a0: 286c 6474 5f73 7472 2c20 6c64 7429 290d  (ldt_str, ldt)).
+0000b7b0: 0a20 2020 2020 2020 2069 6620 6c6f 6361  .        if loca
+0000b7c0: 6c5f 6465 6e73 6974 795f 7468 7265 7368  l_density_thresh
+0000b7d0: 6f6c 6420 6973 204e 6f6e 6520 616e 6420  old is None and 
+0000b7e0: 6c65 6e28 7365 6e73 6564 5f6c 6474 7329  len(sensed_ldts)
+0000b7f0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+0000b800: 2020 2020 6c64 745f 7374 722c 206c 6474      ldt_str, ldt
+0000b810: 203d 2073 656e 7365 645f 6c64 7473 2e70   = sensed_ldts.p
+0000b820: 6f70 2829 0d0a 2020 2020 2020 2020 656c  op()..        el
+0000b830: 6966 206c 6f63 616c 5f64 656e 7369 7479  if local_density
+0000b840: 5f74 6872 6573 686f 6c64 2069 6e20 286c  _threshold in (l
+0000b850: 6474 5b31 5d20 666f 7220 6c64 7420 696e  dt[1] for ldt in
+0000b860: 2073 656e 7365 645f 6c64 7473 293a 0d0a   sensed_ldts):..
+0000b870: 2020 2020 2020 2020 2020 2020 6c64 745f              ldt_
+0000b880: 7374 722c 206c 6474 203d 205b 286c 6474  str, ldt = [(ldt
+0000b890: 5f73 7472 2c20 6c64 7429 2066 6f72 206c  _str, ldt) for l
+0000b8a0: 6474 5f73 7472 2c20 6c64 7420 696e 2073  dt_str, ldt in s
+0000b8b0: 656e 7365 645f 6c64 7473 2069 6620 6c64  ensed_ldts if ld
+0000b8c0: 7420 3d3d 206c 6f63 616c 5f64 656e 7369  t == local_densi
+0000b8d0: 7479 5f74 6872 6573 686f 6c64 5d2e 706f  ty_threshold].po
+0000b8e0: 7028 290d 0a20 2020 2020 2020 2065 6c73  p()..        els
+0000b8f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000b900: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+0000b910: 6f72 2866 226c 6f63 616c 5f64 656e 7369  or(f"local_densi
+0000b920: 7479 5f74 6872 6573 686f 6c64 206f 6620  ty_threshold of 
+0000b930: 7b6c 6f63 616c 5f64 656e 7369 7479 5f74  {local_density_t
+0000b940: 6872 6573 686f 6c64 7d20 646f 6573 206e  hreshold} does n
+0000b950: 6f74 206d 6174 6368 2077 6861 7420 6973  ot match what is
+0000b960: 2069 6e20 7468 6520 634e 4d46 2072 6573   in the cNMF res
+0000b970: 756c 7420 6469 7265 6374 6f72 793a 207b  ult directory: {
+0000b980: 7365 6e73 6564 5f6c 6474 737d 2229 0d0a  sensed_ldts}")..
+0000b990: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+0000b9a0: 7461 2e75 6e73 5b22 6c64 7422 5d20 3d20  ta.uns["ldt"] = 
+0000b9b0: 6c64 740d 0a20 2020 2020 2020 2073 656c  ldt..        sel
+0000b9c0: 662e 6164 6174 612e 756e 735b 226c 6e73  f.adata.uns["lns
+0000b9d0: 225d 203d 206c 6f63 616c 5f6e 6569 6768  "] = local_neigh
+0000b9e0: 626f 7268 6f6f 645f 7369 7a65 0d0a 2020  borhood_size..  
+0000b9f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000ba00: 2020 2020 2320 496d 706f 7274 2047 4550      # Import GEP
+0000ba10: 730d 0a20 2020 2020 2020 2072 6573 756c  s..        resul
+0000ba20: 745f 7479 7065 7320 3d20 7b0d 0a20 2020  t_types = {..   
+0000ba30: 2020 2020 2020 2020 2022 6765 6e65 5f73           "gene_s
+0000ba40: 7065 6374 7261 5f73 636f 7265 223a 2022  pectra_score": "
+0000ba50: 636e 6d66 5f67 6570 5f73 636f 7265 222c  cnmf_gep_score",
+0000ba60: 0d0a 2020 2020 2020 2020 2020 2020 2267  ..            "g
+0000ba70: 656e 655f 7370 6563 7472 615f 7470 6d22  ene_spectra_tpm"
+0000ba80: 3a20 2263 6e6d 665f 6765 705f 7470 6d22  : "cnmf_gep_tpm"
+0000ba90: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+0000baa0: 7370 6563 7472 6122 3a20 2263 6e6d 665f  spectra": "cnmf_
+0000bab0: 6765 705f 7261 7722 0d0a 2020 2020 2020  gep_raw"..      
+0000bac0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+0000bad0: 2066 6f72 206d 6174 6368 7374 722c 2072   for matchstr, r
+0000bae0: 6573 756c 745f 7479 7065 2069 6e20 7265  esult_type in re
+0000baf0: 7375 6c74 5f74 7970 6573 2e69 7465 6d73  sult_types.items
+0000bb00: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0000bb10: 206c 6f67 6769 6e67 2e69 6e66 6f28 6622   logging.info(f"
+0000bb20: 496d 706f 7274 696e 6720 4745 5073 3a20  Importing GEPs: 
+0000bb30: 7b6d 6174 6368 7374 727d 2229 2020 0d0a  {matchstr}")  ..
+0000bb40: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+0000bb50: 5f77 203d 205b 5d0d 0a20 2020 2020 2020  _w = []..       
+0000bb60: 2020 2020 2066 6f72 2066 6e20 696e 2067       for fn in g
+0000bb70: 6c6f 6228 6f73 2e70 6174 682e 6a6f 696e  lob(os.path.join
+0000bb80: 2863 6e6d 665f 6f75 7470 7574 5f64 6972  (cnmf_output_dir
+0000bb90: 2c20 636e 6d66 5f6e 616d 652c 2066 227b  , cnmf_name, f"{
+0000bba0: 636e 6d66 5f6e 616d 657d 2a2e 7b6d 6174  cnmf_name}*.{mat
+0000bbb0: 6368 7374 727d 2e6b 5f2a 2e7b 6c64 745f  chstr}.k_*.{ldt_
+0000bbc0: 7374 727d 2e2a 7478 7422 2929 3a0d 0a20  str}.*txt")):.. 
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+0000bbe0: 203d 2069 6e74 286f 732e 7061 7468 2e62   = int(os.path.b
+0000bbf0: 6173 656e 616d 6528 666e 292e 7265 6d6f  asename(fn).remo
+0000bc00: 7665 7072 6566 6978 2866 227b 636e 6d66  veprefix(f"{cnmf
+0000bc10: 5f6e 616d 657d 2e7b 6d61 7463 6873 7472  _name}.{matchstr
+0000bc20: 7d2e 2229 2e73 706c 6974 2822 2e22 295b  }.").split(".")[
+0000bc30: 305d 2e72 6570 6c61 6365 2822 6b5f 222c  0].replace("k_",
+0000bc40: 2022 2229 290d 0a20 2020 2020 2020 2020   ""))..         
+0000bc50: 2020 2020 2020 2077 203d 2070 642e 7265         w = pd.re
+0000bc60: 6164 5f74 6162 6c65 2866 6e2c 2069 6e64  ad_table(fn, ind
+0000bc70: 6578 5f63 6f6c 3d30 290d 0a20 2020 2020  ex_col=0)..     
+0000bc80: 2020 2020 2020 2020 2020 2077 2e69 6e64             w.ind
+0000bc90: 6578 203d 2073 7472 286b 2920 2b20 222e  ex = str(k) + ".
+0000bca0: 2220 2b20 772e 696e 6465 782e 6173 7479  " + w.index.asty
+0000bcb0: 7065 2873 7472 290d 0a20 2020 2020 2020  pe(str)..       
+0000bcc0: 2020 2020 2020 2020 206d 6574 615f 772e           meta_w.
+0000bcd0: 6170 7065 6e64 2877 290d 0a20 2020 2020  append(w)..     
+0000bce0: 2020 2020 2020 206d 6574 615f 7720 3d20         meta_w = 
+0000bcf0: 7064 2e63 6f6e 6361 7428 6d65 7461 5f77  pd.concat(meta_w
+0000bd00: 2c20 6178 6973 3d30 292e 542e 7265 696e  , axis=0).T.rein
+0000bd10: 6465 7828 7365 6c66 2e61 6461 7461 2e76  dex(self.adata.v
+0000bd20: 6172 2e69 6e64 6578 292e 7265 6e61 6d65  ar.index).rename
+0000bd30: 5f61 7869 7328 5b22 6b2e 6765 7022 5d2c  _axis(["k.gep"],
+0000bd40: 2061 7869 733d 3129 0d0a 2020 2020 2020   axis=1)..      
+0000bd50: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+0000bd60: 2e76 6172 6d5b 7265 7375 6c74 5f74 7970  .varm[result_typ
+0000bd70: 655d 203d 206d 6574 615f 770d 0a0d 0a20  e] = meta_w.... 
+0000bd80: 2020 2020 2020 2023 2049 6d70 6f72 7420         # Import 
+0000bd90: 5573 6167 6573 0d0a 2020 2020 2020 2020  Usages..        
+0000bda0: 6c6f 6767 696e 672e 696e 666f 2866 2249  logging.info(f"I
+0000bdb0: 6d70 6f72 7469 6e67 2055 7361 6765 7322  mporting Usages"
+0000bdc0: 2920 200d 0a20 2020 2020 2020 2075 7361  )  ..        usa
+0000bdd0: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+0000bde0: 2066 6f72 2066 6e20 696e 2067 6c6f 6228   for fn in glob(
+0000bdf0: 6f73 2e70 6174 682e 6a6f 696e 2863 6e6d  os.path.join(cnm
+0000be00: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
+0000be10: 6d66 5f6e 616d 652c 2066 227b 636e 6d66  mf_name, f"{cnmf
+0000be20: 5f6e 616d 657d 2a2e 7573 6167 6573 2e6b  _name}*.usages.k
+0000be30: 5f2a 2e7b 6c64 745f 7374 727d 2e2a 7478  _*.{ldt_str}.*tx
+0000be40: 7422 2929 3a0d 0a20 2020 2020 2020 2020  t")):..         
+0000be50: 2020 206b 203d 2069 6e74 286f 732e 7061     k = int(os.pa
+0000be60: 7468 2e62 6173 656e 616d 6528 666e 292e  th.basename(fn).
+0000be70: 7265 6d6f 7665 7072 6566 6978 2866 227b  removeprefix(f"{
+0000be80: 636e 6d66 5f6e 616d 657d 2e75 7361 6765  cnmf_name}.usage
+0000be90: 732e 2229 2e73 706c 6974 2822 2e22 295b  s.").split(".")[
+0000bea0: 305d 2e72 6570 6c61 6365 2822 6b5f 222c  0].replace("k_",
+0000beb0: 2022 2229 290d 0a20 2020 2020 2020 2020   ""))..         
+0000bec0: 2020 2068 203d 2070 642e 7265 6164 5f74     h = pd.read_t
+0000bed0: 6162 6c65 2866 6e2c 2069 6e64 6578 5f63  able(fn, index_c
+0000bee0: 6f6c 3d30 290d 0a20 2020 2020 2020 2020  ol=0)..         
+0000bef0: 2020 2068 2e63 6f6c 756d 6e73 203d 2073     h.columns = s
+0000bf00: 7472 286b 2920 2b20 222e 2220 2b20 682e  tr(k) + "." + h.
+0000bf10: 636f 6c75 6d6e 732e 6173 7479 7065 2873  columns.astype(s
+0000bf20: 7472 290d 0a20 2020 2020 2020 2020 2020  tr)..           
+0000bf30: 2075 7361 6765 2e61 7070 656e 6428 6829   usage.append(h)
+0000bf40: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+0000bf50: 6461 7461 2e6f 6273 6d5b 2263 6e6d 665f  data.obsm["cnmf_
+0000bf60: 7573 6167 6522 5d20 3d20 7064 2e63 6f6e  usage"] = pd.con
+0000bf70: 6361 7428 7573 6167 652c 2061 7869 733d  cat(usage, axis=
+0000bf80: 3129 2e73 6f72 745f 696e 6465 7828 6178  1).sort_index(ax
+0000bf90: 6973 3d31 292e 7265 6e61 6d65 5f61 7869  is=1).rename_axi
+0000bfa0: 7328 5b22 6b2e 6765 7022 5d2c 2061 7869  s(["k.gep"], axi
+0000bfb0: 733d 3129 0d0a 2020 2020 2020 2020 0d0a  s=1)..        ..
+0000bfc0: 2020 2020 2020 2020 2320 496d 706f 7274          # Import
+0000bfd0: 2067 656e 6520 6c69 7374 2075 7365 6420   gene list used 
+0000bfe0: 666f 7220 6661 6374 6f72 697a 6174 696f  for factorizatio
+0000bff0: 6e0d 0a20 2020 2020 2020 2077 6974 6820  n..        with 
+0000c000: 6f70 656e 286f 732e 7061 7468 2e6a 6f69  open(os.path.joi
+0000c010: 6e28 636e 6d66 5f6f 7574 7075 745f 6469  n(cnmf_output_di
+0000c020: 722c 2063 6e6d 665f 6e61 6d65 2c20 6622  r, cnmf_name, f"
+0000c030: 7b63 6e6d 665f 6e61 6d65 7d2e 6f76 6572  {cnmf_name}.over
+0000c040: 6469 7370 6572 7365 645f 6765 6e65 732e  dispersed_genes.
+0000c050: 7478 7422 2929 2061 7320 663a 0d0a 2020  txt")) as f:..  
+0000c060: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c070: 6461 7461 2e75 6e73 5b22 6765 6e65 5f6c  data.uns["gene_l
+0000c080: 6973 7422 5d20 3d20 5b6c 696e 652e 7374  ist"] = [line.st
+0000c090: 7269 7028 2920 666f 7220 6c69 6e65 2069  rip() for line i
+0000c0a0: 6e20 662e 7265 6164 6c69 6e65 7328 295d  n f.readlines()]
+0000c0b0: 0d0a 0d0a 2020 2020 2020 2020 2320 496d  ....        # Im
+0000c0c0: 706f 7274 204b 2d73 656c 6563 7469 6f6e  port K-selection
+0000c0d0: 2073 7461 7473 0d0a 2020 2020 2020 2020   stats..        
+0000c0e0: 6b76 616c 7320 3d20 7064 2e44 6174 6146  kvals = pd.DataF
+0000c0f0: 7261 6d65 282a 2a6e 702e 6c6f 6164 286f  rame(**np.load(o
+0000c100: 732e 7061 7468 2e6a 6f69 6e28 636e 6d66  s.path.join(cnmf
+0000c110: 5f6f 7574 7075 745f 6469 722c 2063 6e6d  _output_dir, cnm
+0000c120: 665f 6e61 6d65 2c20 6622 7b63 6e6d 665f  f_name, f"{cnmf_
+0000c130: 6e61 6d65 7d2e 6b5f 7365 6c65 6374 696f  name}.k_selectio
+0000c140: 6e5f 7374 6174 732e 6466 2e6e 707a 2229  n_stats.df.npz")
+0000c150: 2c20 616c 6c6f 775f 7069 636b 6c65 3d54  , allow_pickle=T
+0000c160: 7275 6529 292e 7365 745f 696e 6465 7828  rue)).set_index(
+0000c170: 226b 2229 5b5b 2273 7461 6269 6c69 7479  "k")[["stability
+0000c180: 222c 2022 7072 6564 6963 7469 6f6e 5f65  ", "prediction_e
+0000c190: 7272 6f72 225d 5d0d 0a20 2020 2020 2020  rror"]]..       
+0000c1a0: 206b 7661 6c73 2e69 6e64 6578 203d 206b   kvals.index = k
+0000c1b0: 7661 6c73 2e69 6e64 6578 2e61 7374 7970  vals.index.astyp
+0000c1c0: 6528 696e 7429 0d0a 2020 2020 2020 2020  e(int)..        
+0000c1d0: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+0000c1e0: 6b76 616c 7322 5d20 3d20 6b76 616c 730d  kvals"] = kvals.
+0000c1f0: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
+0000c200: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
+0000c210: 2263 4e4d 4620 7265 7375 6c74 7320 6164  "cNMF results ad
+0000c220: 6465 6420 6672 6f6d 206f 7574 7075 7420  ded from output 
+0000c230: 6469 7265 6374 6f72 7920 7b63 6e6d 665f  directory {cnmf_
+0000c240: 6f75 7470 7574 5f64 6972 7d2f 7b63 6e6d  output_dir}/{cnm
+0000c250: 665f 6e61 6d65 7d22 290d 0a0d 0a20 2020  f_name}")....   
+0000c260: 2064 6566 2072 656d 6f76 655f 636e 6d66   def remove_cnmf
+0000c270: 5f72 6573 756c 7473 2873 656c 6629 3a0d  _results(self):.
+0000c280: 0a20 2020 2020 2020 2066 6f72 2072 6573  .        for res
+0000c290: 756c 745f 7479 7065 2069 6e20 2822 636e  ult_type in ("cn
+0000c2a0: 6d66 5f67 6570 5f73 636f 7265 222c 2022  mf_gep_score", "
+0000c2b0: 636e 6d66 5f67 6570 5f74 706d 222c 2022  cnmf_gep_tpm", "
+0000c2c0: 636e 6d66 5f67 6570 5f72 6177 2229 3a0d  cnmf_gep_raw"):.
+0000c2d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c2e0: 662e 6164 6174 612e 7661 726d 2e70 6f70  f.adata.varm.pop
+0000c2f0: 2872 6573 756c 745f 7479 7065 290d 0a20  (result_type).. 
+0000c300: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+0000c310: 612e 6f62 736d 2e70 6f70 2822 636e 6d66  a.obsm.pop("cnmf
+0000c320: 5f75 7361 6765 2229 0d0a 2020 2020 2020  _usage")..      
+0000c330: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
+0000c340: 2e70 6f70 2822 6765 6e65 5f6c 6973 7422  .pop("gene_list"
+0000c350: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000c360: 6164 6174 612e 756e 732e 706f 7028 226b  adata.uns.pop("k
+0000c370: 7661 6c73 2229 0d0a 2020 2020 2020 2020  vals")..        
+0000c380: 7365 6c66 2e61 7070 656e 645f 746f 5f68  self.append_to_h
+0000c390: 6973 746f 7279 2822 634e 4d46 2072 6573  istory("cNMF res
+0000c3a0: 756c 7473 2072 656d 6f76 6564 2e22 290d  ults removed.").
+0000c3b0: 0a0d 0a0d 0a20 2020 2064 6566 2067 6574  .....    def get
+0000c3c0: 5f75 7361 6765 7328 7365 6c66 2c0d 0a20  _usages(self,.. 
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3e0: 2020 6b3a 2055 6e69 6f6e 5b69 6e74 2c20    k: Union[int, 
+0000c3f0: 4974 6572 6162 6c65 5d20 3d20 4e6f 6e65  Iterable] = None
+0000c400: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c410: 2020 2020 2020 6469 7363 7265 7469 7a65        discretize
+0000c420: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+0000c430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c440: 2020 2020 6e6f 726d 616c 697a 653a 2062      normalize: b
+0000c450: 6f6f 6c20 3d20 4661 6c73 650d 0a20 2020  ool = False..   
+0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c470: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
+0000c480: 653a 0d0a 2020 2020 2020 2020 2222 220d  e:..        """.
+0000c490: 0a20 2020 2020 2020 2043 616c 6375 6c61  .        Calcula
+0000c4a0: 7465 2075 7361 6765 206f 6620 6561 6368  te usage of each
+0000c4b0: 2047 4550 2069 6e20 6561 6368 2073 616d   GEP in each sam
+0000c4c0: 706c 652f 6f62 7365 7276 6174 696f 6e2e  ple/observation.
+0000c4d0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
+0000c4e0: 616d 206b 3a20 4966 2061 6e20 696e 7465  am k: If an inte
+0000c4f0: 6765 7220 6f72 206c 6973 7420 6f66 2069  ger or list of i
+0000c500: 6e74 6567 6572 732c 2072 6574 7572 6e73  ntegers, returns
+0000c510: 2075 7361 6765 7320 6f6e 6c79 2066 6f72   usages only for
+0000c520: 2073 7065 6369 6669 6564 2072 616e 6b73   specified ranks
+0000c530: 2e20 4f74 6865 7277 6973 652c 2072 6574  . Otherwise, ret
+0000c540: 7572 6e73 2075 7361 6765 206f 6620 616c  urns usage of al
+0000c550: 6c20 4745 5073 2061 6372 6f73 7320 7261  l GEPs across ra
+0000c560: 6e6b 732e 2044 6566 6175 6c74 7320 746f  nks. Defaults to
+0000c570: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
+0000c580: 7479 7065 206b 3a20 696e 742c 206f 7074  type k: int, opt
+0000c590: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+0000c5a0: 7061 7261 6d20 6469 7363 7265 7469 7a65  param discretize
+0000c5b0: 3a20 4469 7363 7265 7469 7a65 7320 7468  : Discretizes th
+0000c5c0: 6520 7573 6167 6520 6d61 7472 6978 2073  e usage matrix s
+0000c5d0: 7563 6820 7468 6174 2066 6f72 2065 6163  uch that for eac
+0000c5e0: 6820 7661 6c75 6520 6f66 206b 2c20 6561  h value of k, ea
+0000c5f0: 6368 2073 616d 706c 6520 6861 7320 7573  ch sample has us
+0000c600: 6167 6520 6f66 206f 6e6c 7920 3120 4745  age of only 1 GE
+0000c610: 5020 2874 6865 206f 6e65 2077 6974 6820  P (the one with 
+0000c620: 7468 6520 6d61 7869 6d75 6d20 7573 6167  the maximum usag
+0000c630: 6529 2e20 4465 6661 756c 7473 2074 6f20  e). Defaults to 
+0000c640: 4661 6c73 650d 0a20 2020 2020 2020 203a  False..        :
+0000c650: 7479 7065 2064 6973 6372 6574 697a 653a  type discretize:
+0000c660: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+0000c670: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000c680: 6e6f 726d 616c 697a 653a 204e 6f72 6d61  normalize: Norma
+0000c690: 6c69 7a65 2074 6865 2047 4550 2075 7361  lize the GEP usa
+0000c6a0: 6765 206d 6174 7269 7820 7375 6368 2074  ge matrix such t
+0000c6b0: 6861 7420 666f 7220 6561 6368 2076 616c  hat for each val
+0000c6c0: 7565 206f 6620 6b2c 2075 7361 6765 206f  ue of k, usage o
+0000c6d0: 6620 616c 6c20 4745 5073 2073 756d 7320  f all GEPs sums 
+0000c6e0: 746f 2031 2e20 4465 6661 756c 7473 2074  to 1. Defaults t
+0000c6f0: 6f20 4661 6c73 650d 0a20 2020 2020 2020  o False..       
+0000c700: 203a 7479 7065 206e 6f72 6d61 6c69 7a65   :type normalize
+0000c710: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+0000c720: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+0000c730: 6e3a 206f 6273 6572 7661 7469 6f6e 20c3  n: observation .
+0000c740: 9720 4745 5020 6d61 7472 6978 0d0a 2020  . GEP matrix..  
+0000c750: 2020 2020 2020 3a72 7479 7065 3a20 7064        :rtype: pd
+0000c760: 2e44 6174 6146 7261 6d65 0d0a 2020 2020  .DataFrame..    
+0000c770: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000c780: 2064 6620 3d20 7365 6c66 2e61 6461 7461   df = self.adata
+0000c790: 2e6f 6273 6d5b 2263 6e6d 665f 7573 6167  .obsm["cnmf_usag
+0000c7a0: 6522 5d2e 636f 7079 2829 0d0a 2020 2020  e"].copy()..    
+0000c7b0: 2020 2020 6466 2e63 6f6c 756d 6e73 203d      df.columns =
+0000c7c0: 2070 642e 4d75 6c74 6949 6e64 6578 2e66   pd.MultiIndex.f
+0000c7d0: 726f 6d5f 7475 706c 6573 2864 662e 636f  rom_tuples(df.co
+0000c7e0: 6c75 6d6e 732e 7374 722e 7370 6c69 7428  lumns.str.split(
+0000c7f0: 222e 2229 2e74 6f5f 6c69 7374 2829 290d  ".").to_list()).
+0000c800: 0a20 2020 2020 2020 2064 662e 636f 6c75  .        df.colu
+0000c810: 6d6e 7320 3d20 6466 2e63 6f6c 756d 6e73  mns = df.columns
+0000c820: 2e73 6574 5f6c 6576 656c 7328 5b6c 2e61  .set_levels([l.a
+0000c830: 7374 7970 6528 2269 6e74 2229 2066 6f72  stype("int") for
+0000c840: 206c 2069 6e20 6466 2e63 6f6c 756d 6e73   l in df.columns
+0000c850: 2e6c 6576 656c 735d 290d 0a20 2020 2020  .levels])..     
+0000c860: 2020 2069 6620 6e6f 726d 616c 697a 653a     if normalize:
+0000c870: 0d0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
+0000c880: 726d 616c 697a 6564 203d 205b 5d0d 0a20  rmalized = [].. 
+0000c890: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
+0000c8a0: 2c20 7375 6264 6620 696e 2064 662e 542e  , subdf in df.T.
+0000c8b0: 6772 6f75 7062 7928 6c65 7665 6c3d 3029  groupby(level=0)
+0000c8c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c8d0: 2020 206e 6f72 6d61 6c69 7a65 642e 6170     normalized.ap
+0000c8e0: 7065 6e64 2873 7562 6466 2e64 6976 2873  pend(subdf.div(s
+0000c8f0: 7562 6466 2e73 756d 2829 2929 0d0a 2020  ubdf.sum()))..  
+0000c900: 2020 2020 2020 2020 2020 6466 203d 2070            df = p
+0000c910: 642e 636f 6e63 6174 286e 6f72 6d61 6c69  d.concat(normali
+0000c920: 7a65 6429 2e54 0d0a 2020 2020 2020 2020  zed).T..        
+0000c930: 6966 2064 6973 6372 6574 697a 653a 0d0a  if discretize:..
+0000c940: 2020 2020 2020 2020 2020 2020 6469 7363              disc
+0000c950: 7265 7469 7a65 6420 3d20 5b5d 0d0a 2020  retized = []..  
+0000c960: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
+0000c970: 2073 7562 6466 2069 6e20 6466 2e54 2e67   subdf in df.T.g
+0000c980: 726f 7570 6279 286c 6576 656c 3d30 293a  roupby(level=0):
+0000c990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c9a0: 2020 6469 7363 7265 7469 7a65 642e 6170    discretized.ap
+0000c9b0: 7065 6e64 2873 7562 6466 2e65 7128 7375  pend(subdf.eq(su
+0000c9c0: 6264 662e 6d61 7828 2929 2e61 7374 7970  bdf.max()).astyp
+0000c9d0: 6528 696e 7429 290d 0a20 2020 2020 2020  e(int))..       
+0000c9e0: 2020 2020 2064 6620 3d20 7064 2e63 6f6e       df = pd.con
+0000c9f0: 6361 7428 6469 7363 7265 7469 7a65 6429  cat(discretized)
+0000ca00: 2e54 2020 2020 2020 2020 0d0a 2020 2020  .T        ..    
+0000ca10: 2020 2020 6966 206b 2069 7320 6e6f 7420      if k is not 
+0000ca20: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000ca30: 2020 2064 6620 3d20 6466 2e6c 6f63 5b3a     df = df.loc[:
+0000ca40: 2c20 6b5d 0d0a 2020 2020 2020 2020 6466  , k]..        df
+0000ca50: 203d 2064 662e 736f 7274 5f69 6e64 6578   = df.sort_index
+0000ca60: 2861 7869 733d 3129 2020 200d 0a20 2020  (axis=1)   ..   
+0000ca70: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+0000ca80: 0d0a 2020 2020 6465 6620 6765 745f 7072  ..    def get_pr
+0000ca90: 6f67 7261 6d73 2873 656c 662c 0d0a 2020  ograms(self,..  
+0000caa0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+0000cab0: 3a20 556e 696f 6e5b 696e 742c 2049 7465  : Union[int, Ite
+0000cac0: 7261 626c 655d 203d 204e 6f6e 652c 0d0a  rable] = None,..
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cae0: 2074 7970 653d 2263 6e6d 665f 6765 705f   type="cnmf_gep_
+0000caf0: 7363 6f72 6522 0d0a 2020 2020 2020 2020  score"..        
+0000cb00: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
+0000cb10: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
+0000cb20: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000cb30: 2020 4765 7420 6665 6174 7572 6520 7363    Get feature sc
+0000cb40: 6f72 6573 2066 6f72 2070 726f 6772 616d  ores for program
+0000cb50: 732e 0d0a 0d0a 2020 2020 2020 2020 3a70  s.....        :p
+0000cb60: 6172 616d 206b 3a20 4966 2061 6e20 696e  aram k: If an in
+0000cb70: 7465 6765 7220 6f72 206c 6973 7420 6f66  teger or list of
+0000cb80: 2069 6e74 6567 6572 732c 2072 6574 7572   integers, retur
+0000cb90: 6e73 2047 4550 7320 6f6e 6c79 2066 6f72  ns GEPs only for
+0000cba0: 2073 7065 6369 6669 6564 2072 616e 6b73   specified ranks
+0000cbb0: 2e20 4f74 6865 7277 6973 652c 2072 6574  . Otherwise, ret
+0000cbc0: 7572 6e73 2047 4550 7320 6672 6f6d 2061  urns GEPs from a
+0000cbd0: 6c6c 2072 616e 6b73 2e20 4465 6661 756c  ll ranks. Defaul
+0000cbe0: 7473 2074 6f20 4e6f 6e65 0d0a 2020 2020  ts to None..    
+0000cbf0: 2020 2020 3a74 7970 6520 6b3a 2055 6e69      :type k: Uni
+0000cc00: 6f6e 5b69 6e74 2c20 4974 6572 6162 6c65  on[int, Iterable
+0000cc10: 5d2c 206f 7074 696f 6e61 6c0d 0a20 2020  ], optional..   
+0000cc20: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
+0000cc30: 3a20 2263 6e6d 665f 6765 705f 7363 6f72  : "cnmf_gep_scor
+0000cc40: 6522 206f 7220 2263 6e6d 665f 6765 705f  e" or "cnmf_gep_
+0000cc50: 7470 6d22 2c20 6465 6661 756c 7473 2074  tpm", defaults t
+0000cc60: 6f20 2263 6e6d 665f 6765 705f 7363 6f72  o "cnmf_gep_scor
+0000cc70: 6522 0d0a 2020 2020 2020 2020 3a74 7970  e"..        :typ
+0000cc80: 6520 7479 7065 3a20 7374 722c 206f 7074  e type: str, opt
+0000cc90: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+0000cca0: 7265 7475 726e 3a20 6665 6174 7572 6573  return: features
+0000ccb0: 20c3 9720 4745 5020 6d61 7472 6978 0d0a   .. GEP matrix..
+0000ccc0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+0000ccd0: 7064 2e44 6174 6146 7261 6d65 0d0a 2020  pd.DataFrame..  
+0000cce0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000ccf0: 2020 2061 7373 6572 7420 7365 6c66 2e68     assert self.h
+0000cd00: 6173 5f63 6e6d 665f 7265 7375 6c74 730d  as_cnmf_results.
+0000cd10: 0a20 2020 2020 2020 2064 6620 3d20 7365  .        df = se
+0000cd20: 6c66 2e61 6461 7461 2e76 6172 6d5b 7479  lf.adata.varm[ty
+0000cd30: 7065 5d2e 636f 7079 2829 0d0a 2020 2020  pe].copy()..    
+0000cd40: 2020 2020 6466 2e63 6f6c 756d 6e73 203d      df.columns =
+0000cd50: 2070 642e 4d75 6c74 6949 6e64 6578 2e66   pd.MultiIndex.f
+0000cd60: 726f 6d5f 7475 706c 6573 2864 662e 636f  rom_tuples(df.co
+0000cd70: 6c75 6d6e 732e 7374 722e 7370 6c69 7428  lumns.str.split(
+0000cd80: 222e 2229 2e74 6f5f 6c69 7374 2829 290d  ".").to_list()).
+0000cd90: 0a20 2020 2020 2020 2064 662e 636f 6c75  .        df.colu
+0000cda0: 6d6e 7320 3d20 6466 2e63 6f6c 756d 6e73  mns = df.columns
+0000cdb0: 2e73 6574 5f6c 6576 656c 7328 5b6c 2e61  .set_levels([l.a
+0000cdc0: 7374 7970 6528 2269 6e74 2229 2066 6f72  stype("int") for
+0000cdd0: 206c 2069 6e20 6466 2e63 6f6c 756d 6e73   l in df.columns
+0000cde0: 2e6c 6576 656c 735d 290d 0a20 2020 2020  .levels])..     
+0000cdf0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000ce00: 286b 2c20 2869 6e74 2c20 6e70 2e69 6e74  (k, (int, np.int
+0000ce10: 6567 6572 2929 3a0d 0a20 2020 2020 2020  eger)):..       
+0000ce20: 2020 2020 2064 6620 3d20 6466 2e6c 6f63       df = df.loc
+0000ce30: 5b3a 2c20 6b5d 0d0a 2020 2020 2020 2020  [:, k]..        
+0000ce40: 2020 2020 6466 203d 2064 662e 7265 6e61      df = df.rena
+0000ce50: 6d65 5f61 7869 7328 636f 6c75 6d6e 733d  me_axis(columns=
+0000ce60: 5b22 7072 6f67 7261 6d22 5d29 2e73 6f72  ["program"]).sor
+0000ce70: 745f 696e 6465 7828 6178 6973 3d31 290d  t_index(axis=1).
+0000ce80: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+0000ce90: 696e 7374 616e 6365 286b 2c20 4974 6572  instance(k, Iter
+0000cea0: 6162 6c65 293a 0d0a 2020 2020 2020 2020  able):..        
+0000ceb0: 2020 2020 6466 203d 2064 662e 6c6f 635b      df = df.loc[
+0000cec0: 3a2c 206b 5d0d 0a20 2020 2020 2020 2020  :, k]..         
+0000ced0: 2020 2064 6620 3d20 6466 2e72 656e 616d     df = df.renam
+0000cee0: 655f 6178 6973 2863 6f6c 756d 6e73 3d5b  e_axis(columns=[
+0000cef0: 226b 222c 2022 7072 6f67 7261 6d22 5d29  "k", "program"])
+0000cf00: 2e73 6f72 745f 696e 6465 7828 6178 6973  .sort_index(axis
+0000cf10: 3d31 290d 0a20 2020 2020 2020 2072 6574  =1)..        ret
+0000cf20: 7572 6e20 6466 0d0a 2020 2020 0d0a 2020  urn df..    ..  
+0000cf30: 2020 6465 6620 6765 745f 6170 7072 6f78    def get_approx
+0000cf40: 696d 6174 696f 6e28 7365 6c66 2c0d 0a20  imation(self,.. 
+0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf60: 2020 2020 2020 2020 206b 3a20 4f70 7469           k: Opti
+0000cf70: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0000cf80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000cf90: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+0000cfa0: 6772 616d 5f74 7970 653a 204c 6974 6572  gram_type: Liter
+0000cfb0: 616c 5b22 636e 6d66 5f67 6570 5f74 706d  al["cnmf_gep_tpm
+0000cfc0: 222c 2022 636e 6d66 5f67 6570 5f72 6177  ", "cnmf_gep_raw
+0000cfd0: 225d 203d 2022 636e 6d66 5f67 6570 5f74  "] = "cnmf_gep_t
+0000cfe0: 706d 220d 0a20 2020 2020 2020 2020 2020  pm"..           
+0000cff0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000d000: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
+0000d010: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000d020: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+0000d030: 6520 6170 7072 6f78 696d 6174 6564 2064  e approximated d
+0000d040: 6174 6120 6279 206d 756c 7469 706c 7969  ata by multiplyi
+0000d050: 6e67 2074 6865 2070 726f 6772 616d 7320  ng the programs 
+0000d060: 616e 6420 7573 6167 6520 6d61 7472 6963  and usage matric
+0000d070: 6573 2066 6f72 2061 2067 6976 656e 2072  es for a given r
+0000d080: 616e 6b20 286b 292e 2044 6566 6175 6c74  ank (k). Default
+0000d090: 7320 746f 2074 6865 2068 6967 6865 7374  s to the highest
+0000d0a0: 2072 616e 6b20 6176 6169 6c61 626c 652e   rank available.
+0000d0b0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
+0000d0c0: 616d 206b 3a20 7261 6e6b 2c20 6465 6661  am k: rank, defa
+0000d0d0: 756c 7473 2074 6f20 4e6f 6e65 0d0a 2020  ults to None..  
+0000d0e0: 2020 2020 2020 3a74 7970 6520 6b3a 2069        :type k: i
+0000d0f0: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+0000d100: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
+0000d110: 7070 726f 7869 6d61 7469 6f6e 206f 6620  pproximation of 
+0000d120: 6461 7461 7365 7420 6261 7365 6420 6f6e  dataset based on
+0000d130: 2070 726f 6772 616d 7320 616e 6420 7573   programs and us
+0000d140: 6167 6573 0d0a 2020 2020 2020 2020 3a72  ages..        :r
+0000d150: 7479 7065 3a20 7064 2e44 6174 6146 7261  type: pd.DataFra
+0000d160: 6d65 0d0a 2020 2020 2020 2020 2222 220d  me..        """.
+0000d170: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000d180: 7365 6c66 2e68 6173 5f63 6e6d 665f 7265  self.has_cnmf_re
+0000d190: 7375 6c74 730d 0a20 2020 2020 2020 2069  sults..        i
+0000d1a0: 6620 6b20 6973 204e 6f6e 653a 0d0a 2020  f k is None:..  
+0000d1b0: 2020 2020 2020 2020 2020 6b20 3d20 7365            k = se
+0000d1c0: 6c66 2e61 6461 7461 2e75 6e73 5b22 6b76  lf.adata.uns["kv
+0000d1d0: 616c 7322 5d2e 696e 6465 782e 6d61 7828  als"].index.max(
+0000d1e0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+0000d1f0: 2020 2020 2061 7070 726f 7869 6d61 7469       approximati
+0000d200: 6f6e 203d 2028 7365 6c66 2e67 6574 5f75  on = (self.get_u
+0000d210: 7361 6765 7328 6b3d 6b29 2020 4020 7365  sages(k=k)  @ se
+0000d220: 6c66 2e67 6574 5f70 726f 6772 616d 7328  lf.get_programs(
+0000d230: 7479 7065 3d70 726f 6772 616d 5f74 7970  type=program_typ
+0000d240: 652c 206b 3d6b 292e 5429 0d0a 0d0a 2020  e, k=k).T)....  
+0000d250: 2020 2020 2020 7265 7475 726e 2061 7070        return app
+0000d260: 726f 7869 6d61 7469 6f6e 0d0a 2020 2020  roximation..    
+0000d270: 2020 2020 0d0a 2020 2020 6465 6620 6361      ..    def ca
+0000d280: 6c63 756c 6174 655f 636e 6d66 5f70 7265  lculate_cnmf_pre
+0000d290: 6469 6374 696f 6e5f 6572 726f 7228 7365  diction_error(se
+0000d2a0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 2020 2020 2020 2020 2020 2020 6b3a 204f              k: O
+0000d2d0: 7074 696f 6e61 6c5b 556e 696f 6e5b 696e  ptional[Union[in
+0000d2e0: 742c 2049 7465 7261 626c 655d 5d20 3d20  t, Iterable]] = 
+0000d2f0: 4e6f 6e65 2920 2d3e 2055 6e69 6f6e 5b66  None) -> Union[f
+0000d300: 6c6f 6174 2c20 7064 2e53 6572 6965 735d  loat, pd.Series]
+0000d310: 3a0d 0a20 2020 2020 2020 2022 2222 4361  :..        """Ca
+0000d320: 6c63 756c 6174 6520 634e 4d46 2070 7265  lculate cNMF pre
+0000d330: 6469 6374 696f 6e20 6572 726f 7220 7573  diction error us
+0000d340: 696e 6720 7468 6520 6d65 7468 6f64 2069  ing the method i
+0000d350: 6e20 7468 6520 6f72 6967 696e 616c 2063  n the original c
+0000d360: 4e4d 4620 7061 636b 6167 652e 0d0a 0d0a  NMF package.....
+0000d370: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+0000d380: 3a20 5370 6563 6966 7920 6f6e 6520 6f72  : Specify one or
+0000d390: 206d 6f72 6520 6b20 7661 6c75 6573 2074   more k values t
+0000d3a0: 6f20 6361 6c63 756c 6174 6520 7072 6564  o calculate pred
+0000d3b0: 6963 7469 6f6e 2065 7272 6f72 2e20 5370  iction error. Sp
+0000d3c0: 6563 6966 7920 4e6f 6e65 2074 6f20 6361  ecify None to ca
+0000d3d0: 6c63 756c 6174 6520 666f 7220 616c 6c20  lculate for all 
+0000d3e0: 6176 6169 6c61 626c 6520 6b2e 2064 6566  available k. def
+0000d3f0: 6175 6c74 7320 746f 204e 6f6e 650d 0a20  aults to None.. 
+0000d400: 2020 2020 2020 203a 7479 7065 206b 3a20         :type k: 
+0000d410: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b69  Optional[Union[i
+0000d420: 6e74 2c20 4974 6572 6162 6c65 5d5d 2c20  nt, Iterable]], 
+0000d430: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+0000d440: 2020 3a72 6169 7365 7320 5661 6c75 6545    :raises ValueE
+0000d450: 7272 6f72 3a20 6966 2069 6e76 616c 6964  rror: if invalid
+0000d460: 206b 2069 7320 7370 6563 6966 6965 640d   k is specified.
+0000d470: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000d480: 3a20 7363 616c 6172 206f 7220 7665 6374  : scalar or vect
+0000d490: 6f72 0d0a 2020 2020 2020 2020 3a72 7479  or..        :rty
+0000d4a0: 7065 3a20 5f74 7970 655f 0d0a 2020 2020  pe: _type_..    
+0000d4b0: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
+0000d4c0: 2020 2066 726f 6d20 736b 6c65 6172 6e2e     from sklearn.
+0000d4d0: 6465 636f 6d70 6f73 6974 696f 6e20 696d  decomposition im
+0000d4e0: 706f 7274 206e 6f6e 5f6e 6567 6174 6976  port non_negativ
+0000d4f0: 655f 6661 6374 6f72 697a 6174 696f 6e0d  e_factorization.
+0000d500: 0a0d 0a0d 0a20 2020 2020 2020 2069 6620  .....        if 
+0000d510: 6b20 6973 204e 6f6e 653a 0d0a 2020 2020  k is None:..    
+0000d520: 2020 2020 2020 2020 6b76 616c 7320 3d20          kvals = 
+0000d530: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+0000d540: 6b76 616c 7322 5d2e 696e 6465 780d 0a20  kvals"].index.. 
+0000d550: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+0000d560: 7374 616e 6365 286b 2c20 4974 6572 6162  stance(k, Iterab
+0000d570: 6c65 293a 0d0a 2020 2020 2020 2020 2020  le):..          
+0000d580: 2020 6b76 616c 7320 3d20 6b0d 0a20 2020    kvals = k..   
+0000d590: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+0000d5a0: 616e 6365 286b 2c20 2869 6e74 2c20 6e70  ance(k, (int, np
+0000d5b0: 2e69 6e74 6567 6572 2929 3a0d 0a20 2020  .integer)):..   
+0000d5c0: 2020 2020 2020 2020 206b 7661 6c73 203d           kvals =
+0000d5d0: 205b 6b5d 0d0a 2020 2020 2020 2020 656c   [k]..        el
+0000d5e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000d5f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000d600: 720d 0a20 2020 2020 2020 200d 0a20 2020  r..        ..   
+0000d610: 2020 2020 206e 6f72 6d5f 636f 756e 7473       norm_counts
+0000d620: 203d 2073 656c 662e 6164 6174 612e 746f   = self.adata.to
+0000d630: 5f64 6628 292e 6c6f 635b 3a2c 2073 656c  _df().loc[:, sel
+0000d640: 662e 6164 6174 612e 7661 725b 2273 656c  f.adata.var["sel
+0000d650: 6563 7465 6422 5d5d 0d0a 2020 2020 2020  ected"]]..      
+0000d660: 2020 6e6f 726d 5f63 6f75 6e74 7320 2f3d    norm_counts /=
+0000d670: 206e 6f72 6d5f 636f 756e 7473 2e73 7464   norm_counts.std
+0000d680: 2861 7869 733d 302c 2064 646f 663d 3129  (axis=0, ddof=1)
+0000d690: 0d0a 0d0a 2020 2020 2020 2020 7072 6564  ....        pred
+0000d6a0: 5f65 7272 6f72 203d 2070 642e 5365 7269  _error = pd.Seri
+0000d6b0: 6573 2869 6e64 6578 3d6b 7661 6c73 2c20  es(index=kvals, 
+0000d6c0: 6e61 6d65 3d22 634e 4d46 2070 7265 6469  name="cNMF predi
+0000d6d0: 6374 696f 6e5f 6572 726f 7222 290d 0a20  ction_error").. 
+0000d6e0: 2020 2020 2020 2066 6f72 206b 7661 6c20         for kval 
+0000d6f0: 696e 206b 7661 6c73 3a0d 0a20 2020 2020  in kvals:..     
+0000d700: 2020 2020 2020 2023 206f 6274 6169 6e20         # obtain 
+0000d710: 7265 636f 6e73 7472 7563 7465 6420 6e6f  reconstructed no
+0000d720: 726d 616c 697a 6564 2063 6f75 6e74 7320  rmalized counts 
+0000d730: 6d61 7472 6978 2062 7920 7265 2d66 6974  matrix by re-fit
+0000d740: 7469 6e67 2075 7361 6765 2061 6e64 2063  ting usage and c
+0000d750: 6f6d 7075 7469 6e67 2064 6f74 2070 726f  omputing dot pro
+0000d760: 6475 6374 3a20 7573 6167 652e 646f 7428  duct: usage.dot(
+0000d770: 7370 6563 7472 6129 0d0a 2020 2020 2020  spectra)..      
+0000d780: 2020 2020 2020 6d65 6469 616e 5f73 7065        median_spe
+0000d790: 6374 7261 203d 2073 656c 662e 6765 745f  ctra = self.get_
+0000d7a0: 7072 6f67 7261 6d73 286b 3d6b 7661 6c2c  programs(k=kval,
+0000d7b0: 2074 7970 653d 2263 6e6d 665f 6765 705f   type="cnmf_gep_
+0000d7c0: 7261 7722 292e 6472 6f70 6e61 2829 0d0a  raw").dropna()..
+0000d7d0: 2020 2020 2020 2020 2020 2020 7266 5f75              rf_u
+0000d7e0: 7361 6765 732c 2072 665f 7370 6563 7472  sages, rf_spectr
+0000d7f0: 612c 206e 6974 6572 203d 206e 6f6e 5f6e  a, niter = non_n
+0000d800: 6567 6174 6976 655f 6661 6374 6f72 697a  egative_factoriz
+0000d810: 6174 696f 6e28 583d 6e6f 726d 5f63 6f75  ation(X=norm_cou
+0000d820: 6e74 732e 7661 6c75 6573 2e61 7374 7970  nts.values.astyp
+0000d830: 6528 6e70 2e66 6c6f 6174 3634 292c 0d0a  e(np.float64),..
 0000d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d850: 616c 7068 615f 483d 302e 302c 2061 6c70  alpha_H=0.0, alp
-0000d860: 6861 5f57 3d30 2e30 2c20 6265 7461 5f6c  ha_W=0.0, beta_l
-0000d870: 6f73 733d 226b 756c 6c62 6163 6b2d 6c65  oss="kullback-le
-0000d880: 6962 6c65 7222 2c20 696e 6974 3d22 7261  ibler", init="ra
-0000d890: 6e64 6f6d 222c 0d0a 2020 2020 2020 2020  ndom",..        
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 2020 2020 2020 2020 2020 6c31 5f72              l1_r
-0000d8d0: 6174 696f 3d30 2e30 2c20 6d61 785f 6974  atio=0.0, max_it
-0000d8e0: 6572 3d31 3030 302c 2073 6f6c 7665 723d  er=1000, solver=
-0000d8f0: 226d 7522 2c20 746f 6c3d 302e 3030 3031  "mu", tol=0.0001
-0000d900: 2c20 6e5f 636f 6d70 6f6e 656e 7473 3d6b  , n_components=k
-0000d910: 7661 6c2c 2048 3d6d 6564 6961 6e5f 7370  val, H=median_sp
-0000d920: 6563 7472 612e 542e 7661 6c75 6573 2e61  ectra.T.values.a
-0000d930: 7374 7970 6528 6e70 2e66 6c6f 6174 3634  stype(np.float64
-0000d940: 292c 2075 7064 6174 655f 483d 4661 6c73  ), update_H=Fals
-0000d950: 6529 0d0a 0d0a 2020 2020 2020 2020 2020  e)....          
-0000d960: 2020 7266 5f75 7361 6765 7320 3d20 7064    rf_usages = pd
-0000d970: 2e44 6174 6146 7261 6d65 2872 665f 7573  .DataFrame(rf_us
-0000d980: 6167 6573 2c20 696e 6465 783d 6e6f 726d  ages, index=norm
-0000d990: 5f63 6f75 6e74 732e 696e 6465 782c 2063  _counts.index, c
-0000d9a0: 6f6c 756d 6e73 3d6d 6564 6961 6e5f 7370  olumns=median_sp
-0000d9b0: 6563 7472 612e 542e 696e 6465 7829 0d0a  ectra.T.index)..
-0000d9c0: 2020 2020 2020 2020 2020 2020 7266 5f70              rf_p
-0000d9d0: 7265 645f 6e6f 726d 5f63 6f75 6e74 7320  red_norm_counts 
-0000d9e0: 3d20 7266 5f75 7361 6765 732e 646f 7428  = rf_usages.dot(
-0000d9f0: 6d65 6469 616e 5f73 7065 6374 7261 2e54  median_spectra.T
-0000da00: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-0000da10: 7265 645f 6572 726f 725b 6b76 616c 5d20  red_error[kval] 
-0000da20: 3d20 2828 6e6f 726d 5f63 6f75 6e74 7320  = ((norm_counts 
-0000da30: 2d20 7266 5f70 7265 645f 6e6f 726d 5f63  - rf_pred_norm_c
-0000da40: 6f75 6e74 7329 2a2a 3229 2e73 756d 2829  ounts)**2).sum()
-0000da50: 2e73 756d 2829 0d0a 0d0a 2020 2020 2020  .sum()....      
-0000da60: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000da70: 6b2c 2028 696e 742c 206e 702e 696e 7465  k, (int, np.inte
-0000da80: 6765 7229 293a 0d0a 2020 2020 2020 2020  ger)):..        
-0000da90: 2020 2020 7265 7475 726e 2070 7265 645f      return pred_
-0000daa0: 6572 726f 725b 6b5d 0d0a 2020 2020 2020  error[k]..      
-0000dab0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000dac0: 2020 2020 2072 6574 7572 6e20 7072 6564       return pred
-0000dad0: 5f65 7272 6f72 0d0a 0d0a 2020 2020 6465  _error....    de
-0000dae0: 6620 7661 6c69 6461 7465 5f63 6e6d 665f  f validate_cnmf_
-0000daf0: 7072 6564 6963 7469 6f6e 5f65 7272 6f72  prediction_error
-0000db00: 7328 7365 6c66 2c20 746f 6c65 7261 6e63  s(self, toleranc
-0000db10: 653a 2066 6c6f 6174 203d 2031 652d 3429  e: float = 1e-4)
-0000db20: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
-0000db30: 3a0d 0a20 2020 2020 2020 2022 2222 5661  :..        """Va
-0000db40: 6c69 6461 7465 2074 6865 2064 6174 6173  lidate the datas
-0000db50: 6574 2061 6e64 2063 4e4d 4620 736f 6c75  et and cNMF solu
-0000db60: 7469 6f6e 7320 666f 7220 6561 6368 2072  tions for each r
-0000db70: 616e 6b20 6279 2063 6f6d 7061 7269 6e67  ank by comparing
-0000db80: 2074 6865 0d0a 2020 2020 2020 2020 7072   the..        pr
-0000db90: 6564 6963 7469 6f6e 2065 7272 6f72 2076  ediction error v
-0000dba0: 616c 7565 7320 7374 6f72 6564 2069 6e20  alues stored in 
-0000dbb0: 7468 6520 6f62 6a65 6374 205b 7365 6c66  the object [self
-0000dbc0: 2e61 6461 7461 2e75 6e73 2e6b 7661 6c73  .adata.uns.kvals
-0000dbd0: 5d20 746f 2074 686f 7365 2063 616c 6375  ] to those calcu
-0000dbe0: 6c61 7465 6420 6672 6f6d 2074 6865 0d0a  lated from the..
-0000dbf0: 2020 2020 2020 2020 6461 7461 7365 7427          dataset'
-0000dc00: 7320 6461 7461 206d 6174 7269 6365 7320  s data matrices 
-0000dc10: 5b62 6173 6564 206f 6e20 7365 6c66 2e61  [based on self.a
-0000dc20: 6461 7461 2e58 2061 6e64 2073 656c 662e  data.X and self.
-0000dc30: 6164 6174 612e 7661 726d 5b27 636e 6d66  adata.varm['cnmf
-0000dc40: 5f67 6570 5f72 6177 275d 5d2e 2054 6869  _gep_raw']]. Thi
-0000dc50: 7320 6361 6e20 6265 2061 2071 7569 636b  s can be a quick
-0000dc60: 2061 6e64 2073 656e 7369 7469 7665 2077   and sensitive w
-0000dc70: 6179 2074 6f20 6173 7365 7373 0d0a 2020  ay to assess..  
-0000dc80: 2020 2020 2020 7468 6174 2074 6865 2064        that the d
-0000dc90: 6174 6173 6574 2061 6e64 2074 6865 2063  ataset and the c
-0000dca0: 4e4d 4620 736f 6c75 7469 6f6e 7320 6861  NMF solutions ha
-0000dcb0: 7665 206e 6f74 2062 6565 6e20 616c 7465  ve not been alte
-0000dcc0: 7265 642e 0d0a 0d0a 2020 2020 2020 2020  red.....        
-0000dcd0: 3a70 6172 616d 2074 6f6c 6572 616e 6365  :param tolerance
-0000dce0: 3a20 6d61 7869 6d75 6d20 7265 6c61 7469  : maximum relati
-0000dcf0: 7665 2065 7272 6f72 2066 6f72 2061 6e79  ve error for any
-0000dd00: 206b 2077 6865 6e20 636f 6d70 7574 696e   k when computin
-0000dd10: 6720 7468 6520 7072 6564 6963 7469 6f6e  g the prediction
-0000dd20: 2065 7272 6f72 2c20 6465 6661 756c 7473   error, defaults
-0000dd30: 2074 6f20 302e 3030 3031 0d0a 2020 2020   to 0.0001..    
-0000dd40: 2020 2020 3a74 7970 6520 746f 6c65 7261      :type tolera
-0000dd50: 6e63 653a 2066 6c6f 6174 2c20 6f70 7469  nce: float, opti
-0000dd60: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-0000dd70: 6169 7365 7320 5661 6c75 6545 7272 6f72  aises ValueError
-0000dd80: 3a20 6966 2074 6865 206d 6178 696d 756d  : if the maximum
-0000dd90: 2072 656c 6174 6976 6520 6572 726f 7220   relative error 
-0000dda0: 6578 6365 6564 7320 7468 6520 746f 6c65  exceeds the tole
-0000ddb0: 7261 6e63 650d 0a20 2020 2020 2020 203a  rance..        :
-0000ddc0: 7265 7475 726e 3a20 4461 7461 4672 616d  return: DataFram
-0000ddd0: 6520 7769 7468 2073 746f 7265 6420 616e  e with stored an
-0000dde0: 6420 636f 6d70 7574 6564 2070 7265 6469  d computed predi
-0000ddf0: 6374 696f 6e20 6572 726f 722c 2061 6e64  ction error, and
-0000de00: 2072 656c 6174 6976 6520 6572 726f 7220   relative error 
-0000de10: 666f 7220 6561 6368 2072 616e 6b0d 0a20  for each rank.. 
-0000de20: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
-0000de30: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
-0000de40: 2020 2020 2022 2222 0d0a 200d 0a20 2020       """.. ..   
-0000de50: 2020 2020 2070 7265 645f 6572 726f 7220       pred_error 
-0000de60: 3d20 7064 2e53 6572 6965 7328 290d 0a20  = pd.Series().. 
-0000de70: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-0000de80: 7365 6c66 2e61 6461 7461 2e75 6e73 5b27  self.adata.uns['
-0000de90: 6b76 616c 7327 5d2e 696e 6465 783a 0d0a  kvals'].index:..
-0000dea0: 2020 2020 2020 2020 2020 2020 7072 6564              pred
-0000deb0: 5f65 7272 6f72 5b6b 5d20 3d20 7365 6c66  _error[k] = self
-0000dec0: 2e63 616c 6375 6c61 7465 5f63 6e6d 665f  .calculate_cnmf_
-0000ded0: 7072 6564 6963 7469 6f6e 5f65 7272 6f72  prediction_error
-0000dee0: 286b 3d6b 290d 0a20 2020 2020 2020 2023  (k=k)..        #
-0000def0: 2076 616c 6964 6174 6520 6572 726f 7220   validate error 
-0000df00: 6f66 2074 6865 2073 6f6c 7574 696f 6e73  of the solutions
-0000df10: 206d 6174 6368 6573 2063 4e4d 4627 7320   matches cNMF's 
-0000df20: 7374 6f72 6564 2065 7272 6f72 2076 616c  stored error val
-0000df30: 7565 730d 0a20 2020 2020 2020 2064 6620  ues..        df 
-0000df40: 3d20 7064 2e44 6174 6146 7261 6d65 287b  = pd.DataFrame({
-0000df50: 2273 746f 7265 6422 3a20 7365 6c66 2e61  "stored": self.a
-0000df60: 6461 7461 2e75 6e73 5b27 6b76 616c 7327  data.uns['kvals'
-0000df70: 5d5b 2270 7265 6469 6374 696f 6e5f 6572  ]["prediction_er
-0000df80: 726f 7222 5d2c 0d0a 2020 2020 2020 2020  ror"],..        
-0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfa0: 2020 2022 636f 6d70 7574 6564 223a 2070     "computed": p
-0000dfb0: 7265 645f 6572 726f 727d 290d 0a20 2020  red_error})..   
-0000dfc0: 2020 2020 2064 665b 2272 656c 6174 6976       df["relativ
-0000dfd0: 655f 6572 726f 7222 5d20 3d20 2864 665b  e_error"] = (df[
-0000dfe0: 2263 6f6d 7075 7465 6422 5d20 2d20 6466  "computed"] - df
-0000dff0: 5b22 7374 6f72 6564 225d 292e 6162 7328  ["stored"]).abs(
-0000e000: 2920 2f20 6466 5b22 7374 6f72 6564 225d  ) / df["stored"]
-0000e010: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0000e020: 2020 2020 6966 2028 6466 5b22 7265 6c61      if (df["rela
-0000e030: 7469 7665 5f65 7272 6f72 225d 203e 2074  tive_error"] > t
-0000e040: 6f6c 6572 616e 6365 292e 616e 7928 293a  olerance).any():
-0000e050: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-0000e060: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-0000e070: 2244 6174 6173 6574 2076 616c 6964 6174  "Dataset validat
-0000e080: 696f 6e20 6661 696c 6564 2075 7369 6e67  ion failed using
-0000e090: 2063 4e4d 4620 7072 6564 6963 7469 6f6e   cNMF prediction
-0000e0a0: 2065 7272 6f72 2074 6f6c 6572 616e 6365   error tolerance
-0000e0b0: 206f 6620 7b74 6f6c 6572 616e 6365 7d2e   of {tolerance}.
-0000e0c0: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2022 5468 6973 2063 616e 206f 6363 7572   "This can occur
-0000e0f0: 2077 6865 6e20 6461 7461 7365 7420 6f62   when dataset ob
-0000e100: 6a65 6374 7320 6172 6520 756e 696e 7465  jects are uninte
-0000e110: 6e74 696f 6e61 6c6c 7920 616c 7465 7265  ntionally altere
-0000e120: 6420 616e 6420 7468 6520 6d61 7472 6963  d and the matric
-0000e130: 6573 2022 0d0a 2020 2020 2020 2020 2020  es "..          
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 2022 6172 6520 6e6f 7420 636f 6e73     "are not cons
-0000e160: 6973 7465 6e74 2077 6974 6820 7468 6520  istent with the 
-0000e170: 6f72 6967 696e 616c 206f 6e65 7320 7573  original ones us
-0000e180: 6564 2066 6f72 2066 6163 746f 7269 7a61  ed for factoriza
-0000e190: 7469 6f6e 2e22 290d 0a0d 0a20 2020 2020  tion.")....     
-0000e1a0: 2020 2072 6574 7572 6e20 6466 0d0a 2020     return df..  
-0000e1b0: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
-0000e1c0: 6620 6765 745f 6d65 7461 6461 7461 5f64  f get_metadata_d
-0000e1d0: 6628 7365 6c66 2c0d 0a20 2020 2020 2020  f(self,..       
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2069 6e63 6c75 6465 5f63 6174 6567 6f72   include_categor
-0000e200: 6963 616c 3a20 626f 6f6c 203d 2054 7275  ical: bool = Tru
-0000e210: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000e220: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-0000e230: 7564 655f 6e75 6d65 7269 6361 6c3a 2062  ude_numerical: b
-0000e240: 6f6f 6c20 3d20 5472 7565 0d0a 2020 2020  ool = True..    
-0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e260: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
-0000e270: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
-0000e280: 2222 2247 6574 2073 616d 706c 652f 6f62  """Get sample/ob
-0000e290: 7365 7276 6174 696f 6e20 6d65 7461 6461  servation metada
-0000e2a0: 7461 2e0d 0a0d 0a20 2020 2020 2020 203a  ta.....        :
-0000e2b0: 7061 7261 6d20 696e 636c 7564 655f 6361  param include_ca
-0000e2c0: 7465 676f 7269 6361 6c3a 2049 6e63 6c75  tegorical: Inclu
-0000e2d0: 6465 2063 6174 6567 6f72 6963 616c 206d  de categorical m
-0000e2e0: 6574 6164 6174 6120 6c61 7965 7273 2c20  etadata layers, 
-0000e2f0: 6465 6661 756c 7473 2074 6f20 5472 7565  defaults to True
-0000e300: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000e310: 696e 636c 7564 655f 6361 7465 676f 7269  include_categori
-0000e320: 6361 6c3a 2062 6f6f 6c2c 206f 7074 696f  cal: bool, optio
-0000e330: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-0000e340: 7261 6d20 696e 636c 7564 655f 6e75 6d65  ram include_nume
-0000e350: 7269 6361 6c3a 2049 6e63 6c75 6465 206e  rical: Include n
-0000e360: 756d 6572 6963 616c 206d 6574 6164 6174  umerical metadat
-0000e370: 6120 6c61 7965 7273 2c20 6465 6661 756c  a layers, defaul
-0000e380: 7473 2074 6f20 5472 7565 0d0a 2020 2020  ts to True..    
-0000e390: 2020 2020 3a74 7970 6520 696e 636c 7564      :type includ
-0000e3a0: 655f 6e75 6d65 7269 6361 6c3a 2062 6f6f  e_numerical: boo
-0000e3b0: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-0000e3c0: 2020 2020 203a 7261 6973 6573 2056 616c       :raises Val
-0000e3d0: 7565 4572 726f 723a 2045 7272 6f72 2069  ueError: Error i
-0000e3e0: 6620 6d65 7461 6461 7461 2074 7970 6573  f metadata types
-0000e3f0: 2061 7265 206e 6f74 2072 6563 6f67 6e69   are not recogni
-0000e400: 7a65 640d 0a20 2020 2020 2020 203a 7265  zed..        :re
-0000e410: 7475 726e 3a20 6f62 7365 7276 6174 696f  turn: observatio
-0000e420: 6e73 20c3 9720 6d65 7461 6461 7461 206d  ns .. metadata m
-0000e430: 6174 7269 780d 0a20 2020 2020 2020 203a  atrix..        :
-0000e440: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
-0000e450: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
-0000e460: 0d0a 2020 2020 2020 2020 6474 7970 6573  ..        dtypes
-0000e470: 203d 205b 5d0d 0a20 2020 2020 2020 2069   = []..        i
-0000e480: 6620 696e 636c 7564 655f 6361 7465 676f  f include_catego
-0000e490: 7269 6361 6c3a 0d0a 2020 2020 2020 2020  rical:..        
-0000e4a0: 2020 2020 6474 7970 6573 2e61 7070 656e      dtypes.appen
-0000e4b0: 6428 2263 6174 6567 6f72 7922 290d 0a20  d("category").. 
-0000e4c0: 2020 2020 2020 2069 6620 696e 636c 7564         if includ
-0000e4d0: 655f 6e75 6d65 7269 6361 6c3a 0d0a 2020  e_numerical:..  
-0000e4e0: 2020 2020 2020 2020 2020 6474 7970 6573            dtypes
-0000e4f0: 202b 3d20 5b22 666c 6f61 7422 2c20 2269   += ["float", "i
-0000e500: 6e74 225d 0d0a 2020 2020 2020 2020 756e  nt"]..        un
-0000e510: 6578 706c 6169 6e65 645f 636f 6c73 203d  explained_cols =
-0000e520: 2073 656c 662e 6164 6174 612e 6f62 732e   self.adata.obs.
-0000e530: 7365 6c65 6374 5f64 7479 7065 7328 6578  select_dtypes(ex
-0000e540: 636c 7564 653d 2822 6361 7465 676f 7279  clude=("category
-0000e550: 222c 2022 666c 6f61 7422 2c20 2269 6e74  ", "float", "int
-0000e560: 2229 292e 636f 6c75 6d6e 730d 0a20 2020  ")).columns..   
-0000e570: 2020 2020 2069 6620 6c65 6e28 756e 6578       if len(unex
-0000e580: 706c 6169 6e65 645f 636f 6c73 2920 3e20  plained_cols) > 
-0000e590: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-0000e5a0: 756e 6578 706c 6169 6e65 645f 636f 6c5f  unexplained_col_
-0000e5b0: 7374 7220 3d20 222c 2022 2e6a 6f69 6e28  str = ", ".join(
-0000e5c0: 756e 6578 706c 6169 6e65 645f 636f 6c73  unexplained_cols
-0000e5d0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0000e5e0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000e5f0: 6622 7b75 6e65 7870 6c61 696e 6564 5f63  f"{unexplained_c
-0000e600: 6f6c 5f73 7472 7d20 6d65 7461 6461 7461  ol_str} metadata
-0000e610: 2063 6f6c 756d 6e73 2068 6176 6520 756e   columns have un
-0000e620: 7265 636f 676e 697a 6564 2064 7479 7065  recognized dtype
-0000e630: 732e 2229 0d0a 2020 2020 2020 2020 6466  s.")..        df
-0000e640: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
-0000e650: 732e 7365 6c65 6374 5f64 7479 7065 7328  s.select_dtypes(
-0000e660: 696e 636c 7564 653d 6474 7970 6573 290d  include=dtypes).
-0000e670: 0a20 2020 2020 2020 2064 6620 3d20 6466  .        df = df
-0000e680: 2e64 726f 706e 6128 6178 6973 3d31 2c20  .dropna(axis=1, 
-0000e690: 686f 773d 2261 6c6c 2229 0d0a 2020 2020  how="all")..    
-0000e6a0: 2020 2020 6466 203d 2064 662e 7265 706c      df = df.repl
-0000e6b0: 6163 6528 226e 616e 222c 206e 702e 4e61  ace("nan", np.Na
-0000e6c0: 4e29 2020 2354 4f44 4f3a 2041 6464 7265  N)  #TODO: Addre
-0000e6d0: 7373 2065 7272 6f72 3a20 2f68 6f6d 652f  ss error: /home/
-0000e6e0: 7462 7665 7268 6579 2f6d 696e 6963 6f6e  tbverhey/minicon
-0000e6f0: 6461 332f 656e 7673 2f6d 6f73 6169 636d  da3/envs/mosaicm
-0000e700: 7069 2f6c 6962 2f70 7974 686f 6e33 2e31  pi/lib/python3.1
-0000e710: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
-0000e720: 6d6f 7361 6963 6d70 692f 6461 7461 7365  mosaicmpi/datase
-0000e730: 742e 7079 3a31 3032 313a 2046 7574 7572  t.py:1021: Futur
-0000e740: 6557 6172 6e69 6e67 3a20 5468 6520 6265  eWarning: The be
-0000e750: 6861 7669 6f72 206f 6620 5365 7269 6573  havior of Series
-0000e760: 2e72 6570 6c61 6365 2028 616e 6420 4461  .replace (and Da
-0000e770: 7461 4672 616d 652e 7265 706c 6163 6529  taFrame.replace)
-0000e780: 2077 6974 6820 4361 7465 676f 7269 6361   with Categorica
-0000e790: 6c44 7479 7065 2069 7320 6465 7072 6563  lDtype is deprec
-0000e7a0: 6174 6564 2e20 496e 2061 2066 7574 7572  ated. In a futur
-0000e7b0: 6520 7665 7273 696f 6e2c 2072 6570 6c61  e version, repla
-0000e7c0: 6365 2077 696c 6c20 6f6e 6c79 2062 6520  ce will only be 
-0000e7d0: 7573 6564 2066 6f72 2063 6173 6573 2074  used for cases t
-0000e7e0: 6861 7420 7072 6573 6572 7665 2074 6865  hat preserve the
-0000e7f0: 2063 6174 6567 6f72 6965 732e 2054 6f20   categories. To 
-0000e800: 6368 616e 6765 2074 6865 2063 6174 6567  change the categ
-0000e810: 6f72 6965 732c 2075 7365 2073 6572 2e63  ories, use ser.c
-0000e820: 6174 2e72 656e 616d 655f 6361 7465 676f  at.rename_catego
-0000e830: 7269 6573 2069 6e73 7465 6164 2e0d 0a20  ries instead... 
-0000e840: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-0000e850: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-0000e860: 6765 745f 6361 7465 676f 7279 5f6f 7665  get_category_ove
-0000e870: 7272 6570 7265 7365 6e74 6174 696f 6e28  rrepresentation(
-0000e880: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-0000e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000e8b0: 6179 6572 3a20 7374 722c 0d0a 2020 2020  ayer: str,..    
-0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8e0: 2020 2020 7472 756e 6361 7465 5f6e 6567      truncate_neg
-0000e8f0: 6174 6976 653a 2062 6f6f 6c20 3d20 5472  ative: bool = Tr
-0000e900: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e920: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-0000e930: 7365 745f 6361 7465 676f 7269 6573 3a20  set_categories: 
-0000e940: 436f 6c6c 6563 7469 6f6e 5b73 7472 5d20  Collection[str] 
-0000e950: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e980: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
-0000e990: 653a 0d0a 2020 2020 2020 2020 2222 2243  e:..        """C
-0000e9a0: 616c 6375 6c61 7465 2050 6561 7273 6f6e  alculate Pearson
-0000e9b0: 2072 6573 6964 7561 6c20 6f66 2063 6869   residual of chi
-0000e9c0: 2d73 7175 6172 6564 2074 6573 742c 2061  -squared test, a
-0000e9d0: 7373 6f63 6961 7469 6e67 2070 726f 6772  ssociating progr
-0000e9e0: 616d 7320 666f 7220 6561 6368 2072 616e  ams for each ran
-0000e9f0: 6b20 286b 2920 746f 2063 6174 6567 6f72  k (k) to categor
-0000ea00: 6965 7320 6f66 2073 616d 706c 6573 2f6f  ies of samples/o
-0000ea10: 6273 6572 7661 7469 6f6e 732e 2042 7920  bservations. By 
-0000ea20: 6465 6661 756c 742c 2074 7275 6e63 6174  default, truncat
-0000ea30: 6573 206e 6567 6174 6976 6520 7661 6c75  es negative valu
-0000ea40: 6573 2e0d 0a0d 0a20 2020 2020 2020 203a  es.....        :
-0000ea50: 7061 7261 6d20 6c61 7965 723a 206e 616d  param layer: nam
-0000ea60: 6520 6f66 2063 6174 6567 6f72 6963 616c  e of categorical
-0000ea70: 2064 6174 6120 6c61 7965 720d 0a20 2020   data layer..   
-0000ea80: 2020 2020 203a 7479 7065 206c 6179 6572       :type layer
-0000ea90: 3a20 7374 720d 0a20 2020 2020 2020 203a  : str..        :
-0000eaa0: 7061 7261 6d20 7472 756e 6361 7465 5f6e  param truncate_n
-0000eab0: 6567 6174 6976 653a 2054 7275 6e63 6174  egative: Truncat
-0000eac0: 6520 6e65 6761 7469 7665 2072 6573 6964  e negative resid
-0000ead0: 7561 6c73 2074 6f20 302c 2064 6566 6175  uals to 0, defau
-0000eae0: 6c74 7320 746f 2054 7275 650d 0a20 2020  lts to True..   
-0000eaf0: 2020 2020 203a 7479 7065 2074 7275 6e63       :type trunc
-0000eb00: 6174 655f 6e65 6761 7469 7665 3a20 626f  ate_negative: bo
-0000eb10: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
-0000eb20: 2020 2020 2020 3a70 6172 616d 2073 7562        :param sub
-0000eb30: 7365 745f 6361 7465 676f 7269 6573 3a20  set_categories: 
-0000eb40: 5072 6f76 6964 6520 6120 7375 6273 6574  Provide a subset
-0000eb50: 206f 6620 6361 7465 676f 7269 6573 2066   of categories f
-0000eb60: 6f72 2063 616c 6375 6c61 7469 6e67 206f  or calculating o
-0000eb70: 7665 7272 6570 7265 7365 6e74 6174 696f  verrepresentatio
-0000eb80: 6e0d 0a20 2020 2020 2020 203a 7479 7065  n..        :type
-0000eb90: 2073 7562 7365 745f 6361 7465 676f 7269   subset_categori
-0000eba0: 6573 3a20 436f 6c6c 6563 7469 6f6e 5b73  es: Collection[s
-0000ebb0: 7472 5d0d 0a20 2020 2020 2020 203a 7265  tr]..        :re
-0000ebc0: 7475 726e 3a20 6361 7465 676f 7279 20c3  turn: category .
-0000ebd0: 9720 7072 6f67 7261 6d20 6d61 7472 6978  . program matrix
-0000ebe0: 206f 6620 6f76 6572 7265 7072 6573 656e   of overrepresen
-0000ebf0: 7461 7469 6f6e 2076 616c 7565 730d 0a20  tation values.. 
-0000ec00: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
-0000ec10: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
-0000ec20: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000ec30: 2020 7573 6167 6520 3d20 7365 6c66 2e67    usage = self.g
-0000ec40: 6574 5f75 7361 6765 7328 6e6f 726d 616c  et_usages(normal
-0000ec50: 697a 653d 5472 7565 292e 636f 7079 2829  ize=True).copy()
-0000ec60: 0d0a 2020 2020 2020 2020 7361 6d70 6c65  ..        sample
-0000ec70: 5f74 6f5f 636c 6173 7320 3d20 7365 6c66  _to_class = self
-0000ec80: 2e67 6574 5f6d 6574 6164 6174 615f 6466  .get_metadata_df
-0000ec90: 2829 5b6c 6179 6572 5d0d 0a20 2020 2020  ()[layer]..     
-0000eca0: 2020 2069 6620 7375 6273 6574 5f63 6174     if subset_cat
-0000ecb0: 6567 6f72 6965 7320 6973 206e 6f74 204e  egories is not N
-0000ecc0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000ecd0: 2020 7361 6d70 6c65 5f74 6f5f 636c 6173    sample_to_clas
-0000ece0: 735b 7e73 616d 706c 655f 746f 5f63 6c61  s[~sample_to_cla
-0000ecf0: 7373 2e69 7369 6e28 7375 6273 6574 5f63  ss.isin(subset_c
-0000ed00: 6174 6567 6f72 6965 7329 5d20 3d20 6e70  ategories)] = np
-0000ed10: 2e4e 614e 0d0a 2020 2020 2020 2020 7573  .NaN..        us
-0000ed20: 6167 652e 696e 6465 7820 3d20 7573 6167  age.index = usag
-0000ed30: 652e 696e 6465 782e 6d61 7028 7361 6d70  e.index.map(samp
-0000ed40: 6c65 5f74 6f5f 636c 6173 7329 0d0a 2020  le_to_class)..  
-0000ed50: 2020 2020 2020 6f62 7365 7276 6564 203d        observed =
-0000ed60: 2075 7361 6765 2e67 726f 7570 6279 286c   usage.groupby(l
-0000ed70: 6576 656c 3d30 2c20 6f62 7365 7276 6564  evel=0, observed
-0000ed80: 3d54 7275 6529 2e73 756d 2829 0d0a 2020  =True).sum()..  
-0000ed90: 2020 2020 2020 6f62 7365 7276 6564 203d        observed =
-0000eda0: 206f 6273 6572 7665 645b 6f62 7365 7276   observed[observ
-0000edb0: 6564 2e73 756d 2861 7869 733d 3129 203e  ed.sum(axis=1) >
-0000edc0: 2030 5d0d 0a20 2020 2020 2020 206e 5f63   0]..        n_c
-0000edd0: 6174 6567 6f72 6965 7320 3d20 6f62 7365  ategories = obse
-0000ede0: 7276 6564 2e73 6861 7065 5b30 5d0d 0a20  rved.shape[0].. 
-0000edf0: 2020 2020 2020 2069 6620 6e5f 6361 7465         if n_cate
-0000ee00: 676f 7269 6573 203c 2032 3a0d 0a20 2020  gories < 2:..   
-0000ee10: 2020 2020 2020 2020 2069 6620 6c61 7965           if laye
-0000ee20: 7220 213d 2022 6876 675f 616c 6c5f 3022  r != "hvg_all_0"
-0000ee30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ee40: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-0000ee50: 6e67 2866 224f 7665 7272 6570 7265 7365  ng(f"Overreprese
-0000ee60: 6e74 6174 696f 6e20 636f 756c 6420 6e6f  ntation could no
-0000ee70: 7420 6265 2063 616c 6375 6c61 7465 6420  t be calculated 
-0000ee80: 666f 7220 6c61 7965 7220 277b 6c61 7965  for layer '{laye
-0000ee90: 727d 272c 2061 7320 6f6e 6c79 207b 6e5f  r}', as only {n_
-0000eea0: 6361 7465 676f 7269 6573 7d20 6361 7465  categories} cate
-0000eeb0: 676f 7269 6573 2077 6572 6520 666f 756e  gories were foun
-0000eec0: 6420 696e 2074 6865 2064 6174 612e 2022  d in the data. "
-0000eed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eef0: 2020 6622 4e6f 7465 2074 6861 7420 656d    f"Note that em
-0000ef00: 7074 7920 7661 6c75 6573 2069 6e20 7468  pty values in th
-0000ef10: 6520 6d65 7461 6461 7461 2061 7265 206e  e metadata are n
-0000ef20: 6f74 2063 6f6e 7369 6465 7265 6420 6120  ot considered a 
-0000ef30: 6361 7465 676f 7279 2e20 220d 0a20 2020  category. "..   
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 2020 2020 2020 2020 2020 2020 2066 224f               f"O
-0000ef60: 7665 7272 6570 7265 7365 6e74 6174 696f  verrepresentatio
-0000ef70: 6e20 6361 6e6e 6f74 2062 6520 6361 6c63  n cannot be calc
-0000ef80: 756c 6174 6564 2077 6974 6820 6665 7765  ulated with fewe
-0000ef90: 7220 7468 616e 2032 2063 6174 6567 6f72  r than 2 categor
-0000efa0: 6965 7320 666f 7220 6561 6368 206c 6179  ies for each lay
-0000efb0: 6572 2e20 2229 0d0a 2020 2020 2020 2020  er. ")..        
-0000efc0: 2020 2020 7265 7475 726e 2070 642e 4461      return pd.Da
-0000efd0: 7461 4672 616d 6528 6e70 2e4e 614e 2c20  taFrame(np.NaN, 
-0000efe0: 696e 6465 7820 3d20 6f62 7365 7276 6564  index = observed
-0000eff0: 2e69 6e64 6578 2c20 636f 6c75 6d6e 733d  .index, columns=
-0000f000: 6f62 7365 7276 6564 2e63 6f6c 756d 6e73  observed.columns
-0000f010: 290d 0a20 2020 2020 2020 2065 7870 6563  )..        expec
-0000f020: 7465 6420 3d20 5b5d 0d0a 2020 2020 2020  ted = []..      
-0000f030: 2020 666f 7220 6b2c 206f 6273 5f6b 2069    for k, obs_k i
-0000f040: 6e20 6f62 7365 7276 6564 2e54 2e67 726f  n observed.T.gro
-0000f050: 7570 6279 286c 6576 656c 3d31 293a 0d0a  upby(level=1):..
-0000f060: 2020 2020 2020 2020 2020 2020 6578 705f              exp_
-0000f070: 6b20 3d20 7064 2e44 6174 6146 7261 6d65  k = pd.DataFrame
-0000f080: 286f 6273 5f6b 2e73 756d 2861 7869 733d  (obs_k.sum(axis=
-0000f090: 3129 2920 4020 7064 2e44 6174 6146 7261  1)) @ pd.DataFra
-0000f0a0: 6d65 286f 6273 5f6b 2e73 756d 2861 7869  me(obs_k.sum(axi
-0000f0b0: 733d 3029 292e 5420 2f20 6f62 735f 6b2e  s=0)).T / obs_k.
-0000f0c0: 7375 6d28 292e 7375 6d28 290d 0a20 2020  sum().sum()..   
-0000f0d0: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
-0000f0e0: 642e 6170 7065 6e64 2865 7870 5f6b 290d  d.append(exp_k).
-0000f0f0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-0000f100: 6420 3d20 7064 2e63 6f6e 6361 7428 6578  d = pd.concat(ex
-0000f110: 7065 6374 6564 292e 540d 0a20 2020 2020  pected).T..     
-0000f120: 2020 2063 6869 7371 5f72 6573 6964 203d     chisq_resid =
-0000f130: 2028 6f62 7365 7276 6564 202d 2065 7870   (observed - exp
-0000f140: 6563 7465 6429 202f 206e 702e 7371 7274  ected) / np.sqrt
-0000f150: 2865 7870 6563 7465 6429 2020 2320 7065  (expected)  # pe
-0000f160: 6172 736f 6e20 7265 7369 6475 616c 206f  arson residual o
-0000f170: 6620 6368 692d 7371 7561 7265 6420 7465  f chi-squared te
-0000f180: 7374 206f 6620 636f 6e74 696e 6765 6e63  st of contingenc
-0000f190: 7920 7461 626c 650d 0a20 2020 2020 2020  y table..       
-0000f1a0: 2069 6620 7472 756e 6361 7465 5f6e 6567   if truncate_neg
-0000f1b0: 6174 6976 653a 0d0a 2020 2020 2020 2020  ative:..        
-0000f1c0: 2020 2020 6368 6973 715f 7265 7369 6420      chisq_resid 
-0000f1d0: 3d20 6368 6973 715f 7265 7369 642e 636c  = chisq_resid.cl
-0000f1e0: 6970 286c 6f77 6572 3d30 290d 0a20 2020  ip(lower=0)..   
-0000f1f0: 2020 2020 2072 6574 7572 6e20 6368 6973       return chis
-0000f200: 715f 7265 7369 640d 0a20 2020 200d 0a20  q_resid..    .. 
-0000f210: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-0000f220: 2067 6574 5f6d 6574 6164 6174 615f 636f   get_metadata_co
-0000f230: 7272 656c 6174 696f 6e28 7365 6c66 2c20  rrelation(self, 
-0000f240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f260: 2020 206c 6179 6572 3a20 7374 722c 0d0a     layer: str,..
-0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f290: 206d 6574 686f 643a 2073 7472 203d 2022   method: str = "
-0000f2a0: 7065 6172 736f 6e22 0d0a 2020 2020 2020  pearson"..      
-0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2c0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-0000f2d0: 7064 2e53 6572 6965 733a 0d0a 2020 2020  pd.Series:..    
-0000f2e0: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-0000f2f0: 2050 6561 7273 6f6e 2063 6f72 7265 6c61   Pearson correla
-0000f300: 7469 6f6e 206f 6620 4745 5020 7573 6167  tion of GEP usag
-0000f310: 6520 746f 206e 756d 6572 6963 616c 206d  e to numerical m
-0000f320: 6574 6164 6174 6120 6163 726f 7373 2073  etadata across s
-0000f330: 616d 706c 6573 2f6f 6273 6572 7661 7469  amples/observati
-0000f340: 6f6e 732e 0d0a 0d0a 2020 2020 2020 2020  ons.....        
-0000f350: 3a70 6172 616d 206c 6179 6572 3a20 6e61  :param layer: na
-0000f360: 6d65 206f 6620 6e75 6d65 7269 6361 6c20  me of numerical 
-0000f370: 6461 7461 206c 6179 6572 0d0a 2020 2020  data layer..    
-0000f380: 2020 2020 3a74 7970 6520 6c61 7965 723a      :type layer:
-0000f390: 2073 7472 0d0a 2020 2020 2020 2020 3a70   str..        :p
-0000f3a0: 6172 616d 206d 6574 686f 643a 2043 6f72  aram method: Cor
-0000f3b0: 7265 6c61 7469 6f6e 206d 6574 686f 643a  relation method:
-0000f3c0: 2022 7065 6172 736f 6e22 2c20 2273 7065   "pearson", "spe
-0000f3d0: 6172 6d61 6e22 2c20 6f72 2022 6b65 6e64  arman", or "kend
-0000f3e0: 616c 6c22 2e20 4465 6661 756c 7473 2074  all". Defaults t
-0000f3f0: 6f20 2270 6561 7273 6f6e 220d 0a20 2020  o "pearson"..   
-0000f400: 2020 2020 203a 7479 7065 206d 6574 686f       :type metho
-0000f410: 643a 2073 7472 2c20 6f70 7469 6f6e 616c  d: str, optional
-0000f420: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-0000f430: 6e3a 2063 6f72 7265 6c61 7469 6f6e 206f  n: correlation o
-0000f440: 6620 4745 5020 746f 206d 6574 6164 6174  f GEP to metadat
-0000f450: 610d 0a20 2020 2020 2020 203a 7274 7970  a..        :rtyp
-0000f460: 653a 2070 642e 5365 7269 6573 0d0a 2020  e: pd.Series..  
-0000f470: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000f480: 2020 2075 7361 6765 203d 2073 656c 662e     usage = self.
-0000f490: 6765 745f 7573 6167 6573 2829 2e63 6f70  get_usages().cop
-0000f4a0: 7928 290d 0a20 2020 2020 2020 206d 6574  y()..        met
-0000f4b0: 6164 6174 6120 3d20 7365 6c66 2e67 6574  adata = self.get
-0000f4c0: 5f6d 6574 6164 6174 615f 6466 2829 5b6c  _metadata_df()[l
-0000f4d0: 6179 6572 5d0d 0a20 2020 2020 2020 206d  ayer]..        m
-0000f4e0: 645f 636f 7272 203d 2075 7361 6765 2e63  d_corr = usage.c
-0000f4f0: 6f72 7277 6974 6828 6d65 7461 6461 7461  orrwith(metadata
-0000f500: 2c20 6d65 7468 6f64 3d6d 6574 686f 6429  , method=method)
-0000f510: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000f520: 206d 645f 636f 7272 0d0a 2020 2020 2020   md_corr..      
-0000f530: 2020 0d0a 2020 2020 6465 6620 6170 7065    ..    def appe
-0000f540: 6e64 5f74 6f5f 6869 7374 6f72 7928 7365  nd_to_history(se
-0000f550: 6c66 2c20 656e 7472 7929 3a0d 0a20 2020  lf, entry):..   
-0000f560: 2020 2020 2022 2222 4164 6420 656e 7472       """Add entr
-0000f570: 7920 746f 2044 6174 6173 6574 2068 6973  y to Dataset his
-0000f580: 746f 7279 2e0d 0a0d 0a20 2020 2020 2020  tory.....       
-0000f590: 203a 7061 7261 6d20 656e 7472 793a 2044   :param entry: D
-0000f5a0: 6573 6372 6970 7469 6f6e 206f 6620 6576  escription of ev
-0000f5b0: 656e 7420 746f 2072 6563 6f72 6420 696e  ent to record in
-0000f5c0: 2074 6865 2068 6973 746f 7279 2e0d 0a20   the history... 
-0000f5d0: 2020 2020 2020 203a 7479 7065 2065 6e74         :type ent
-0000f5e0: 7279 3a20 7374 720d 0a20 2020 2020 2020  ry: str..       
-0000f5f0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-0000f600: 6c66 2e61 6461 7461 2e75 6e73 5b22 6869  lf.adata.uns["hi
-0000f610: 7374 6f72 7922 5d5b 6461 7465 7469 6d65  story"][datetime
-0000f620: 2e75 7463 6e6f 7728 292e 6973 6f66 6f72  .utcnow().isofor
-0000f630: 6d61 7428 295d 203d 2065 6e74 7279 0d0a  mat()] = entry..
-0000f640: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-0000f650: 6620 6765 745f 6869 7374 6f72 7928 7365  f get_history(se
-0000f660: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-0000f670: 2252 6574 7572 6e73 2074 696d 6573 7461  "Returns timesta
-0000f680: 6d70 6564 2068 6973 746f 7279 206f 6620  mped history of 
-0000f690: 4461 7461 7365 7420 6f62 6a65 6374 2e0d  Dataset object..
-0000f6a0: 0a0d 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
-0000f6b0: 726e 3a20 6869 7374 6f72 790d 0a20 2020  rn: history..   
-0000f6c0: 2020 2020 203a 7274 7970 653a 2064 6963       :rtype: dic
-0000f6d0: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
-0000f6e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000f6f0: 656c 662e 6164 6174 612e 756e 735b 2268  elf.adata.uns["h
-0000f700: 6973 746f 7279 225d                      istory"]
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d870: 2020 2020 616c 7068 615f 483d 302e 302c      alpha_H=0.0,
+0000d880: 2061 6c70 6861 5f57 3d30 2e30 2c20 6265   alpha_W=0.0, be
+0000d890: 7461 5f6c 6f73 733d 226b 756c 6c62 6163  ta_loss="kullbac
+0000d8a0: 6b2d 6c65 6962 6c65 7222 2c20 696e 6974  k-leibler", init
+0000d8b0: 3d22 7261 6e64 6f6d 222c 0d0a 2020 2020  ="random",..    
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8f0: 6c31 5f72 6174 696f 3d30 2e30 2c20 6d61  l1_ratio=0.0, ma
+0000d900: 785f 6974 6572 3d31 3030 302c 2073 6f6c  x_iter=1000, sol
+0000d910: 7665 723d 226d 7522 2c20 746f 6c3d 302e  ver="mu", tol=0.
+0000d920: 3030 3031 2c20 6e5f 636f 6d70 6f6e 656e  0001, n_componen
+0000d930: 7473 3d6b 7661 6c2c 2048 3d6d 6564 6961  ts=kval, H=media
+0000d940: 6e5f 7370 6563 7472 612e 542e 7661 6c75  n_spectra.T.valu
+0000d950: 6573 2e61 7374 7970 6528 6e70 2e66 6c6f  es.astype(np.flo
+0000d960: 6174 3634 292c 2075 7064 6174 655f 483d  at64), update_H=
+0000d970: 4661 6c73 6529 0d0a 0d0a 2020 2020 2020  False)....      
+0000d980: 2020 2020 2020 7266 5f75 7361 6765 7320        rf_usages 
+0000d990: 3d20 7064 2e44 6174 6146 7261 6d65 2872  = pd.DataFrame(r
+0000d9a0: 665f 7573 6167 6573 2c20 696e 6465 783d  f_usages, index=
+0000d9b0: 6e6f 726d 5f63 6f75 6e74 732e 696e 6465  norm_counts.inde
+0000d9c0: 782c 2063 6f6c 756d 6e73 3d6d 6564 6961  x, columns=media
+0000d9d0: 6e5f 7370 6563 7472 612e 542e 696e 6465  n_spectra.T.inde
+0000d9e0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000d9f0: 7266 5f70 7265 645f 6e6f 726d 5f63 6f75  rf_pred_norm_cou
+0000da00: 6e74 7320 3d20 7266 5f75 7361 6765 732e  nts = rf_usages.
+0000da10: 646f 7428 6d65 6469 616e 5f73 7065 6374  dot(median_spect
+0000da20: 7261 2e54 290d 0a20 2020 2020 2020 2020  ra.T)..         
+0000da30: 2020 2070 7265 645f 6572 726f 725b 6b76     pred_error[kv
+0000da40: 616c 5d20 3d20 2828 6e6f 726d 5f63 6f75  al] = ((norm_cou
+0000da50: 6e74 7320 2d20 7266 5f70 7265 645f 6e6f  nts - rf_pred_no
+0000da60: 726d 5f63 6f75 6e74 7329 2a2a 3229 2e73  rm_counts)**2).s
+0000da70: 756d 2829 2e73 756d 2829 0d0a 0d0a 2020  um().sum()....  
+0000da80: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000da90: 6e63 6528 6b2c 2028 696e 742c 206e 702e  nce(k, (int, np.
+0000daa0: 696e 7465 6765 7229 293a 0d0a 2020 2020  integer)):..    
+0000dab0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+0000dac0: 7265 645f 6572 726f 725b 6b5d 0d0a 2020  red_error[k]..  
+0000dad0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000dae0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000daf0: 7072 6564 5f65 7272 6f72 0d0a 0d0a 2020  pred_error....  
+0000db00: 2020 6465 6620 7661 6c69 6461 7465 5f63    def validate_c
+0000db10: 6e6d 665f 7072 6564 6963 7469 6f6e 5f65  nmf_prediction_e
+0000db20: 7272 6f72 7328 7365 6c66 2c20 746f 6c65  rrors(self, tole
+0000db30: 7261 6e63 653a 2066 6c6f 6174 203d 2031  rance: float = 1
+0000db40: 652d 3429 202d 3e20 7064 2e44 6174 6146  e-4) -> pd.DataF
+0000db50: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
+0000db60: 2222 5661 6c69 6461 7465 2074 6865 2064  ""Validate the d
+0000db70: 6174 6173 6574 2061 6e64 2063 4e4d 4620  ataset and cNMF 
+0000db80: 736f 6c75 7469 6f6e 7320 666f 7220 6561  solutions for ea
+0000db90: 6368 2072 616e 6b20 6279 2063 6f6d 7061  ch rank by compa
+0000dba0: 7269 6e67 2074 6865 0d0a 2020 2020 2020  ring the..      
+0000dbb0: 2020 7072 6564 6963 7469 6f6e 2065 7272    prediction err
+0000dbc0: 6f72 2076 616c 7565 7320 7374 6f72 6564  or values stored
+0000dbd0: 2069 6e20 7468 6520 6f62 6a65 6374 205b   in the object [
+0000dbe0: 7365 6c66 2e61 6461 7461 2e75 6e73 2e6b  self.adata.uns.k
+0000dbf0: 7661 6c73 5d20 746f 2074 686f 7365 2063  vals] to those c
+0000dc00: 616c 6375 6c61 7465 6420 6672 6f6d 2074  alculated from t
+0000dc10: 6865 0d0a 2020 2020 2020 2020 6461 7461  he..        data
+0000dc20: 7365 7427 7320 6461 7461 206d 6174 7269  set's data matri
+0000dc30: 6365 7320 5b62 6173 6564 206f 6e20 7365  ces [based on se
+0000dc40: 6c66 2e61 6461 7461 2e58 2061 6e64 2073  lf.adata.X and s
+0000dc50: 656c 662e 6164 6174 612e 7661 726d 5b27  elf.adata.varm['
+0000dc60: 636e 6d66 5f67 6570 5f72 6177 275d 5d2e  cnmf_gep_raw']].
+0000dc70: 2054 6869 7320 6361 6e20 6265 2061 2071   This can be a q
+0000dc80: 7569 636b 2061 6e64 2073 656e 7369 7469  uick and sensiti
+0000dc90: 7665 2077 6179 2074 6f20 6173 7365 7373  ve way to assess
+0000dca0: 0d0a 2020 2020 2020 2020 7468 6174 2074  ..        that t
+0000dcb0: 6865 2064 6174 6173 6574 2061 6e64 2074  he dataset and t
+0000dcc0: 6865 2063 4e4d 4620 736f 6c75 7469 6f6e  he cNMF solution
+0000dcd0: 7320 6861 7665 206e 6f74 2062 6565 6e20  s have not been 
+0000dce0: 616c 7465 7265 642e 0d0a 0d0a 2020 2020  altered.....    
+0000dcf0: 2020 2020 3a70 6172 616d 2074 6f6c 6572      :param toler
+0000dd00: 616e 6365 3a20 6d61 7869 6d75 6d20 7265  ance: maximum re
+0000dd10: 6c61 7469 7665 2065 7272 6f72 2066 6f72  lative error for
+0000dd20: 2061 6e79 206b 2077 6865 6e20 636f 6d70   any k when comp
+0000dd30: 7574 696e 6720 7468 6520 7072 6564 6963  uting the predic
+0000dd40: 7469 6f6e 2065 7272 6f72 2c20 6465 6661  tion error, defa
+0000dd50: 756c 7473 2074 6f20 302e 3030 3031 0d0a  ults to 0.0001..
+0000dd60: 2020 2020 2020 2020 3a74 7970 6520 746f          :type to
+0000dd70: 6c65 7261 6e63 653a 2066 6c6f 6174 2c20  lerance: float, 
+0000dd80: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+0000dd90: 2020 3a72 6169 7365 7320 5661 6c75 6545    :raises ValueE
+0000dda0: 7272 6f72 3a20 6966 2074 6865 206d 6178  rror: if the max
+0000ddb0: 696d 756d 2072 656c 6174 6976 6520 6572  imum relative er
+0000ddc0: 726f 7220 6578 6365 6564 7320 7468 6520  ror exceeds the 
+0000ddd0: 746f 6c65 7261 6e63 650d 0a20 2020 2020  tolerance..     
+0000dde0: 2020 203a 7265 7475 726e 3a20 4461 7461     :return: Data
+0000ddf0: 4672 616d 6520 7769 7468 2073 746f 7265  Frame with store
+0000de00: 6420 616e 6420 636f 6d70 7574 6564 2070  d and computed p
+0000de10: 7265 6469 6374 696f 6e20 6572 726f 722c  rediction error,
+0000de20: 2061 6e64 2072 656c 6174 6976 6520 6572   and relative er
+0000de30: 726f 7220 666f 7220 6561 6368 2072 616e  ror for each ran
+0000de40: 6b0d 0a20 2020 2020 2020 203a 7274 7970  k..        :rtyp
+0000de50: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
+0000de60: 0a20 2020 2020 2020 2022 2222 0d0a 200d  .        """.. .
+0000de70: 0a20 2020 2020 2020 2070 7265 645f 6572  .        pred_er
+0000de80: 726f 7220 3d20 7064 2e53 6572 6965 7328  ror = pd.Series(
+0000de90: 290d 0a20 2020 2020 2020 2066 6f72 206b  )..        for k
+0000dea0: 2069 6e20 7365 6c66 2e61 6461 7461 2e75   in self.adata.u
+0000deb0: 6e73 5b27 6b76 616c 7327 5d2e 696e 6465  ns['kvals'].inde
+0000dec0: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
+0000ded0: 7072 6564 5f65 7272 6f72 5b6b 5d20 3d20  pred_error[k] = 
+0000dee0: 7365 6c66 2e63 616c 6375 6c61 7465 5f63  self.calculate_c
+0000def0: 6e6d 665f 7072 6564 6963 7469 6f6e 5f65  nmf_prediction_e
+0000df00: 7272 6f72 286b 3d6b 290d 0a20 2020 2020  rror(k=k)..     
+0000df10: 2020 2023 2076 616c 6964 6174 6520 6572     # validate er
+0000df20: 726f 7220 6f66 2074 6865 2073 6f6c 7574  ror of the solut
+0000df30: 696f 6e73 206d 6174 6368 6573 2063 4e4d  ions matches cNM
+0000df40: 4627 7320 7374 6f72 6564 2065 7272 6f72  F's stored error
+0000df50: 2076 616c 7565 730d 0a20 2020 2020 2020   values..       
+0000df60: 2064 6620 3d20 7064 2e44 6174 6146 7261   df = pd.DataFra
+0000df70: 6d65 287b 2273 746f 7265 6422 3a20 7365  me({"stored": se
+0000df80: 6c66 2e61 6461 7461 2e75 6e73 5b27 6b76  lf.adata.uns['kv
+0000df90: 616c 7327 5d5b 2270 7265 6469 6374 696f  als']["predictio
+0000dfa0: 6e5f 6572 726f 7222 5d2c 0d0a 2020 2020  n_error"],..    
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfc0: 2020 2020 2020 2022 636f 6d70 7574 6564         "computed
+0000dfd0: 223a 2070 7265 645f 6572 726f 727d 290d  ": pred_error}).
+0000dfe0: 0a20 2020 2020 2020 2064 665b 2272 656c  .        df["rel
+0000dff0: 6174 6976 655f 6572 726f 7222 5d20 3d20  ative_error"] = 
+0000e000: 2864 665b 2263 6f6d 7075 7465 6422 5d20  (df["computed"] 
+0000e010: 2d20 6466 5b22 7374 6f72 6564 225d 292e  - df["stored"]).
+0000e020: 6162 7328 2920 2f20 6466 5b22 7374 6f72  abs() / df["stor
+0000e030: 6564 225d 0d0a 2020 2020 2020 2020 0d0a  ed"]..        ..
+0000e040: 2020 2020 2020 2020 6966 2028 6466 5b22          if (df["
+0000e050: 7265 6c61 7469 7665 5f65 7272 6f72 225d  relative_error"]
+0000e060: 203e 2074 6f6c 6572 616e 6365 292e 616e   > tolerance).an
+0000e070: 7928 293a 0d0a 2020 2020 2020 2020 2020  y():..          
+0000e080: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000e090: 6f72 2866 2244 6174 6173 6574 2076 616c  or(f"Dataset val
+0000e0a0: 6964 6174 696f 6e20 6661 696c 6564 2075  idation failed u
+0000e0b0: 7369 6e67 2063 4e4d 4620 7072 6564 6963  sing cNMF predic
+0000e0c0: 7469 6f6e 2065 7272 6f72 2074 6f6c 6572  tion error toler
+0000e0d0: 616e 6365 206f 6620 7b74 6f6c 6572 616e  ance of {toleran
+0000e0e0: 6365 7d2e 2022 0d0a 2020 2020 2020 2020  ce}. "..        
+0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e100: 2020 2020 2022 5468 6973 2063 616e 206f       "This can o
+0000e110: 6363 7572 2077 6865 6e20 6461 7461 7365  ccur when datase
+0000e120: 7420 6f62 6a65 6374 7320 6172 6520 756e  t objects are un
+0000e130: 696e 7465 6e74 696f 6e61 6c6c 7920 616c  intentionally al
+0000e140: 7465 7265 6420 616e 6420 7468 6520 6d61  tered and the ma
+0000e150: 7472 6963 6573 2022 0d0a 2020 2020 2020  trices "..      
+0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e170: 2020 2020 2020 2022 6172 6520 6e6f 7420         "are not 
+0000e180: 636f 6e73 6973 7465 6e74 2077 6974 6820  consistent with 
+0000e190: 7468 6520 6f72 6967 696e 616c 206f 6e65  the original one
+0000e1a0: 7320 7573 6564 2066 6f72 2066 6163 746f  s used for facto
+0000e1b0: 7269 7a61 7469 6f6e 2e22 290d 0a0d 0a20  rization.").... 
+0000e1c0: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+0000e1d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000e1e0: 6465 6620 7661 6c69 6461 7465 5f66 6561  def validate_fea
+0000e1f0: 7475 7265 5f73 7461 7473 2873 656c 662c  ture_stats(self,
+0000e200: 2074 6f6c 6572 616e 6365 3a20 666c 6f61   tolerance: floa
+0000e210: 7420 3d20 3165 2d34 2920 2d3e 2070 642e  t = 1e-4) -> pd.
+0000e220: 4461 7461 4672 616d 653a 0d0a 2020 2020  DataFrame:..    
+0000e230: 2020 2020 2222 2256 616c 6964 6174 6520      """Validate 
+0000e240: 7468 6520 6461 7461 7365 7420 616e 6420  the dataset and 
+0000e250: 634e 4d46 2073 6f6c 7574 696f 6e73 2066  cNMF solutions f
+0000e260: 6f72 2065 6163 6820 7261 6e6b 2062 7920  or each rank by 
+0000e270: 636f 6d70 6172 696e 6720 7468 650d 0a20  comparing the.. 
+0000e280: 2020 2020 2020 2063 616c 6375 6c61 7465         calculate
+0000e290: 6420 6665 6174 7572 6520 7374 6174 6973  d feature statis
+0000e2a0: 7469 6373 2028 6d65 616e 2c20 5344 2c20  tics (mean, SD, 
+0000e2b0: 7661 7269 616e 6365 2920 7374 6f72 6564  variance) stored
+0000e2c0: 2069 6e20 7468 6520 6f62 6a65 6374 205b   in the object [
+0000e2d0: 7365 6c66 2e61 6461 7461 2e76 6172 5d20  self.adata.var] 
+0000e2e0: 746f 2074 686f 7365 2063 616c 6375 6c61  to those calcula
+0000e2f0: 7465 6420 6672 6f6d 2074 6865 0d0a 2020  ted from the..  
+0000e300: 2020 2020 2020 6461 7461 7365 7427 7320        dataset's 
+0000e310: 6461 7461 206d 6174 7269 6365 7320 5b62  data matrices [b
+0000e320: 6173 6564 206f 6e20 7365 6c66 2e61 6461  ased on self.ada
+0000e330: 7461 2e58 5d2e 2054 6869 7320 6361 6e20  ta.X]. This can 
+0000e340: 6265 2061 2071 7569 636b 2061 6e64 2073  be a quick and s
+0000e350: 656e 7369 7469 7665 2077 6179 2074 6f20  ensitive way to 
+0000e360: 6173 7365 7373 0d0a 2020 2020 2020 2020  assess..        
+0000e370: 7468 6174 2074 6865 2064 6174 6173 6574  that the dataset
+0000e380: 2773 2075 6e64 6572 6c79 696e 6720 6461  's underlying da
+0000e390: 7461 2068 6173 206e 6f74 2062 6565 6e20  ta has not been 
+0000e3a0: 616c 7465 7265 642e 0d0a 0d0a 2020 2020  altered.....    
+0000e3b0: 2020 2020 3a70 6172 616d 2074 6f6c 6572      :param toler
+0000e3c0: 616e 6365 3a20 6d61 7869 6d75 6d20 7265  ance: maximum re
+0000e3d0: 6c61 7469 7665 2065 7272 6f72 2066 6f72  lative error for
+0000e3e0: 2061 6e79 206b 2077 6865 6e20 636f 6d70   any k when comp
+0000e3f0: 7574 696e 6720 7468 6520 7072 6564 6963  uting the predic
+0000e400: 7469 6f6e 2065 7272 6f72 2c20 6465 6661  tion error, defa
+0000e410: 756c 7473 2074 6f20 302e 3030 3031 0d0a  ults to 0.0001..
+0000e420: 2020 2020 2020 2020 3a74 7970 6520 746f          :type to
+0000e430: 6c65 7261 6e63 653a 2066 6c6f 6174 2c20  lerance: float, 
+0000e440: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+0000e450: 2020 3a72 6169 7365 7320 5661 6c75 6545    :raises ValueE
+0000e460: 7272 6f72 3a20 6966 2074 6865 206d 6178  rror: if the max
+0000e470: 696d 756d 2072 656c 6174 6976 6520 6572  imum relative er
+0000e480: 726f 7220 6578 6365 6564 7320 7468 6520  ror exceeds the 
+0000e490: 746f 6c65 7261 6e63 650d 0a20 2020 2020  tolerance..     
+0000e4a0: 2020 203a 7265 7475 726e 3a20 4461 7461     :return: Data
+0000e4b0: 4672 616d 6520 7769 7468 2072 656c 6174  Frame with relat
+0000e4c0: 6976 6520 6572 726f 7220 666f 7220 6561  ive error for ea
+0000e4d0: 6368 2066 6561 7475 7265 0d0a 2020 2020  ch feature..    
+0000e4e0: 2020 2020 3a72 7479 7065 3a20 7064 2e44      :rtype: pd.D
+0000e4f0: 6174 6146 7261 6d65 0d0a 2020 2020 2020  ataFrame..      
+0000e500: 2020 2222 220d 0a20 2020 2020 2020 2058    """..        X
+0000e510: 203d 2073 656c 662e 746f 5f64 6628 290d   = self.to_df().
+0000e520: 0a20 2020 2020 2020 2063 616c 635f 7364  .        calc_sd
+0000e530: 203d 2058 2e73 7464 2829 0d0a 2020 2020   = X.std()..    
+0000e540: 2020 2020 6361 6c63 5f76 6172 203d 2058      calc_var = X
+0000e550: 2e76 6172 2829 0d0a 2020 2020 2020 2020  .var()..        
+0000e560: 6361 6c63 5f6d 6561 6e20 3d20 582e 6d65  calc_mean = X.me
+0000e570: 616e 2829 0d0a 2020 2020 2020 2020 7374  an()..        st
+0000e580: 6f72 6564 5f73 6420 3d20 7365 6c66 2e61  ored_sd = self.a
+0000e590: 6461 7461 2e76 6172 5b22 7364 225d 0d0a  data.var["sd"]..
+0000e5a0: 2020 2020 2020 2020 7374 6f72 6564 5f76          stored_v
+0000e5b0: 6172 203d 2073 656c 662e 6164 6174 612e  ar = self.adata.
+0000e5c0: 7661 725b 2276 6172 6961 6e63 6522 5d0d  var["variance"].
+0000e5d0: 0a20 2020 2020 2020 2073 746f 7265 645f  .        stored_
+0000e5e0: 6d65 616e 203d 2073 656c 662e 6164 6174  mean = self.adat
+0000e5f0: 612e 7661 725b 226d 6561 6e22 5d0d 0a0d  a.var["mean"]...
+0000e600: 0a20 2020 2020 2020 2064 6620 3d20 7064  .        df = pd
+0000e610: 2e44 6174 6146 7261 6d65 287b 2273 6422  .DataFrame({"sd"
+0000e620: 3a20 2863 616c 635f 7364 202d 2073 746f  : (calc_sd - sto
+0000e630: 7265 645f 7364 2920 2f20 7374 6f72 6564  red_sd) / stored
+0000e640: 5f73 642c 0d0a 2020 2020 2020 2020 2020  _sd,..          
+0000e650: 2020 2020 2020 2020 2020 2276 6172 6961            "varia
+0000e660: 6e63 6522 3a20 2863 616c 635f 7661 7220  nce": (calc_var 
+0000e670: 2d20 7374 6f72 6564 5f76 6172 2920 2f20  - stored_var) / 
+0000e680: 7374 6f72 6564 5f76 6172 2c0d 0a20 2020  stored_var,..   
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 2022 6d65 616e 223a 2028 6361 6c63 5f6d   "mean": (calc_m
+0000e6b0: 6561 6e20 2d20 7374 6f72 6564 5f6d 6561  ean - stored_mea
+0000e6c0: 6e29 202f 2073 746f 7265 645f 6d65 616e  n) / stored_mean
+0000e6d0: 7d29 0d0a 0d0a 2020 2020 2020 2020 6966  })....        if
+0000e6e0: 2064 662e 6162 7328 292e 6d61 7828 292e   df.abs().max().
+0000e6f0: 6d61 7828 2920 3e20 746f 6c65 7261 6e63  max() > toleranc
+0000e700: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000e710: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000e720: 2866 2244 6174 6173 6574 2076 616c 6964  (f"Dataset valid
+0000e730: 6174 696f 6e20 6661 696c 6564 2075 7369  ation failed usi
+0000e740: 6e67 2066 6561 7475 7265 2d77 6973 6520  ng feature-wise 
+0000e750: 5344 2c20 7661 7269 616e 6365 2c20 616e  SD, variance, an
+0000e760: 642f 6f72 206d 6561 6e20 7769 7468 2061  d/or mean with a
+0000e770: 2072 656c 6174 6976 6520 6572 726f 7220   relative error 
+0000e780: 7769 7468 696e 207b 746f 6c65 7261 6e63  within {toleranc
+0000e790: 657d 2e20 220d 0a20 2020 2020 2020 2020  e}. "..         
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7b0: 2020 2022 5468 6973 2063 616e 206f 6363     "This can occ
+0000e7c0: 7572 2077 6865 6e20 6461 7461 7365 7420  ur when dataset 
+0000e7d0: 6f62 6a65 6374 7320 6172 6520 756e 696e  objects are unin
+0000e7e0: 7465 6e74 696f 6e61 6c6c 7920 616c 7465  tentionally alte
+0000e7f0: 7265 6420 616e 6420 7468 6520 6d61 7472  red and the matr
+0000e800: 6963 6573 2022 0d0a 2020 2020 2020 2020  ices "..        
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2020 2020 2261 7265 206e 6f74 2063 6f6e      "are not con
+0000e830: 7369 7374 656e 7420 7769 7468 2074 6865  sistent with the
+0000e840: 206f 7269 6769 6e61 6c20 6f6e 6573 2075   original ones u
+0000e850: 7365 6420 666f 7220 6661 6374 6f72 697a  sed for factoriz
+0000e860: 6174 696f 6e2e 2229 0d0a 2020 2020 2020  ation.")..      
+0000e870: 2020 7265 7475 726e 2064 660d 0a0d 0a20    return df.... 
+0000e880: 2020 2064 6566 2067 6574 5f6d 6574 6164     def get_metad
+0000e890: 6174 615f 6466 2873 656c 662c 0d0a 2020  ata_df(self,..  
+0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8b0: 2020 2020 2020 696e 636c 7564 655f 6361        include_ca
+0000e8c0: 7465 676f 7269 6361 6c3a 2062 6f6f 6c20  tegorical: bool 
+0000e8d0: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8f0: 2069 6e63 6c75 6465 5f6e 756d 6572 6963   include_numeric
+0000e900: 616c 3a20 626f 6f6c 203d 2054 7275 650d  al: bool = True.
+0000e910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e920: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
+0000e930: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
+0000e940: 2020 2020 2022 2222 4765 7420 7361 6d70       """Get samp
+0000e950: 6c65 2f6f 6273 6572 7661 7469 6f6e 206d  le/observation m
+0000e960: 6574 6164 6174 612e 0d0a 0d0a 2020 2020  etadata.....    
+0000e970: 2020 2020 3a70 6172 616d 2069 6e63 6c75      :param inclu
+0000e980: 6465 5f63 6174 6567 6f72 6963 616c 3a20  de_categorical: 
+0000e990: 496e 636c 7564 6520 6361 7465 676f 7269  Include categori
+0000e9a0: 6361 6c20 6d65 7461 6461 7461 206c 6179  cal metadata lay
+0000e9b0: 6572 732c 2064 6566 6175 6c74 7320 746f  ers, defaults to
+0000e9c0: 2054 7275 650d 0a20 2020 2020 2020 203a   True..        :
+0000e9d0: 7479 7065 2069 6e63 6c75 6465 5f63 6174  type include_cat
+0000e9e0: 6567 6f72 6963 616c 3a20 626f 6f6c 2c20  egorical: bool, 
+0000e9f0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+0000ea00: 2020 3a70 6172 616d 2069 6e63 6c75 6465    :param include
+0000ea10: 5f6e 756d 6572 6963 616c 3a20 496e 636c  _numerical: Incl
+0000ea20: 7564 6520 6e75 6d65 7269 6361 6c20 6d65  ude numerical me
+0000ea30: 7461 6461 7461 206c 6179 6572 732c 2064  tadata layers, d
+0000ea40: 6566 6175 6c74 7320 746f 2054 7275 650d  efaults to True.
+0000ea50: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
+0000ea60: 6e63 6c75 6465 5f6e 756d 6572 6963 616c  nclude_numerical
+0000ea70: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+0000ea80: 0d0a 2020 2020 2020 2020 3a72 6169 7365  ..        :raise
+0000ea90: 7320 5661 6c75 6545 7272 6f72 3a20 4572  s ValueError: Er
+0000eaa0: 726f 7220 6966 206d 6574 6164 6174 6120  ror if metadata 
+0000eab0: 7479 7065 7320 6172 6520 6e6f 7420 7265  types are not re
+0000eac0: 636f 676e 697a 6564 0d0a 2020 2020 2020  cognized..      
+0000ead0: 2020 3a72 6574 7572 6e3a 206f 6273 6572    :return: obser
+0000eae0: 7661 7469 6f6e 7320 c397 206d 6574 6164  vations .. metad
+0000eaf0: 6174 6120 6d61 7472 6978 0d0a 2020 2020  ata matrix..    
+0000eb00: 2020 2020 3a72 7479 7065 3a20 7064 2e44      :rtype: pd.D
+0000eb10: 6174 6146 7261 6d65 0d0a 2020 2020 2020  ataFrame..      
+0000eb20: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
+0000eb30: 7479 7065 7320 3d20 5b5d 0d0a 2020 2020  types = []..    
+0000eb40: 2020 2020 6966 2069 6e63 6c75 6465 5f63      if include_c
+0000eb50: 6174 6567 6f72 6963 616c 3a0d 0a20 2020  ategorical:..   
+0000eb60: 2020 2020 2020 2020 2064 7479 7065 732e           dtypes.
+0000eb70: 6170 7065 6e64 2822 6361 7465 676f 7279  append("category
+0000eb80: 2229 0d0a 2020 2020 2020 2020 6966 2069  ")..        if i
+0000eb90: 6e63 6c75 6465 5f6e 756d 6572 6963 616c  nclude_numerical
+0000eba0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+0000ebb0: 7479 7065 7320 2b3d 205b 2266 6c6f 6174  types += ["float
+0000ebc0: 222c 2022 696e 7422 5d0d 0a20 2020 2020  ", "int"]..     
+0000ebd0: 2020 2075 6e65 7870 6c61 696e 6564 5f63     unexplained_c
+0000ebe0: 6f6c 7320 3d20 7365 6c66 2e61 6461 7461  ols = self.adata
+0000ebf0: 2e6f 6273 2e73 656c 6563 745f 6474 7970  .obs.select_dtyp
+0000ec00: 6573 2865 7863 6c75 6465 3d28 2263 6174  es(exclude=("cat
+0000ec10: 6567 6f72 7922 2c20 2266 6c6f 6174 222c  egory", "float",
+0000ec20: 2022 696e 7422 2929 2e63 6f6c 756d 6e73   "int")).columns
+0000ec30: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0000ec40: 2875 6e65 7870 6c61 696e 6564 5f63 6f6c  (unexplained_col
+0000ec50: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
+0000ec60: 2020 2020 2075 6e65 7870 6c61 696e 6564       unexplained
+0000ec70: 5f63 6f6c 5f73 7472 203d 2022 2c20 222e  _col_str = ", ".
+0000ec80: 6a6f 696e 2875 6e65 7870 6c61 696e 6564  join(unexplained
+0000ec90: 5f63 6f6c 7329 0d0a 2020 2020 2020 2020  _cols)..        
+0000eca0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000ecb0: 7272 6f72 2866 227b 756e 6578 706c 6169  rror(f"{unexplai
+0000ecc0: 6e65 645f 636f 6c5f 7374 727d 206d 6574  ned_col_str} met
+0000ecd0: 6164 6174 6120 636f 6c75 6d6e 7320 6861  adata columns ha
+0000ece0: 7665 2075 6e72 6563 6f67 6e69 7a65 6420  ve unrecognized 
+0000ecf0: 6474 7970 6573 2e22 290d 0a20 2020 2020  dtypes.")..     
+0000ed00: 2020 2064 6620 3d20 7365 6c66 2e61 6461     df = self.ada
+0000ed10: 7461 2e6f 6273 2e73 656c 6563 745f 6474  ta.obs.select_dt
+0000ed20: 7970 6573 2869 6e63 6c75 6465 3d64 7479  ypes(include=dty
+0000ed30: 7065 7329 0d0a 2020 2020 2020 2020 6466  pes)..        df
+0000ed40: 203d 2064 662e 6472 6f70 6e61 2861 7869   = df.dropna(axi
+0000ed50: 733d 312c 2068 6f77 3d22 616c 6c22 290d  s=1, how="all").
+0000ed60: 0a20 2020 2020 2020 2064 6620 3d20 6466  .        df = df
+0000ed70: 2e72 6570 6c61 6365 2822 6e61 6e22 2c20  .replace("nan", 
+0000ed80: 6e70 2e4e 614e 2920 2023 544f 444f 3a20  np.NaN)  #TODO: 
+0000ed90: 4164 6472 6573 7320 6572 726f 723a 202f  Address error: /
+0000eda0: 686f 6d65 2f74 6276 6572 6865 792f 6d69  home/tbverhey/mi
+0000edb0: 6e69 636f 6e64 6133 2f65 6e76 732f 6d6f  niconda3/envs/mo
+0000edc0: 7361 6963 6d70 692f 6c69 622f 7079 7468  saicmpi/lib/pyth
+0000edd0: 6f6e 332e 3131 2f73 6974 652d 7061 636b  on3.11/site-pack
+0000ede0: 6167 6573 2f6d 6f73 6169 636d 7069 2f64  ages/mosaicmpi/d
+0000edf0: 6174 6173 6574 2e70 793a 3130 3231 3a20  ataset.py:1021: 
+0000ee00: 4675 7475 7265 5761 726e 696e 673a 2054  FutureWarning: T
+0000ee10: 6865 2062 6568 6176 696f 7220 6f66 2053  he behavior of S
+0000ee20: 6572 6965 732e 7265 706c 6163 6520 2861  eries.replace (a
+0000ee30: 6e64 2044 6174 6146 7261 6d65 2e72 6570  nd DataFrame.rep
+0000ee40: 6c61 6365 2920 7769 7468 2043 6174 6567  lace) with Categ
+0000ee50: 6f72 6963 616c 4474 7970 6520 6973 2064  oricalDtype is d
+0000ee60: 6570 7265 6361 7465 642e 2049 6e20 6120  eprecated. In a 
+0000ee70: 6675 7475 7265 2076 6572 7369 6f6e 2c20  future version, 
+0000ee80: 7265 706c 6163 6520 7769 6c6c 206f 6e6c  replace will onl
+0000ee90: 7920 6265 2075 7365 6420 666f 7220 6361  y be used for ca
+0000eea0: 7365 7320 7468 6174 2070 7265 7365 7276  ses that preserv
+0000eeb0: 6520 7468 6520 6361 7465 676f 7269 6573  e the categories
+0000eec0: 2e20 546f 2063 6861 6e67 6520 7468 6520  . To change the 
+0000eed0: 6361 7465 676f 7269 6573 2c20 7573 6520  categories, use 
+0000eee0: 7365 722e 6361 742e 7265 6e61 6d65 5f63  ser.cat.rename_c
+0000eef0: 6174 6567 6f72 6965 7320 696e 7374 6561  ategories instea
+0000ef00: 642e 0d0a 2020 2020 2020 2020 7265 7475  d...        retu
+0000ef10: 726e 2064 660d 0a20 2020 200d 0a20 2020  rn df..    ..   
+0000ef20: 2064 6566 2067 6574 5f63 6174 6567 6f72   def get_categor
+0000ef30: 795f 6f76 6572 7265 7072 6573 656e 7461  y_overrepresenta
+0000ef40: 7469 6f6e 2873 656c 662c 0d0a 2020 2020  tion(self,..    
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef70: 2020 2020 6c61 7965 723a 2073 7472 2c0d      layer: str,.
+0000ef80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2020 2020 2020 2020 2074 7275 6e63 6174           truncat
+0000efb0: 655f 6e65 6761 7469 7665 3a20 626f 6f6c  e_negative: bool
+0000efc0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eff0: 2020 7375 6273 6574 5f63 6174 6567 6f72    subset_categor
+0000f000: 6965 733a 2043 6f6c 6c65 6374 696f 6e5b  ies: Collection[
+0000f010: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+0000f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f040: 2020 2020 2029 202d 3e20 7064 2e44 6174       ) -> pd.Dat
+0000f050: 6146 7261 6d65 3a0d 0a20 2020 2020 2020  aFrame:..       
+0000f060: 2022 2222 4361 6c63 756c 6174 6520 5065   """Calculate Pe
+0000f070: 6172 736f 6e20 7265 7369 6475 616c 206f  arson residual o
+0000f080: 6620 6368 692d 7371 7561 7265 6420 7465  f chi-squared te
+0000f090: 7374 2c20 6173 736f 6369 6174 696e 6720  st, associating 
+0000f0a0: 7072 6f67 7261 6d73 2066 6f72 2065 6163  programs for eac
+0000f0b0: 6820 7261 6e6b 2028 6b29 2074 6f20 6361  h rank (k) to ca
+0000f0c0: 7465 676f 7269 6573 206f 6620 7361 6d70  tegories of samp
+0000f0d0: 6c65 732f 6f62 7365 7276 6174 696f 6e73  les/observations
+0000f0e0: 2e20 4279 2064 6566 6175 6c74 2c20 7472  . By default, tr
+0000f0f0: 756e 6361 7465 7320 6e65 6761 7469 7665  uncates negative
+0000f100: 2076 616c 7565 732e 0d0a 0d0a 2020 2020   values.....    
+0000f110: 2020 2020 3a70 6172 616d 206c 6179 6572      :param layer
+0000f120: 3a20 6e61 6d65 206f 6620 6361 7465 676f  : name of catego
+0000f130: 7269 6361 6c20 6461 7461 206c 6179 6572  rical data layer
+0000f140: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+0000f150: 6c61 7965 723a 2073 7472 0d0a 2020 2020  layer: str..    
+0000f160: 2020 2020 3a70 6172 616d 2074 7275 6e63      :param trunc
+0000f170: 6174 655f 6e65 6761 7469 7665 3a20 5472  ate_negative: Tr
+0000f180: 756e 6361 7465 206e 6567 6174 6976 6520  uncate negative 
+0000f190: 7265 7369 6475 616c 7320 746f 2030 2c20  residuals to 0, 
+0000f1a0: 6465 6661 756c 7473 2074 6f20 5472 7565  defaults to True
+0000f1b0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+0000f1c0: 7472 756e 6361 7465 5f6e 6567 6174 6976  truncate_negativ
+0000f1d0: 653a 2062 6f6f 6c2c 206f 7074 696f 6e61  e: bool, optiona
+0000f1e0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+0000f1f0: 6d20 7375 6273 6574 5f63 6174 6567 6f72  m subset_categor
+0000f200: 6965 733a 2050 726f 7669 6465 2061 2073  ies: Provide a s
+0000f210: 7562 7365 7420 6f66 2063 6174 6567 6f72  ubset of categor
+0000f220: 6965 7320 666f 7220 6361 6c63 756c 6174  ies for calculat
+0000f230: 696e 6720 6f76 6572 7265 7072 6573 656e  ing overrepresen
+0000f240: 7461 7469 6f6e 0d0a 2020 2020 2020 2020  tation..        
+0000f250: 3a74 7970 6520 7375 6273 6574 5f63 6174  :type subset_cat
+0000f260: 6567 6f72 6965 733a 2043 6f6c 6c65 6374  egories: Collect
+0000f270: 696f 6e5b 7374 725d 0d0a 2020 2020 2020  ion[str]..      
+0000f280: 2020 3a72 6574 7572 6e3a 2063 6174 6567    :return: categ
+0000f290: 6f72 7920 c397 2070 726f 6772 616d 206d  ory .. program m
+0000f2a0: 6174 7269 7820 6f66 206f 7665 7272 6570  atrix of overrep
+0000f2b0: 7265 7365 6e74 6174 696f 6e20 7661 6c75  resentation valu
+0000f2c0: 6573 0d0a 2020 2020 2020 2020 3a72 7479  es..        :rty
+0000f2d0: 7065 3a20 7064 2e44 6174 6146 7261 6d65  pe: pd.DataFrame
+0000f2e0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000f2f0: 2020 2020 2020 2075 7361 6765 203d 2073         usage = s
+0000f300: 656c 662e 6765 745f 7573 6167 6573 286e  elf.get_usages(n
+0000f310: 6f72 6d61 6c69 7a65 3d54 7275 6529 2e63  ormalize=True).c
+0000f320: 6f70 7928 290d 0a20 2020 2020 2020 2073  opy()..        s
+0000f330: 616d 706c 655f 746f 5f63 6c61 7373 203d  ample_to_class =
+0000f340: 2073 656c 662e 6765 745f 6d65 7461 6461   self.get_metada
+0000f350: 7461 5f64 6628 295b 6c61 7965 725d 0d0a  ta_df()[layer]..
+0000f360: 2020 2020 2020 2020 6966 2073 7562 7365          if subse
+0000f370: 745f 6361 7465 676f 7269 6573 2069 7320  t_categories is 
+0000f380: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000f390: 2020 2020 2020 2073 616d 706c 655f 746f         sample_to
+0000f3a0: 5f63 6c61 7373 5b7e 7361 6d70 6c65 5f74  _class[~sample_t
+0000f3b0: 6f5f 636c 6173 732e 6973 696e 2873 7562  o_class.isin(sub
+0000f3c0: 7365 745f 6361 7465 676f 7269 6573 295d  set_categories)]
+0000f3d0: 203d 206e 702e 4e61 4e0d 0a20 2020 2020   = np.NaN..     
+0000f3e0: 2020 2075 7361 6765 2e69 6e64 6578 203d     usage.index =
+0000f3f0: 2075 7361 6765 2e69 6e64 6578 2e6d 6170   usage.index.map
+0000f400: 2873 616d 706c 655f 746f 5f63 6c61 7373  (sample_to_class
+0000f410: 290d 0a20 2020 2020 2020 206f 6273 6572  )..        obser
+0000f420: 7665 6420 3d20 7573 6167 652e 6772 6f75  ved = usage.grou
+0000f430: 7062 7928 6c65 7665 6c3d 302c 206f 6273  pby(level=0, obs
+0000f440: 6572 7665 643d 5472 7565 292e 7375 6d28  erved=True).sum(
+0000f450: 290d 0a20 2020 2020 2020 206f 6273 6572  )..        obser
+0000f460: 7665 6420 3d20 6f62 7365 7276 6564 5b6f  ved = observed[o
+0000f470: 6273 6572 7665 642e 7375 6d28 6178 6973  bserved.sum(axis
+0000f480: 3d31 2920 3e20 305d 0d0a 2020 2020 2020  =1) > 0]..      
+0000f490: 2020 6e5f 6361 7465 676f 7269 6573 203d    n_categories =
+0000f4a0: 206f 6273 6572 7665 642e 7368 6170 655b   observed.shape[
+0000f4b0: 305d 0d0a 2020 2020 2020 2020 6966 206e  0]..        if n
+0000f4c0: 5f63 6174 6567 6f72 6965 7320 3c20 323a  _categories < 2:
+0000f4d0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000f4e0: 206c 6179 6572 2021 3d20 2268 7667 5f61   layer != "hvg_a
+0000f4f0: 6c6c 5f30 223a 0d0a 2020 2020 2020 2020  ll_0":..        
+0000f500: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+0000f510: 7761 726e 696e 6728 6622 4f76 6572 7265  warning(f"Overre
+0000f520: 7072 6573 656e 7461 7469 6f6e 2063 6f75  presentation cou
+0000f530: 6c64 206e 6f74 2062 6520 6361 6c63 756c  ld not be calcul
+0000f540: 6174 6564 2066 6f72 206c 6179 6572 2027  ated for layer '
+0000f550: 7b6c 6179 6572 7d27 2c20 6173 206f 6e6c  {layer}', as onl
+0000f560: 7920 7b6e 5f63 6174 6567 6f72 6965 737d  y {n_categories}
+0000f570: 2063 6174 6567 6f72 6965 7320 7765 7265   categories were
+0000f580: 2066 6f75 6e64 2069 6e20 7468 6520 6461   found in the da
+0000f590: 7461 2e20 220d 0a20 2020 2020 2020 2020  ta. "..         
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5b0: 2020 2020 2020 2066 224e 6f74 6520 7468         f"Note th
+0000f5c0: 6174 2065 6d70 7479 2076 616c 7565 7320  at empty values 
+0000f5d0: 696e 2074 6865 206d 6574 6164 6174 6120  in the metadata 
+0000f5e0: 6172 6520 6e6f 7420 636f 6e73 6964 6572  are not consider
+0000f5f0: 6564 2061 2063 6174 6567 6f72 792e 2022  ed a category. "
+0000f600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 6622 4f76 6572 7265 7072 6573 656e    f"Overrepresen
+0000f630: 7461 7469 6f6e 2063 616e 6e6f 7420 6265  tation cannot be
+0000f640: 2063 616c 6375 6c61 7465 6420 7769 7468   calculated with
+0000f650: 2066 6577 6572 2074 6861 6e20 3220 6361   fewer than 2 ca
+0000f660: 7465 676f 7269 6573 2066 6f72 2065 6163  tegories for eac
+0000f670: 6820 6c61 7965 722e 2022 290d 0a20 2020  h layer. ")..   
+0000f680: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000f690: 7064 2e44 6174 6146 7261 6d65 286e 702e  pd.DataFrame(np.
+0000f6a0: 4e61 4e2c 2069 6e64 6578 203d 206f 6273  NaN, index = obs
+0000f6b0: 6572 7665 642e 696e 6465 782c 2063 6f6c  erved.index, col
+0000f6c0: 756d 6e73 3d6f 6273 6572 7665 642e 636f  umns=observed.co
+0000f6d0: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
+0000f6e0: 6578 7065 6374 6564 203d 205b 5d0d 0a20  expected = [].. 
+0000f6f0: 2020 2020 2020 2066 6f72 206b 2c20 6f62         for k, ob
+0000f700: 735f 6b20 696e 206f 6273 6572 7665 642e  s_k in observed.
+0000f710: 542e 6772 6f75 7062 7928 6c65 7665 6c3d  T.groupby(level=
+0000f720: 3129 3a0d 0a20 2020 2020 2020 2020 2020  1):..           
+0000f730: 2065 7870 5f6b 203d 2070 642e 4461 7461   exp_k = pd.Data
+0000f740: 4672 616d 6528 6f62 735f 6b2e 7375 6d28  Frame(obs_k.sum(
+0000f750: 6178 6973 3d31 2929 2040 2070 642e 4461  axis=1)) @ pd.Da
+0000f760: 7461 4672 616d 6528 6f62 735f 6b2e 7375  taFrame(obs_k.su
+0000f770: 6d28 6178 6973 3d30 2929 2e54 202f 206f  m(axis=0)).T / o
+0000f780: 6273 5f6b 2e73 756d 2829 2e73 756d 2829  bs_k.sum().sum()
+0000f790: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+0000f7a0: 7065 6374 6564 2e61 7070 656e 6428 6578  pected.append(ex
+0000f7b0: 705f 6b29 0d0a 2020 2020 2020 2020 6578  p_k)..        ex
+0000f7c0: 7065 6374 6564 203d 2070 642e 636f 6e63  pected = pd.conc
+0000f7d0: 6174 2865 7870 6563 7465 6429 2e54 0d0a  at(expected).T..
+0000f7e0: 2020 2020 2020 2020 6368 6973 715f 7265          chisq_re
+0000f7f0: 7369 6420 3d20 286f 6273 6572 7665 6420  sid = (observed 
+0000f800: 2d20 6578 7065 6374 6564 2920 2f20 6e70  - expected) / np
+0000f810: 2e73 7172 7428 6578 7065 6374 6564 2920  .sqrt(expected) 
+0000f820: 2023 2070 6561 7273 6f6e 2072 6573 6964   # pearson resid
+0000f830: 7561 6c20 6f66 2063 6869 2d73 7175 6172  ual of chi-squar
+0000f840: 6564 2074 6573 7420 6f66 2063 6f6e 7469  ed test of conti
+0000f850: 6e67 656e 6379 2074 6162 6c65 0d0a 2020  ngency table..  
+0000f860: 2020 2020 2020 6966 2074 7275 6e63 6174        if truncat
+0000f870: 655f 6e65 6761 7469 7665 3a0d 0a20 2020  e_negative:..   
+0000f880: 2020 2020 2020 2020 2063 6869 7371 5f72           chisq_r
+0000f890: 6573 6964 203d 2063 6869 7371 5f72 6573  esid = chisq_res
+0000f8a0: 6964 2e63 6c69 7028 6c6f 7765 723d 3029  id.clip(lower=0)
+0000f8b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000f8c0: 2063 6869 7371 5f72 6573 6964 0d0a 2020   chisq_resid..  
+0000f8d0: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+0000f8e0: 2020 6465 6620 6765 745f 6d65 7461 6461    def get_metada
+0000f8f0: 7461 5f63 6f72 7265 6c61 7469 6f6e 2873  ta_correlation(s
+0000f900: 656c 662c 200d 0a20 2020 2020 2020 2020  elf, ..         
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f920: 2020 2020 2020 2020 6c61 7965 723a 2073          layer: s
+0000f930: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
+0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f950: 2020 2020 2020 6d65 7468 6f64 3a20 7374        method: st
+0000f960: 7220 3d20 2270 6561 7273 6f6e 220d 0a20  r = "pearson".. 
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f990: 2920 2d3e 2070 642e 5365 7269 6573 3a0d  ) -> pd.Series:.
+0000f9a0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
+0000f9b0: 756c 6174 6520 5065 6172 736f 6e20 636f  ulate Pearson co
+0000f9c0: 7272 656c 6174 696f 6e20 6f66 2047 4550  rrelation of GEP
+0000f9d0: 2075 7361 6765 2074 6f20 6e75 6d65 7269   usage to numeri
+0000f9e0: 6361 6c20 6d65 7461 6461 7461 2061 6372  cal metadata acr
+0000f9f0: 6f73 7320 7361 6d70 6c65 732f 6f62 7365  oss samples/obse
+0000fa00: 7276 6174 696f 6e73 2e0d 0a0d 0a20 2020  rvations.....   
+0000fa10: 2020 2020 203a 7061 7261 6d20 6c61 7965       :param laye
+0000fa20: 723a 206e 616d 6520 6f66 206e 756d 6572  r: name of numer
+0000fa30: 6963 616c 2064 6174 6120 6c61 7965 720d  ical data layer.
+0000fa40: 0a20 2020 2020 2020 203a 7479 7065 206c  .        :type l
+0000fa50: 6179 6572 3a20 7374 720d 0a20 2020 2020  ayer: str..     
+0000fa60: 2020 203a 7061 7261 6d20 6d65 7468 6f64     :param method
+0000fa70: 3a20 436f 7272 656c 6174 696f 6e20 6d65  : Correlation me
+0000fa80: 7468 6f64 3a20 2270 6561 7273 6f6e 222c  thod: "pearson",
+0000fa90: 2022 7370 6561 726d 616e 222c 206f 7220   "spearman", or 
+0000faa0: 226b 656e 6461 6c6c 222e 2044 6566 6175  "kendall". Defau
+0000fab0: 6c74 7320 746f 2022 7065 6172 736f 6e22  lts to "pearson"
+0000fac0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+0000fad0: 6d65 7468 6f64 3a20 7374 722c 206f 7074  method: str, opt
+0000fae0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+0000faf0: 7265 7475 726e 3a20 636f 7272 656c 6174  return: correlat
+0000fb00: 696f 6e20 6f66 2047 4550 2074 6f20 6d65  ion of GEP to me
+0000fb10: 7461 6461 7461 0d0a 2020 2020 2020 2020  tadata..        
+0000fb20: 3a72 7479 7065 3a20 7064 2e53 6572 6965  :rtype: pd.Serie
+0000fb30: 730d 0a20 2020 2020 2020 2022 2222 0d0a  s..        """..
+0000fb40: 2020 2020 2020 2020 7573 6167 6520 3d20          usage = 
+0000fb50: 7365 6c66 2e67 6574 5f75 7361 6765 7328  self.get_usages(
+0000fb60: 292e 636f 7079 2829 0d0a 2020 2020 2020  ).copy()..      
+0000fb70: 2020 6d65 7461 6461 7461 203d 2073 656c    metadata = sel
+0000fb80: 662e 6765 745f 6d65 7461 6461 7461 5f64  f.get_metadata_d
+0000fb90: 6628 295b 6c61 7965 725d 0d0a 2020 2020  f()[layer]..    
+0000fba0: 2020 2020 6d64 5f63 6f72 7220 3d20 7573      md_corr = us
+0000fbb0: 6167 652e 636f 7272 7769 7468 286d 6574  age.corrwith(met
+0000fbc0: 6164 6174 612c 206d 6574 686f 643d 6d65  adata, method=me
+0000fbd0: 7468 6f64 290d 0a20 2020 2020 2020 2072  thod)..        r
+0000fbe0: 6574 7572 6e20 6d64 5f63 6f72 720d 0a20  eturn md_corr.. 
+0000fbf0: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+0000fc00: 2061 7070 656e 645f 746f 5f68 6973 746f   append_to_histo
+0000fc10: 7279 2873 656c 662c 2065 6e74 7279 293a  ry(self, entry):
+0000fc20: 0d0a 2020 2020 2020 2020 2222 2241 6464  ..        """Add
+0000fc30: 2065 6e74 7279 2074 6f20 4461 7461 7365   entry to Datase
+0000fc40: 7420 6869 7374 6f72 792e 0d0a 0d0a 2020  t history.....  
+0000fc50: 2020 2020 2020 3a70 6172 616d 2065 6e74        :param ent
+0000fc60: 7279 3a20 4465 7363 7269 7074 696f 6e20  ry: Description 
+0000fc70: 6f66 2065 7665 6e74 2074 6f20 7265 636f  of event to reco
+0000fc80: 7264 2069 6e20 7468 6520 6869 7374 6f72  rd in the histor
+0000fc90: 792e 0d0a 2020 2020 2020 2020 3a74 7970  y...        :typ
+0000fca0: 6520 656e 7472 793a 2073 7472 0d0a 2020  e entry: str..  
+0000fcb0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000fcc0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+0000fcd0: 735b 2268 6973 746f 7279 225d 5b64 6174  s["history"][dat
+0000fce0: 6574 696d 652e 7574 636e 6f77 2829 2e69  etime.utcnow().i
+0000fcf0: 736f 666f 726d 6174 2829 5d20 3d20 656e  soformat()] = en
+0000fd00: 7472 790d 0a20 2020 2020 2020 200d 0a20  try..        .. 
+0000fd10: 2020 2064 6566 2067 6574 5f68 6973 746f     def get_histo
+0000fd20: 7279 2873 656c 6629 3a0d 0a20 2020 2020  ry(self):..     
+0000fd30: 2020 2022 2222 5265 7475 726e 7320 7469     """Returns ti
+0000fd40: 6d65 7374 616d 7065 6420 6869 7374 6f72  mestamped histor
+0000fd50: 7920 6f66 2044 6174 6173 6574 206f 626a  y of Dataset obj
+0000fd60: 6563 742e 0d0a 0d0a 2020 2020 2020 2020  ect.....        
+0000fd70: 3a72 6574 7572 6e3a 2068 6973 746f 7279  :return: history
+0000fd80: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+0000fd90: 3a20 6469 6374 0d0a 2020 2020 2020 2020  : dict..        
+0000fda0: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+0000fdb0: 7572 6e20 7365 6c66 2e61 6461 7461 2e75  urn self.adata.u
+0000fdc0: 6e73 5b22 6869 7374 6f72 7922 5d         ns["history"]
```

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/gprofiler.py` & `mosaicmpi-2.5.2/src/mosaicmpi/gprofiler.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/integration.py` & `mosaicmpi-2.5.2/src/mosaicmpi/integration.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/nancorrmp.py` & `mosaicmpi-2.5.2/src/mosaicmpi/nancorrmp.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/network.py` & `mosaicmpi-2.5.2/src/mosaicmpi/network.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/orphan.py` & `mosaicmpi-2.5.2/src/mosaicmpi/orphan.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/plots.py` & `mosaicmpi-2.5.2/src/mosaicmpi/plots.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi/utils.py` & `mosaicmpi-2.5.2/src/mosaicmpi/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi.egg-info/PKG-INFO` & `mosaicmpi-2.5.2/src/mosaicmpi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicmpi
-Version: 2.5.1
+Version: 2.5.2
 Summary: mosaicMPI: Mosaic Multi-resolution Program Integration
 Home-page: https://github.com/MorrissyLab/mosaicMPI
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/mosaicMPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 Requires-Dist: fastcluster
 Requires-Dist: tqdm
 
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
 # mosaicMPI: Mosaic Multi-resolution Program Integration
 
-![version badge](https://img.shields.io/badge/version-2.5.1-blue)
+![version badge](https://img.shields.io/badge/version-2.5.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
```

### Comparing `mosaicmpi-2.5.1/src/mosaicmpi.egg-info/SOURCES.txt` & `mosaicmpi-2.5.2/src/mosaicmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

