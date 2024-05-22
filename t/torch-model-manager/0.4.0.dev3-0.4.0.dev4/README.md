# Comparing `tmp/torch_model_manager-0.4.0.dev3.tar.gz` & `tmp/torch_model_manager-0.4.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev3.tar", last modified: Wed May 22 11:03:46 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev4.tar", last modified: Wed May 22 11:35:18 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev3.tar` & `torch_model_manager-0.4.0.dev4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.597359 torch_model_manager-0.4.0.dev3/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 11:03:46.597359 torch_model_manager-0.4.0.dev3/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev3/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 11:03:46.597359 torch_model_manager-0.4.0.dev3/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2121 2024-05-22 11:03:44.000000 torch_model_manager-0.4.0.dev3/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.593359 torch_model_manager-0.4.0.dev3/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.593359 torch_model_manager-0.4.0.dev3/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.593359 torch_model_manager-0.4.0.dev3/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev3/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.593359 torch_model_manager-0.4.0.dev3/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev3/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev3/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev3/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12970 2024-05-22 10:55:39.000000 torch_model_manager-0.4.0.dev3/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev3/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev3/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.597359 torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 11:03:46.000000 torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 11:03:46.000000 torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 11:03:46.000000 torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      185 2024-05-22 11:03:46.000000 torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 11:03:46.000000 torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:03:46.597359 torch_model_manager-0.4.0.dev3/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev3/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev3/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2121 2024-05-22 11:35:16.000000 torch_model_manager-0.4.0.dev4/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.330740 torch_model_manager-0.4.0.dev4/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12948 2024-05-22 11:06:57.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev4/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      185 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 11:35:18.000000 torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 11:35:18.334740 torch_model_manager-0.4.0.dev4/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev4/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev4/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev3/PKG-INFO` & `torch_model_manager-0.4.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev3
+Version: 0.4.0.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev3/README.md` & `torch_model_manager-0.4.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/setup.py` & `torch_model_manager-0.4.0.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev3',
+    version='0.4.0.dev4',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev4/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev4/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev4/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.0.dev4/torch_model_manager/segmentation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch
 import torchvision
 import supervision as sv
 
 import sys
 import os
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-from GroundingDINO.groundingdino.util.inference import Model
+from groundingdino.util.inference import Model
 from utils import helpers
 from segment_anything import sam_model_registry, SamPredictor
 from scipy.stats import hmean
 import pandas as pd
 from tqdm import tqdm
 
 DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
@@ -27,15 +27,15 @@
         g_dino_checkpoint_path = "weights/GroundingDINO"
         sam_checkpoint_path = "weights/SAM"
         sam_type = None
 
 
         helpers.create_hierarchy(g_dino_checkpoint_path)
         helpers.create_hierarchy(sam_checkpoint_path)
-        
+
         if sam_backbone == "sam_vit_h":
             sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_h_4b8939.pth")
             sam_type = "vit_h"
             if not os.path.exists(sam_checkpoint_path):
                 os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth")
                 os.system(f"mv sam_vit_h_4b8939.pth {sam_checkpoint_path}")
```

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev4/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev4/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev3
+Version: 0.4.0.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev3/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev4/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev3/utils/helpers.py` & `torch_model_manager-0.4.0.dev4/utils/helpers.py`

 * *Files identical despite different names*

