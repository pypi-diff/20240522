# Comparing `tmp/distnet2d-0.1.6.tar.gz` & `tmp/distnet2d-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distnet2d-0.1.6.tar", last modified: Thu May 16 15:37:09 2024, max compression
+gzip compressed data, was "distnet2d-0.1.7.tar", last modified: Wed May 22 20:38:15 2024, max compression
```

## Comparing `distnet2d-0.1.6.tar` & `distnet2d-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:37:09.855377 distnet2d-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:37:09.855377 distnet2d-0.1.6/DiSTNet2D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-16 15:37:09.000000 distnet2d-0.1.6/DiSTNet2D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 15:37:09.000000 distnet2d-0.1.6/DiSTNet2D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:37:09.000000 distnet2d-0.1.6/DiSTNet2D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 15:37:09.000000 distnet2d-0.1.6/DiSTNet2D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 15:37:09.000000 distnet2d-0.1.6/DiSTNet2D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 15:37:05.000000 distnet2d-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-16 15:37:09.855377 distnet2d-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-16 15:37:05.000000 distnet2d-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:37:09.851377 distnet2d-0.1.6/distnet_2d/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:37:09.851377 distnet2d-0.1.6/distnet_2d/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/data/dydx_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/data/medoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/data/swim1d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:37:09.851377 distnet2d-0.1.6/distnet_2d/model/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)    37691 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/distnet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/distnet_2d_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/gradient_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/model/spatial_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:37:09.855377 distnet2d-0.1.6/distnet_2d/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/agc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/metrics_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-05-16 15:37:05.000000 distnet2d-0.1.6/distnet_2d/utils/objectwise_computation_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:37:09.855377 distnet2d-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 15:37:05.000000 distnet2d-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.671552 distnet2d-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.671552 distnet2d-0.1.7/DiSTNet2D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 20:38:12.000000 distnet2d-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-22 20:38:15.671552 distnet2d-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-22 20:38:12.000000 distnet2d-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.667552 distnet2d-0.1.7/distnet_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.667552 distnet2d-0.1.7/distnet_2d/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/dydx_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/medoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/swim1d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.667552 distnet2d-0.1.7/distnet_2d/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/distnet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/distnet_2d_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/gradient_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/spatial_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.671552 distnet2d-0.1.7/distnet_2d/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/agc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/metrics_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/objectwise_computation_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:38:15.671552 distnet2d-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 20:38:12.000000 distnet2d-0.1.7/setup.py
```

### Comparing `distnet2d-0.1.6/DiSTNet2D.egg-info/PKG-INFO` & `distnet2d-0.1.7/DiSTNet2D.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.6
+Version: 0.1.7
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.6/distnet2d-0.1.6.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.7/distnet2d-0.1.7.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -18,15 +18,15 @@
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow>=2.7.1
 Requires-Dist: edt>=2.0.2
 Requires-Dist: scikit-fmm
 Requires-Dist: numba
