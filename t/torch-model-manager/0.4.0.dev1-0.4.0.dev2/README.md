# Comparing `tmp/torch_model_manager-0.4.0.dev1.tar.gz` & `tmp/torch_model_manager-0.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev1.tar", last modified: Wed May 22 10:46:26 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev2.tar", last modified: Wed May 22 10:59:27 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev1.tar` & `torch_model_manager-0.4.0.dev2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.726062 torch_model_manager-0.4.0.dev1/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9032 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 10:46:26.726062 torch_model_manager-0.4.0.dev1/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2082 2024-05-22 10:46:24.000000 torch_model_manager-0.4.0.dev1/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.718062 torch_model_manager-0.4.0.dev1/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.718062 torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.718062 torch_model_manager-0.4.0.dev1/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12708 2024-05-22 10:44:37.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9032 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      168 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     8619 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev1/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.939204 torch_model_manager-0.4.0.dev2/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 10:59:27.939204 torch_model_manager-0.4.0.dev2/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev2/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 10:59:27.939204 torch_model_manager-0.4.0.dev2/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2121 2024-05-22 10:59:26.000000 torch_model_manager-0.4.0.dev2/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.935204 torch_model_manager-0.4.0.dev2/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.935204 torch_model_manager-0.4.0.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.935204 torch_model_manager-0.4.0.dev2/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.939204 torch_model_manager-0.4.0.dev2/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev2/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev2/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12970 2024-05-22 10:55:39.000000 torch_model_manager-0.4.0.dev2/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev2/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev2/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.939204 torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9079 2024-05-22 10:59:27.000000 torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 10:59:27.000000 torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 10:59:27.000000 torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      185 2024-05-22 10:59:27.000000 torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 10:59:27.000000 torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:59:27.939204 torch_model_manager-0.4.0.dev2/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev2/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev2/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev1/PKG-INFO` & `torch_model_manager-0.4.0.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev1
+Version: 0.4.0.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,16 @@
 Requires-Dist: wandb
 Requires-Dist: ydata_profiling
 Requires-Dist: diffusers
 Requires-Dist: transformers
 Requires-Dist: accelerate
 Requires-Dist: scipy
 Requires-Dist: safetensors
+Requires-Dist: supervision
+Requires-Dist: tqdm
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.4.0.dev1/README.md` & `torch_model_manager-0.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/setup.py` & `torch_model_manager-0.4.0.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev1',
+    version='0.4.0.dev2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh', 
@@ -48,15 +48,17 @@
         'graphviz',
         'wandb',
         'ydata_profiling',
         'diffusers',
         'transformers',
         'accelerate',
         'scipy',
-        'safetensors'
+        'safetensors',
+        'supervision',
+        'tqdm'
         # Add any other dependencies here
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
```

### Comparing `torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev2/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev2/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.0.dev2/torch_model_manager/segmentation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import os
 import cv2
 import numpy as np
 import torch
 import torchvision
 import supervision as sv
 
-from groundingdino.util.inference import Model
+import sys
+import os
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+from GroundingDINO.groundingdino.util.inference import Model
+from utils import helpers
 from segment_anything import sam_model_registry, SamPredictor
 from scipy.stats import hmean
 import pandas as pd
 from tqdm import tqdm
 
 DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
@@ -21,15 +25,17 @@
         # Paths for checkpoints and configs
         g_dino_model_config_path = "GroundingDINO/groundingdino/config"
         g_dino_checkpoint_path = "weights/GroundingDINO"
         sam_checkpoint_path = "weights/SAM"
         sam_type = None
 
 
-
+        helpers.create_hierarchy(g_dino_checkpoint_path)
+        helpers.create_hierarchy(sam_checkpoint_path)
+        
         if sam_backbone == "sam_vit_h":
             sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_h_4b8939.pth")
             sam_type = "vit_h"
             if not os.path.exists(sam_checkpoint_path):
                 os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth")
                 os.system(f"mv sam_vit_h_4b8939.pth {sam_checkpoint_path}")
                 
@@ -65,14 +71,16 @@
         sam = sam_model_registry[sam_type](checkpoint=sam_checkpoint_path)
         sam.to(device=self.device)
         self.sam_predictor = SamPredictor(sam)
 
     def load_image(self, image_path):
         return cv2.imread(image_path)
 
+
+
     def detect_objects(self, image, classes, box_threshold=0.25, text_threshold=0.25):
         detections = self.grounding_dino_model.predict_with_classes(
             image=image,
             classes=classes,
             box_threshold=box_threshold,
             text_threshold=text_threshold
         )
```

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev2/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev1
+Version: 0.4.0.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,16 @@
 Requires-Dist: wandb
 Requires-Dist: ydata_profiling
 Requires-Dist: diffusers
 Requires-Dist: transformers
 Requires-Dist: accelerate
 Requires-Dist: scipy
 Requires-Dist: safetensors
+Requires-Dist: supervision
+Requires-Dist: tqdm
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev2/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev1/utils/helpers.py` & `torch_model_manager-0.4.0.dev2/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Any
 import matplotlib.pyplot as plt
 import torch
 from torchvision import transforms
 import json
 import pickle
+import os
 
 def required_kernel(in_size: int, out_size:int, stride=1, padding=1):
     assert in_size > 0, "Input size must be greater than 0"
     assert out_size > 0, "Output size must be greater than 0"
     assert in_size >= out_size, "Input size must be greater than or equal to output size"
     assert stride > 0, "Stride must be greater than 0"
     assert padding >= 0, "Padding must be greater than or equal to 0"
@@ -270,7 +271,24 @@
     assert isinstance(file_path, str), "file_path must be a string"
     try:
         with open(file_path, 'wb') as file:
             pickle.dump(data, file)
 
     except (IOError, FileNotFoundError, PermissionError) as e:
         print(f"Error during dump_data: {e}")
+
+def create_hierarchy(path):
+    """
+    Create a hierarchy of directories from a given path.
+
+    Args:
+        path (str): The path to create the hierarchy of directories.
+
+    Returns:
+        None
+    """
+    try:
+        os.makedirs(path)
+    except FileExistsError:
+        print(f"Directory {path} already exists.")
+    except Exception as e:
+        print(f"Error during create_hierarchy: {e}")
```

