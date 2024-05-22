# Comparing `tmp/torch_model_manager-0.4.0.dev5.tar.gz` & `tmp/torch_model_manager-0.4.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev5.tar", last modified: Wed May 22 12:31:09 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev6.tar", last modified: Wed May 22 12:43:46 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev5.tar` & `torch_model_manager-0.4.0.dev6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-22 12:31:07.000000 torch_model_manager-0.4.0.dev5/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12948 2024-05-22 11:06:57.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev5/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.219915 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 12:31:09.000000 torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:31:09.215915 torch_model_manager-0.4.0.dev5/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev5/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev5/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-22 12:43:44.000000 torch_model_manager-0.4.0.dev6/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.642125 torch_model_manager-0.4.0.dev6/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12997 2024-05-22 12:43:34.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev6/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev5/PKG-INFO` & `torch_model_manager-0.4.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev5
+Version: 0.4.0.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev5/README.md` & `torch_model_manager-0.4.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/setup.py` & `torch_model_manager-0.4.0.dev6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev5',
+    version='0.4.0.dev6',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev6/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev6/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev6/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.0.dev6/torch_model_manager/segmentation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,30 +296,31 @@
             tensor[i] = mat
 
         return tensor, matrix.index, classes
     
     
     def save_image(self, image, path):
         cv2.imwrite(path, image)
-# Example usage
-if __name__ == "__main__":
-    SOURCE_IMAGE_PATH = "G0041951.JPG"
-    CLASSES = ["person", "banner", "finger", "hand", "foot", "glasses", "desert", "sky", "clouds"]
-    BOX_THRESHOLD = 0.3
-    TEXT_THRESHOLD = 0.25
-    NMS_THRESHOLD = 0.3
+        
+# # Example usage
+# if __name__ == "__main__":
+#     SOURCE_IMAGE_PATH = "G0041951.JPG"
+#     CLASSES = ["person", "banner", "finger", "hand", "foot", "glasses", "desert", "sky", "clouds"]
+#     BOX_THRESHOLD = 0.3
+#     TEXT_THRESHOLD = 0.25
+#     NMS_THRESHOLD = 0.3
 
-    manager = SegmentationManager()
+#     manager = SegmentationManager()
 
-    # Apply the grounding SAM pipeline
-    # detections = manager.grounding_sam(SOURCE_IMAGE_PATH, CLASSES, BOX_THRESHOLD, TEXT_THRESHOLD, NMS_THRESHOLD, "grounded_sam_annotated_image.jpg")
+#     # Apply the grounding SAM pipeline
+#     # detections = manager.grounding_sam(SOURCE_IMAGE_PATH, CLASSES, BOX_THRESHOLD, TEXT_THRESHOLD, NMS_THRESHOLD, "grounded_sam_annotated_image.jpg")
 
-    # Create an annotation matrix for a dataset
-    dataset_path = "test_dataset"
-    annotation_matrix = manager.occ_proba_disjoint_tensor(matrix = None, 
-                                                          apply_on_annotation_matrix=True, 
-                                                          dataset_path=dataset_path, 
-                                                          classes=CLASSES, 
-                                                          box_threshold=BOX_THRESHOLD, 
-                                                          text_threshold=TEXT_THRESHOLD, 
-                                                          nms_threshold=NMS_THRESHOLD)
-    print(annotation_matrix)
+#     # Create an annotation matrix for a dataset
+#     dataset_path = "test_dataset"
+#     annotation_matrix = manager.occ_proba_disjoint_tensor(matrix = None, 
+#                                                           apply_on_annotation_matrix=True, 
+#                                                           dataset_path=dataset_path, 
+#                                                           classes=CLASSES, 
+#                                                           box_threshold=BOX_THRESHOLD, 
+#                                                           text_threshold=TEXT_THRESHOLD, 
+#                                                           nms_threshold=NMS_THRESHOLD)
+#     print(annotation_matrix)
```

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev6/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev6/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev5
+Version: 0.4.0.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev5/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev5/utils/helpers.py` & `torch_model_manager-0.4.0.dev6/utils/helpers.py`

 * *Files identical despite different names*

