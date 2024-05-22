# Comparing `tmp/opensr-utils-0.4.8.tar.gz` & `tmp/opensr-utils-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr-utils-0.4.8.tar", last modified: Thu Feb 15 12:20:57 2024, max compression
+gzip compressed data, was "opensr-utils-0.4.9.tar", last modified: Thu Feb 15 15:02:45 2024, max compression
```

## Comparing `opensr-utils-0.4.8.tar` & `opensr-utils-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:20:57.411897 opensr-utils-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-15 12:20:57.411897 opensr-utils-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:20:57.407897 opensr-utils-0.4.8/opensr_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/bands10m_stacked_from_S2_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/bands20m_stacked_from_S2_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/denormalize_image_per_band_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    25178 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/pl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/stretching.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/weighted_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/opensr_utils/xAI_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:20:57.411897 opensr-utils-0.4.8/opensr_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-15 12:20:57.000000 opensr-utils-0.4.8/opensr_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-15 12:20:57.000000 opensr-utils-0.4.8/opensr_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 12:20:57.000000 opensr-utils-0.4.8/opensr_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-15 12:20:57.000000 opensr-utils-0.4.8/opensr_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-15 12:20:57.000000 opensr-utils-0.4.8/opensr_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 12:20:57.411897 opensr-utils-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-15 12:20:47.000000 opensr-utils-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:02:45.317717 opensr-utils-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-02-15 15:02:45.317717 opensr-utils-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:02:45.313717 opensr-utils-0.4.9/opensr_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/bands10m_stacked_from_S2_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/bands20m_stacked_from_S2_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/denormalize_image_per_band_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25178 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/pl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/stretching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/weighted_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/opensr_utils/xAI_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:02:45.313717 opensr-utils-0.4.9/opensr_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-02-15 15:02:45.000000 opensr-utils-0.4.9/opensr_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-15 15:02:45.000000 opensr-utils-0.4.9/opensr_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 15:02:45.000000 opensr-utils-0.4.9/opensr_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-15 15:02:45.000000 opensr-utils-0.4.9/opensr_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-15 15:02:45.000000 opensr-utils-0.4.9/opensr_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 15:02:45.317717 opensr-utils-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-15 15:02:36.000000 opensr-utils-0.4.9/setup.py
```

### Comparing `opensr-utils-0.4.8/LICENSE.md` & `opensr-utils-0.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/PKG-INFO` & `opensr-utils-0.4.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,60 @@
-Metadata-Version: 2.1
-Name: opensr-utils
-Version: 0.4.8
-Summary: Utilities supporting the ESA opensr-model package for Super-Resolution of Senintel-2 Imagery
-Home-page: https://isp.uv.es/opensr/
-Author: Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis
-Author-email: accounts@donike.net
-License: MIT
-Project-URL: Source Code, https://github.com/ESAopenSR/opensr-utils
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy==1.23.5
-Requires-Dist: einops==0.6.0
-Requires-Dist: rasterio==1.3.6
-Requires-Dist: tqdm==4.64.1
-Requires-Dist: torch==1.13.1
-Requires-Dist: scikit-image==0.19.3
-
 # opensr-utils - Supplementary Code for the ESA OpenSR project
 
 *WARNING*  
 The 'eliminate_pixel' functionality is currently experimental and can in some cases return unexpected results.  
 Only the combination of overlap:40 and eliminate_pixel:20 is proven to work. Set to 0 to disable.  
   
   
-
-
 *UPDATE*  
 The current version supports PyTorch Lightning multi-GPU inference, but the documentation hasnt updated yet.
   
   
+
+*Description*  
+This package performs super-resolution with any PyTorch or PyTorch lighning model for Sentinel-2 10m and 20m bands.  
 This package provides useful functions to perform super-resolution of raw Sentinel-2 tiles.  
 Funcitonalities:
