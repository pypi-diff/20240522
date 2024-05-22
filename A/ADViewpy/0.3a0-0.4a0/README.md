# Comparing `tmp/ADViewpy-0.3a0.tar.gz` & `tmp/ADViewpy-0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADViewpy-0.3a0.tar", last modified: Wed May 22 13:48:54 2024, max compression
+gzip compressed data, was "ADViewpy-0.4a0.tar", last modified: Wed May 22 13:55:03 2024, max compression
```

## Comparing `ADViewpy-0.3a0.tar` & `ADViewpy-0.4a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:48:54.064397 ADViewpy-0.3a0/
-drwxrwxrwx   0        0        0        0 2024-05-22 13:48:54.056354 ADViewpy-0.3a0/ADViewpy/
--rw-rw-rw-   0        0        0    46666 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/ADViewpy.py
--rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.3a0/ADViewpy/__init__.py
--rw-rw-rw-   0        0        0    19348 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/myCanvas.py
--rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.3a0/ADViewpy/myUtils.py
--rw-rw-rw-   0        0        0    56158 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/pairwiseCanvas.py
--rw-rw-rw-   0        0        0    23499 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/rtCanvas.py
--rw-rw-rw-   0        0        0    65738 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/tcCanvas.py
--rw-rw-rw-   0        0        0    21925 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/treeDistributionView.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:48:54.064397 ADViewpy-0.3a0/ADViewpy.egg-info/
--rw-rw-rw-   0        0        0     6202 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6202 2024-05-22 13:48:54.065402 ADViewpy-0.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.3a0/README.md
--rw-rw-rw-   0        0        0      539 2024-05-22 13:47:29.000000 ADViewpy-0.3a0/pyproject.toml
--rw-rw-rw-   0        0        0       94 2024-05-22 13:48:54.066403 ADViewpy-0.3a0/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-22 13:47:29.000000 ADViewpy-0.3a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:55:03.828775 ADViewpy-0.4a0/
+drwxrwxrwx   0        0        0        0 2024-05-22 13:55:03.821261 ADViewpy-0.4a0/ADViewpy/
+-rw-rw-rw-   0        0        0    46666 2024-05-22 13:41:29.000000 ADViewpy-0.4a0/ADViewpy/ADViewpy.py
+-rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.4a0/ADViewpy/__init__.py
+-rw-rw-rw-   0        0        0    19348 2024-05-22 13:41:29.000000 ADViewpy-0.4a0/ADViewpy/myCanvas.py
+-rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.4a0/ADViewpy/myUtils.py
+-rw-rw-rw-   0        0        0    56158 2024-05-22 13:41:29.000000 ADViewpy-0.4a0/ADViewpy/pairwiseCanvas.py
+-rw-rw-rw-   0        0        0    23499 2024-05-22 13:41:29.000000 ADViewpy-0.4a0/ADViewpy/rtCanvas.py
+-rw-rw-rw-   0        0        0    65738 2024-05-22 13:41:29.000000 ADViewpy-0.4a0/ADViewpy/tcCanvas.py
+-rw-rw-rw-   0        0        0    21925 2024-05-22 13:41:29.000000 ADViewpy-0.4a0/ADViewpy/treeDistributionView.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:55:03.827768 ADViewpy-0.4a0/ADViewpy.egg-info/
+-rw-rw-rw-   0        0        0     6202 2024-05-22 13:55:03.000000 ADViewpy-0.4a0/ADViewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-22 13:55:03.000000 ADViewpy-0.4a0/ADViewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:55:03.000000 ADViewpy-0.4a0/ADViewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-22 13:55:03.000000 ADViewpy-0.4a0/ADViewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 13:55:03.000000 ADViewpy-0.4a0/ADViewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6202 2024-05-22 13:55:03.828775 ADViewpy-0.4a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.4a0/README.md
+-rw-rw-rw-   0        0        0      553 2024-05-22 13:54:58.000000 ADViewpy-0.4a0/pyproject.toml
+-rw-rw-rw-   0        0        0       94 2024-05-22 13:55:03.830286 ADViewpy-0.4a0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-22 13:54:58.000000 ADViewpy-0.4a0/setup.py
```

### Comparing `ADViewpy-0.3a0/ADViewpy/ADViewpy.py` & `ADViewpy-0.4a0/ADViewpy/ADViewpy.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy/myCanvas.py` & `ADViewpy-0.4a0/ADViewpy/myCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy/myUtils.py` & `ADViewpy-0.4a0/ADViewpy/myUtils.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy/pairwiseCanvas.py` & `ADViewpy-0.4a0/ADViewpy/pairwiseCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy/rtCanvas.py` & `ADViewpy-0.4a0/ADViewpy/rtCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy/tcCanvas.py` & `ADViewpy-0.4a0/ADViewpy/tcCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy/treeDistributionView.py` & `ADViewpy-0.4a0/ADViewpy/treeDistributionView.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/ADViewpy.egg-info/PKG-INFO` & `ADViewpy-0.4a0/ADViewpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.3a0
+Version: 0.4a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.3a0/PKG-INFO` & `ADViewpy-0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.3a0
+Version: 0.4a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.3a0/README.md` & `ADViewpy-0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.3a0/pyproject.toml` & `ADViewpy-0.4a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2241 4456 6965 7770 7922 0d0a 7665  = "ADViewpy"..ve
-00000020: 7273 696f 6e20 3d20 2730 2e33 2e61 6c70  rsion = '0.3.alp
+00000020: 7273 696f 6e20 3d20 2730 2e34 2e61 6c70  rsion = '0.4.alp
 00000030: 6861 270d 0a64 6573 6372 6970 7469 6f6e  ha'..description
 00000040: 203d 2022 4144 5669 6577 7079 2069 7320   = "ADViewpy is 
 00000050: 5079 7468 6f6e 204c 6962 7261 7279 2074  Python Library t
 00000060: 6f20 7669 7375 616c 6c79 2063 6f6d 7061  o visually compa
 00000070: 7265 2070 6879 6c6f 6765 6e65 7469 6320  re phylogenetic 
 00000080: 7472 6565 7322 0d0a 7265 6164 6d65 203d  trees"..readme =
