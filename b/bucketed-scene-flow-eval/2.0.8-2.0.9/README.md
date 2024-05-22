# Comparing `tmp/bucketed_scene_flow_eval-2.0.8.tar.gz` & `tmp/bucketed_scene_flow_eval-2.0.9.tar.gz`

## Comparing `bucketed_scene_flow_eval-2.0.8.tar` & `bucketed_scene_flow_eval-2.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/build_pypi.sh
--rw-r--r--   0        0        0    49683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/deflowpp_differences.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py
--rw-r--r--   0        0        0    22724 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/dataset.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_metacategories.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_raw_data.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_scene_flow.py
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/waymoopen/__init__.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/__init__.py
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/camera_projection.py
--rw-r--r--   0        0        0     8717 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/dataclasses.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/pointcloud.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/rgb_image.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/se2.py
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/se3.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/__init__.py
--rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py
--rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/bucketed_epe.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/eval.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/threeway_epe.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/abstract_dataset.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/utils/__init__.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/utils/loaders.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/integration_tests.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/integration_tests.sh
--rwxr-xr-x   0        0        0     4217 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/setup.sh
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/datasets/argoverse2/av2_small_tests.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/datasets/argoverse2/av2_tiny_tests.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/datasets/nuscenes/nuscenes_tests.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/datastructures/rgb.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/eval/bucketed_epe.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/tests/eval/threeway_epe.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/LICENSE
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/build_pypi.sh
+-rw-r--r--   0        0        0    49683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/deflowpp_differences.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py
+-rw-r--r--   0        0        0    22724 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/dataset.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_metacategories.py
+-rw-r--r--   0        0        0    16079 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_raw_data.py
+-rw-r--r--   0        0        0    11762 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_scene_flow.py
+-rw-r--r--   0        0        0    10213 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/waymoopen/__init__.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/__init__.py
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/camera_projection.py
+-rw-r--r--   0        0        0     8717 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/dataclasses.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/pointcloud.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/rgb_image.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/se2.py
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/se3.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/__init__.py
+-rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py
+-rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/bucketed_epe.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/eval.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/threeway_epe.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/abstract_dataset.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/utils/__init__.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/utils/loaders.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/integration_tests.py
+-rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/integration_tests.sh
+-rwxr-xr-x   0        0        0     4217 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/setup.sh
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/datasets/argoverse2/av2_small_tests.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/datasets/argoverse2/av2_tiny_tests.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/datasets/nuscenes/nuscenes_tests.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/datastructures/rgb.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/eval/bucketed_epe.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/tests/eval/threeway_epe.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/LICENSE
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.9/PKG-INFO
```

### Comparing `bucketed_scene_flow_eval-2.0.8/deflowpp_differences.txt` & `bucketed_scene_flow_eval-2.0.9/deflowpp_differences.txt`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/__init__.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/dataset.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import copy
 from pathlib import Path
 from typing import Optional, Union
 
+from bucketed_scene_flow_eval.datasets.argoverse2.argoverse_raw_data import (
+    DEFAULT_POINT_CLOUD_RANGE,
+    PointCloudRange,
+)
 from bucketed_scene_flow_eval.datastructures import *
 from bucketed_scene_flow_eval.eval import (
     BucketedEPEEvaluator,
     Evaluator,
     ThreeWayEPEEvaluator,
 )
 from bucketed_scene_flow_eval.interfaces import (
     CausalSeqLoaderDataset,
     EvalType,
     NonCausalSeqLoaderDataset,
 )
 
-from bucketed_scene_flow_eval.datasets.argoverse2.argoverse_raw_data import DEFAULT_POINT_CLOUD_RANGE, PointCloudRange
+from .nuscenes_metacategories import (
+    BUCKETED_METACATAGORIES,
+    THREEWAY_EPE_METACATAGORIES,
+)
 from .nuscenes_scene_flow import (
     CATEGORY_MAP,
     NuScenesNoFlowSequenceLoader,
     NuScenesSceneFlowSequenceLoader,
 )
-from .nuscenes_metacategories import BUCKETED_METACATAGORIES, THREEWAY_EPE_METACATAGORIES
 
 
 def _make_evaluator(eval_type: EvalType, eval_args: dict) -> Evaluator:
     eval_args_copy = copy.deepcopy(eval_args)
     # Builds the evaluator object for this dataset.
     if eval_type == EvalType.BUCKETED_EPE:
         if "meta_class_lookup" not in eval_args_copy:
@@ -43,14 +49,15 @@
 
 
 class NuScenesCausalSceneFlow(CausalSeqLoaderDataset):
     def __init__(
         self,
         root_dir: Union[Path, list[Path]],
         nuscenes_version: str,
+        split: str,
         subsequence_length: int = 2,
         with_ground: bool = True,
         with_rgb: bool = False,
         cache_root: Path = Path("/tmp/"),
         use_gt_flow: bool = True,
         flow_data_path: Optional[Union[Path, list[Path]]] = None,
         eval_type: str = "bucketed_epe",
@@ -60,24 +67,26 @@
         use_cache=True,
         load_flow: bool = True,
     ) -> None:
         if load_flow:
             self.sequence_loader = NuScenesSceneFlowSequenceLoader(
                 raw_data_path=root_dir,
                 nuscenes_version=nuscenes_version,
+                split=split,
                 with_rgb=with_rgb,
                 use_gt_flow=use_gt_flow,
                 flow_data_path=flow_data_path,
                 expected_camera_shape=expected_camera_shape,
                 point_cloud_range=point_cloud_range,
             )
         else:
             self.sequence_loader = NuScenesNoFlowSequenceLoader(
                 raw_data_path=root_dir,
                 nuscenes_version=nuscenes_version,
+                split=split,
                 with_rgb=with_rgb,
                 expected_camera_shape=expected_camera_shape,
                 point_cloud_range=point_cloud_range,
             )
         super().__init__(
             sequence_loader=self.sequence_loader,
             subsequence_length=subsequence_length,
@@ -92,14 +101,16 @@
         return _make_evaluator(self.eval_type, self.eval_args)
 
 
 class NuScenesNonCausalSceneFlow(NonCausalSeqLoaderDataset):
     def __init__(
         self,
         root_dir: Union[Path, list[Path]],
+        nuscenes_version: str,
+        split: str,
         subsequence_length: int = 2,
         with_ground: bool = True,
         with_rgb: bool = False,
         cache_root: Path = Path("/tmp/"),
         use_gt_flow: bool = True,
         flow_data_path: Optional[Union[Path, list[Path]]] = None,
         eval_type: str = "bucketed_epe",
@@ -107,22 +118,24 @@
         expected_camera_shape: tuple[int, int, int] = (1550, 2048, 3),
         use_cache=True,
         load_flow: bool = True,
     ) -> None:
         if load_flow:
             self.sequence_loader = NuScenesSceneFlowSequenceLoader(
                 root_dir,
+                nuscenes_version=nuscenes_version,
+                split=split,
                 with_rgb=with_rgb,
                 use_gt_flow=use_gt_flow,
                 flow_data_path=flow_data_path,
                 expected_camera_shape=expected_camera_shape,
             )
         else:
             self.sequence_loader = NuScenesNoFlowSequenceLoader(
-                root_dir, with_rgb=with_rgb, expected_camera_shape=expected_camera_shape
+                root_dir, nuscenes_version=nuscenes_version, split=split, with_rgb=with_rgb, expected_camera_shape=expected_camera_shape
             )
         super().__init__(
             sequence_loader=self.sequence_loader,
             subsequence_length=subsequence_length,
             with_ground=with_ground,
             idx_lookup_cache_root=cache_root,
             eval_type=eval_type,
```

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_metacategories.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_metacategories.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_raw_data.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_raw_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Union
 
 import numpy as np
