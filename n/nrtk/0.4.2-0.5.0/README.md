# Comparing `tmp/nrtk-0.4.2.tar.gz` & `tmp/nrtk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrtk-0.4.2.tar", max compression
+gzip compressed data, was "nrtk-0.5.0.tar", max compression
```

## Comparing `nrtk-0.4.2.tar` & `nrtk-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10173 2024-05-09 17:42:51.201762 nrtk-0.4.2/LICENSE
--rw-r--r--   0        0        0      554 2024-05-09 17:42:51.201762 nrtk-0.4.2/NOTICE
--rw-r--r--   0        0        0     2006 2024-05-09 17:42:51.201762 nrtk-0.4.2/README.md
--rw-r--r--   0        0        0      246 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
--rw-r--r--   0        0        0     1986 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
--rw-r--r--   0        0        0     3302 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image/generic/PIL/__init__.py
--rw-r--r--   0        0        0     4774 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/perturb_image/generic/PIL/enhance.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image/generic/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image/generic/cv2/__init__.py
--rw-r--r--   0        0        0     2702 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/perturb_image/generic/cv2/blur.py
--rw-r--r--   0        0        0      706 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/perturb_image/generic/nop_perturber.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image/generic/skimage/__init__.py
--rw-r--r--   0        0        0     6560 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/perturb_image/generic/skimage/random_noise.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/__init__.py
--rw-r--r--   0        0        0     4534 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/perturber.py
--rw-r--r--   0        0        0     5065 2024-05-09 17:42:51.233762 nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/scenario.py
--rw-r--r--   0        0        0     9671 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/sensor.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image_factory/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/perturb_image_factory/generic/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/perturb_image_factory/generic/step.py
--rw-r--r--   0        0        0     4065 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/perturb_image_factory/pybsm.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/impls/score_detections/__init__.py
--rw-r--r--   0        0        0     2661 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
--rw-r--r--   0        0        0     4277 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/score_detections/coco_scorer.py
--rw-r--r--   0        0        0     1346 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/score_detections/nop_scorer.py
--rw-r--r--   0        0        0     1617 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/impls/score_detections/random_scorer.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/interfaces/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/gen_blackbox_response.py
--rw-r--r--   0        0        0     5401 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/gen_classifier_blackbox_response.py
--rw-r--r--   0        0        0     5394 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/gen_object_detector_blackbox_response.py
--rw-r--r--   0        0        0     1121 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/perturb_image.py
--rw-r--r--   0        0        0     2750 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/perturb_image_factory.py
--rw-r--r--   0        0        0     1345 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/score_classifications.py
--rw-r--r--   0        0        0     1572 2024-05-09 17:42:51.237763 nrtk-0.4.2/nrtk/interfaces/score_detections.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/interop/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/py.typed
--rw-r--r--   0        0        0        0 2024-05-09 17:51:13.771902 nrtk-0.4.2/nrtk/utils/__init__.py
--rw-r--r--   0        0        0     4345 2024-05-09 17:42:51.237763 nrtk-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 nrtk-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-22 19:02:00.874833 nrtk-0.5.0/LICENSE
+-rw-r--r--   0        0        0      554 2024-05-22 19:02:00.874833 nrtk-0.5.0/NOTICE
+-rw-r--r--   0        0        0     2006 2024-05-22 19:02:00.874833 nrtk-0.5.0/README.md
+-rw-r--r--   0        0        0      246 2024-05-22 19:02:00.906833 nrtk-0.5.0/nrtk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
+-rw-r--r--   0        0        0     1986 2024-05-22 19:02:00.906833 nrtk-0.5.0/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
+-rw-r--r--   0        0        0     3302 2024-05-22 19:02:00.906833 nrtk-0.5.0/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image/generic/PIL/__init__.py
+-rw-r--r--   0        0        0     4774 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/generic/PIL/enhance.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image/generic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image/generic/cv2/__init__.py
+-rw-r--r--   0        0        0     2702 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/generic/cv2/blur.py
+-rw-r--r--   0        0        0      706 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/generic/nop_perturber.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image/generic/skimage/__init__.py
+-rw-r--r--   0        0        0     6560 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/generic/skimage/random_noise.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/__init__.py
+-rw-r--r--   0        0        0     4534 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/perturber.py
+-rw-r--r--   0        0        0     5065 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/scenario.py
+-rw-r--r--   0        0        0     9671 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/sensor.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image_factory/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/perturb_image_factory/generic/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image_factory/generic/step.py
+-rw-r--r--   0        0        0     4065 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/perturb_image_factory/pybsm.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/impls/score_detections/__init__.py
+-rw-r--r--   0        0        0     2661 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
+-rw-r--r--   0        0        0     4277 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/score_detections/coco_scorer.py
+-rw-r--r--   0        0        0     1346 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/score_detections/nop_scorer.py
+-rw-r--r--   0        0        0     1617 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/impls/score_detections/random_scorer.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/interfaces/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/gen_blackbox_response.py
+-rw-r--r--   0        0        0     5401 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/gen_classifier_blackbox_response.py
+-rw-r--r--   0        0        0     5394 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/gen_object_detector_blackbox_response.py
+-rw-r--r--   0        0        0     1121 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/perturb_image.py
+-rw-r--r--   0        0        0     2750 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/perturb_image_factory.py
+-rw-r--r--   0        0        0     1345 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/score_classifications.py
+-rw-r--r--   0        0        0     1572 2024-05-22 19:02:00.910833 nrtk-0.5.0/nrtk/interfaces/score_detections.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/interop/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/py.typed
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:39.506019 nrtk-0.5.0/nrtk/utils/__init__.py
+-rw-r--r--   0        0        0     4345 2024-05-22 19:02:00.914832 nrtk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 nrtk-0.5.0/PKG-INFO
```

### Comparing `nrtk-0.4.2/LICENSE` & `nrtk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/NOTICE` & `nrtk-0.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/README.md` & `nrtk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py` & `nrtk-0.5.0/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py` & `nrtk-0.5.0/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/generic/PIL/enhance.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/generic/PIL/enhance.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/generic/cv2/blur.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/generic/cv2/blur.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/generic/nop_perturber.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/generic/nop_perturber.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/generic/skimage/random_noise.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/generic/skimage/random_noise.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/perturber.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/perturber.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/scenario.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/scenario.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image/pybsm/sensor.py` & `nrtk-0.5.0/nrtk/impls/perturb_image/pybsm/sensor.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image_factory/generic/step.py` & `nrtk-0.5.0/nrtk/impls/perturb_image_factory/generic/step.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/perturb_image_factory/pybsm.py` & `nrtk-0.5.0/nrtk/impls/perturb_image_factory/pybsm.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py` & `nrtk-0.5.0/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/score_detections/coco_scorer.py` & `nrtk-0.5.0/nrtk/impls/score_detections/coco_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/score_detections/nop_scorer.py` & `nrtk-0.5.0/nrtk/impls/score_detections/nop_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/impls/score_detections/random_scorer.py` & `nrtk-0.5.0/nrtk/impls/score_detections/random_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/gen_blackbox_response.py` & `nrtk-0.5.0/nrtk/interfaces/gen_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/gen_classifier_blackbox_response.py` & `nrtk-0.5.0/nrtk/interfaces/gen_classifier_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/gen_object_detector_blackbox_response.py` & `nrtk-0.5.0/nrtk/interfaces/gen_object_detector_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/perturb_image.py` & `nrtk-0.5.0/nrtk/interfaces/perturb_image.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/perturb_image_factory.py` & `nrtk-0.5.0/nrtk/interfaces/perturb_image_factory.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/score_classifications.py` & `nrtk-0.5.0/nrtk/interfaces/score_classifications.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/nrtk/interfaces/score_detections.py` & `nrtk-0.5.0/nrtk/interfaces/score_detections.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.2/pyproject.toml` & `nrtk-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ###############################################################################
 [tool.poetry]
 name = "nrtk"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # This package prefers to use the strict numbering standard when possible.