-Requires-Dist: dataset_iterator>=0.4.2
+Requires-Dist: dataset_iterator>=0.4.5
 Requires-Dist: elasticdeform>=0.4.7
 
 # DistNet2D: Leveraging long-range temporal information for efficient segmentation and tracking
 
 This repository contains python code for training the neural network.
 
 [Link to preprint](https://arxiv.org/abs/2310.19641)
```

### Comparing `distnet2d-0.1.6/DiSTNet2D.egg-info/SOURCES.txt` & `distnet2d-0.1.7/DiSTNet2D.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,13 +16,12 @@
 distnet_2d/model/distnet_2d.py
 distnet_2d/model/distnet_2d_seg.py
 distnet_2d/model/gradient_accumulator.py
 distnet_2d/model/layers.py
 distnet_2d/model/spatial_attention.py
 distnet_2d/utils/__init__.py
 distnet_2d/utils/agc.py
-distnet_2d/utils/callbacks.py
 distnet_2d/utils/helpers.py
 distnet_2d/utils/losses.py
 distnet_2d/utils/lovasz_loss.py
 distnet_2d/utils/metrics_tf.py
 distnet_2d/utils/objectwise_computation_tf.py
```

### Comparing `distnet2d-0.1.6/LICENSE.txt` & `distnet2d-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/PKG-INFO` & `distnet2d-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.6
+Version: 0.1.7
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.6/distnet2d-0.1.6.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.7/distnet2d-0.1.7.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -18,15 +18,15 @@
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow>=2.7.1
 Requires-Dist: edt>=2.0.2
 Requires-Dist: scikit-fmm
 Requires-Dist: numba
-Requires-Dist: dataset_iterator>=0.4.2
+Requires-Dist: dataset_iterator>=0.4.5
 Requires-Dist: elasticdeform>=0.4.7
 
 # DistNet2D: Leveraging long-range temporal information for efficient segmentation and tracking
 
 This repository contains python code for training the neural network.
 
 [Link to preprint](https://arxiv.org/abs/2310.19641)
```

### Comparing `distnet2d-0.1.6/README.md` & `distnet2d-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/data/dydx_iterator.py` & `distnet2d-0.1.7/distnet_2d/data/dydx_iterator.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/data/swim1d.py` & `distnet2d-0.1.7/distnet_2d/data/swim1d.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/model/architectures.py` & `distnet2d-0.1.7/distnet_2d/model/architectures.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/model/distnet_2d.py` & `distnet2d-0.1.7/distnet_2d/model/distnet_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,43 +4,44 @@
 from .spatial_attention import SpatialAttention2D
 from ..utils.helpers import ensure_multiplicity, flatten_list
 from ..utils.losses import weighted_loss_by_category, balanced_category_loss, PseudoHuber
 from ..utils.agc import adaptive_clip_grad
 from .gradient_accumulator import GradientAccumulator
 import time
 
-class DistnetModel(tf.keras.Model):
+class DiSTNetModel(tf.keras.Model):
     def __init__(self, *args, spatial_dims,
-        edm_loss_weight:float=1,
-        center_loss_weight:float=1,
-        displacement_loss_weight:float=1,
-        category_loss_weight:float=1,
-        edm_loss= PseudoHuber(1),
-        center_loss = PseudoHuber(1),
-        displacement_loss = PseudoHuber(1),
-        category_weights = None, # array of weights: [normal, division, no previous cell] or None = auto
-        category_class_frequency_range=[1/50, 50],
-        next = True,
-        frame_window = 3,
-        long_term:bool = True,
-        predict_next_displacement:bool = True,
-        print_gradients:bool=False, # for optimization, available in eager mode only
-        accum_steps=1, use_agc=False, agc_clip_factor=0.1, agc_eps=1e-3, agc_exclude_output=False, # lower clip factor clips more
-        **kwargs):
+                 edm_loss_weight:float=1,
+                 center_loss_weight:float=1,
+                 displacement_loss_weight:float=1,
+                 category_loss_weight:float=1,
+                 edm_loss=PseudoHuber(1),
+                 gcdm_loss=PseudoHuber(1), gcdm_gradients:bool=False,
+                 displacement_loss=PseudoHuber(1),
+                 category_weights=None,  # array of weights: [normal, division, no previous cell] or None = auto
+                 category_class_frequency_range=[1/50, 50],
+                 next=True,
+                 frame_window=3,
+                 long_term:bool=True,
+                 predict_next_displacement:bool=True,
+                 print_gradients:bool=False,  # for optimization, available in eager mode only
+                 accum_steps=1, use_agc=False, agc_clip_factor=0.1, agc_eps=1e-3, agc_exclude_output=False,  # lower clip factor clips more
+                 **kwargs):
         super().__init__(*args, **kwargs)
         self.edm_weight = edm_loss_weight
         self.center_weight = center_loss_weight
         self.displacement_weight = displacement_loss_weight
         self.category_weight = category_loss_weight
         self.spatial_dims = spatial_dims
         self.next = next
         self.predict_next_displacement=predict_next_displacement
         self.frame_window = frame_window
         self.edm_loss = edm_loss
-        self.center_loss=center_loss
+        self.gdcm_loss=gcdm_loss
+        self.gcdm_gradients=gcdm_gradients
         self.displacement_loss = displacement_loss
 
         min_class_frequency=category_class_frequency_range[0]
         max_class_frequency=category_class_frequency_range[1]
         if category_weights is not None:
             assert len(category_weights)==3, "3 category weights should be provided: normal cell, dividing cell, cell with no previous cell"
             self.category_loss=weighted_loss_by_category(tf.keras.losses.CategoricalCrossentropy(), category_weights, remove_background=True)
@@ -91,21 +92,21 @@
                 edm_loss = self.edm_loss(y[0], y_pred[0]) #, sample_weight = weight_map)
                 losses["edm"] = edm_loss
                 loss_weights["edm"] = edm_weight
 
             # center
             if center_weight>0:
                 center_pred_inside=tf.where(cell_mask, y_pred[1], 0) # do not predict anything outside
-                center_loss = self.center_loss(y[1], center_pred_inside)
+                center_loss = self.gdcm_loss(y[1], center_pred_inside)
                 losses["center"] = center_loss
                 loss_weights["center"] = center_weight
 
             #regression displacement loss
             if displacement_weight>0:
-                loss_dY, loss_dX = self._compute_displacement_loss(y, y_pred, cell_mask)
+                loss_dY, loss_dX = self._compute_displacement_loss(y, y_pred, cell_mask, spatial_gradients=self.gcdm_gradients)
                 losses["dY"] = loss_dY
                 loss_weights["dY"] = displacement_weight
                 losses["dX"] = loss_dX
                 loss_weights["dX"] = displacement_weight
 
             # category loss
             if category_weight>0:
@@ -152,15 +153,15 @@
         if not self.use_grad_acc:
             self.optimizer.apply_gradients(zip(gradients, self.trainable_variables)) #Update weights
         else:
             self.gradient_accumulator.accumulate_gradients(gradients)
             self.gradient_accumulator.apply_gradients()
         return losses
 
-    def _compute_displacement_loss(self, y, y_pred, cell_mask):
+    def _compute_displacement_loss(self, y, y_pred, cell_mask, spatial_gradients:bool=False):
         fw = self.frame_window
         mask = cell_mask[..., 1:]
         if self.predict_next_displacement:
             mask_next = cell_mask[..., :-1]
         if self.long_term and fw > 1:
             mask_center = tf.tile(mask[..., fw - 1:fw], [1, 1, 1, fw - 1])
             if self.predict_next_displacement:
@@ -174,15 +175,22 @@
                 else:
                     mask = tf.concat([mask, mask_center], -1)
         elif self.predict_next_displacement:
             mask = tf.concat([mask, mask_next], -1)
 
         dy_inside = tf.where(mask, y_pred[2], 0)  # do not predict anything outside
         dx_inside = tf.where(mask, y_pred[3], 0)  # do not predict anything outside
-
+        if spatial_gradients:
+            dy_dy, dx_dy = tf.image.image_gradients(y[2])
+            dy_dx, dx_dx = tf.image.image_gradients(y[3])
+            dy_dy_pred, dx_dy_pred = tf.image.image_gradients(y[2])
+            dy_dy_pred, dx_dy_pred = tf.where(mask, dy_dy_pred, 0), tf.where(mask, dx_dy_pred, 0)
+            dy_dx_pred, dx_dx_pred = tf.image.image_gradients(y[3])
+            dy_dx_pred, dx_dx_pred = tf.where(mask, dy_dx_pred, 0), tf.where(mask, dx_dx_pred, 0)
+            return 1./3 * (self.displacement_loss(y[2], dy_inside) + self.displacement_loss(dy_dy, dy_dy_pred) + self.displacement_loss(dx_dy, dx_dy_pred)), 1./3 * (self.displacement_loss(y[3], dx_inside) + self.displacement_loss(dy_dx, dy_dx_pred) + self.displacement_loss(dx_dx, dx_dx_pred))
         return self.displacement_loss(y[2], dy_inside), self.displacement_loss(y[3], dx_inside)
 
     def _compute_category_loss(self, y, y_pred, n_frame_pairs, n_fp_mul):
         cat_loss = 0.
         for i in range(n_frame_pairs * n_fp_mul):
             inside_mask = tf.math.greater(y[4][..., i:i + 1], 0)
             cat_pred_inside = tf.where(inside_mask, y_pred[4][..., 3 * i:3 * i + 3], 1)
@@ -210,39 +218,40 @@
             next:bool,
             config,
             name: str="DiSTNet2D",
             **kwargs):
 
     return get_distnet_2d_model(input_shape, upsampling_mode = config.upsampling_mode, downsampling_mode=config.downsampling_mode, skip_stop_gradient=False, skip_connections=config.skip_connections, encoder_settings=config.encoder_settings, feature_settings=config.feature_settings, feature_blending_settings=config.feature_blending_settings, decoder_settings=config.decoder_settings, feature_decoder_settings=config.feature_decoder_settings, attention=config.attention, attention_dropout=config.dropout, self_attention=config.self_attention, combine_kernel_size=config.combine_kernel_size, pair_combine_kernel_size=config.pair_combine_kernel_size, blending_filter_factor=config.blending_filter_factor, frame_window=frame_window, next=next, name=name, **kwargs)
 