-- Reading and stacking of the 10 and 20m bands of Sentinel-2 '.SAFE' file format (worrks with Sen2 downloads straight out of the box)
-- Patching of input images by selectable size (eg 128x128)
-- Super-Resolution of individual patches
-- writing of georeferenced output raster
-- overlapping and averaging of patches by selectable quantity to reduce patching artifacts
-- Processing is performed on the same device as the model that is passed to the funciton
+- The Input can be either:  
+	- a ".SAFE" folder, the format straight from the Copenricus Hub download.  Then, stacking of the 10 and 20m bands of Sentinel-2 '.SAFE' file format is performed (works with Sen2 downloads straight out of the box)
+	- any ".tif" file or similar that can be laoded by rasterio. Either 4- or 6-band for the different models.
+- The following is performed automatically:  
+	- Patching of input images by selectable size (eg 128x128)
+	- Super-Resolution of individual patches with provided model
+	- writing of georeferenced output raster
+	- overlapping and linear weightning of patches by selectable quantity to reduce patching artifacts
+	- Processing is performed on the same device as the model that is passed to the funciton
+- Supported Models:  
+	- 'torch.nn.Module': Any SR model with a .forward() function can be passed. The drawback is that for this model type, multi-GPU and multi-batch processing is not supported. This is therefore considerably slower.
+	- 'LightningModule': Any PL Lightning model with a .predict() function. If this model type is passed, multi-GPU and multi-batch processing is activated, which lkeads to a significant inference speed increase.
 
 Usage example:
 ```python
 !pip install opensr-utils
 import opensr_utils
 from opensr_utils.main import windowed_SR_and_saving 
 
+# Create SR Object
 file_path = "/yourfilepath/S2A_MSIL2A_20230729T100031_N0509_R122_T33TUG_20230729T134559.SAFE/" # define unzipped folder location of .SAFE format
 sr_obj = windowed_SR_and_saving(file_path) # create required class object
 
+# Create Model
+from yourmodel import sr_model_10m,sr_model_20m
+model_10m = sr_model_10m()
+model_20m = sr_model_20m()
+
 # perform windowed SR - 10m
-sr_obj.start_super_resolution(band_selection="10m",model=None,forward_call="forward",overlap=20, eliminate_border_px=10)
+sr_obj.start_super_resolution(band_selection="10m",model=model_10m,forward_call="forward",overlap=20, eliminate_border_px=10)
 # perform windowed SR - 20m
-sr_obj.start_super_resolution(band_selection="20m",model=None,forward_call="forward",overlap=20, eliminate_border_px=10)
+sr_obj.start_super_resolution(band_selection="20m",model=model_20m,forward_call="forward",overlap=20, eliminate_border_px=10)
 ```
 To start the Super-Resolution, you need to pass a model to the 'start_super_resolution' function of the 'windowed_SR_and_saving' object.  
-If the call model to SR is different than 'forward',such as PyTorch lightnings 'predict' you can pass the name of the call as an argument.
+If the call model to SR is different than 'forward' for torch.nn.Module types, you can pass the name of the call as an argument. If the input is a PyTorch Lightning model, the .predict() funciton is called.
 
-For more information, this is the doctring of the only important function for now:
+For more information, this is the doctring of the only important function for now (not up to date):
 ```
 	Class that performs windowed super-resolution on a Sentinel-2 image and saves the result. Steps:
         - Copies the 10m and 20m bands to new tiff files in the input directory.
         - 10m and 20m bands can be called separately and preformed with different models.
         - SR Results are saved with an averaged overlap and georeferenced in the input folder.
 
         Inputs:
@@ -83,9 +78,10 @@
             # perform super-resolution on 20m bands
             sr_obj.start_super_resolution(band_selection="20m")
             # perform super-resolution on 10m bands
             sr_obj.start_super_resolution(band_selection="10m")
             # delete LR stack
             sr_obj.delete_LR_stack()
 ```