+import open3d as o3d
 from numpy.typing import NDArray
 from nuscenes.utils.data_classes import LidarPointCloud as NuscLidarPointCloud
 from PIL import Image
 from pyquaternion import Quaternion
-import open3d as o3d
 
 from bucketed_scene_flow_eval.datasets.argoverse2.argoverse_raw_data import (
-    PointCloudRange,
     DEFAULT_POINT_CLOUD_RANGE,
+    PointCloudRange,
 )
 from bucketed_scene_flow_eval.datastructures import (
     SE3,
     CameraModel,
     CameraProjection,
     PointCloud,
     PointCloudFrame,
@@ -24,15 +24,15 @@
     RGBFrameLookup,
     RGBImage,
     TimeSyncedAVLidarData,
     TimeSyncedRawFrame,
 )
 from bucketed_scene_flow_eval.interfaces import AbstractSequence, CachedSequenceLoader
 
-from .nuscenes_utils import NuScenesWithInstanceBoxes
+from .nuscenes_utils import NuScenesWithInstanceBoxes, create_splits_tokens
 
 NuscDict = dict[str, Union[str, int, list]]
 NuscSample = dict[str, NuscDict]
 NuscSampleData = NuscDict
 NuscCalibratedSensor = NuscDict
 NuscEgoPose = NuscDict
 