-def get_distnet_2d_model(input_shape, # Y, X
-            encoder_settings:list,
-            feature_settings: list,
-            feature_blending_settings: list,
-            feature_decoder_settings:list,
-            decoder_settings: list,
-            upsampling_mode:str="tconv", # tconv, up_nn, up_bilinear
-            downsampling_mode:str = "maxpool_and_stride", #maxpool, stride, maxpool_and_stride
-            combine_kernel_size:int = 1,
-            pair_combine_kernel_size:int = 1,
-            blending_filter_factor:float = 0.5,
-            skip_stop_gradient:bool = False,
-            skip_connections = [-1], # bool or list. -1 = feature level
-            skip_combine_mode:str="conv", #conv, wsconv
-            attention : int = 0,
-            attention_dropout:float = 0.1,
-            self_attention: int = 0,
-            frame_window:int = 1,
-            next:bool=True,
-            long_term:bool = True,
-            predict_next_displacement:bool = True,
-            l2_reg:float = 0,
-            name: str="DiSTNet2D",
-            **kwargs,
-    ):
+def get_distnet_2d_model(input_shape,  # Y, X
+                         encoder_settings:list,
+                         feature_settings: list,
+                         feature_blending_settings: list,
+                         feature_decoder_settings:list,
+                         decoder_settings: list,
+                         upsampling_mode:str="tconv",  # tconv, up_nn, up_bilinear
+                         downsampling_mode:str = "maxpool_and_stride",  #maxpool, stride, maxpool_and_stride
+                         combine_kernel_size:int = 1,
+                         pair_combine_kernel_size:int = 1,
+                         blending_filter_factor:float = 0.5,
+                         skip_stop_gradient:bool = False,
+                         skip_connections = [-1],  # bool or list. -1 = feature level
+                         skip_combine_mode:str="conv",  #conv, wsconv
+                         attention : int = 0,
+                         attention_dropout:float = 0.1,
+                         self_attention: int = 0,
+                         frame_window:int = 1,
+                         next:bool=True,
+                         long_term:bool = True,
+                         predict_next_displacement:bool = True,
+                         gcdm_gradients:bool=False,
+                         l2_reg:float = 0,
+                         name: str="DiSTNet2D",
+                         **kwargs,
+                         ):
         total_contraction = np.prod([np.prod([params.get("downscale", 1) for params in param_list]) for param_list in encoder_settings])
         assert len(encoder_settings)==len(decoder_settings), "decoder should have same length as encoder"
         if attention>0 or self_attention>0:
             spatial_dims = ensure_multiplicity(2, input_shape)
             if isinstance(spatial_dims, tuple):
                 spatial_dims = list(spatial_dims)
         else:
