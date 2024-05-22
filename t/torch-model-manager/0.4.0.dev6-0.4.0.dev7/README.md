# Comparing `tmp/torch_model_manager-0.4.0.dev6.tar.gz` & `tmp/torch_model_manager-0.4.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev6.tar", last modified: Wed May 22 12:43:46 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev7.tar", last modified: Wed May 22 13:20:16 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev6.tar` & `torch_model_manager-0.4.0.dev7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-22 12:43:44.000000 torch_model_manager-0.4.0.dev6/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.642125 torch_model_manager-0.4.0.dev6/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12997 2024-05-22 12:43:34.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev6/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 12:43:46.000000 torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 12:43:46.646125 torch_model_manager-0.4.0.dev6/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev6/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev6/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev7/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-22 13:20:14.000000 torch_model_manager-0.4.0.dev7/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.556835 torch_model_manager-0.4.0.dev7/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev7/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev7/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev7/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev7/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev7/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev7/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    13915 2024-05-22 13:19:56.000000 torch_model_manager-0.4.0.dev7/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev7/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev7/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 13:20:16.000000 torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 13:20:16.000000 torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 13:20:16.000000 torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-22 13:20:16.000000 torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 13:20:16.000000 torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:20:16.560835 torch_model_manager-0.4.0.dev7/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev7/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev7/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev6/PKG-INFO` & `torch_model_manager-0.4.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev6
+Version: 0.4.0.dev7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev6/README.md` & `torch_model_manager-0.4.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/setup.py` & `torch_model_manager-0.4.0.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev6',
+    version='0.4.0.dev7',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev7/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev7/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev7/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.0.dev7/torch_model_manager/segmentation_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -274,18 +274,32 @@
 
         Parameters:
         - matrix (np.ndarray): Annotation matrix with shape (num_images, num_classes).
 
         Returns:
         - np.ndarray: Occurrence probability disjoint matrix with shape (num_classes, num_classes).
         """
+        dataset_path = kwargs.get("dataset_path", None)
+        classes = kwargs.get("classes", None)
+        box_threshold = kwargs.get("box_threshold", 0.25)
+        text_threshold = kwargs.get("text_threshold", 0.25)
+        nms_threshold = kwargs.get("nms_threshold", 0.8)
+        agg = kwargs.get("agg", hmean)
+        annotation_matrix_processing = kwargs.get("annotation_matrix_processing", None)
         if apply_on_annotation_matrix:
             assert matrix is None, "Annotation matrix should not be provided."
-            matrix = self.create_annotation_matrix(**kwargs)
-
+            matrix = self.create_annotation_matrix(dataset_path=dataset_path, 
+                                                   classes=classes, 
+                                                   box_threshold=box_threshold, 
+                                                   text_threshold=text_threshold,
+                                                   nms_threshold=nms_threshold, 
+                                                   agg=agg)
+        if annotation_matrix_processing is not None:
+            matrix = annotation_matrix_processing(matrix)
+            
         classes = matrix.columns
         num_rows, num_cols = matrix.shape
 
         tensor = np.zeros(shape=(num_cols, num_rows, num_rows))
         for i, c in enumerate(classes):
             column = matrix.loc[:, c].values
             column = np.array([float(val) for val in column]).reshape(len(column), 1)
```

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev7/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev7/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev6
+Version: 0.4.0.dev7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev6/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev7/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev6/utils/helpers.py` & `torch_model_manager-0.4.0.dev7/utils/helpers.py`

 * *Files identical despite different names*