@@ -346,26 +346,28 @@
         return len(self.synced_sensors)
 
 
 class NuScenesRawSequenceLoader(CachedSequenceLoader):
     def __init__(
         self,
         sequence_dir: Path,
+        split: str,
         version: str = "v1.0-mini",
         verbose: bool = False,
         point_cloud_range: PointCloudRange | None = DEFAULT_POINT_CLOUD_RANGE,
     ):
         super().__init__()
         self.dataset_dir = Path(sequence_dir)
         self.verbose = verbose
         assert self.dataset_dir.is_dir(), f"dataset_dir {sequence_dir} does not exist"
         self.nusc = NuScenesWithInstanceBoxes(
             version=version, dataroot=sequence_dir, verbose=verbose
         )
         self.log_lookup: dict[str, NuscDict] = {e["token"]: e for e in self.nusc.scene}
+        self.log_lookup: dict[str, NuscDict] = {k: self.log_lookup[k] for k in create_splits_tokens(split, self.nusc)}
 
         self.point_cloud_range = point_cloud_range
 
         if self.verbose:
             print(f"Loaded {len(self)} logs")
 
     def __len__(self):
```

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_scene_flow.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_scene_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,22 @@
     SemanticClassIdArray,
     SupervisedPointCloudFrame,
     TimeSyncedAVLidarData,
     TimeSyncedRawFrame,
     TimeSyncedSceneFlowFrame,
     VectorArray,
 )
-from bucketed_scene_flow_eval.interfaces import AbstractAVLidarSequence, CachedSequenceLoader
+from bucketed_scene_flow_eval.interfaces import (
+    AbstractAVLidarSequence,
+    CachedSequenceLoader,
+)
 from bucketed_scene_flow_eval.utils.loaders import load_feather
 
+from .nuscenes_utils import create_splits_tokens
+
 CATEGORY_MAP = {
     -1: "background",
     0: "animal",
     1: "human.pedestrian.adult",
     2: "human.pedestrian.child",
     3: "human.pedestrian.construction_worker",
     4: "human.pedestrian.personal_mobility",
@@ -187,14 +192,15 @@
         return NuScenesSceneFlowSequenceLoader.category_name_to_id(category_name)
 
 
 class NuScenesSceneFlowSequenceLoader(ArgoverseSceneFlowSequenceLoader, CachedSequenceLoader):
     def __init__(
         self,
         raw_data_path: Path | list[Path],
+        split: str,
         nuscenes_version: str = "v1.0-mini",
         flow_data_path: Path | list[Path] | None = None,
         use_gt_flow: bool = True,
         with_rgb: bool = False,
         log_subset: list[str] | None = None,
         expected_camera_shape: tuple[int, int, int] = (1550, 2048, 3),
         point_cloud_range: PointCloudRange | None = DEFAULT_POINT_CLOUD_RANGE,
@@ -205,14 +211,15 @@
         self.with_rgb = with_rgb
         self.expected_camera_shape = expected_camera_shape
         self.point_cloud_range = point_cloud_range
         self.nuscenes = NuScenesWithInstanceBoxes(nuscenes_version, raw_data_path)
         self.sequence_id_to_raw_data: dict[str, NuscDict] = {
             e["token"]: e for e in self.nuscenes.scene
         }
+        self.sequence_id_to_raw_data: dict[str, NuscDict] = {k: self.sequence_id_to_raw_data[k] for k in create_splits_tokens(split, self.nuscenes)}
         self.sequence_id_lst: list[str] = sorted(self.sequence_id_to_raw_data.keys())
         self._setup_flow_data(use_gt_flow, flow_data_path)
         self._subset_log(log_subset)
 
     def _load_sequence_uncached(self, sequence_id: str) -> NuScenesSceneFlowSequence:
         assert (
             sequence_id in self.sequence_id_to_flow_data
@@ -258,14 +265,15 @@
         return super().load(idx, relative_to_idx, with_flow=False)
 
 
 class NuScenesNoFlowSequenceLoader(NuScenesSceneFlowSequenceLoader):
     def __init__(
         self,
         raw_data_path: Path | list[Path],
+        split: str,
         nuscenes_version: str = "v1.0-mini",
         with_rgb: bool = False,
         log_subset: list[str] | None = None,
         expected_camera_shape: tuple[int, int, int] = (1550, 2048, 3),
         point_cloud_range: PointCloudRange | None = DEFAULT_POINT_CLOUD_RANGE,
     ):
         CachedSequenceLoader.__init__(self)
@@ -274,14 +282,15 @@
         self.with_rgb = with_rgb
         self.expected_camera_shape = expected_camera_shape
         self.point_cloud_range = point_cloud_range
         self.nuscenes = NuScenesWithInstanceBoxes(nuscenes_version, raw_data_path)
         self.sequence_id_to_raw_data: dict[str, NuscDict] = {
             e["token"]: e for e in self.nuscenes.scene
         }
+        self.sequence_id_to_raw_data: dict[str, NuscDict] = {k: self.sequence_id_to_raw_data[k] for k in create_splits_tokens(split, self.nuscenes)}
         self.sequence_id_lst: list[str] = sorted(self.sequence_id_to_raw_data.keys())
         self._subset_log(log_subset)
 
     def _load_sequence_uncached(self, sequence_id: str) -> NuScenesNoFlowSequence:
         assert (
             sequence_id in self.sequence_id_to_raw_data
         ), f"sequence_id {sequence_id} does not exist"
```

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_utils.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,55 @@
 """This file contains utility functions helpful for using the NuScenes dataset."""
 
 import numpy as np
 from nuscenes.nuscenes import NuScenes
 from nuscenes.utils.data_classes import Box