@@ -399,15 +408,15 @@
                         output_per_dec[output_name] = up_out
                 if predict_next_displacement: # merge outputs ending by Next
                     for k in list(output_per_dec.keys()):
                         if k.endswith("Next"):
                             output_name = k.replace("Next", "")
                             output_per_dec[output_name] = tf.keras.layers.Concatenate(axis = -1, name = decoder_output_names[decoder_name][output_name])([output_per_dec[output_name], output_per_dec.pop(k)])
                 outputs.extend(output_per_dec.values())
-        return DistnetModel([input], outputs, name=name, frame_window=frame_window, next = next, spatial_dims=spatial_dims if attention>0 or self_attention>0 else None, long_term=long_term, predict_next_displacement=predict_next_displacement, **kwargs)
+        return DiSTNetModel([input], outputs, name=name, frame_window=frame_window, next = next, spatial_dims=spatial_dims if attention > 0 or self_attention > 0 else None, long_term=long_term, predict_next_displacement=predict_next_displacement, gcdm_gradients=gcdm_gradients, **kwargs)
 
 def encoder_op(param_list, downsampling_mode, skip_stop_gradient:bool = False, l2_reg:float=0, last_input_filters:int=0, name: str="EncoderLayer", layer_idx:int=1):
     name=f"{name}{layer_idx}"
     maxpool = downsampling_mode=="maxpool"
     maxpool_and_stride = downsampling_mode == "maxpool_and_stride"
     sequence, down_sequence, total_contraction, residual_filters, out_filters = parse_param_list(param_list, name, ignore_stride=maxpool, l2_reg=l2_reg, last_input_filters = last_input_filters if maxpool_and_stride else 0)
     assert total_contraction>1, "invalid parameters: no contraction specified"
