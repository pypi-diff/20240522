# Comparing `tmp/torch_model_manager-0.4.0.dev4.tar.gz` & `tmp/torch_model_manager-0.4.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev4.tar", last modified: Wed May 22 11:35:18 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev5.tar", last modified: Wed May 22 12:31:09 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev4.tar` & `torch_model_manager-0.4.0.dev5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2121 2024-05-22 11:35:16.000000 torch_model_manager-0.4.0.dev4/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.330740 torch_model_manager-0.4.0.dev4/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12948 2024-05-22 11:06:57.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      185 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev4/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-22 12:31:07.000000 torch_model_manager-0.4.0.dev5/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12948 2024-05-22 11:06:57.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev5/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev4/PKG-INFO` & `torch_model_manager-0.4.0.dev5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev4
+Version: 0.4.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,19 @@
 Requires-Dist: diffusers
 Requires-Dist: transformers
 Requires-Dist: accelerate
 Requires-Dist: scipy
 Requires-Dist: safetensors
 Requires-Dist: supervision
 Requires-Dist: tqdm
+Requires-Dist: pycocotools
+Requires-Dist: opencv-python
+Requires-Dist: addict
+Requires-Dist: yapf
+Requires-Dist: timm
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.4.0.dev4/README.md` & `torch_model_manager-0.4.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/setup.py` & `torch_model_manager-0.4.0.dev5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev4',
+    version='0.4.0.dev5',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh', 
@@ -50,15 +50,20 @@
         'ydata_profiling',
         'diffusers',
         'transformers',
         'accelerate',
         'scipy',
         'safetensors',
         'supervision',
-        'tqdm'
+        'tqdm',
+        'pycocotools',
+        'opencv-python',
+        'addict',
+        'yapf',
+        'timm'
         # Add any other dependencies here
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
```

### Comparing `torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev5/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev5/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev5/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.0.dev5/torch_model_manager/segmentation_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev5/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev5/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev4
+Version: 0.4.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,19 @@
 Requires-Dist: diffusers
 Requires-Dist: transformers
 Requires-Dist: accelerate
 Requires-Dist: scipy
 Requires-Dist: safetensors
 Requires-Dist: supervision
 Requires-Dist: tqdm
+Requires-Dist: pycocotools
+Requires-Dist: opencv-python
+Requires-Dist: addict
+Requires-Dist: yapf
+Requires-Dist: timm
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev4/utils/helpers.py` & `torch_model_manager-0.4.0.dev5/utils/helpers.py`

 * *Files identical despite different names*