-version = "0.4.2"
+version = "0.5.0"
 description = "An open source toolkit for evaluating the natural robustness of computer vision algorithms."
 license = "Apache-2.0"
 authors = ["Kitware, Inc. <nrtk@kitware.com>"]
 readme = "README.md"
 packages = [{include = "nrtk"}]
 documentation = "https://nrtk.readthedocs.io/"
 classifiers = [
@@ -29,29 +29,29 @@
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 numpy = [
-    {version = ">=1.23.1,<1.25", python = ">=3.8,<3.12"},
+    {version = ">=1.23.1,<1.26", python = ">=3.8,<3.12"},
     {version = ">=1.26", python = "^3.12"}
 ]
 opencv-python = ">=4.6"
 Pillow = ">=10.2.0"
 scikit-image = [
     {version = ">=0.21,<0.22", python = ">=3.8,<3.12"},
     {version = ">=0.22", python = ">=3.12"}
 ]
 smqtk-classifier = ">=0.19.0"
 smqtk-core = ">=0.19"
 smqtk-detection = ">=0.19.0"
 smqtk-image-io = ">=0.17.1"
 tqdm = ">=4.64"
-pybsm = ">=0.2.0"
+pybsm = ">=0.3.1"
 pycocotools = ">=2.0.6"
 setuptools = ">=65.6.1"
 
 [tool.poetry.extras]
 
 [tool.poetry.group.dev.dependencies]
 # Linting
```

### Comparing `nrtk-0.4.2/PKG-INFO` & `nrtk-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrtk
-Version: 0.4.2
+Version: 0.5.0
 Summary: An open source toolkit for evaluating the natural robustness of computer vision algorithms.
 License: Apache-2.0
 Author: Kitware, Inc.
 Author-email: nrtk@kitware.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: Pillow (>=10.2.0)
-Requires-Dist: numpy (>=1.23.1,<1.25) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: numpy (>=1.23.1,<1.26) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: numpy (>=1.26) ; python_version >= "3.12" and python_version < "4.0"
 Requires-Dist: opencv-python (>=4.6)
-Requires-Dist: pybsm (>=0.2.0)
+Requires-Dist: pybsm (>=0.3.1)
 Requires-Dist: pycocotools (>=2.0.6)
 Requires-Dist: scikit-image (>=0.21,<0.22) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: scikit-image (>=0.22) ; python_version >= "3.12"
 Requires-Dist: setuptools (>=65.6.1)
 Requires-Dist: smqtk-classifier (>=0.19.0)
 Requires-Dist: smqtk-core (>=0.19)
 Requires-Dist: smqtk-detection (>=0.19.0)
```