```

### Comparing `distnet2d-0.1.6/distnet_2d/model/distnet_2d_seg.py` & `distnet2d-0.1.7/distnet_2d/model/distnet_2d_seg.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/model/gradient_accumulator.py` & `distnet2d-0.1.7/distnet_2d/model/gradient_accumulator.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/model/layers.py` & `distnet2d-0.1.7/distnet_2d/model/layers.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/model/spatial_attention.py` & `distnet2d-0.1.7/distnet_2d/model/spatial_attention.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/utils/agc.py` & `distnet2d-0.1.7/distnet_2d/utils/agc.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/utils/helpers.py` & `distnet2d-0.1.7/distnet_2d/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/utils/losses.py` & `distnet2d-0.1.7/distnet_2d/utils/losses.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/utils/lovasz_loss.py` & `distnet2d-0.1.7/distnet_2d/utils/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/utils/metrics_tf.py` & `distnet2d-0.1.7/distnet_2d/utils/metrics_tf.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/distnet_2d/utils/objectwise_computation_tf.py` & `distnet2d-0.1.7/distnet_2d/utils/objectwise_computation_tf.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.6/setup.py` & `distnet2d-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DiSTNet2D",
-    version="0.1.6",
+    version="0.1.7",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="tensorflow/keras implementation of DiSTNet 2D",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/distnet2d",
-    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.6/distnet2d-0.1.6.tar.gz',
+    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.7/distnet2d-0.1.7.tar.gz',
     packages=setuptools.find_packages(),
     keywords=['Segmentation', 'Tracking', 'Cell', 'Tensorflow', 'Keras'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3',
-    install_requires=['numpy', 'scipy', 'tensorflow>=2.7.1', 'edt>=2.0.2', 'scikit-fmm', 'numba', 'dataset_iterator>=0.4.2', 'elasticdeform>=0.4.7']
+    install_requires=['numpy', 'scipy', 'tensorflow>=2.7.1', 'edt>=2.0.2', 'scikit-fmm', 'numba', 'dataset_iterator>=0.4.5', 'elasticdeform>=0.4.7']
 )
```