-00000090: 2022 5245 4144 4d45 2e6d 6422 0d0a 6465   "README.md"..de
-000000a0: 7065 6e64 656e 6369 6573 3d5b 0d0a 2020  pendencies=[..  
-000000b0: 2020 2020 2020 2764 656e 6472 6f70 7927        'dendropy'
-000000c0: 2c0d 0a20 2020 2020 2020 2027 6970 7963  ,..        'ipyc
-000000d0: 616e 7661 7327 2c0d 0a20 2020 2020 2020  anvas',..       
-000000e0: 2027 6970 7977 6964 6765 7473 272c 0d0a   'ipywidgets',..
-000000f0: 2020 2020 2020 2020 2773 6369 6b69 742d          'scikit-
-00000100: 6c65 6172 6e27 2c0d 0a20 2020 2020 2020  learn',..       
-00000110: 2027 6e75 6d70 7927 2c0d 0a20 2020 2020   'numpy',..     
-00000120: 2020 2027 706c 6f74 6c79 270d 0a20 2020     'plotly'..   
-00000130: 205d 0d0a 0d0a 5b70 726f 6a65 6374 2e75   ]....[project.u
-00000140: 726c 735d 0d0a 486f 6d65 7061 6765 203d  rls]..Homepage =
-00000150: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000160: 2e63 6f6d 2f43 6f72 616c 6e77 732f 4144  .com/Coralnws/AD
-00000170: 5669 6577 7079 2d61 6c70 6861 2e67 6974  Viewpy-alpha.git
-00000180: 220d 0a0d 0a5b 6275 696c 642d 7379 7374  "....[build-syst
-00000190: 656d 5d0d 0a72 6571 7569 7265 7320 3d20  em]..requires = 
-000001a0: 5b27 6465 6e64 726f 7079 272c 0d0a 2020  ['dendropy',..  
-000001b0: 2020 2020 2020 2769 7079 6361 6e76 6173        'ipycanvas
-000001c0: 272c 0d0a 2020 2020 2020 2020 2769 7079  ',..        'ipy
-000001d0: 7769 6467 6574 7327 2c0d 0a20 2020 2020  widgets',..     
-000001e0: 2020 2027 7363 696b 6974 2d6c 6561 726e     'scikit-learn
-000001f0: 272c 0d0a 2020 2020 2020 2020 276e 756d  ',..        'num
-00000200: 7079 272c 0d0a 2020 2020 2020 2020 2770  py',..        'p
-00000210: 6c6f 746c 7927 5d0d 0a0d 0a              lotly']....
+00000090: 2022 5245 4144 4d45 2e6d 6422 0d0a 2364   "README.md"..#d
+000000a0: 6570 656e 6465 6e63 6965 733d 5b0d 0a23  ependencies=[..#
+000000b0: 2020 2020 2020 2020 2764 656e 6472 6f70          'dendrop
+000000c0: 7927 2c0d 0a23 2020 2020 2020 2020 2769  y',..#        'i
+000000d0: 7079 6361 6e76 6173 272c 0d0a 2320 2020  pycanvas',..#   
+000000e0: 2020 2020 2027 6970 7977 6964 6765 7473       'ipywidgets
+000000f0: 272c 0d0a 2320 2020 2020 2020 2027 7363  ',..#        'sc
+00000100: 696b 6974 2d6c 6561 726e 272c 0d0a 2320  ikit-learn',..# 
+00000110: 2020 2020 2020 2027 6e75 6d70 7927 2c0d         'numpy',.
+00000120: 0a23 2020 2020 2020 2020 2770 6c6f 746c  .#        'plotl
+00000130: 7927 0d0a 2320 2020 205d 0d0a 0d0a 5b70  y'..#    ]....[p
+00000140: 726f 6a65 6374 2e75 726c 735d 0d0a 486f  roject.urls]..Ho
+00000150: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
+00000160: 2f2f 6769 7468 7562 2e63 6f6d 2f43 6f72  //github.com/Cor
+00000170: 616c 6e77 732f 4144 5669 6577 7079 2d61  alnws/ADViewpy-a
+00000180: 6c70 6861 2e67 6974 220d 0a0d 0a5b 6275  lpha.git"....[bu
+00000190: 696c 642d 7379 7374 656d 5d0d 0a23 7265  ild-system]..#re
+000001a0: 7175 6972 6573 203d 205b 2764 656e 6472  quires = ['dendr
+000001b0: 6f70 7927 2c0d 0a23 2020 2020 2020 2020  opy',..#        
+000001c0: 2769 7079 6361 6e76 6173 272c 0d0a 2320  'ipycanvas',..# 
+000001d0: 2020 2020 2020 2027 6970 7977 6964 6765         'ipywidge
+000001e0: 7473 272c 0d0a 2320 2020 2020 2020 2027  ts',..#        '
+000001f0: 7363 696b 6974 2d6c 6561 726e 272c 0d0a  scikit-learn',..
+00000200: 2320 2020 2020 2020 2027 6e75 6d70 7927  #        'numpy'
+00000210: 2c0d 0a23 2020 2020 2020 2020 2770 6c6f  ,..#        'plo
+00000220: 746c 7927 5d0d 0a0d 0a                   tly']....
```

### Comparing `ADViewpy-0.3a0/setup.py` & `ADViewpy-0.4a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.3.alpha'
+VERSION = '0.4.alpha'
 DESCRIPTION = ('ADViewpy is Python Library to visually compare phylogenetic trees')
 LONG_DESCRIPTION = 'ADViewpy is Python Library to visually compare phylogenetic trees, utilizing Aggregated Dendrogram for phylogenetic tree visualization. '
 
 
 setup(
     name="ADViewpy",
     version=VERSION,
```

