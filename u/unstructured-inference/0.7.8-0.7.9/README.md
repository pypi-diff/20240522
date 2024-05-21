# Comparing `tmp/unstructured_inference-0.7.8.tar.gz` & `tmp/unstructured_inference-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.7.8.tar", last modified: Tue Oct 17 17:49:41 2023, max compression
+gzip compressed data, was "unstructured_inference-0.7.9.tar", last modified: Tue Oct 17 17:52:05 2023, max compression
```

## Comparing `unstructured_inference-0.7.8.tar` & `unstructured_inference-0.7.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.248963 unstructured_inference-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-17 17:47:09.000000 unstructured_inference-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-17 17:49:41.248963 unstructured_inference-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-10-17 17:47:09.000000 unstructured_inference-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.232963 unstructured_inference-0.7.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-17 17:47:09.000000 unstructured_inference-0.7.8/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-17 17:47:09.000000 unstructured_inference-0.7.8/requirements/sg.in
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-17 17:49:41.248963 unstructured_inference-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.236963 unstructured_inference-0.7.8/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.240963 unstructured_inference-0.7.8/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    22421 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/inference/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.248963 unstructured_inference-0.7.8/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23326 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/chipper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/super_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)    24262 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    28922 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.248963 unstructured_inference-0.7.8/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2023-10-17 17:47:10.000000 unstructured_inference-0.7.8/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.236963 unstructured_inference-0.7.8/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-17 17:49:40.000000 unstructured_inference-0.7.8/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-17 17:49:41.000000 unstructured_inference-0.7.8/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 17:49:40.000000 unstructured_inference-0.7.8/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-17 17:49:40.000000 unstructured_inference-0.7.8/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-17 17:49:40.000000 unstructured_inference-0.7.8/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.583878 unstructured_inference-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-17 17:49:40.000000 unstructured_inference-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-17 17:52:05.583878 unstructured_inference-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-10-17 17:49:40.000000 unstructured_inference-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.559876 unstructured_inference-0.7.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-17 17:49:40.000000 unstructured_inference-0.7.9/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-17 17:49:40.000000 unstructured_inference-0.7.9/requirements/sg.in
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-17 17:52:05.583878 unstructured_inference-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.563876 unstructured_inference-0.7.9/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.571877 unstructured_inference-0.7.9/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22421 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/inference/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.579877 unstructured_inference-0.7.9/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23326 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/chipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/super_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24262 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29904 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.579877 unstructured_inference-0.7.9/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2023-10-17 17:49:41.000000 unstructured_inference-0.7.9/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:52:05.567877 unstructured_inference-0.7.9/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-17 17:52:05.000000 unstructured_inference-0.7.9/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-17 17:52:05.000000 unstructured_inference-0.7.9/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 17:52:05.000000 unstructured_inference-0.7.9/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-17 17:52:05.000000 unstructured_inference-0.7.9/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-17 17:52:05.000000 unstructured_inference-0.7.9/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.7.8/PKG-INFO` & `unstructured_inference-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.7.8
+Version: 0.7.9
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.7.8/README.md` & `unstructured_inference-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/setup.py` & `unstructured_inference-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/config.py` & `unstructured_inference-0.7.9/unstructured_inference/config.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/constants.py` & `unstructured_inference-0.7.9/unstructured_inference/constants.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/inference/elements.py` & `unstructured_inference-0.7.9/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/inference/layout.py` & `unstructured_inference-0.7.9/unstructured_inference/inference/layout.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.7.9/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.7.9/unstructured_inference/inference/ordering.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/inference/pdf.py` & `unstructured_inference-0.7.9/unstructured_inference/inference/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/logger.py` & `unstructured_inference-0.7.9/unstructured_inference/logger.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/math.py` & `unstructured_inference-0.7.9/unstructured_inference/math.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/base.py` & `unstructured_inference-0.7.9/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/chipper.py` & `unstructured_inference-0.7.9/unstructured_inference/models/chipper.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.7.9/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.7.9/unstructured_inference/models/detectron2onnx.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/donut.py` & `unstructured_inference-0.7.9/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/eval.py` & `unstructured_inference-0.7.9/unstructured_inference/models/eval.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/paddle_ocr.py` & `unstructured_inference-0.7.9/unstructured_inference/models/paddle_ocr.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/super_gradients.py` & `unstructured_inference-0.7.9/unstructured_inference/models/super_gradients.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.7.9/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/tables.py` & `unstructured_inference-0.7.9/unstructured_inference/models/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # https://github.com/microsoft/table-transformer/blob/main/src/inference.py
 # https://github.com/NielsRogge/Transformers-Tutorials/blob/master/Table%20Transformer/Using_Table_Transformer_for_table_detection_and_table_structure_recognition.ipynb
 import logging
 import os
 import xml.etree.ElementTree as ET
 from collections import defaultdict
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import cv2
 import numpy as np
 import pandas as pd
 import pytesseract
 import torch
 from PIL import Image
