# Comparing `tmp/dataset_iterator-0.4.4.tar.gz` & `tmp/dataset_iterator-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.4.4.tar", last modified: Thu May 16 15:35:04 2024, max compression
+gzip compressed data, was "dataset_iterator-0.4.5.tar", last modified: Wed May 22 20:42:17 2024, max compression
```

## Comparing `dataset_iterator-0.4.4.tar` & `dataset_iterator-0.4.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/dataset_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/concat_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/dataset_iterator/datasetIO/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/group_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/h5pyIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/memoryIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/hard_sample_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22252 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/image_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/index_array_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57901 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/multichannel_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/ordered_enqueuer_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/tile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/tracking_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/dataset_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.423889 dataset_iterator-0.4.5/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.423889 dataset_iterator-0.4.5/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22252 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/keras_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57911 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/ordered_enqueuer_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/setup.py
```

### Comparing `dataset_iterator-0.4.4/LICENSE.txt` & `dataset_iterator-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/PKG-INFO` & `dataset_iterator-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.4
+Version: 0.4.5
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.4/dataset_iterator-0.4.4.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.5/dataset_iterator-0.4.5.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.4/README.md` & `dataset_iterator-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/__init__.py` & `dataset_iterator-0.4.5/dataset_iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.4.5/dataset_iterator/concat_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/memoryIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/memoryIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/hard_sample_mining.py` & `dataset_iterator-0.4.5/dataset_iterator/hard_sample_mining.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/helpers.py` & `dataset_iterator-0.4.5/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.4.5/dataset_iterator/image_data_generator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.4.5/dataset_iterator/index_array_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.4.5/dataset_iterator/multichannel_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import warnings
 import numpy as np
 from random import uniform
 from dataset_iterator import IndexArrayIterator
 from .utils import remove_duplicates, pick_from_array
 from sklearn.model_selection import train_test_split
 import time
```

### Comparing `dataset_iterator-0.4.4/dataset_iterator/ordered_enqueuer_cf.py` & `dataset_iterator-0.4.5/dataset_iterator/ordered_enqueuer_cf.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/pre_processing.py` & `dataset_iterator-0.4.5/dataset_iterator/pre_processing.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/shared_memory.py` & `dataset_iterator-0.4.5/dataset_iterator/shared_memory.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/tile_utils.py` & `dataset_iterator-0.4.5/dataset_iterator/tile_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.4.5/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator/utils.py` & `dataset_iterator-0.4.5/dataset_iterator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.4/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.4.5/dataset_iterator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.4
+Version: 0.4.5
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.4/dataset_iterator-0.4.4.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.5/dataset_iterator-0.4.5.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.4/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.4.5/dataset_iterator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 dataset_iterator/__init__.py
 dataset_iterator/concat_iterator.py
 dataset_iterator/hard_sample_mining.py
 dataset_iterator/helpers.py
 dataset_iterator/image_data_generator.py
 dataset_iterator/index_array_iterator.py
+dataset_iterator/keras_callbacks.py
 dataset_iterator/multichannel_iterator.py
 dataset_iterator/ordered_enqueuer_cf.py
 dataset_iterator/pre_processing.py
 dataset_iterator/shared_memory.py
 dataset_iterator/tile_utils.py
 dataset_iterator/tracking_iterator.py
 dataset_iterator/utils.py
```

### Comparing `dataset_iterator-0.4.4/setup.py` & `dataset_iterator-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.4.4",
+    version="0.4.5",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.4/dataset_iterator-0.4.4.tar.gz',
+    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.5/dataset_iterator-0.4.5.tar.gz',
     keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