+from nuscenes.utils.splits import create_splits_scenes
 from pyquaternion import Quaternion
 
 from bucketed_scene_flow_eval.datastructures.se3 import SE3
 
+
+def create_splits_tokens(split: str, nusc: 'NuScenes') -> list[str]:
+    """
+    Returns the logs in each dataset split of nuScenes.
+    Note: Previously this script included the teaser dataset splits. Since new scenes from those logs were added and
+          others removed in the full dataset, that code is incompatible and was removed.
+    :param split: NuScenes split.
+    :param nusc: NuScenes instance.
+    :return: A list of logs in that split.
+    """
+    # Load splits on a scene-level.
+    scene_splits = create_splits_scenes(verbose=False)
+
+    assert split in scene_splits.keys(), 'Requested split {} which is not a known nuScenes split.'.format(split)
+
+    # Check compatibility of split with nusc_version.
+    version = nusc.version
+    if split in {'train', 'val', 'train_detect', 'train_track'}:
+        assert version.endswith('trainval'), \
+            'Requested split {} which is not compatible with NuScenes version {}'.format(split, version)
+    elif split in {'mini_train', 'mini_val'}:
+        assert version.endswith('mini'), \
+            'Requested split {} which is not compatible with NuScenes version {}'.format(split, version)
+    elif split == 'test':
+        assert version.endswith('test'), \
+            'Requested split {} which is not compatible with NuScenes version {}'.format(split, version)
+    else:
+        raise ValueError('Requested split {} which this function cannot map to logs.'.format(split))
+
+    # Get logs for this split.
+    scene_to_log = {scene['name']: scene['token'] for scene in nusc.scene}
+    logs = set()
+    scenes = scene_splits[split]
+    for scene in scenes:
+        logs.add(scene_to_log[scene])
+
+    return list(logs)
+
 class InstanceBox(Box):
     def __init__(
         self,
         center: list[float],
         size: list[float],
         orientation: Quaternion,
         label: int = np.nan,
```

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/__init__.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/camera_projection.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/camera_projection.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/dataclasses.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/pointcloud.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/pointcloud.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/rgb_image.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/rgb_image.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/se2.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/se2.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/datastructures/se3.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/datastructures/se3.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/bucketed_epe.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/bucketed_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/eval/threeway_epe.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/eval/threeway_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/__init__.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/abstract_dataset.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/abstract_dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/utils/__init__.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/bucketed_scene_flow_eval/utils/loaders.py` & `bucketed_scene_flow_eval-2.0.9/bucketed_scene_flow_eval/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/integration_tests.py` & `bucketed_scene_flow_eval-2.0.9/tests/integration_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/setup.sh` & `bucketed_scene_flow_eval-2.0.9/tests/setup.sh`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/datasets/argoverse2/av2_small_tests.py` & `bucketed_scene_flow_eval-2.0.9/tests/datasets/argoverse2/av2_small_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/datasets/argoverse2/av2_tiny_tests.py` & `bucketed_scene_flow_eval-2.0.9/tests/datasets/argoverse2/av2_tiny_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/datasets/nuscenes/nuscenes_tests.py` & `bucketed_scene_flow_eval-2.0.9/tests/datasets/nuscenes/nuscenes_tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 
 @pytest.fixture
 def nuscenes_loader() -> NuScenesRawSequenceLoader:
     return NuScenesRawSequenceLoader(
         sequence_dir=Path("/tmp/nuscenes"),
         version="v1.0-mini",
+        split="mini_train",
         verbose=False,
     )
 
 
 def test_nuscenes_loader_basic_load_and_len_check(nuscenes_loader: NuScenesRawSequenceLoader):
     assert len(nuscenes_loader) > 0, f"no sequences found in {nuscenes_loader}"
-    expected_lens = [236, 239, 236, 236, 233, 223, 239, 231, 231, 228]
+    expected_lens= [236, 236, 236, 233, 223, 239, 231, 231]
     assert len(nuscenes_loader) == len(
         expected_lens
     ), f"expected {len(expected_lens)} sequences, got {len(nuscenes_loader)}"
 
     num_loop_iterations = 0
     for sequence_id, expected_len in zip(nuscenes_loader.get_sequence_ids(), expected_lens):
         num_loop_iterations += 1
```

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/datastructures/rgb.py` & `bucketed_scene_flow_eval-2.0.9/tests/datastructures/rgb.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/eval/bucketed_epe.py` & `bucketed_scene_flow_eval-2.0.9/tests/eval/bucketed_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/tests/eval/threeway_epe.py` & `bucketed_scene_flow_eval-2.0.9/tests/eval/threeway_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/LICENSE` & `bucketed_scene_flow_eval-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/README.md` & `bucketed_scene_flow_eval-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.8/pyproject.toml` & `bucketed_scene_flow_eval-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "/data_prep_scripts",
   "/launch.sh",
   "/README.md",
 ]
 
 [project]
 name = "bucketed_scene_flow_eval"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
   { name="Kyle Vedder", email="kvedder@seas.upenn.edu" },
 ]
 description = "Bucketed Scene Flow Evaluation"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `bucketed_scene_flow_eval-2.0.8/PKG-INFO` & `bucketed_scene_flow_eval-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bucketed_scene_flow_eval
-Version: 2.0.8
+Version: 2.0.9
 Summary: Bucketed Scene Flow Evaluation
 Author-email: Kyle Vedder <kvedder@seas.upenn.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