@@ -29,18 +29,32 @@
 
 class UnstructuredTableTransformerModel(UnstructuredModel):
     """Unstructured model wrapper for table-transformer."""
 
     def __init__(self):
         pass
 
-    def predict(self, x: Image):
-        """Predict table structure deferring to run_prediction"""
+    def predict(self, x: Image, ocr_tokens: Optional[List[Dict]] = None):
+        """Predict table structure deferring to run_prediction with ocr tokens
+
+        Note:
+        `ocr_tokens` is a list of dictionaries representing OCR tokens,
+        where each dictionary has the following format:
+        {
+            "bbox": [int, int, int, int],  # Bounding box coordinates of the token
+            "block_num": int,  # Block number
+            "line_num": int,   # Line number
+            "span_num": int,   # Span number
+            "text": str,  # Text content of the token
+        }
+        The bounding box coordinates should match the table structure.
+        FIXME: refactor token data into a dataclass so we have clear expectations of the fields
+        """
         super().predict(x)
-        return self.run_prediction(x)
+        return self.run_prediction(x, ocr_tokens=ocr_tokens)
 
     def initialize(
         self,
         model: Union[str, Path, TableTransformerForObjectDetection] = None,
         device: Optional[str] = "cuda" if torch.cuda.is_available() else "cpu",
     ):
         """Loads the donut model using the specified parameters"""
@@ -157,20 +171,26 @@
             outputs_structure["pad_for_structure_detection"] = pad_for_structure_detection
             return outputs_structure
 
     def run_prediction(
         self,
         x: Image,
         pad_for_structure_detection: int = inference_config.TABLE_IMAGE_BACKGROUND_PAD,
+        ocr_tokens: Optional[List[Dict]] = None,
     ):
         """Predict table structure"""
         outputs_structure = self.get_structure(x, pad_for_structure_detection)
-        tokens = self.get_tokens(x=x)
+        if ocr_tokens is None:
+            logger.warning(
+                "Table OCR from get_tokens method will be deprecated. "
+                "In the future the OCR tokens are expected to be passed in.",
+            )
+            ocr_tokens = self.get_tokens(x=x)
 
-        html = recognize(outputs_structure, x, tokens=tokens, out_html=True)["html"]
+        html = recognize(outputs_structure, x, tokens=ocr_tokens, out_html=True)["html"]
         prediction = html[0] if html else ""
         return prediction
 
 
 tables_agent: UnstructuredTableTransformerModel = UnstructuredTableTransformerModel()
```

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.7.9/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/models/yolox.py` & `unstructured_inference-0.7.9/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.7.9/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/utils.py` & `unstructured_inference-0.7.9/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference/visualize.py` & `unstructured_inference-0.7.9/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.7.8/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.7.9/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.7.8
+Version: 0.7.9
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.7.8/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.7.9/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