-## TODo:
-- Enable multi-batch calculation of the SR. Currently, the tool only super-resolutes one image at a time (1,4,128,128)
+
+
+[![Downloads](https://static.pepy.tech/badge/opensr-utils)](https://pepy.tech/project/opensr-utils)
```

### Comparing `opensr-utils-0.4.8/README.md` & `opensr-utils-0.4.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,79 @@
+Metadata-Version: 2.1
+Name: opensr-utils
+Version: 0.4.9
+Summary: Utilities supporting the ESA opensr-model package for Super-Resolution of Senintel-2 Imagery
+Home-page: https://isp.uv.es/opensr/
+Author: Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis
+Author-email: accounts@donike.net
+License: MIT
+Project-URL: Source Code, https://github.com/ESAopenSR/opensr-utils
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy==1.23.5
+Requires-Dist: einops==0.6.0
+Requires-Dist: rasterio==1.3.6
+Requires-Dist: tqdm==4.64.1
+Requires-Dist: torch==1.13.1
+Requires-Dist: scikit-image==0.19.3
+Requires-Dist: pytorch-lightning==1.9.0
+
 # opensr-utils - Supplementary Code for the ESA OpenSR project
 
 *WARNING*  
 The 'eliminate_pixel' functionality is currently experimental and can in some cases return unexpected results.  
 Only the combination of overlap:40 and eliminate_pixel:20 is proven to work. Set to 0 to disable.  
   
   
-
-
 *UPDATE*  
 The current version supports PyTorch Lightning multi-GPU inference, but the documentation hasnt updated yet.
   
   
+
+*Description*  
+This package performs super-resolution with any PyTorch or PyTorch lighning model for Sentinel-2 10m and 20m bands.  
 This package provides useful functions to perform super-resolution of raw Sentinel-2 tiles.  
 Funcitonalities:
-- Reading and stacking of the 10 and 20m bands of Sentinel-2 '.SAFE' file format (worrks with Sen2 downloads straight out of the box)
-- Patching of input images by selectable size (eg 128x128)
-- Super-Resolution of individual patches
-- writing of georeferenced output raster
-- overlapping and averaging of patches by selectable quantity to reduce patching artifacts
-- Processing is performed on the same device as the model that is passed to the funciton
+- The Input can be either:  
+	- a ".SAFE" folder, the format straight from the Copenricus Hub download.  Then, stacking of the 10 and 20m bands of Sentinel-2 '.SAFE' file format is performed (works with Sen2 downloads straight out of the box)
+	- any ".tif" file or similar that can be laoded by rasterio. Either 4- or 6-band for the different models.
+- The following is performed automatically:  
+	- Patching of input images by selectable size (eg 128x128)
+	- Super-Resolution of individual patches with provided model
+	- writing of georeferenced output raster
+	- overlapping and linear weightning of patches by selectable quantity to reduce patching artifacts
+	- Processing is performed on the same device as the model that is passed to the funciton
+- Supported Models:  
+	- 'torch.nn.Module': Any SR model with a .forward() function can be passed. The drawback is that for this model type, multi-GPU and multi-batch processing is not supported. This is therefore considerably slower.
+	- 'LightningModule': Any PL Lightning model with a .predict() function. If this model type is passed, multi-GPU and multi-batch processing is activated, which lkeads to a significant inference speed increase.
 
 Usage example:
 ```python
 !pip install opensr-utils
 import opensr_utils
 from opensr_utils.main import windowed_SR_and_saving 
 
+# Create SR Object
 file_path = "/yourfilepath/S2A_MSIL2A_20230729T100031_N0509_R122_T33TUG_20230729T134559.SAFE/" # define unzipped folder location of .SAFE format
 sr_obj = windowed_SR_and_saving(file_path) # create required class object
 
+# Create Model
+from yourmodel import sr_model_10m,sr_model_20m
+model_10m = sr_model_10m()
+model_20m = sr_model_20m()
+
 # perform windowed SR - 10m
-sr_obj.start_super_resolution(band_selection="10m",model=None,forward_call="forward",overlap=20, eliminate_border_px=10)
+sr_obj.start_super_resolution(band_selection="10m",model=model_10m,forward_call="forward",overlap=20, eliminate_border_px=10)
 # perform windowed SR - 20m
-sr_obj.start_super_resolution(band_selection="20m",model=None,forward_call="forward",overlap=20, eliminate_border_px=10)
+sr_obj.start_super_resolution(band_selection="20m",model=model_20m,forward_call="forward",overlap=20, eliminate_border_px=10)
 ```
 To start the Super-Resolution, you need to pass a model to the 'start_super_resolution' function of the 'windowed_SR_and_saving' object.  
-If the call model to SR is different than 'forward',such as PyTorch lightnings 'predict' you can pass the name of the call as an argument.
+If the call model to SR is different than 'forward' for torch.nn.Module types, you can pass the name of the call as an argument. If the input is a PyTorch Lightning model, the .predict() funciton is called.
 
-For more information, this is the doctring of the only important function for now:
+For more information, this is the doctring of the only important function for now (not up to date):
 ```
 	Class that performs windowed super-resolution on a Sentinel-2 image and saves the result. Steps:
         - Copies the 10m and 20m bands to new tiff files in the input directory.
         - 10m and 20m bands can be called separately and preformed with different models.
         - SR Results are saved with an averaged overlap and georeferenced in the input folder.
 
         Inputs:
@@ -65,9 +97,10 @@
             # perform super-resolution on 20m bands
             sr_obj.start_super_resolution(band_selection="20m")
             # perform super-resolution on 10m bands
             sr_obj.start_super_resolution(band_selection="10m")
             # delete LR stack
             sr_obj.delete_LR_stack()
 ```
-## TODo:
-- Enable multi-batch calculation of the SR. Currently, the tool only super-resolutes one image at a time (1,4,128,128)
+
+
+[![Downloads](https://static.pepy.tech/badge/opensr-utils)](https://pepy.tech/project/opensr-utils)
```

### Comparing `opensr-utils-0.4.8/opensr_utils/bands10m_stacked_from_S2_folder.py` & `opensr-utils-0.4.9/opensr_utils/bands10m_stacked_from_S2_folder.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils/bands20m_stacked_from_S2_folder.py` & `opensr-utils-0.4.9/opensr_utils/bands20m_stacked_from_S2_folder.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils/denormalize_image_per_band_batch.py` & `opensr-utils-0.4.9/opensr_utils/denormalize_image_per_band_batch.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils/main.py` & `opensr-utils-0.4.9/opensr_utils/main.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils/pl_utils.py` & `opensr-utils-0.4.9/opensr_utils/pl_utils.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils/stretching.py` & `opensr-utils-0.4.9/opensr_utils/stretching.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils/weighted_overlap.py` & `opensr-utils-0.4.9/opensr_utils/weighted_overlap.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,12 +171,23 @@
         weights_inverse[:, 0:offset_squares, -offset_squares:] = right_center_inverse
     
         
     # reset NaN values to 0 from earlier
     weights = np.nan_to_num(weights)
     weights_inverse =  np.nan_to_num(weights_inverse)
     
-    assert np.all(weights+weights_inverse)==1., "weights dont sum um to 1. for every single pixel. Abort."
+    
+    try:
+        assert np.all(weights+weights_inverse)==1., "weights dont sum um to 1. for every single pixel. Abort."
+    except AssertionError:
+        import warnings
+        warnings.warn("Weight matrix in valid in weighted overlap. Returning zero tensor.", UserWarning)
+    
     # perform weighting
-    weighted_image = (weights*im) + (weights_inverse*ph)
-
-    return(weighted_image)
+    try:
+        weighted_image = (weights*im) + (weights_inverse*ph)
+        return(weighted_image)
+    except:
+        import warnings
+        warnings.warn("Weighted overlap failed due to weight dimensions. Returning zero tensor.", UserWarning)
+        return(torch.zeros_like(sr))
+
```

### Comparing `opensr-utils-0.4.8/opensr_utils/xAI_utils.py` & `opensr-utils-0.4.9/opensr_utils/xAI_utils.py`

 * *Files identical despite different names*

### Comparing `opensr-utils-0.4.8/opensr_utils.egg-info/PKG-INFO` & `opensr-utils-0.4.9/opensr_utils.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 Metadata-Version: 2.1
 Name: opensr-utils
-Version: 0.4.8
+Version: 0.4.9
 Summary: Utilities supporting the ESA opensr-model package for Super-Resolution of Senintel-2 Imagery
 Home-page: https://isp.uv.es/opensr/
 Author: Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis
 Author-email: accounts@donike.net
 License: MIT
 Project-URL: Source Code, https://github.com/ESAopenSR/opensr-utils
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy==1.23.5
 Requires-Dist: einops==0.6.0
 Requires-Dist: rasterio==1.3.6
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: torch==1.13.1
 Requires-Dist: scikit-image==0.19.3
+Requires-Dist: pytorch-lightning==1.9.0
 
 # opensr-utils - Supplementary Code for the ESA OpenSR project
 
 *WARNING*  
 The 'eliminate_pixel' functionality is currently experimental and can in some cases return unexpected results.  
 Only the combination of overlap:40 and eliminate_pixel:20 is proven to work. Set to 0 to disable.  
   
   
-
-
 *UPDATE*  
 The current version supports PyTorch Lightning multi-GPU inference, but the documentation hasnt updated yet.
   
   
+
+*Description*  
+This package performs super-resolution with any PyTorch or PyTorch lighning model for Sentinel-2 10m and 20m bands.  
 This package provides useful functions to perform super-resolution of raw Sentinel-2 tiles.  
 Funcitonalities:
-- Reading and stacking of the 10 and 20m bands of Sentinel-2 '.SAFE' file format (worrks with Sen2 downloads straight out of the box)
-- Patching of input images by selectable size (eg 128x128)
-- Super-Resolution of individual patches
-- writing of georeferenced output raster
-- overlapping and averaging of patches by selectable quantity to reduce patching artifacts
-- Processing is performed on the same device as the model that is passed to the funciton
+- The Input can be either:  
+	- a ".SAFE" folder, the format straight from the Copenricus Hub download.  Then, stacking of the 10 and 20m bands of Sentinel-2 '.SAFE' file format is performed (works with Sen2 downloads straight out of the box)
+	- any ".tif" file or similar that can be laoded by rasterio. Either 4- or 6-band for the different models.
+- The following is performed automatically:  
+	- Patching of input images by selectable size (eg 128x128)
+	- Super-Resolution of individual patches with provided model
+	- writing of georeferenced output raster
+	- overlapping and linear weightning of patches by selectable quantity to reduce patching artifacts
+	- Processing is performed on the same device as the model that is passed to the funciton
+- Supported Models:  
+	- 'torch.nn.Module': Any SR model with a .forward() function can be passed. The drawback is that for this model type, multi-GPU and multi-batch processing is not supported. This is therefore considerably slower.
+	- 'LightningModule': Any PL Lightning model with a .predict() function. If this model type is passed, multi-GPU and multi-batch processing is activated, which lkeads to a significant inference speed increase.
 
 Usage example:
 ```python
 !pip install opensr-utils
 import opensr_utils
 from opensr_utils.main import windowed_SR_and_saving 
 
+# Create SR Object
 file_path = "/yourfilepath/S2A_MSIL2A_20230729T100031_N0509_R122_T33TUG_20230729T134559.SAFE/" # define unzipped folder location of .SAFE format
 sr_obj = windowed_SR_and_saving(file_path) # create required class object
 
+# Create Model
+from yourmodel import sr_model_10m,sr_model_20m
+model_10m = sr_model_10m()
+model_20m = sr_model_20m()
+
 # perform windowed SR - 10m
-sr_obj.start_super_resolution(band_selection="10m",model=None,forward_call="forward",overlap=20, eliminate_border_px=10)
+sr_obj.start_super_resolution(band_selection="10m",model=model_10m,forward_call="forward",overlap=20, eliminate_border_px=10)
 # perform windowed SR - 20m
-sr_obj.start_super_resolution(band_selection="20m",model=None,forward_call="forward",overlap=20, eliminate_border_px=10)
+sr_obj.start_super_resolution(band_selection="20m",model=model_20m,forward_call="forward",overlap=20, eliminate_border_px=10)
 ```
 To start the Super-Resolution, you need to pass a model to the 'start_super_resolution' function of the 'windowed_SR_and_saving' object.  
-If the call model to SR is different than 'forward',such as PyTorch lightnings 'predict' you can pass the name of the call as an argument.
+If the call model to SR is different than 'forward' for torch.nn.Module types, you can pass the name of the call as an argument. If the input is a PyTorch Lightning model, the .predict() funciton is called.
 
-For more information, this is the doctring of the only important function for now:
+For more information, this is the doctring of the only important function for now (not up to date):
 ```
 	Class that performs windowed super-resolution on a Sentinel-2 image and saves the result. Steps:
         - Copies the 10m and 20m bands to new tiff files in the input directory.
         - 10m and 20m bands can be called separately and preformed with different models.
         - SR Results are saved with an averaged overlap and georeferenced in the input folder.
 
         Inputs:
@@ -83,9 +97,10 @@
             # perform super-resolution on 20m bands
             sr_obj.start_super_resolution(band_selection="20m")
             # perform super-resolution on 10m bands
             sr_obj.start_super_resolution(band_selection="10m")
             # delete LR stack
             sr_obj.delete_LR_stack()
 ```
-## TODo:
-- Enable multi-batch calculation of the SR. Currently, the tool only super-resolutes one image at a time (1,4,128,128)
+
+
+[![Downloads](https://static.pepy.tech/badge/opensr-utils)](https://pepy.tech/project/opensr-utils)
```

### Comparing `opensr-utils-0.4.8/setup.py` & `opensr-utils-0.4.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='opensr-utils',
-    version='0.4.8',
+    version='0.4.9',
     author = "Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis",
     author_email = "accounts@donike.net",
     description = "Utilities supporting the ESA opensr-model package for Super-Resolution of Senintel-2 Imagery",
     url = "https://isp.uv.es/opensr/",
     project_urls={'Source Code': 'https://github.com/ESAopenSR/opensr-utils'},
     license='MIT',
     packages=find_packages(),
@@ -18,9 +18,10 @@
     long_description_content_type='text/markdown',
     install_requires=[
 	'numpy==1.23.5',
 	'einops==0.6.0',
 	'rasterio==1.3.6',
 	'tqdm==4.64.1',
 	'torch==1.13.1',
-	'scikit-image==0.19.3'],
+	'scikit-image==0.19.3',
+        'pytorch-lightning==1.9.0'],
 )
```

