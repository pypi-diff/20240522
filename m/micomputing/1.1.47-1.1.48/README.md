# Comparing `tmp/micomputing-1.1.47.tar.gz` & `tmp/micomputing-1.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.47.tar", last modified: Sun Mar 31 01:38:48 2024, max compression
+gzip compressed data, was "micomputing-1.1.48.tar", last modified: Wed May 22 09:35:23 2024, max compression
```

## Comparing `micomputing-1.1.47.tar` & `micomputing-1.1.48.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-31 01:38:48.234260 micomputing-1.1.47/
--rw-r--r--   0 admin      (501) staff       (20)       99 2024-03-31 01:38:48.000000 micomputing-1.1.47/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)      394 2024-03-31 01:38:48.234119 micomputing-1.1.47/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2024-03-31 01:38:48.000000 micomputing-1.1.47/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-31 01:38:48.231909 micomputing-1.1.47/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     3077 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    60518 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    39911 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54665 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23653 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    24832 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    44391 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1183 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/test_dismap.py
--rw-r--r--   0 admin      (501) staff       (20)   157221 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-31 01:38:48.233045 micomputing-1.1.47/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-31 01:38:48.233892 micomputing-1.1.47/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)    19178 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/__pycache__/TRS.cpython-311.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)    17706 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/__pycache__/exec.cpython-311.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing/zxhtools/image2.FFD
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-31 01:38:48.232613 micomputing-1.1.47/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      394 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      880 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       83 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2024-03-31 01:38:48.000000 micomputing-1.1.47/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-03-31 01:38:48.234337 micomputing-1.1.47/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      713 2024-03-31 01:38:48.000000 micomputing-1.1.47/setup_micomputing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-22 09:35:23.982408 micomputing-1.1.48/
+-rw-r--r--   0 admin      (501) staff       (20)       99 2024-05-22 09:35:23.000000 micomputing-1.1.48/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)      394 2024-05-22 09:35:23.982289 micomputing-1.1.48/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2024-05-22 09:35:23.000000 micomputing-1.1.48/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-22 09:35:23.980067 micomputing-1.1.48/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     3142 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    63800 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    39911 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54643 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/metrics.py
+-rwxr-xr-x   0 admin      (501) staff       (20)    33404 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/micfunctions.so
+-rw-r--r--   0 admin      (501) staff       (20)    35063 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    29982 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    44425 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1183 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/test_dismap.py
+-rw-r--r--   0 admin      (501) staff       (20)   160592 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-22 09:35:23.981276 micomputing-1.1.48/micomputing/zxhtools/
+-rw-r--r--   0 admin      (501) staff       (20)     7454 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/TRS.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-22 09:35:23.982115 micomputing-1.1.48/micomputing/zxhtools/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)    19178 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/__pycache__/TRS.cpython-311.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     9153 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8988 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)    17706 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/__pycache__/exec.cpython-311.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8071 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/exec.py
+-rw-r--r--   0 admin      (501) staff       (20)      507 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/image2.AFF
+-rw-r--r--   0 admin      (501) staff       (20)    21032 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing/zxhtools/image2.FFD
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-22 09:35:23.980735 micomputing-1.1.48/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      394 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      880 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       83 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2024-05-22 09:35:23.000000 micomputing-1.1.48/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-22 09:35:23.982452 micomputing-1.1.48/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      713 2024-05-22 09:35:23.000000 micomputing-1.1.48/setup_micomputing.py
```

### Comparing `micomputing-1.1.47/README.md` & `micomputing-1.1.48/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/__init__.py` & `micomputing-1.1.48/micomputing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.46',
+    version = '1.1.47',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'matplotlib', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
     update = '2023-07-10 20:53:03',
     package_data = True
 ).check()
-__version__ = '1.1.46'
-from .trans import Transformation, ComposedTransformation, CompoundTransformation, interpolation, interpolation_forward, Identity, Id, Rotation90, Rotation180, Rotation270, Reflect, Reflection, Permutedim, DimPermutation, Rescale, Rescaling, rand_Rescaling, Translate, Translation, rand_Translation, Rigid, Rig, rand_Rigidity, rand_Rig, Affine, Aff, rand_Affinity, rand_Aff, PolyAffine, rand_PolyAffine, logEuclidean, logEu, rand_logEuclidean, rand_logEu, LocallyAffine, LARM, rand_LocallyAffine, rand_LARM, FreeFormDeformation, FFD, rand_FreeFormDeformation, rand_FFD, DenseDisplacementField, DDF, rand_DenseDisplacementField, rand_DDF, VelocityField, VF, rand_VelocityField, rand_VF #*
+__version__ = '1.1.47'
+from .trans import Transformation, ComposedTransformation, CompoundTransformation, interpolation, interpolation_forward, Identity, Id, Rotation90, Rotation180, Rotation270, Reflect, Reflection, Permutedim, DimPermutation, Rescale, Rescaling, rand_Rescaling, Translate, Translation, rand_Translation, Rigid, Rig, rand_Rigidity, rand_Rig, Affine, Aff, rand_Affinity, rand_Aff, PolyAffine, rand_PolyAffine, logEuclidean, logEu, rand_logEuclidean, rand_logEu, LocallyAffine, LARM, rand_LocallyAffine, rand_LARM, FreeFormDeformation, FFD, rand_FreeFormDeformation, rand_FFD, DenseDisplacementField, DDF, rand_DenseDisplacementField, rand_DDF, VelocityField, VF, rand_VelocityField, rand_VF, Normalize, Cropping #*
 from . import plot as plt
-from .stdio import IMG, dcm2nii, nii2dcm #*
-from .data import Key, DataObject, Slicer, Dataset #*
-from .network import U_Net, CNN, FCN
+from .stdio import IMG, dcm2nii, nii2dcm, affine2orient #*
+from .data import Key, DataObject, Slicer, Dataset, LossCollector #*
+from .network import U_Net, CNN, FCN, NeuralODE #*
 from .funcs import reorient, rescale, dilate, blur, bending, distance_map, registration, local_prior, center_of_gravity #*
 # from .trans import Transformation, WoldCoordsTransformation, ImageCoordsTransformation, IntensityTransformation, ComposedTransformation, CompoundTransformation, Identity, Id, Rotation90, Rotation180, Rotation270, Reflect, Reflection, Permutedim, DimPermutation, Rescale, Rescaling, Translate, Translation, Rigid, Rig, Affine, Aff, PolyAffine, logEu, LocallyAffine, LARM, FreeFormDeformation, FFD, DenseDisplacementField, DDF, MultiLayerPerception, MLP, Normalize, resample, interpolation, interpolation_forward, Affine2D2Matrix, Quaterns2Matrix, Matrix2Quaterns #*
 from .metrics import metric, ITKMetric, ITKLabelMetric, MutualInformation, NormalizedMutualInformation, KLDivergence, CorrelationOfLocalEstimation, NormalizedVectorInformation, Cos2Theta, SumSquaredDifference, MeanSquaredErrors, PeakSignalToNoiseRatio, CrossEntropy, CrossCorrelation, NormalizedCrossCorrelation, StructuralSimilarity, Dice, DiceScore, DiceScoreCoefficient, LabelDice, LabelDiceScore, LabelDiceScoreCoefficient, ITKDiceScore, ITKJaccardCoefficient, ITKVolumeSimilarity, ITKFalsePositive, ITKFalseNegative, ITKHausdorffDistance, ITKMedianSurfaceDistance, ITKAverageSurfaceDistance, ITKDivergenceOfSurfaceDistance, ITKLabelDiceScore, ITKLabelJaccardCoefficient, ITKLabelVolumeSimilarity, ITKLabelFalsePositive, ITKLabelFalseNegative, ITKLabelHausdorffDistance, ITKLabelMedianSurfaceDistance, ITKLabelAverageSurfaceDistance, ITKLabelDivergenceOfSurfaceDistance, LocalNonOrthogonality, RigidProjectionError, joint_hist #*
```

### Comparing `micomputing-1.1.47/micomputing/data.py` & `micomputing-1.1.48/micomputing/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     from pycamia import avouch, touch, to_tuple, arg_tuple, execblock
 
 __all__ = """
     Key
     DataObject
     Slicer
     Dataset
+    LossCollector
 """.split()
     # Subject
     # ImageObject
     # Dataset
     # MedicalDataset
     
 def deapprox(x):
@@ -49,40 +50,65 @@
 			""".split() if op]:
 			exec(f"def {__op__}(self, other): return approx(getattr(deapprox(self), '{__op__}')(deapprox(other)))")
 		def __str__(self): return '≈' + super().__str__()
 	return approx_T(x)
 
 class SortedDict(dict):
     
-    def __new__(cls, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         if len(args) > 0 and isinstance(args[0], dict):
-            return SortedDict.__new__dict(*args, **kwargs)
+            return self.__init__dict(*args, **kwargs)
         if len(args) > 1 and not isinstance(args[0], str):
-            return SortedDict.__new__keyvalue(*args, **kwargs)
-        return SortedDict.__new__default(*args, **kwargs)
+            return self.__init__keyvalue(*args, **kwargs)
+        return self.__init__default(*args, **kwargs)
 
-    @classmethod
-    def __new__keyvalue(cls, keys:list=[], values:list=[]):
-        self = super().__new__(cls, zip(keys, values))
+    def __init__keyvalue(self, keys:list=[], values:list=[]):
+        super().__init__(zip(keys, values))
         self.key_order = keys
-        return self
 
-    @classmethod
-    def __new__dict(cls, dic:dict, order=None):
-        self = super().__new__(cls, dic)
+    def __init__dict(self, dic:dict, order=None):
+        super().__init__(dic)
         if order is None: self.key_order = list(dic.keys())
         else: self.key_order = order
-        return self
 
-    @classmethod
-    def __new__default(cls, *args, **kwargs):
-        self = super().__new__(cls, kwargs)
+    def __init__default(self, *args, **kwargs):
+        super().__init__(kwargs)
         if len(args) == 0: self.key_order = list(kwargs.keys())
         else: self.key_order = list(arg_tuple(args))
-        return self
+    
+    # def __init__(self, *args, **kwargs): ...
+    
+    # def __new__(cls, *args, **kwargs):
+    #     if len(args) > 0 and isinstance(args[0], dict):
+    #         return SortedDict.__new__dict(*args, **kwargs)
+    #     if len(args) > 1 and not isinstance(args[0], str):
+    #         return SortedDict.__new__keyvalue(*args, **kwargs)
+    #     return SortedDict.__new__default(*args, **kwargs)
+
+    # @classmethod
+    # def __new__keyvalue(cls, keys:list=[], values:list=[]):
+    #     self = super().__new__(cls, zip(keys, values))
+    #     self.key_order = keys
+    #     return self
+
+    # @classmethod
+    # def __new__dict(cls, dic:dict, order=None):
+    #     self = super().__new__(cls, dic)
+    #     if order is None: self.key_order = list(dic.keys())
+    #     else: self.key_order = order
+    #     return self
+
+    # @classmethod
+    # def __new__default(cls, *args, **kwargs):
+    #     self = super().__new__(cls, kwargs)
+    #     if len(args) == 0: self.key_order = list(kwargs.keys())
+    #     else: self.key_order = list(arg_tuple(args))
+    #     return self
+    
+    # def __init__(self, *args, **kwargs): ...
 
     def sort(self): self.key_order.sort()
 
     def shuffle(self): random.shuffle(self.key_order)
         
     def first(self): return self.key_order[0], self[self.key_order[0]]
 
@@ -130,14 +156,20 @@
         if isinstance(k, slice):
             key_order = self.key_order[k]
             return SortedDict({i: self[i] for i in key_order}, key_order)
         return_value = super().get(k, None)
         if return_value is None and isinstance(k, int): return_value = self[self.get_key(k)]
         return return_value
     
+    def filter(self, new_key_list):
+        return SortedDict(
+            [k for k in new_key_list if k in self.key_order], 
+            [self[k] for k in new_key_list if k in self.key_order]
+        )
+    
 def is_subkey(key_sub, key_cons):
     for k, v in key_cons.items():
         if v == ...: continue
         if isinstance(v, (list, tuple)):
             cv = key.get(k, None)
             if cv in v: ...
             elif cv == v: ...
@@ -498,15 +530,15 @@
         slice_str = ''
         if self.i_slice is not None: slice_str = f" (slice {i_slice})"
         return f"<DataObject at {self.path.filename}{slice_str} [{load_state}]>"
     
     @property
     def data(self):
         if self._data is None: self.load()
-        return self.__getitem__() if self.i_slice is not None else self._data
+        return self.__getitem__(self.i_slice) if self.i_slice is not None else self._data
     
 class Slicer:
     
     def __init__(self, path, loader=None):
         self.data_obj = DataObject(path, loader=loader)
         self.valid_slices = None
         self.slice_pointer = 0
@@ -576,70 +608,71 @@
         elif isinstance(obj, list):
             self.valid_slices = obj
         elif callable(obj): self.valid_slices = obj
         else: raise TypeError(f"Unknown valid slice type {obj}. ")
         return self
 
 class Dataset:
+    """
+    Create a dataset object. 
     
-    def __init__(self, *args, name = None, main_key_name = 'subject_id', batch_pattern = 'unpaired'):
-        """
-        Create a dataset object. 
-        
-        Args:
-            paths (str): The main folders of the dataset. Dataset will browse all the files within. 
-            name (str): The name of the dataset, one can also identify it in the function name of the loading function. 
-            main_key_name (str): The main key defined to distinguish different subjects. Defaults to 'subject_id'. 
-            batch_pattern (str: unpaired/ paired/ random or list[Key]): Whether the images inside are paired. Defaults to 'unpaired'.
-                unpaired: Values with different Key should be taken as independent data. 
-                paired: Only values with different 'main_key' should be regarded as independent data, the input for batch function would be a tuple of such data. 
-                random: Values with different Key are regarded as independent data, but the input for batch function would randomly pick the data of the same non-main_key keys. 
-                list[Key]: A list of Key objects to constraint each element of the batch input. 
-                    unpaired <==> Key()
-                    paired   <==> e.g. [Key(subject_id=..., modality='CT', is_label=False), Key(subject_id=..., modality='T1', is_label=False), Key(subject_id=..., modality='T1', is_label=True)] # ... here is Ellipsis indicating the same subject_id
-                    random   <==> e.g. [Key(modality='CT', is_label=False), Key(modality='T1', is_label=False), Key(modality='T1', is_label=True)]
-            Note: the training/ validation/ test sub-datasets are split according to the 'main_key'.
-        
-        Examples::
-            >>> from micomputing import data
-            >>> @data.Dataset("folderpath1", "folderpath2")
-            ... def <datasetname>(path):
-            ...     '''
-            ...     The main function maps path to a Key-value pair
-            ...     Note that:
-            ...     1) A list should be returned if multiple elements are obtained from a single path, e.g.,
-            ...            return [Key(patient_id = path.split()[1], modality = path.name, slice_id = i), DataObject(path, i_slice=i) for i in range(n_slice)]
-            ...     2) A single pair of Key-value is also allowed. 
-            ...          The value should be replaced by a Slicer object for image slices, which can generate slice data after the image is loaded.
-            ...          In which case the Key object should leave out namescope 'slice_id' by a default value None to be filled afterwards, e.g., 
-            ...            return Key(patient_id = path.split()[1], modality = path.name, slice_id = None), Slicer(path)
-            ...     3) No identical keys are allowed. One needs to set another property even for elements from a single datum, e.g.,
-            ...            Key(..., slice_id = xx), DataObject(path) for '*.dcm' or '*.ima' slice files. 
-            ...     4) None should be returned if the path is to be omitted. 
-            ...     '''
-            ...     return Key(patientID = path.split()[1], modality = path.name), DataObject(path)
-            ... 
-            >>> <datasetname>
-            <datasetname> Dataset (121 images): 
-            ==================================================
-            patientID = 152
-            || modality = MR
-            || modality = CT
-            ...
-            patientID = 174
-            || modality = CT
-        """
+    Args:
+        paths (str): The main folders of the dataset. Dataset will browse all the files within. 
+        name (str): The name of the dataset, one can also identify it in the function name of the loading function. 
+        main_key_name (str): The main key defined to distinguish different subjects. Defaults to 'subject_id'. 
+        batch_pattern (str: unpaired/ paired/ random or list[Key]): Whether the images inside are paired. Defaults to 'unpaired'.
+            unpaired: Values with different Key should be taken as independent data. 
+            paired: Only values with different 'main_key' should be regarded as independent data, the input for batch function would be a tuple of such data. 
+            random: Values with different Key are regarded as independent data, but the input for batch function would randomly pick the data of the same non-main_key keys. 
+            list[Key]: A list of Key objects to constraint each element of the batch input. 
+                unpaired <==> Key()
+                paired   <==> e.g. [Key(subject_id=..., modality='CT', is_label=False), Key(subject_id=..., modality='T1', is_label=False), Key(subject_id=..., modality='T1', is_label=True)] # ... here is Ellipsis indicating the same subject_id
+                random   <==> e.g. [Key(modality='CT', is_label=False), Key(modality='T1', is_label=False), Key(modality='T1', is_label=True)]
+        Note: the training/ validation/ test sub-datasets are split according to the 'main_key'.
+    
+    Examples::
+        >>> from micomputing import data
+        >>> @data.Dataset("folderpath1", "folderpath2")
+        ... def <datasetname>(path):
+        ...     '''
+        ...     The main function maps path to a Key-value pair
+        ...     Note that:
+        ...     1) A list should be returned if multiple elements are obtained from a single path, e.g.,
+        ...            return [Key(patient_id = path.split()[1], modality = path.name, slice_id = i), DataObject(path, i_slice=i) for i in range(n_slice)]
+        ...     2) A single pair of Key-value is also allowed. 
+        ...          The value should be replaced by a Slicer object for image slices, which can generate slice data after the image is loaded.
+        ...          In which case the Key object should leave out namescope 'slice_id' by a default value None to be filled afterwards, e.g., 
+        ...            return Key(patient_id = path.split()[1], modality = path.name, slice_id = None), Slicer(path)
+        ...     3) No identical keys are allowed. One needs to set another property even for elements from a single datum, e.g.,
+        ...            Key(..., slice_id = xx), DataObject(path) for '*.dcm' or '*.ima' slice files. 
+        ...     4) None should be returned if the path is to be omitted. 
+        ...     '''
+        ...     return Key(patientID = path.split()[1], modality = path.name), DataObject(path)
+        ... 
+        >>> <datasetname>
+        <datasetname> Dataset (121 images): 
+        ==================================================
+        patientID = 152
+        || modality = MR
+        || modality = CT
+        ...
+        patientID = 174
+        || modality = CT
+    """
+    
+    def __init__(self, *args, name = None, main_key_name = 'subject_id', batch_pattern = 'unpaired', preprocess = None):
         self.n_slice_record = []
         self.use_slice_elements = False
         self.name = name
         self.main_key_name = main_key_name
         self.batch_pattern = batch_pattern
-        self.subject_index = {}
-        self.batch_index = {}
-        self._training_set = []
+        self.preprocess = preprocess
+        self.subject_index = {}    # {(main key)-key paired dict}
+        self.batch_index = {}      # {batch pattern (in Key): (main key)-(key candidates list) paired sorted dict}
+        self._training_set = []    # list of main keys
         self._validation_set = []
         self._testing_set = []
         if len(args) == 1:
             x = args[0]
             if isinstance(x, dict): self.__init__dict(*args)
             elif isinstance(x, str): self.__init__str(*args)
             else: self.__init__sequence(*args)
@@ -747,21 +780,22 @@
                 if paired: # if the element needs paired
                     candidates = [k for k in self.subject_index[sid] if is_subkey(k, bk(**{bk.main_key_name: sid}))]
                 else: # no paired element needed
                     candidates = [k for k in self.subject_index[sid] if is_subkey(k, bk)]
                 if len(candidates) > 0: self.batch_index[bk][sid] = candidates; continue # subimage found
                 elif paired: remove_list.append(sid) # paired images missing member
         if len(remove_list) == self.n_main_key or any(len(cand) == 0 for cand in self.batch_index.values()):
-            raise TypeError(f"Cannot find required image output following batch pattern {self.batch_pattern} for {self.name} dataset. ")
+            error_bps = [bp for bp, cand in self.batch_index.items() if len(cand) == 0]
+            raise TypeError(f"Cannot find required image output following batch pattern {error_bps} for {self.name} dataset. ")
         for sid in remove_list:
             for k in self.subject_index[sid]: self.data.pop(k, None) # remove from dataset
             for bk in self.batch_pattern: self.batch_index[bk].pop(sid, None) # remove from content index
 
         self.data.sort()
-        self.split_datasets(training=0.7, validation=0.2)
+        # self.split_datasets(training=0.7, validation=0.2, shuffle=shuffle)
     
     @property
     def main_keys(self):
         return list(set(k.main_key for k in self.data.keys()))
     
     @alias("n_subject")
     @property
@@ -797,15 +831,17 @@
                 count += 1
                 if count == 3: str_print('...')
                 if count > self.n_main_key - 2: count = 0
             if should_omit and count > 2: continue
             for i, k in enumerate(d.visible_keys()):
                 if i < first_diff: continue
                 if i < len(d) - 1: str_print(prefix(i), f"{k} = {d[k]}", sep=''); continue
-                skey = f"{k} = {d[k]}: "
+                used = ''
+                if not self.needed_in_batch(d): used = " [not used]"
+                skey = f"{k} = {d[k]}{used}: "
                 str_v = str(v).split('=' * 10)[-1].lstrip('=').strip()
                 str_print(prefix(i), skey, str_v.replace('\n', '\n' + prefix(i) + ' ' * len(skey)), sep='')
         return str_print.text
 
     def setdefault(self, k, v):
         if k not in self.data: self.data[k] = v
 
@@ -864,48 +900,58 @@
     def __getattr__(self, k):
         try: return getattr(super(), k, None)
         except KeyError as e: raise AttributeError(str(e))
 
     def __iter__(self):
         return iter(self.data)
 
-    def split_datasets(self, training = None, validation = None, testing = None):
+    def split_datasets(self, training = None, validation = None, testing = None, shuffle = True):
         """
         Split dataset to training, validation and test sets by ratio. e.g. split_dataset(training=0.8, validation = 0.1)
         """
         self.check_data()
         if validation is None and (training is None or testing is None): validation = 0.
         if testing is None and training is None: testing = 0.
         if training is None: training = 1. - validation - testing
         elif validation is None: validation = 1. - testing - training
         elif testing is None: testing = 1. - training - validation
         avouch(abs(training + testing + validation - 1.) < 1e-3, "Invalid ratios for function 'split_datasets' (Sum is not 1). ")
         main_keys = self.main_keys
         n_train = int(training * len(main_keys))
         n_valid = int(validation * len(main_keys))
-        random.shuffle(main_keys)
-        def add_subimage(main_key_set):
-            return sum((self.subject_index[mk] for mk in main_key_set), [])
-        self._training_set = add_subimage(main_keys[:n_train])
-        self._validation_set = add_subimage(main_keys[n_train:n_train + n_valid])
-        self._testing_set = add_subimage(main_keys[n_train + n_valid:])
+        if shuffle: random.shuffle(main_keys)
+        self._training_set = main_keys[:n_train]
+        self._validation_set = main_keys[n_train:n_train + n_valid]
+        self._testing_set = main_keys[n_train + n_valid:]
+        # def add_subimage(main_key_set):
+        #     return sum((self.subject_index[mk] for mk in main_key_set), [])
+        # self._training_set = add_subimage(main_keys[:n_train])
+        # self._validation_set = add_subimage(main_keys[n_train:n_train + n_valid])
+        # self._testing_set = add_subimage(main_keys[n_train + n_valid:])
         return self
     
     def needed_in_batch(self, key, batch_pattern=None):
         if batch_pattern is None: batch_pattern = self.batch_pattern
         for const in batch_pattern:
             if is_subkey(key, const): return True
         return False
     
     @property
-    def n_training_subject(self): return len(list(set(k.main_key for k in self._training_set))) if self._training_set else None
+    def n_training_subject(self): return len(self._training_set) if self._training_set else None
     @property
-    def n_validation_subject(self): return len(list(set(k.main_key for k in self._validation_set))) if self._validation_set else None
+    def n_validation_subject(self): return len(self._validation_set) if self._validation_set else None
     @property
-    def n_testing_subject(self): return len(list(set(k.main_key for k in self._testing_set))) if self._testing_set else None
+    def n_testing_subject(self): return len(self._testing_set) if self._testing_set else None
+    
+    # @property
+    # def n_training_subject(self): return len(list(set(k.main_key for k in self._training_set))) if self._training_set else None
+    # @property
+    # def n_validation_subject(self): return len(list(set(k.main_key for k in self._validation_set))) if self._validation_set else None
+    # @property
+    # def n_testing_subject(self): return len(list(set(k.main_key for k in self._testing_set))) if self._testing_set else None
     
     @property
     def n_data(self):
         if self.data is None: return
         total_item = 0
         for key in self.data:
             if not self.needed_in_batch(key): continue
@@ -915,52 +961,71 @@
             else: total_item += 1
         return total_item
     @property
     def n_training(self):
         if not self._training_set: return
         total_item = 0
         for key in self.data:
-            if key not in self._training_set: continue
+            if key.main_key not in self._training_set: continue
             if not self.needed_in_batch(key): continue
             if self.use_slice_elements: 
                 if not self.data[key].is_loaded: total_item = total_item + self.estimated_n_slice
                 else: total_item += self.data[key].n_slice
             else: total_item += 1
         return total_item
     @property
     def n_validation(self):
         if not self._validation_set: return
         total_item = 0
         for key in self.data:
-            if key not in self._validation_set: continue
+            if key.main_key not in self._validation_set: continue
             if not self.needed_in_batch(key): continue
             if self.use_slice_elements: 
                 if not self.data[key].is_loaded: total_item = total_item + self.estimated_n_slice
                 else: total_item += self.data[key].n_slice
             else: total_item += 1
         return total_item
     @property
     def n_testing(self):
         if not self._testing_set: return
         total_item = 0
         for key in self.data:
-            if key not in self._testing_set: continue
+            if key.main_key not in self._testing_set: continue
             if not self.needed_in_batch(key): continue
             if self.use_slice_elements: 
                 if not self.data[key].is_loaded: total_item = total_item + self.estimated_n_slice
                 else: total_item += self.data[key].n_slice
             else: total_item += 1
         return total_item
 
     @alias("train_batch")
     def training_batch(self, n, **kwargs): return self.batch('training', n, **kwargs)
     @alias("valid_batch")
     def validation_batch(self, n, **kwargs): return self.batch('validation', n, **kwargs)
     @alias("test_batch")
     def testing_batch(self, n, **kwargs): return self.batch('testing', n, **kwargs)
+
+    @alias("train_batch")
+    def training_batches(self, n, **kwargs):
+        while True:
+            cur_batch = self.batch('training', n, **kwargs)
+            if cur_batch is None: break
+            yield cur_batch
+    @alias("valid_batch")
+    def validation_batches(self, n, **kwargs):
+        while True:
+            cur_batch = self.batch('validation', n, **kwargs)
+            if cur_batch is None: break
+            yield cur_batch
+    @alias("test_batch")
+    def testing_batches(self, n, **kwargs):
+        while True:
+            cur_batch = self.batch('testing', n, **kwargs)
+            if cur_batch is None: break
+            yield cur_batch
     
     def batch(self, stage='training', n_batch=4, shuffle=True, drop_last=True, none_each_epoch=True, restart=False):
         """
         Create a batch data. 
 
         Args:
             stage (str, 'training'|'validation'|'testing'): The stage we are in, determining the subset we are using. Defaults to 'training'.
@@ -972,33 +1037,33 @@
                 Whether to drop the last data which is less than a batch. Defaults to True.
                 [True]: Drop the remaining data.
                 [False]: Use the remaining data to create a batch with a batch size smaller than normal ones. 
             none_each_epoch (bool): Whether to output a None value at the end of each epoch. Defaults to True.
             restart (bool): Manually use a restart of epoch for this batch. Defaults to False.
         """
         self.check_data()
-        if not self._training_set: self.split_datasets(training=0.7, validation=0.2)
+        if not self._training_set: self.split_datasets(training=0.7, validation=0.2, shuffle=shuffle)
         stage = stage.lower()
         if stage == 'training': subset = self._training_set
         elif stage == 'validation': subset = self._validation_set
         elif stage == 'testing': subset = self._testing_set
         
         selected_items = []
         batch_list = []
         new_epoch = False
         release_list = []
         for bp in self.batch_pattern:
-            candidates = self.batch_index[bp]
+            candidates = self.batch_index[bp].filter(subset)
             cur_pointer = 0 if restart else self.batch_pointer[stage].get(bp, 0)
             if cur_pointer == 0 and self.use_slice_elements: cur_pointer = 0, 0
             batch_sids = []
             if bp.main_key == ... and selected_items:
                 if self.use_slice_elements:
-                    batch_list.append([self.data[random.choice(candidates[img.main_key])].slice(slc) for img, slc in selected_items])
-                else: batch_list.append([self.data[random.choice(candidates[img.main_key])] for img in selected_items])
+                    batch_list.append([self.data[random.choice(candidates[img_key])].slice(slc) for img_key, slc in selected_items])
+                else: batch_list.append([self.data[random.choice(candidates[img_key])] for img_key in selected_items])
             else:
                 cum_n_batch = 0
                 if self.use_slice_elements:
                     cur_pointer, slice_pointer = cur_pointer
                     batched_slices = []
                     for i in range(n_batch):
                         image_key = random.choice(candidates[cur_pointer])
@@ -1008,31 +1073,29 @@
                         n_remain_batch = n_batch - len(batched_slices)
                         new_slice_pointer = slice_pointer + n_remain_batch
                         selected_items.extend([(image_key, i) for i in range(slice_pointer, min(new_slice_pointer, sample_image.n_slice))])
                         batched_slices.extend([sample_image.slice(i) for i in range(slice_pointer, min(new_slice_pointer, sample_image.n_slice))])
                         if new_slice_pointer >= sample_image.n_slice: new_slice_pointer = 0; cur_pointer += 1; release_list.append(sample_image)
                         if len(batched_slices) >= n_batch: break
                     batch_list.append(batched_slices)
-                    if cur_pointer >= len(candidates): cur_pointer = 0; new_slice_pointer = 0; new_epoch = True
+                    if len(selected_items) == 0: cur_pointer = 0; new_slice_pointer = 0; new_epoch = True; break
                     self.batch_pointer[stage][bp] = cur_pointer, new_slice_pointer
                 else: 
                     new_pointer = cur_pointer + n_batch
-                    selected_items = random.choice(candidates[cur_pointer: new_pointer])
-                    batch_list.append([self.data[cand] for cand in selected_items])
-                    if new_pointer >= len(candidates): new_pointer = 0; new_epoch = True
+                    selected_items = candidates[cur_pointer: new_pointer]
+                    if len(selected_items) == 0: new_pointer = 0; new_epoch = True; break
+                    batch_list.append([self.data[random.choice(candidates[img_key])] for img_key in selected_items])
                     self.batch_pointer[stage][bp] = new_pointer
 
         is_partial_batch = any(len(x) < n_batch for x in batch_list)
-        if is_partial_batch: new_epoch = True
+        if is_partial_batch and drop_last: new_epoch = True
         if new_epoch: 
             self.batch_pointer = {'training': {}, 'validation': {}, 'testing': {}}
             if shuffle:
                 for bp in self.batch_pattern: self.batch_index[bp].shuffle()
-
-        if is_partial_batch and drop_last:
             for r in release_list: r.release()
             if none_each_epoch: return
             else: return self.batch(stage=stage, n_batch=n_batch, shuffle=shuffle, 
                                     drop_last=drop_last, none_each_epoch=none_each_epoch, restart=restart)
         return_value = self.get_batch(batch_list)
         for r in release_list: r.release()
         return return_value
@@ -1045,22 +1108,37 @@
             batch_list (list): a list of length equal to *.batch_pattern; with each element a list of length n_batch. 
                 The nested elements are DataObjects (Slicer output in major function would result in DataObjects with i_slice). 
         """
         res_list = []
         for output_batch in batch_list:
             ref = output_batch[0]
             if isinstance(ref, DataObject):
-                output_batch = [x.data for x in output_batch]
+                if self.preprocess is None: prepcs = lambda x: x
+                else: prepcs = self.preprocess
+                output_batch = [prepcs(x.data) for x in output_batch]
                 ref = ref.data
             elif isinstance(ref, bt.Tensor): ...
             else: res_list.append(output_batch); continue
             avouch(isinstance(ref, bt.Tensor))
             if ref.has_batch: res_list.append(bt.cat(output_batch, {}, crop=True).detach())
             else: res_list.append(bt.stack(output_batch, {}, crop=True).detach())
         return tuple(res_list)
+    
+class LossCollector:
+    
+    def __init__(self):
+        self.collection = {}
+    
+    def __call__(self, **kwargs):
+        for k, v in kwargs.items():
+            self.collection.setdefault(k, bt.zeros(0))
+            self.collection[k] = bt.cat(self.collection[k], bt.to_bttensor(v, device=self.collection[k].device))
+            
+    def __str__(self):
+        return ', '.join([f"{k} [{v.mean_std}]" for k, v in self.collection.items()])
 
 # class MedicalSubImage(Dataset):
     
 #     def __getitem__(self, k):
 #         try:
 #             if isinstance(k, Subject): return self.data[k.subimage]
 #         except KeyError: raise KeyError(f"Invalid key {k}.")
```

### Comparing `micomputing-1.1.47/micomputing/funcs.py` & `micomputing-1.1.48/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/metrics.py` & `micomputing-1.1.48/micomputing/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             if Version(bt.__version__) >= '1.9': window = bt.stack(bt.meshgrid(*([bt.arange(-1, 3)] * n_image), indexing='ij'), 0).flatten(1).transpose(0, 1).to(device) # (4 ^ n_image, n_image)
             else: window = bt.stack(bt.meshgrid(*([bt.arange(-1, 3)] * n_image), indexing='ij'), 0).flatten(1).transpose(0, 1).to(device) # (4 ^ n_image, n_image)
             for shift in window:
                 shift = shift.view({1}, [2], 1) # ({1}, [n_image], 1) -> (1, n_image, 1)
                 hist_pos = data_pair * n_bin # ({n_batch}, [n_image], n_data) -> (n_batch, n_image, n_data)
                 index = bt.clamp(bt.floor(hist_pos).long() + shift.long(), 0, n_bin - 1)
                 decimal = hist_pos - bt.floor(hist_pos)
-                value = grad_output[(bt.arange(n_batch).long().unsqueeze(-1).expand(n_batch, n_data).to(device),) + tuple(x.squeeze(1) for x in index.split(1, 1))] # ({n_batch}, n_data) -> (n_batch, n_data)
+                value = grad_output[(bt.arange({n_batch}).long().duplicate(n_data, -1).to(device),) + tuple(x.squeeze(1) for x in index.split(1, 1))] # ({n_batch}, n_data) -> (n_batch, n_data)
                 dEdI1 += value * multi_dBspline(shift, decimal, 0) # ({n_batch}, n_data) -> (n_batch, n_data)
                 dEdI2 += value * multi_dBspline(shift, decimal, 1)
             # dEdI1 = bt.tensor(dEdI1.data).view(Ishape) * n_bin / n_data
             # dEdI2 = bt.tensor(dEdI2.data).view(Ishape) * n_bin / n_data
             n_dim = len(Ishape) - 1
             dEdI1 = dEdI1.data.view(Ishape) * mask * n_bin / mask.flatten(1).sum(1).view((n_batch,) + (1,) * n_dim)
             dEdI2 = dEdI2.data.view(Ishape) * mask * n_bin / mask.flatten(1).sum(1).view((n_batch,) + (1,) * n_dim)
@@ -604,16 +604,16 @@
     The metrics between A and B where A and B are 0-1 masks. 
     The sizes are as follows: 
     A: ({n_batch}, [n_label: optional], n@1, n@2, ..., n@n_dim)
     B: ({n_batch}, [n_label: optional], n@1, n@2, ..., n@n_dim)
     return: ({n_batch}, [n_label: optional])
     '''
     func = 'Metric ' + metric
-    avouch(isinstance(A, bt.Tensor), f"Please use 'babt.Tensor' objects for '{func}' in 'micomputing'. Use X.as_subclass(bt.Tensor) to create one. ")
-    avouch(isinstance(B, bt.Tensor), f"Please use 'babt.Tensor' objects for '{func}' in 'micomputing'. Use X.as_subclass(bt.Tensor) to create one. ")
+    avouch(isinstance(A, bt.Tensor), f"Please use 'bt.Tensor' objects for '{func}' in 'micomputing'. Use X.as_subclass(bt.Tensor) to create one. ")
+    avouch(isinstance(B, bt.Tensor), f"Please use 'bt.Tensor' objects for '{func}' in 'micomputing'. Use X.as_subclass(bt.Tensor) to create one. ")
     avouch(A.has_batch and B.has_batch, f"Please make sure inputs of '{func}' have batch dimensions. Use X.batch_dim = 0 to identify (or X.unsqueeze({{}}) if no existed batch).")
     avouch(A.shape == B.shape, f"Please make sure inputs of '{func}' have the same shape.")
 
     n_batch = A.n_batch
     has_channel = False
     if A.has_channel and B.has_channel:
         has_channel = True
@@ -622,16 +622,16 @@
         B = B.mergedims([], {})
     n_maps = A.n_batch
     filter_A = A.sum(...) != 0
     filter_B = B.sum(...) != 0
     filter_both = filter_A & filter_B
     A = A[filter_both]
     B = B[filter_both]
-    A = np.array(A) != 0
-    B = np.array(B) != 0
+    A = A.numpy() != 0
+    B = B.numpy() != 0
     spacing = to_tuple(spacing)
     n_dim = A.ndim
     n_data = A.shape[0]
     if len(spacing) == 1: spacing *= n_dim
     Overlap_filter = sitk.LabelOverlapMeasuresImageFilter()
     SD_filter = SurfaceDistanceImageFilter()
     Overlap_execs = {
```

### Comparing `micomputing-1.1.47/micomputing/micfunctions.so` & `micomputing-1.1.48/micomputing/micfunctions.so`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/network.py` & `micomputing-1.1.48/micomputing/network.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     requires = "batorch"
 ).check()
 
 __all__ = """
     U_Net
     CNN
     FCN
+    NeuralODE
 """.split()
     
 import math
 
 with __info__:
     import batorch as bt
     from batorch import nn
@@ -34,38 +35,44 @@
         z = reduction(list_of_items[0], list_of_items[1])
         for i in range(2, len(list_of_items)):
             z = reduction(z, list_of_items[i])
     else: z = list_of_items[0]
     return z
 
 class Convolution_Block(nn.Module):
+    '''
+    Args:
+        dimension (int): The dimension of the images. 
+        in_channels (int): The input channels for the block. 
+        out_channels (int): The output channels for the block. 
+        conv_num (int): The number of convolution layers. 
+        kernel_size (int): The size of the convolution kernels. 
+        padding (int): The image padding for the convolutions. 
+        activation_function (class): The activation function. 
+        final_activation (class): The activation function after the final convolution. 
+        active_args (dict): The arguments for the activation function. 
+        conv_block (str): A string with possible values in ('conv', 'dense', 'residual'), indicating which kind of block the U-Net is using: normal convolution layers, DenseBlock or ResidualBlock. 
+        res_type (function): The combining type for the residual connections.
+    '''
     
     def __init__(self, in_channels, out_channels, **params):
-        '''
-        ::parameters:
-            dimension (int): The dimension of the images. 
-            in_channels (int): The input channels for the block. 
-            out_channels (int): The output channels for the block. 
-            conv_num (int): The number of convolution layers. 
-            kernel_size (int): The size of the convolution kernels. 
-            padding (int): The image padding for the convolutions. 
-            activation_function (class): The activation function. 
-            active_args (dict): The arguments for the activation function. 
-            conv_block (str): A string with possible values in ('conv', 'dense', 'residual'), indicating which kind of block the U-Net is using: normal convolution layers, DenseBlock or ResidualBlock. 
-            res_type (function): The combining type for the residual connections.
-        '''
         super().__init__()
-        default_values = {'dimension': 2, 'conv_num': 1, 'padding': 1, 'kernel_size': 3, 'conv_block': 'conv', 'res_type': bt.add, 'activation_function': nn.ReLU, 'active_args': {}}
+        default_values = {'dimension': 2, 'conv_num': 1, 'padding': 1, 'kernel_size': 3, 'conv_block': 'conv', 'res_type': bt.add, 'activation_function': nn.ReLU, 'final_activation': ..., 'active_args': {}}
         param_values = {}
         param_values.update(default_values)
         param_values.update(params)
         self.__dict__.update(param_values)
         self.in_channels = in_channels
         self.out_channels = out_channels
         
+        if isinstance(self.padding, str): self.padding = {'SAME': self.kernel_size // 2, 'ZERO': 0, 'VALID': 0}.get(self.padding.upper(), self.kernel_size // 2)
+        if self.activation_function is None: self.activation_function = lambda *a, **k: (lambda x: x)
+        if self.final_activation == ...: self.final_activation = self.activation_function
+        if self.final_activation is None: self.final_activation = lambda *a, **k: (lambda x: x)
+        
         self.layers = nn.ModuleList()
         for i in range(self.conv_num):
             ic = self.in_channels if i == 0 else ((self.out_channels * i + self.in_channels) if self.conv_block == 'dense' else self.out_channels)
             conv = eval('nn.Conv%dd' % self.dimension)(ic, self.out_channels, self.kernel_size, 1, self.padding)
             initialize_model, initialize_params = parse(self.initializer)
             eval('nn.init.%s_' % initialize_model)(conv.weight, *initialize_params)
             if self.conv_block != 'dense': self.layers.append(conv)
@@ -75,46 +82,57 @@
             if self.conv_block == 'dense': self.layers.append(conv)
 
     def forward(self, x):
         if self.conv_block == 'dense':
             conv_results = [x]
             conv_layer = True
             for layer in self.layers:
-                if conv_layer: x = layer(bt.cat([bt.crop_as(l, conv_results[-1]) for l in conv_results], 1))
-                else: x = layer(x)
+                try:
+                    if conv_layer: x = layer(bt.cat([bt.crop_as(l, conv_results[-1]) for l in conv_results], 1))
+                    else: x = layer(x)
+                except Exception as e:
+                    raise e.__class__(f"In layer {layer}. " + e.__str__())
                 conv_layer = layer.__class__.__name__.startswith('Conv')
                 if conv_layer: conv_results.append(x)
-            return self.activation_function(**self.active_args)(x)
+            result = self.final_activation(**self.active_args)(x)
         else:
             y = x
-            for layer in self.layers: y = layer(y)
+            for layer in self.layers:
+                try: y = layer(y)
+                except Exception as e:
+                    raise e.__class__(f"In layer {layer}. " + e.__str__())
+            y = y.as_subclass(bt.Tensor).special_from(x)
             if self.conv_block == 'residual': z = self.res_type(bt.crop_as(x, y), y)
             else: z = y
-            return self.activation_function(**self.active_args)(z)
-        
+            result = self.final_activation(**self.active_args)(z)
+        result = result.as_subclass(bt.Tensor).special_from(x)
+        if self.padding == self.kernel_size // 2:
+            return bt.crop_as(result, x)
+        return result
 
 class U_Net(nn.Module):
     '''
-    ::paramerters:
-        dimension (int): The dimension of the images. For conventional U-Net, it is 2. 
-        depth (int): The depth of the U-Net. The conventional U-Net has a depth of 4 there are 4 pooling layers and 4 up-sampling layers.
-        conv_num (int): The number of continuous convolutions in one block. In a conventional U-Net, this is 2. 
-        padding (int or str): Indicate the type of padding used. In a conventional U-Net, padding should be 0 but yet the default value is 'SAME' here. 
-        in_channels (int): The number of channels for the input. In a conventional U-Net, it should be 1.
-        out_channels (int): The number of channels for the output. In a conventional U-Net, it should be 2.
-        block_channels (int): The number of channels for the first block if a number is provided. In a conventional U-Net, it should be 64. 
+    Args:
+        dimension (int): The dimension of the images. Defaults to 2 (see U-Net). 
+        depth (int): The depth of the U-Net. Defaults to 4 indicating 4 pooling layers and 4 up-sampling layers (see U-Net).
+        conv_num (int): The number of continuous convolutions in one block. Defaults to 2. 
+        padding (int or str): Indicate the type of padding used. Defaults to 'SAME' though it is 0 in conventional U-Net. 
+        in_channels (int): The number of channels for the input. Defaults to 1 (see U-Net).
+        out_channels (int): The number of channels for the output. Defaults to 2 (see U-Net).
+        block_channels (int): The number of channels for the first block if a number is provided. Defaults to 64 (see U-Net). 
             If a list is provided, the length should be the same as the number of blocks plus two (2 * depth + 3). It represents the channels before and after each block (with the output channels included). 
             Or else, a function may be provided to compute the output channels given the block index (-1 ~ 2 * depth + 1) [including input_channels at -1 and output_channels at 2 * depth + 1]. 
-        kernel_size (int): The size of the convolution kernels. In a conventional U-Net, it should be 3. 
-        pooling_size (int): The size of the pooling kernels. In a conventional U-Net, it should be 2. 
+        bottleneck_out_channels (int): The number of channels for the bottleneck output. Defaults to 0. 
+        kernel_size (int): The size of the convolution kernels. Defaults to 3 (see U-Net). 
+        pooling_size (int): The size of the pooling kernels. Defaults to 2 (see U-Net). 
         // keep_prob (float): The keep probability for the dropout layers. 
         conv_block (str): A string with possible values in ('conv', 'dense', 'residual'), indicating which kind of block the U-Net is using: normal convolution layers, DenseBlock or ResidualBlock. 
         multi_arms (str): A string with possible values in ('shared(2)', 'seperate(2)'), indicating which kind of encoder arms are used. 
         multi_arms_combine (function): The combining type for multi-arms. See skip_type for details. 
-        skip_type (function): The skip type for the skip connections. The conventional U-Net has a skip connect of catenation (cat). Other possible skip types include torch.mul or torch.add. 
+        skip_type (function): The skip type for the skip connections. Defaults to catenation (cat; see U-Net). Other possible skip types include torch.mul or torch.add. 
         res_type (function): The combining type for the residual connections. It should be torch.add in most occasions. 
         activation_function (class): The activation function used after the convolution layers. Defaults to nn.ReLU. 
         active_args (dict): The arguments for the activation function. Defaults to {}. 
         initializer (str): A string indicating the initialing strategy. Possible values are normal(0, 0.1) or uniform(-0.1, 0.1) or constant(0) (all parameters can be changed)
         with_softmax (bool): Whether a softmax layer is applied at the end of the network. Defaults to True. 
         cum_layers (list): A list consisting two numbers [n, m] indicating that the result would be a summation of the upsamples of the results of the nth to the mth (included) blocks, block_numbers are in range 0 ~ 2 * depth. 
             The negative indices are allowed to indicate the blocks in a inversed order with -1 representing the output for the last block. 
@@ -134,15 +152,14 @@
             self.conv_block = Convolution_Block(**block_params)
 
         def forward(self, x):
             if self.has_pooling: y = self.pooling(x)
             else: y = x
             return self.conv_block(y)
             
-            
     class Decoder_Block(nn.Module):
         
         def __init__(self, list_of_encoders, in_channels, out_channels, params, copies_of_inputs):
             super().__init__()
             block_params = params.copy()
             block_params.update({'in_channels': in_channels, 'out_channels': out_channels})
             self.__dict__.update(block_params)
@@ -159,15 +176,15 @@
             else: to_combine = [bt.crop_as(encoder_result, y) for encoder_result in list_of_encoder_results] + [y]
             joint = combine(to_combine, self.skip_type)
             return self.conv_block(joint)
 
 
     def __init__(self, **params):
         super().__init__()
-        default_values = {'dimension': 2, 'depth': 4, 'conv_num': 2, 'padding': 'SAME', 'in_channels': 1, 'out_channels': 2, 'block_channels': 64, 'kernel_size': 3, 'pooling_size': 2, 'keep_prob': 0.5, 'conv_block': 'conv', 'multi_arms': "shared", 'multi_arms_combine': cat, 'skip_type': cat, 'res_type': bt.add, 'activation_function': nn.ReLU, 'active_args': {}, 'initializer': "normal(0, 0.1)", 'with_softmax': True, 'cum_layers': -1}
+        default_values = {'dimension': 2, 'depth': 4, 'conv_num': 2, 'padding': 'SAME', 'in_channels': 1, 'out_channels': 2, 'block_channels': 64, 'kernel_size': 3, 'pooling_size': 2, 'keep_prob': 0.5, 'conv_block': 'conv', 'multi_arms': "shared", 'multi_arms_combine': cat, 'skip_type': cat, 'res_type': bt.add, 'activation_function': nn.ReLU, 'active_args': {}, 'initializer': "normal(0, 0.1)", 'with_softmax': True, 'cum_layers': -1, 'bottleneck_out_channels': 0}
         param_values = {}
         param_values.update(default_values)
         param_values.update(params)
         self.__dict__.update(param_values)
         
         if isinstance(self.block_channels, int):
             self.block_channels = [self.in_channels] + [self.block_channels << min(i, 2 * self.depth - i) for i in range(2 * self.depth + 1)] + [self.out_channels]
@@ -189,14 +206,18 @@
         self.arm_num = 1 if len(self.arm_num) == 0 else self.arm_num[0]
         if self.arm_type == 'shared': self.dif_arm_num = 1
         else: self.dif_arm_num = self.arm_num
         
         for iarm in range(self.dif_arm_num):
             for k in range(self.depth + 1):
                 setattr(self, 'block%d_%d' % (k, iarm), self.Encoder_Block(self.block_channels(k - 1), self.block_channels(k), k != 0, param_values))
+        
+        if self.bottleneck_out_channels > 0:
+            param_values = {k: v for k, v in param_values.items() if k not in ('in_channels', 'out_channels')}
+            setattr(self, 'bottleneck_out', Convolution_Block(self.block_channels(self.depth) * self.arm_num, self.bottleneck_out_channels, **param_values))
 
         for k in range(self.cum_layers[0], self.depth + 1):
             conv = eval('nn.Conv%dd' % self.dimension)(self.block_channels(k), self.block_channels(2 * self.depth + 1), 1, 1, 0)
             initialize_model, initialize_params = parse(self.initializer)
             eval('nn.init.%s_' % initialize_model)(conv.weight, *initialize_params)
             if k < self.cum_layers[1]:
                 setattr(self, 'block%dout' % k, nn.Sequential(conv, self.activation_function(**self.active_args)))
@@ -219,14 +240,22 @@
                 setattr(self, 'out%dupsample' % k, eval('nn.ConvTranspose%dd' % self.dimension)(
                     self.block_channels(2 * self.depth + 1), self.block_channels(2 * self.depth + 1), self.pooling_size, self.pooling_size, 0
                 ))
             else: setattr(self, 'block%dout' % k, conv)
 
         if self.with_softmax: self.softmax = self.Softmax()
         self.to(bt.get_device().main_device)
+        
+    @property
+    def bottleneck(self):
+        if self.bottleneck_out_channels > 0:
+            result = getattr(self, f'block{self.depth}result', None)
+            if result is None: return
+            return self.bottleneck_out(result).mean(...)
+        else: return
 
     def forward(self, x):
         size = x.size()[1:]
         if len(size) == self.dimension and self.in_channels == 1: x = x.unsqueeze(1)
         elif len(size) == self.dimension + 1 and self.in_channels * self.arm_num == size[0]: pass
         else: raise ValueError(f"The input tensor does not correspond to the U-Net structure: got {size}, but requires ([{self.in_channels * self.arm_num}], n_1, ⋯, n_{self.dimension}). ")
         
@@ -271,50 +300,50 @@
         for i in range(2 * self.depth + 1):
             if i <= self.depth:
                 for iarm in range(self.arm_num):
                     yield 'block%d_%dresult' % (i, iarm), (i, iarm)
             else: yield 'block%dresult' % i, i
 
 class CNN(U_Net):
+    '''
+    Args:
+        dimension (int): The dimension of the images. Defaults to 2 (see VGG). 
+        blocks (int): The number of the downsampling blocks. Defaults to 5 blocks (see VGG).
+        conv_num (int or list of length 'blocks'): The number of continuous convolutions in one block. Defaults to [2, 2, 3, 3, 3] (see VGG).
+            If the numbers for all blocks are the same, one can use one integer.
+        padding (int or str): Indicate the type of padding used. Defaults to 'SAME' indicating a same output shape as the input. 
+        in_channels (int): The number of channels for the input. Defaults to 1 (see VGG).
+        out_elements (int): The number of channels for the output, as the number of classification. Defaults to 1000 for 1000 classes.
+        layer_channels (int or list of length 'blocks'): The number of channels for each block. Defaults to [64, 128, 256, 512, 512] (see VGG). 
+            Or else, a function may be provided to compute the output channels given the block index (-1 ~ 2 * depth + 1). 
+        kernel_size (int): The size of the convolution kernels. Defaults to 3 (see VGG). 
+        pooling_size (int): The size of the pooling kernels. Defaults to 2 (see VGG). 
+        // keep_prob (float): The keep probability for the dropout layers. 
+        conv_block (str): A string with possible values in ('conv', 'dense', 'residual'), indicating which kind of block the U-Net is using: normal convolution layers, DenseBlock or ResidualBlock. 
+        multi_arms (str): A string with possible values in ('shared(2)', 'seperate(2)'), indicating which kind of encoder arms are used. 
+        multi_arms_combine (function): The combining type for multi-arms. Defaults to catenation (cat). Other possible skip types include torch.mul or torch.add. 
+        res_type (function): The combining type for the residual connections. It should be torch.add in most occasions. 
+        activation_function (class): The activation function used after the convolution layers. Defaults to nn.ReLU. 
+        active_args (dict): The arguments for the activation function. Defaults to {}. 
+        initializer (str): A string indicating the initialing strategy. Possible values are normal(0, 0.1) or uniform(-0.1, 0.1) or constant(0) (all parameters can be changed)
+        with_softmax (bool): Whether a softmax layer is applied at the end of the network. Defaults to True. 
+    '''
+    
     def __init__(self, dimension = 2, blocks = 5, conv_num = 2, padding = 'SAME', 
         in_channels = 1, out_elements = 2, layer_channels = 64, kernel_size = 3, 
         pooling_size = 2, keep_prob = 0.5, conv_block = 'conv', multi_arms = "shared", 
         multi_arms_combine = cat, res_type = bt.add, activation_function = nn.ReLU,
         active_args = {}, initializer = "normal(0, 0.1)", with_softmax = True):
-        '''
-        ::paramerters:
-            dimension (int): The dimension of the images. For conventional VGG, it is 2. 
-            blocks (int): The number of the downsampling blocks. The conventional VGG has 5 blocks.
-            conv_num (int or list of length 'blocks'): The number of continuous convolutions in one block. In VGG, this is [2, 2, 3, 3, 3]. If the numbers for all blocks are the same, one can use one integer.
-            padding (int or str): Indicate the type of padding used. In a conventional VGG, padding is 'SAME' indicating . 
-            in_channels (int): The number of channels for the input. In a conventional VGG, it should be 1.
-            out_elements (int): The number of channels for the output, as the number of classification. In a conventional VGG, it should be 1000 for 1000 classes.
-            layer_channels (int or list of length 'blocks'): The number of channels for each block. In a VGG, it should be [64, 128, 256, 512, 512]. 
-                Or else, a function may be provided to compute the output channels given the block index (-1 ~ 2 * depth + 1). 
-            kernel_size (int): The size of the convolution kernels. In a conventional U-Net, it should be 3. 
-            pooling_size (int): The size of the pooling kernels. In a conventional U-Net, it should be 2. 
-            // keep_prob (float): The keep probability for the dropout layers. 
-            conv_block (str): A string with possible values in ('conv', 'dense', 'residual'), indicating which kind of block the U-Net is using: normal convolution layers, DenseBlock or ResidualBlock. 
-            multi_arms (str): A string with possible values in ('shared(2)', 'seperate(2)'), indicating which kind of encoder arms are used. 
-            multi_arms_combine (function): The combining type for multi-arms. See skip_type for details. 
-            skip_type (function): The skip type for the skip connections. The conventional U-Net has a skip connect of catenation (cat). Other possible skip types include torch.mul or torch.add. 
-            res_type (function): The combining type for the residual connections. It should be torch.add in most occasions. 
-            activation_function (class): The activation function used after the convolution layers. Defaults to nn.ReLU. 
-            active_args (dict): The arguments for the activation function. Defaults to {}. 
-            initializer (str): A string indicating the initialing strategy. Possible values are normal(0, 0.1) or uniform(-0.1, 0.1) or constant(0) (all parameters can be changed)
-            with_softmax (bool): Whether a softmax layer is applied at the end of the network. Defaults to True. 
-            cum_layers (list): A list consisting two numbers [n, m] indicating that the result would be a summation of the upsamples of the results of the nth to the mth (included) blocks, block_numbers are in range 0 ~ 2 * depth. The negative indices are allowed to indicate the blocks in a inversed order with -1 representing the output for the last block. 
-        '''
         depth = blocks - 1
         if isinstance(layer_channels, int):
             maxlc = layer_channels
             layer_channels = [in_channels]
-            multiplier = int(math.pow(maxlc / in_channels, 1 / (depth + 1)))
+            multiplier = math.pow(maxlc / in_channels, 1 / (depth + 1))
             for i in range(depth):
-                layer_channels.append(layer_channels[-1] * multiplier)
+                layer_channels.append(int(layer_channels[-1] * multiplier))
             layer_channels.append(maxlc)
             layer_channels.extend([0] * depth)
             layer_channels.append(out_elements)
         super().__init__(dimension = dimension, depth = depth, conv_num = conv_num, 
             padding = padding, in_channels = in_channels, out_channels = out_elements, 
             block_channels = layer_channels, kernel_size = kernel_size, 
             pooling_size = pooling_size, keep_prob = keep_prob, conv_block = conv_block,
@@ -327,26 +356,44 @@
         self.with_softmax = False
         if wsm: r = self.softmax(super().forward(x).flatten(2).mean(-1))
         else: r = super().forward(x).flatten(2).mean(-1)
         self.with_softmax = wsm
         return r
         
 class FCN(nn.Module):
+    '''
+    Fully connected network, with hidden layers of increased and then decreased sizes. 
+        For layer_elements = 64 and layers = 8 and in_elements = out_elements = 8, 
+        the layer sizes are [8, 16, 32, 64, 64, 32, 16, 8]. 
+    
+    Args:
+        layers (int): Indicate the number of fully connected layers. 
+        in_elements (int): The number of elements for the input. Defaults to 1.
+        out_elements (int): The number of elements for the output, as the number of classification. Defaults to 1000 for 1000 classes.
+        layer_elements (int or list of length 'layers'): The number of channels for each block. In a VGG, it should be [64, 128, 256, 512, 512]. 
+            Or else, a function may be provided to compute the output channels given the block index (-1 ~ 2 * depth + 1). 
+        kernel_size (int): The size of the convolution kernels. Defaults to 3. 
+        keep_prob (float): The keep probability for the dropout layers. 
+        activation_function (class): The activation function used after the convolution layers. Defaults to nn.ReLU. 
+        active_args (dict): The arguments for the activation function. Defaults to {}. 
+        initializer (str): A string indicating the initialing strategy. Possible values are normal(0, 0.1) or uniform(-0.1, 0.1) or constant(0) (all parameters can be changed)
+        with_softmax (bool): Whether a softmax layer is applied at the end of the network. Defaults to True. 
+    '''
 
     class Softmax(nn.Module):
         def forward(self, x): return nn.functional.softmax(x, 1)
     def __init__(self, layers = 4, in_elements = 1, out_elements = 2, layer_elements = 64, 
         keep_prob = 0.5, activation_function = nn.ReLU, active_args = {}, 
         initializer = "normal(0, 0.1)", with_softmax = True):
         if isinstance(layer_elements, int):
             maxlc = layer_elements
             layer_elements = [in_elements]
-            multiplier = int(bt.pow(maxlc / in_elements, 1 / (layers // 2 + 1)))
+            multiplier = bt.pow(maxlc / in_elements, 1 / (layers // 2 - 1))
             for i in range(layers // 2 - 1):
-                layer_elements.append(layer_elements[-1] * multiplier)
+                layer_elements.append(int(layer_elements[-1] * multiplier))
             layer_elements.append(maxlc)
             if layers % 2 == 0: layer_elements.extend(layer_elements[-2::-1])
             else: layer_elements.extend(layer_elements[::-1])
             layer_elements[-1] = out_elements
         if isinstance(layer_elements, list):
             lc = layer_elements.copy()
             layer_elements = lambda i: lc[i]
@@ -362,15 +409,178 @@
             elif with_softmax:
                 self.layers.append(self.Softmax())
         self.struct = nn.Sequential(*self.layers)
         self.to(bt.get_device().main_device)
 
     def forward(self, x):
         return self.struct(x)
-
+    
+class NeuralODE(nn.Module):
+    '''
+    Neural ODE structue. 
+    => [dual stream: reference maps] dual_channels
+    => [main stream: inputs] main_channels
+    
+    Args:
+        dimension (int): The dimension of the images. 
+        layers (int): The number accumulated layers. 
+        conv_num (int): The number of continuous convolutions in each layer. Defaults to 2. 
+        dual_channels (int): The number of channels for the dual stream ODE. Defaults to 0, indicating no dual network.
+        main_channels (int): The number of channels for the main stream ODE. Defaults to 2.
+        kernel_size (int): The size of the convolution kernels. Defaults to 3. 
+        padding (int or str): Indicate the type of padding used. Defaults to 'SAME' indicating a same output shape as the input. 
+        conv_block (str): A string with possible values in ('conv', 'dense', 'residual'), indicating which kind of block for the layers: normal convolution layers, DenseBlock or ResidualBlock. 
+        res_type (function): The combining type for the residual connections. It should be torch.add in most occasions. 
+        activation_function (class): The activation function used after the convolution layers. Defaults to nn.ReLU. 
+        final_activation (class): The activation function after the final convolution. Defaults to self.activation_function. 
+        active_args (dict): The arguments for the activation function. Defaults to {}. 
+        initializer (str): A string indicating the initialing strategy. Possible values are normal(0, 0.1) or uniform(-0.1, 0.1) or constant(0) (all parameters can be changed)
+        regularization (func): The regularization term for the delta terms. 
+    '''
+    
+    class Softmax(nn.Module):
+        def forward(self, x): return nn.functional.softmax(x, 1)
+    
+    def __init__(self, dimension = 2, layers = 10, conv_num = 2, kernel_size = 3, padding = 1, 
+        dual_channels = 0, main_channels = 2, conv_block = 'conv', res_type = bt.add, 
+        activation_function = nn.ReLU, final_activation = ..., active_args = {}, initializer = "normal(0, 0.1)", 
+        shared = True, dual_ODE = True, time_channels = 1, auto_grad = False, regularization = None):
+        super().__init__()
+        
+        if dual_channels == True: dual_channels = 64
+        
+        params = dict(dimension=dimension, conv_num=conv_num, kernel_size=kernel_size, padding=padding, 
+            activation_function=activation_function, final_activation=final_activation, active_args=active_args, conv_block=conv_block, res_type=res_type, initializer=initializer)
+        if dual_channels > 0:
+            if dual_ODE:
+                if shared:
+                    self.dual_march_func = Convolution_Block(in_channels=dual_channels + time_channels, out_channels=dual_channels, **params)
+                    self.dual_march = [self.dual_march_func] * layers
+                else:
+                    self.dual_march = []
+                    for i in range(layers):
+                        setattr(self, f'dual_march_func_{i}', Convolution_Block(in_channels=dual_channels + time_channels, out_channels=dual_channels, **params))
+                        self.dual_march.append(getattr(self, f'dual_march_func_{i}'))
+        if shared:
+            self.main_march_func = Convolution_Block(in_channels=main_channels + dual_channels + time_channels, out_channels=main_channels, **params)
+            self.main_march = [self.main_march_func] * layers
+        else:
+            self.main_march = []
+            for i in range(layers):
+                setattr(self, f'main_march_func_{i}', Convolution_Block(in_channels=main_channels + dual_channels + time_channels, out_channels=main_channels, **params))
+                self.main_march.append(getattr(self, f'main_march_func_{i}'))
+        self.layers = layers
+        self.shared = shared
+        self.dual_ODE = dual_ODE
+        self.auto_grad = auto_grad
+        self.dual_channels = dual_channels
+        self.time_channels = time_channels
+        self.regularization = regularization
+    
+    def time(self, i, n_channel):
+        return (i / self.layers) * bt.ones(self.reference.shape.with_feature((n_channel,)), dtype=self.reference.dtype, device=self.reference.device)
+    
+    def integral(self, init_x, diff_func, time_inv = False):
+        x = init_x
+        for i in range(self.layers):
+            i = self.layers - i - 1 if time_inv else i
+            x = [(u - v) if time_inv else (u + v) for u, v in zip(x, diff_func(x, i))]
+        return x
+    
+    def march(self, x, march_funcs, i):
+        if self.time_channels > 0:
+            t = self.time(i, n_channel=self.time_channels)
+            return march_funcs[i](bt.cat(x, t, [])) / self.layers
+        return march_funcs[i](x) / self.layers
+    
+    def forward_diff_func(self, x, i):
+        if self.dual_channels > 0:
+            main_x, dual_x = x
+            delta_main_x = self.march(bt.cat(main_x, dual_x, []), self.main_march, i)
+            if self.dual_ODE: # DSNODE
+                delta_dual_x = self.march(dual_x, self.dual_march, i)
+            else: delta_dual_x = bt.zeros_like(dual_x)
+            return delta_main_x, delta_dual_x # SNODE / DSNODE
+        return [self.march(x[0], self.main_march, i)] # UNODE
+    
+    def forward_func(self, init_x, dual_init_x=None):
+        self.reference = init_x
+        if self.dual_channels > 0:
+            self.output, self.dual = self.integral([init_x, dual_init_x], self.forward_diff_func)
+        else: self.output, = self.integral([init_x], self.forward_diff_func)
+        return self.output
+    
+    def UNODE_backward_diff_func(self, x, i):
+        main_x, d_main = x
+        with bt.enable_grad():
+            main_x = main_x.detach().requires_grad_(True)
+            delta_main_x = self.march(main_x, self.main_march, i)
+            if self.regularization is not None:
+                self.regularization(delta_main_x).backward()
+            delta_main_x.backward(d_main.detach())
+        return delta_main_x.detach(), -main_x.grad
+    
+    def SNODE_backward_diff_func(self, x, i):
+        main_x, d_main, d_dual = x
+        with bt.enable_grad():
+            main_x = main_x.detach().requires_grad_(True)
+            dual_x = self.dual.detach().requires_grad_(True)
+            delta_main_x = self.march(bt.cat(main_x, dual_x, []), self.main_march, i)
+            if self.regularization is not None:
+                self.regularization(delta_main_x).backward()
+            delta_main_x.backward(d_main.detach())
+        return delta_main_x.detach(), -main_x.grad, -dual_x.grad
+    
+    def DSNODE_backward_diff_func(self, x, i):
+        main_x, dual_x, d_main, d_dual = x
+        with bt.enable_grad():
+            main_x = main_x.detach().requires_grad_(True)
+            dual_x = dual_x.detach().requires_grad_(True)
+            delta_main_x = self.march(bt.cat(main_x, dual_x, []), self.main_march, i)
+            delta_dual_x = self.march(dual_x, self.dual_march, i)
+            if self.regularization is not None:
+                self.regularization(delta_main_x).backward()
+            delta_dual_x.backward(d_dual.detach())
+            delta_main_x.backward(d_main.detach())
+        return delta_main_x.detach(), delta_dual_x.detach(), -main_x.grad, -dual_x.grad
+    
+    def backward(self, output_grad):
+        output_grad = output_grad.as_subclass(bt.Tensor).view(self.output.shape)
+        inits = []
+        if self.dual_channels > 0:
+            if self.dual_ODE:
+                inits = [self.output, self.dual, output_grad, bt.zeros_like(self.dual)]
+                ret = self.integral(inits, self.DSNODE_backward_diff_func, time_inv=True)[2:]
+            else:
+                inits = [self.output, output_grad, bt.zeros_like(self.dual)]
+                ret = self.integral(inits, self.SNODE_backward_diff_func, time_inv=True)[1:]
+        else:
+            inits = [self.output, output_grad]
+            ret = self.integral(inits, self.UNODE_backward_diff_func, time_inv=True)[1:]
+        # for mlayer in ([self.main_march[0]] if self.shared else self.main_march):
+        #     for p in mlayer.parameters(): p.grad = -p.grad
+        # if self.dual_channels > 0:
+        #     for mlayer in ([self.dual_march[0]] if self.shared else self.dual_march):
+        #         for p in mlayer.parameters(): p.grad = -p.grad
+        return ret
+    
+    class Autograd_Func(bt.autograd.Function):
+        @staticmethod
+        def forward(ctx, self, init_x, dual_init_x=None):
+            ctx.self = self
+            return self.forward_func(init_x, dual_init_x=dual_init_x)
+        
+        @staticmethod
+        def backward(ctx, output_grad):
+            return None, *ctx.self.backward(output_grad)
+    
+    def forward(self, init_x, dual_init_x=None):
+        if self.auto_grad: return self.forward_func(init_x, dual_init_x=dual_init_x)
+        if self.dual_channels == 0: return self.Autograd_Func.apply(self, init_x)
+        return self.Autograd_Func.apply(self, init_x, dual_init_x)
 
 if __name__ == "__main__":
 #    unet = U_Net(multi_arms="seperate(3)", block_channels=16)
 #    print(unet(bt.rand(10, 3, 100, 100)).size())
 #    print(*[x + ' ' + str(unet[i].size()) for x, i in unet], sep='\n')
     unet = U_Net(
         dimension=3,
```

### Comparing `micomputing-1.1.47/micomputing/stdio.py` & `micomputing-1.1.48/micomputing/stdio.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     requires = ["nibabel", "pydicom"]
 )
 
 __all__ = """
     IMG
     dcm2nii
     nii2dcm
+    affine2orient
 """.split()
 
 import os
 from datetime import datetime as dt
 
 with __info__:
     import SimpleITK as sitk
@@ -74,14 +75,27 @@
 with run("DCM", "NII"), run.all_tags:
     def dcm2nii(file1, file2):
         IMG(file1).astype(IMG.nii).save(file2)
 
     def nii2dcm(file1, file2):
         IMG(file1).astype(IMG.dcm).save(file2)
         
+def affine2orient(affine):
+    aff_abs = np.abs(affine[:-1, :-1])
+    n_dim = aff_abs.shape[-1]
+    orient = [''] * n_dim
+    for d in range(n_dim):
+        k = aff_abs.argmax()
+        i = k // n_dim
+        j = k - i * n_dim
+        orient[j] = ['RL', 'AP', 'SI'][i][affine[i, j] > 0]
+        aff_abs[i] = 0
+        aff_abs[:, j] = 0
+    return ''.join(orient)
+        
 class Spacing(tuple): ...
 
 class IMG:
     
     with run("PNG"), run.use_tag: png = PNG = 'PNG'
     with run("DCM"), run.use_tag: dcm = DCM = 'DCM'
     with run(sitk_supported_modalities), run.all_tags:
@@ -108,15 +122,15 @@
         if not done:
             if not path.exists(): raise FileNotFoundError(f"Cannot find file/folder {path}. ")
             self.ftype = kwargs.get('astype', None)
             if self.ftype is None: raise TypeError(f"micomputing.IMG failed to recognize type of {path}. Use `astype=IMG.nii` or other image format to identify it. ")
             with run(sitk_supported_modalities), run.any_tag:
                 if self.ftype in sitk_supported_modalities: self.__init_sitk__(path, **kwargs); done =True
             with run("DCM"), run.use_tag:
-                if self.ftype == "DCM": self.__init_dcm__(path, **kwargs); done =True
+                if self.ftype in ("DCM", "IMA"): self.__init_dcm__(path, **kwargs); done =True
         if len(self.basics) <= 0: self.basics = basic_tags.copy()
 
     @overload
     def __init__(self, x: sitk.Image, **kwargs):
         self.unresolved_warning = False
         self.has_series = False
         self.ftype = kwargs.get('ftype', None)
@@ -532,19 +546,15 @@
     def shape(self):
         if self.has_series: raise Error('Property')("No property 'shape' for micomputing.IMG with series. ")
         return tuple(self.image.GetSize())
     
     @property
     def orientation(self):
         if self.has_series: raise Error('Property')("No property 'orientation' for micomputing.IMG with series. ")
-        affine = self.affine
-        dim_ord = np.abs(affine[:-1, :-1]).argmax(0).tolist()
-        try: dx = np.array([affine[dim_ord[d], d] for d in range(len(dim_ord))])
-        except ValueError: raise TypeError(f"Invalid affine matrix: {affine}")
-        return ''.join([['RL', 'AP', 'SI'][i][j] for i, j in zip(dim_ord, dx > 0)])
+        return affine2orient(self.affine)
 
     def reorient(self, orient='LPI'):
         if self.has_series: raise Error('Property')("Cannot reorient for micomputing.IMG with series. ")
         axis = {'L':'LR', 'R':'LR', 'A':'AP', 'P':'AP', 'I':'SI', 'S':'SI'}
         from .funcs import reorient
         from .trans import Translation, Reflection, DimPermutation, ComposedTransformation
         orient_axis = [axis[i] for i in self.orientation]
@@ -783,22 +793,21 @@
                 used_path = []
                 for sid in ids:
                     info = infos[sid]
                     p = get_path(sid)
                     if p is None: continue
                     if isdir(p):
                         if not os.path.exists(p): os.mkdir(p)
-                        if self.has_series:
-                            extra = info.copy()
-                            for k in IMG.basic_info: extra.pop(k)
-                            if len(extra) > 0: extra_str = ''.join([f"_{get_alphas(k)}{get_digits(str(v)) if get_digits(str(v)) else get_alphas(str(v))}" for k, v in extra.items()])
-                            else: extra_str = ''
-                            default_name = f"{info['SeriesTime']}_{info['SeriesDescription']}_{info['SeriesNumber']}"
-                            p = os.path.join(p, default_name)
-                            if p in used_path: p += extra_str
+                        extra = info.copy()
+                        for k in IMG.basic_info: extra.pop(k)
+                        if len(extra) > 0: extra_str = ''.join([f"_{get_alphas(k)}{get_digits(str(v)) if get_digits(str(v)) else get_alphas(str(v))}" for k, v in extra.items()])
+                        else: extra_str = ''
+                        default_name = f"{info['SeriesTime']}_{info['SeriesDescription']}_{info['SeriesNumber']}"
+                        p = os.path.join(p, default_name)
+                        if p in used_path: p += extra_str
                         p //= ext
                     if p in used_path:
                         if avoid_conflict:
                             if p | ext: p = p[:-len(ext)]
                             i = 1
                             while True:
                                 if p + f' ({i})' + ext in used_path: i += 1
```

### Comparing `micomputing-1.1.47/micomputing/test_dismap.py` & `micomputing-1.1.48/micomputing/test_dismap.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/trans.py` & `micomputing-1.1.48/micomputing/trans.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     Affine                 Aff         rand_Affinity               rand_Aff
     PolyAffine                         rand_PolyAffine
     logEuclidean           logEu       rand_logEuclidean           rand_logEu
     LocallyAffine          LARM        rand_LocallyAffine          rand_LARM
     FreeFormDeformation    FFD         rand_FreeFormDeformation    rand_FFD
     DenseDisplacementField DDF         rand_DenseDisplacementField rand_DDF
     VelocityField          VF          rand_VelocityField          rand_VF
+    
+    Normalize              Cropping
 """.split()
 #     FreeFormDeformation FFD
 #     DenseDisplacementField DDF
 #     MultiLayerPerception MLP
     
 #     Normalize
     
@@ -70,14 +72,15 @@
 #     return isinstance(x, (WorldCoordsTransformation, ImageCoordsTransformation)) \
 #         or isinstance(x, ComposedTransformation) and x.mode == "spatial"
 
 # def is_world_coords_transformation(x):
 #     return isinstance(x, Transformation) or isinstance(x, ComposedTransformation) and x.mode == "spatial"
 
 def perform_reshape(shape, reshape_args):
+    if len(reshape_args) == 1: return tuple(reshape_args[0])
     n_dim = len(shape)
     padding, scale, *pairs = reshape_args
     if len(scale) == 1: scale *= n_dim
     if len(padding) == 1: padding *= n_dim
     padding = tuple(p if isinstance(p, tuple) else (p, p) for p in padding)
     target_space = [int(x * y + a + b) for x, y, (a, b) in zip(shape, scale, padding)]
     for p, q in pairs: target_space[p], target_space[q] = target_space[q], target_space[p]
@@ -222,15 +225,15 @@
         self.target = None
         self.params = params
         self.kwparams = kwparams
         self.n_dim = None
         self.n_batch = None
         self.reshape = [(0,), (1,)]
         """
-        e.g. [((dl1⁻, dl1⁺), (dl2⁻, dl2⁺), (dl3⁻, dl3⁺)), (s[0], s[1], s[2]), (d[0], d[1]), (d[2], d[3])] means:
+        e.g. [((dl[0]⁻, dl[0]⁺), (dl[1]⁻, dl[1]⁺), (dl[2]⁻, dl[2]⁺)), (s[0], s[1], s[2]), (d[0], d[1]), (d[2], d[3])] means:
             1) transpose dimensions d[2] and d[3]; followed by d[0] with d[1];
             2) rescale at dimension d with s[d];
             3) crop(* < 0) or pad(* > 0) a side by dl[d]♯,
                 where #=+ for the larger side and #=- for the lower side;
         The shape transformation goes from left to right. Only the firt two transformation can be a tuple with length other than 2, 
             meaning scaling and padding instead of transpose. Having a length 1, e.g. (*,), stands for isotropic scaling or padding;
             being (1,) means no scaling, (0,) means no padding.
@@ -305,15 +308,15 @@
                 return_image = True
                 input_images = X
                 if to_shape is None: to_shape = X.space
                 X = bt.image_grid(*perform_reshape(to_shape, self.reshape)).duplicate(self.n_batch if self.n_batch is not None else 1, {})
                 domain = 'image-space'
         else: # domain in ('physical-space', 'image-space')
             avouch(X.has_channel, f"Please use batorch tensor of size ({{n_batch:optional}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim] for {self.__name__}, instead of {X.shape}. ")
-            avouch(X.n_channel == n_dim, f"[n_dim]D {self.__name__} does not take coordinates of size {X.shape}")
+            avouch(X.n_channel == n_dim, f"{n_dim}D {self.__name__} does not take coordinates of size {X.shape}")
 
         Y = X.clone().float()
         if not Y.has_batch:
             if self.n_batch is not None: Y = Y.duplicate(self.n_batch, {})
             else: Y = Y.unsqueeze({})
         elif Y.n_batch == 1 and self.n_batch is not None: Y = Y.amplify(self.n_batch, {})
         
@@ -347,15 +350,15 @@
     __affine__ = NotImplemented
     __inv__ = NotImplemented
     
     @staticmethod
     def __get_affine__(x):
         if isinstance(x, str): x = IMG(x)
         if isinstance(x, IMG): x = x.affine
-        x = bt.to_bttensor(x)
+        x = bt.to_bttensor(x).auto_device()
         avouch(2 <= x.n_dim <= 3, TypeError(f"Invalid affine matrix represented by shape {x.shape}. "))
         avouch(not x.has_func and not x.has_sequence, TypeError(f"Invalid affine matrix represented by shape {x.shape}, only batch/feature dimensions are allowed. "))
         if x.n_dim == 3: x.special_from(bt.Size({1}, [1, 1]))
         else: x.special_from(bt.Size([1, 1]))
         avouch(x.feature[0] == x.feature[1], TypeError(f"Invalid affine matrix represented by shape {x.shape}: should be of shape (n_dim+1, n_dim+1). "))
         return x
     
@@ -764,47 +767,47 @@
     
     def force_inv(self, *size):
         if self.inv != NotImplemented: return self.inv()
         else: return self.num_inv(*size)
 
 @alias("CompoundTransformation")
 class ComposedTransformation(Transformation):
+    """
+    Create a composed transformation. 
+
+    Note: The composed transformation `T` consist of a list of transformations, `[T₁, T₂, ⋯, Tₖ]`. 
+        If domain = image/physical-space, backward = True (represented by image-space transformations):
+            T(X) = T₁(T₂( ⋯ (Tₖ(X)))) for coordinates X, i.e., I∘T = I∘T₁∘T₂∘ ⋯ ∘Tₖ.
+        If domain = image/physical-space, backward = False (represented by image-space transformations):
+            I₁(T₁(x)) = I(x); ⋯ ; Iₖ∘Tₖ(x) = Iₖ₋₁(x), i.e., Iₖ∘Tₖ∘Tₖ₋₁∘ ⋯ ∘T₁ = I; Iₖ∘T = I.
+        If domain = non-spatial:
+            T(X) = Tₖ(Tₖ₋₁( ⋯ (T₁(I)))) for images I, i.e., T∘I = Tₖ∘Tₖ₋₁∘ ⋯ ∘T₁∘I. 
+        Always remember, transformation is performed in order T₁, T₂, ⋯ , Tₖ, 
+            except continuous coordinate transformations go backward. 
+
+    Args:
+        trans_list (list or tuple): The list of transformations, operating one by one onto an image. 
+            A series of backward transformations would be equivalent to a composition of functions from right to left.
+    
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+            OR Images to be transformed. 
+            size: ({n_batch:optional}, [n_channel:optional], n_1, n_2, ..., n_r) [r=n_dim]
+    """
     
     @staticmethod
     def __flat__(trans_list):
         flat_trans_list = []
         for t in trans_list:
             if not isinstance(t, ComposedTransformation): flat_trans_list.append(t)
             else: flat_trans_list.extend(ComposedTransformation.__flat__(t.trans_list))
         return flat_trans_list
 
     def __init__(self, *trans_list, domain=None, backward=None):
-        """
-        Create a composed transformation. 
-
-        Note: The composed transformation `T` consist of a list of transformations, `[T₁, T₂, ⋯, Tₖ]`. 
-            If domain = image/physical-space, backward = True (represented by image-space transformations):
-                T(X) = T₁(T₂( ⋯ (Tₖ(X)))) for coordinates X, i.e., I∘T = I∘T₁∘T₂∘ ⋯ ∘Tₖ.
-            If domain = image/physical-space, backward = False (represented by image-space transformations):
-                I₁(T₁(x)) = I(x); ⋯ ; Iₖ∘Tₖ(x) = Iₖ₋₁(x), i.e., Iₖ∘Tₖ∘Tₖ₋₁∘ ⋯ ∘T₁ = I; Iₖ∘T = I.
-            If domain = non-spatial:
-                T(X) = Tₖ(Tₖ₋₁( ⋯ (T₁(I)))) for images I, i.e., T∘I = Tₖ∘Tₖ₋₁∘ ⋯ ∘T₁∘I. 
-            Always remember, transformation is performed in order T₁, T₂, ⋯ , Tₖ, 
-                except continuous coordinate transformations go backward. 
-
-        Args:
-            trans_list (list or tuple): The list of transformations, operating one by one onto an image. 
-                A series of backward transformations would be equivalent to a composition of functions from right to left.
-        
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-                OR Images to be transformed. 
-                size: ({n_batch:optional}, [n_channel:optional], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         super().__init__()
         
         ##  find uniform n_dim & n_batch ##
         ###################################
         n_dims = set([t.n_dim for t in trans_list if t.n_dim is not None])
         n_batches = set([t.n_batch for t in trans_list if t.n_batch is not None])
         if 1 in n_batches: n_batches.remove(1)
@@ -835,14 +838,16 @@
         self.backward = backward
 
         ##  combine the reshape property ##
         ###################################
         accum = [(0,), (1,)]
         add_pad = lambda x, y: tuple(a+b for a, b in zip(x if isinstance(x, tuple) else (x, x), y if isinstance(y, tuple) else (y, y)))
         for t in self.trans_list:
+            if len(t.reshape) == 1: accum = t.reshape; continue
+            if len(accum) == 1: accum = [perform_reshape(accum[0], t.reshape)]; continue
             padding_a, scale_a, *pairs_a = accum
             padding_t, scale_t, *pairs_t = t.reshape
 
             if len(padding_a) == 1: padding_a *= len(padding_t)
             else:
                 padding_a = list(padding_a)
                 for p, q in pairs_t[::-1]: padding_a[p], padding_a[q] = padding_a[q], padding_a[p]
@@ -927,71 +932,81 @@
     def source(self, _): ...
 
     @property
     def target(self): return self.trans_list[-1].target
     @target.setter
     def target(self, _): ...
 
-    def __call__(self, X, domain=None, **kwargs):
+    def __call__(self, X, domain=None, use_implementation=None, to_shape=None, **kwargs):
         """
         Perform composed transformation. 
         
         domain = physical/image-space::
             X (bt.Tensor): Coordinates to be transformed.
                 size: ({n_batch: optional}, [r], n_1, n_2, ..., n_r) [r=n_dim]
             Returns (bt.Tensor): The transformed coordinates.
                 size: ({n_batch}, [r], n_1, n_2, ..., n_r) [r=n_dim]
         domain = non-spatial::
             X (bt.Tensor): Images to be transformed.
                 size: ({n_batch: optional}, [n_channel:optional], n_1, n_2, ..., n_r) [r=n_dim]
             Returns (bt.Tensor): The transformed images.
                 size: ({n_batch}, [n_channel:optional], n_1, n_2, ..., n_r) [r=n_dim]
+        
+        Other Args:
+            use_implementation (str): The implementation function used to perform transformation. Defaults to the implementation for self.domain. 
+            to_shape (tuple): The output shape for the non-spatial transformation. 
         """
+        if not (X.has_channel and X.n_channel == X.n_space_dim): domain = 'non-spatial'
         if domain is None: domain = self.domain
 
         accum_spatial_trans = []
         for t in self.trans_list + [None]:
             if t is not None and t.domain != 'non-spatial' and (t.backward or t.inv != NotImplemented): accum_spatial_trans.append(t); continue
             if len(accum_spatial_trans) > 0:
                 n_img = sum(t.domain == 'image-space' or (t.source is not None and t.target is not None) for t in accum_spatial_trans)
                 n_phy = sum(t.domain == 'physical-space' or (t.source is not None and t.target is not None) for t in accum_spatial_trans)
                 if n_img == len(accum_spatial_trans) and n_phy == len(accum_spatial_trans):
-                    n_img = sum(t.core_domain == 'image-space' for t in accum_spatial_trans)
-                    n_phy = sum(t.core_domain == 'physical-space' for t in accum_spatial_trans)
-                    if n_img > n_phy: cur_domain = 'image-space'
+                    n_img = sum(t.domain == 'image-space' for t in accum_spatial_trans)
+                    n_phy = sum(t.domain == 'physical-space' for t in accum_spatial_trans)
+                    if n_img > n_phy: core_domain = 'image-space'
                     else: core_domain = 'physical-space'
+                elif n_img == len(accum_spatial_trans): core_domain = 'image-space'
+                elif n_phy == len(accum_spatial_trans): core_domain = 'physical-space'
                 else: core_domain = domain
 
+                return_image = False
                 if domain == 'non-spatial':
                     return_image = True
                     input_images = X
-                    X = bt.image_grid(*perform_reshape(X.space, self.reshape)).duplicate(self.n_batch if self.n_batch is not None else 1, {})
+                    if to_shape is None: to_shape = X.space
+                    X = bt.image_grid(*perform_reshape(to_shape, self.reshape)).duplicate(self.n_batch if self.n_batch is not None else 1, {})
                     domain = 'image-space'
-
+                
                 if domain == core_domain:
                     for st in accum_spatial_trans[::-1]:
                         if st.backward: X = st(X, domain=core_domain)
                         else: X = st.inv()(X, domain=core_domain)
                 else:
                     source = self.source
                     target = self.target
                     avouch(source is not None and target is not None, "Cannot perform image/physical-space transformation for image coordinates without source/target information. ")
 
                     taffine = Transformation.__get_affine__(target)
                     saffine = Transformation.__get_affine__(source)
                     if domain == 'image-space': saffine = saffine.inv()
                     else: taffine = taffine.inv()
-                    X = bt.matmul(taffine, X)
+                    X = (bt.matmul(prev_affine[..., :n_dim, :n_dim], X.flatten(...).add_special_dim(-1, [])) + prev_affine[..., :n_dim, n_dim:]).view_as(X)
                     for st in accum_spatial_trans[::-1]:
                         if st.backward: X = st(X, domain=core_domain)
                         else: X = st.inv()(X, domain=core_domain)
-                    X = bt.matmul(saffine, X)
+                    X = (bt.matmul(post_affine[..., :n_dim, :n_dim], X.flatten(...).add_special_dim(-1, [])) + post_affine[..., :n_dim, n_dim:]).view_as(X)
                 
                 if return_image: X = interpolation(input_images, target_space=X, **kwargs)
-            X = t(X, domain=domain)
+            if t is not None:
+                X = t(X, domain=domain)
         return X
 
     @req_spatial
     def affine(self, n_dim=None):
         # avouch(self.is_spatial, "Cannot get `affine` from composed transformation with non-spatial transformation. ")
         comp = self.compose()
         avouch(len(comp) == 1, "Error in calling `affine`: Only the composition of linear transformations can result in an affine matrix.")
@@ -1031,53 +1046,54 @@
         dic['trans_list'] = [t.to_dict() for t in self.trans_list]
         return dic
 
 # ########### Spatial Transformations ###########
 
 @alias("Id")
 class Identity(Transformation):
+    """
+    Identity transformation.
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates. (Same as X for Identity)
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
 
     def __init__(self, **kwargs):
-        """
-        Identity transformation.
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates. (Same as X for Identity)
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         super().__init__(**kwargs)
 
     def __affine__(self, n_dim=None):
         if n_dim is None: return
         return bt.eye([n_dim + 1]).unsqueeze({})
 
     def __call_image_space__(self, X): return X
 
     def __inv__(self): return Identity()
 
 class Rotation90(Transformation):
+    """
+    Transformation that rotates an image of `image_size` by 90 degrees.
+    
+    Note: The rotation is for coordinates, hence the image rotates clockwise. 
+    
+    Args:
+        dim1, dim2 (int): The plane we rotate on. Direction of the rotation is from `dim1` to `dim2`.
+            i.e. counter-clockwise rotation with dim1 as x-axis and dim2 as y-axis: [dim1, dim2] coordinates (x, y) becomes (ymax-y, x).
+        image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+
     def __init__(self, dim1, dim2, image_size=None, resize_image=True, **kwargs):
-        """
-        Transformation that rotates an image of `image_size` by 90 degrees.
-        
-        Note: The rotation is for coordinates, hence the image rotates clockwise. 
-        
-        Args:
-            dim1, dim2 (int): The plane we rotate on. Direction of the rotation is from `dim1` to `dim2`.
-                i.e. counter-clockwise rotation with dim1 as x-axis and dim2 as y-axis: [dim1, dim2] coordinates (x, y) becomes (ymax-y, x).
-            image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         super().__init__(dim1=dim1, dim2=dim2, image_size=image_size, resize_image=resize_image, **kwargs)
 
         self.dim1, self.dim2 = dim1, dim2
         if isinstance(image_size, bt.torch.Tensor): image_size = image_size.shape
         self.image_size = image_size
         if image_size is not None: self.n_dim = len(image_size)
         if resize_image: self.reshape = [(0,), (1,), (dim1, dim2)]
@@ -1107,31 +1123,32 @@
         aff[dim2][dim2] = 0.
         aff[dim2][dim1] = 1.
         return aff.unsqueeze({})
     
     def __inv__(self): return Rotation270(self.dim1, self.dim2, image_size = self.image_size, resize_image = self.resize_image)
 
 class Rotation270(Transformation):
+    """
+    Transformation that rotates an image by 270 degrees.
+    
+    Note: The rotation is for coordinates, hence the image rotates clockwise. 
+    
+    Args:
+        dim1, dim2 (int): The plane we rotate on. Direction of the rotation is from `dim1` to `dim2`.
+            i.e. counter-clockwise rotation with dim1 as x-axis and dim2 as y-axis: [dim1, dim2] coordinates (x, y) becomes (y, xmax-x).
+        image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, dim1, dim2, image_size=None, resize_image=True, **kwargs):
-        """
-        Transformation that rotates an image by 270 degrees.
-        
-        Note: The rotation is for coordinates, hence the image rotates clockwise. 
-        
-        Args:
-            dim1, dim2 (int): The plane we rotate on. Direction of the rotation is from `dim1` to `dim2`.
-                i.e. counter-clockwise rotation with dim1 as x-axis and dim2 as y-axis: [dim1, dim2] coordinates (x, y) becomes (y, xmax-x).
-            image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         super().__init__(dim1=dim1, dim2=dim2, image_size=image_size, resize_image=resize_image, **kwargs)
 
         self.dim1, self.dim2 = dim1, dim2
         if isinstance(image_size, bt.torch.Tensor): image_size = image_size.shape
         self.image_size = image_size
         if image_size is not None: self.n_dim = len(image_size)
         if resize_image: self.reshape = [(0,), (1,), (dim1, dim2)]
@@ -1161,29 +1178,30 @@
         aff[dim2][dim1] = -1.
         aff[dim2][-1] = float(self.image_size[dim1])
         return aff.unsqueeze({})
     
     def __inv__(self): return Rotation90(self.dim1, self.dim2, image_size = self.image_size, resize_image = self.resize_image)
 
 class Rotation180(Transformation):
+    """
+    Transformation that rotates an image by 180 degrees.
+    
+    Args:
+        dim1, dim2 (int): The plane we rotate on. It is also the central symmetry.
+            i.e. rotation with dim1 as x-axis and dim2 as y-axis: [dim1, dim2] coordinates (x, y) becomes (xmax-x, ymax-y).
+        image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, dim1, dim2, image_size=None, **kwargs):
-        """
-        Transformation that rotates an image by 180 degrees.
-        
-        Args:
-            dim1, dim2 (int): The plane we rotate on. It is also the central symmetry.
-                i.e. rotation with dim1 as x-axis and dim2 as y-axis: [dim1, dim2] coordinates (x, y) becomes (xmax-x, ymax-y).
-            image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         super().__init__(dim1=dim1, dim2=dim2, image_size=image_size, **kwargs)
 
         self.dim1, self.dim2 = dim1, dim2
         if isinstance(image_size, bt.torch.Tensor): image_size = image_size.shape
         self.image_size = image_size
         if image_size is not None: self.n_dim = len(image_size)
 
@@ -1210,29 +1228,30 @@
         aff[dim2][-1] = float(self.image_size[dim2])
         return aff.unsqueeze({})
 
     def __inv__(self): return Rotation180(self.dim1, self.dim2, image_size = self.image_size)
 
 @alias("Reflect")
 class Reflection(Transformation):
+    """
+    Transformation that reflects an image along dimension dim.
+    
+    Args:
+        dims (int's): The dimension we reflect the image along. 
+            i.e. reflection on dims: coordinate x at dim (in dims) becomes x_max-x.
+        image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, *dims, image_size=None, **kwargs):
-        """
-        Transformation that reflects an image along dimension dim.
-        
-        Args:
-            dims (int's): The dimension we reflect the image along. 
-                i.e. reflection on dims: coordinate x at dim (in dims) becomes x_max-x.
-            image_size (tuple or bt.Tensor): The size of the image, or the image itself. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         super().__init__(dims=dims, image_size=image_size, **kwargs)
 
         if len(dims) == 1 and isinstance(dims[0], (list, tuple)): dims = dims[0]
         self.dims = dims
         if isinstance(image_size, bt.torch.Tensor): image_size = image_size.shape
         self.image_size = image_size
         if image_size is not None: self.n_dim = len(image_size)
@@ -1257,38 +1276,39 @@
         for dim in self.dims:
             aff[dim][dim] = -1.
             aff[dim][-1] = float(self.image_size[dim])
         return aff.unsqueeze({})
 
 @alias("Permutedim")
 class DimPermutation(Transformation):
-    def __init__(self, *dims, resize_image=True, **kwargs):
-        """
-        Permute the dimensions for an image, similar to np.transpose or torch/batorch.permute.
-        
-        Args:
-            dims (list or tuple or bt.Tensor): The dimension permuation. 
-                size: length(n_dim) or ({n_batch:optional}, [n_dim]).
+    """
+    Permute the dimensions for an image, similar to np.transpose or torch/batorch.permute.
+    
+    Args:
+        dims (list or tuple or bt.Tensor): The dimension permuation. 
+            size: length(n_dim) or ({n_batch:optional}, [n_dim]).
 
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
+    def __init__(self, *dims, resize_image=True, **kwargs):
         if len(dims) == 1: dims = dims[0]
         if isinstance(dims, tuple): dims = list(dims)
-        dims = bt.to_bttensor(dims).squeeze()
-        dims = dims.long()
-        if dims.n_dim <= 1: dims = dims.unsqueeze({})
-        if dims.n_dim == 2:
-            if not dims.has_batch: dims.batch_dimension = 0
-            if not dims.has_channel: dims.channel_dimension = 0 if dims.batch_dimension > 0 else 1
-        avouch(dims.has_batch and dims.has_channel, f"Please use batorch tensor of size \
-            ({{n_batch:optional}}, [n_dim]) for Translation parameters, instead of {dims.shape}. ")
+        dims = bt.to_bttensor(dims).squeeze().long()
+        bt.input_shape().set(dims = "({n_batch}, [n_dim])")
+        # if dims.n_dim <= 1: dims = dims.unsqueeze({})
+        # if dims.n_dim == 2:
+        #     if not dims.has_batch: dims.batch_dimension = 0
+        #     if not dims.has_channel: dims.channel_dimension = 0 if dims.batch_dimension > 0 else 1
+        # avouch(dims.has_batch and dims.has_channel, f"Please use batorch tensor of size \
+        #     ({{n_batch:optional}}, [n_dim]) for Translation parameters, instead of {dims.shape}. ")
         super().__init__(dims, resize_image=resize_image, **kwargs)
 
         self.dims = dims
         self.n_dim = dims.n_channel
         self.resize_image = resize_image
         if resize_image:
             if dims.n_batch > 1:
@@ -1338,43 +1358,45 @@
             ibatch = bt.arange({n_batch})
             perms[ibatch, idx] = i
             coeffs[ibatch, idx] = 0
         return perms
 
 @alias("Rescale")
 class Rescaling(Transformation):
+    """
+    Scale an image.
+    
+    Note: The scaling is for image coordinates, hence the image would shrink if scale > 1. 
+    
+    Args:
+        scale (float or tuple or bt.Tensor): The scaling for all dimensions (float) 
+            or for each dimension (tuple). >1 means enlarging the coordinates.
+            size: ({n_batch:optional}, [n_dim]) for bt.Tensor.
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, *scale, resize_image=True, **kwargs):
-        """
-        Scale an image.
-        
-        Note: The scaling is for image coordinates, hence the image would shrink if scale > 1. 
-        
-        Args:
-            scale (float or tuple or bt.Tensor): The scaling for all dimensions (float) 
-                or for each dimension (tuple). >1 means enlarging the coordinates.
-                size: ({n_batch:optional}, [n_dim]) for bt.Tensor.
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         if len(scale) == 1 and isinstance(scale[0], (int, float)): scale = scale[0] * bt.ones({1}, [1])
         else:
             if len(scale) == 1: scale = scale[0]
             if isinstance(scale, tuple): scale = list(scale)
             if not isinstance(scale, bt.Tensor): scale = bt.to_bttensor(scale).squeeze()
-            if scale.n_dim <= 1: scale = scale.unsqueeze({})
-            if scale.n_dim == 2:
-                if not scale.has_batch: scale.batch_dimension = 0
-                if not scale.has_channel: scale.channel_dimension = 0 if scale.batch_dimension > 0 else 1
-        avouch(scale.has_batch and scale.has_channel, f"Please use batorch tensor of size \
-            ({{n_batch:optional}}, [n_dim]) for Scaling parameters, instead of {scale.shape}. ")
-        bt.to_device(scale)
+            bt.input_shape().set(scale = "({n_batch}, [n_dim])")
+        #     if scale.n_dim <= 1: scale = scale.unsqueeze({})
+        #     if scale.n_dim == 2:
+        #         if not scale.has_batch: scale.batch_dimension = 0
+        #         if not scale.has_channel: scale.channel_dimension = 0 if scale.batch_dimension > 0 else 1
+        # avouch(scale.has_batch and scale.has_channel, f"Please use batorch tensor of size \
+        #     ({{n_batch:optional}}, [n_dim]) for Scaling parameters, instead of {scale.shape}. ")
+        # bt.to_device(scale)
         super().__init__(scale, resize_image=resize_image, **kwargs)
 
         self.scale = scale
         if self.scale.n_channel > 1: self.n_dim = self.scale.n_channel
         if resize_image:
             avouch((scale - scale[:1]).abs().sum() < eps, "The batch should have a common rescaler if 'resize_image=True', they are being reshaped uniformly.")
             self.reshape = [(0,), tuple((1/scale[0]).tolist())]
@@ -1405,39 +1427,42 @@
         return std * bt.randn([len(shape)]).duplicate(n_batch, {}) + 1,
 
 def rand_Rescaling(image, std=1e-1, **kwargs):
     return Rescaling(*Rescaling.random_init_params(*image.space, n_batch=image.n_batch, std=std), **kwargs)
 
 @alias("Translate")
 class Translation(Transformation):
-    def __init__(self, *translation, **kwargs):
-        """
-        Translate an image.
-        
-        Note: The translation is for coordinates, hence the image would go in the opposite direction. 
+    """
+    Translate an image.
+    
+    Note: The translation is for coordinates, hence the image would go in the opposite direction. 
+    
+    Args:
+        translation (tuple or bt.Tensor): The translation of the coordinates.
+            size: length(n_dim) or ({n_batch:optional}, [n_dim])
         
-        Args:
-            translation (tuple or bt.Tensor): The translation of the coordinates.
-                size: length(n_dim) or ({n_batch:optional}, [n_dim])
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch:optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
+    def __init__(self, *translation, **kwargs):
         if len(translation) == 1: translation = translation[0]
         if isinstance(translation, tuple): translation = list(translation)
         translation = bt.to_bttensor(translation).squeeze()
-        if translation.n_dim <= 1: translation = translation.unsqueeze({})
-        if translation.n_dim == 2:
-            if not translation.has_batch: translation.batch_dimension = 0
-            if not translation.has_channel: translation.channel_dimension = 0 if translation.batch_dimension > 0 else 1
-        avouch(translation.has_batch and translation.has_channel, f"Please use batorch tensor of size \
-            ({{n_batch:optional}}, [n_dim]) for Translation parameters, instead of {translation.shape}. ")
+        if translation.n_dim == 1: translation.channel_dim = 0
+        bt.input_shape().set(translation = "({n_batch}, [n_dim])")
+        # if translation.n_dim <= 1: translation = translation.unsqueeze({})
+        # if translation.n_dim == 2:
+        #     if not translation.has_batch: translation.batch_dimension = 0
+        #     if not translation.has_channel: translation.channel_dimension = 0 if translation.batch_dimension > 0 else 1
+        # avouch(translation.has_batch and translation.has_channel, f"Please use batorch tensor of size \
+        #     ({{n_batch:optional}}, [n_dim]) for Translation parameters, instead of {translation.shape}. ")
         super().__init__(translation, **kwargs)
 
         self.translation = translation
         self.n_dim = self.translation.n_channel
         self.batch_param.append('translation')
 
     def __call_image_space__(self, X):
@@ -1460,116 +1485,142 @@
         return std * bt.randn({n_batch}, [len(shape)]),
 
 def rand_Translation(image, std=5, **kwargs):
     return Translation(*Translation.random_init_params(*image.space, n_batch=image.n_batch, std=std), **kwargs)
 
 @alias("Rig")
 class Rigid(Transformation):
+    """
+    Rigid transformation with respect to parameters.
+    !!Attention: It's domain is 'physical-space' by default. 
+    
+    Args (usage 1):
+        angle (bt.Tensor or np.numpy): the [clockwise] rotation angles about the axises (or z direction for 2D). It is counter-clockwise for image.
+            size: ({n_batch},)
+        axis (bt.Tensor or np.numpy): the rotation axises, normalized vectors, None for 2D. 
+            size: ({n_batch}, [n_dim])
+        translation (bt.Tensor or np.numpy): the translations after the rotation, zeros by default. 
+            size: ({n_batch}, [n_dim])
+        center (bt.Tensor or np.numpy): the center for the rotations, zeros by default. 
+            size: ({n_batch}, [n_dim])
+        trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
+    
+    Args (usage 2):
+        matrix (bt.Tensor or np.numpy): the affine matrix, it should be orthogonal or will be projected by Procrustes Problem. 
+            size: ({n_batch}, [n_dim + 1, n_dim + 1])
+        trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, angle, axis=None, translation=None, center=None, trans_stretch=None, **kwargs):
-        """
-        Rigid transformation with respect to parameters.
-        !!Attention: It's domain is 'physical-space' by default. 
-        
-        Args (usage 1):
-            angle (bt.Tensor or np.numpy): the [clockwise] rotation angles about the axises (or z direction for 2D). It is counter-clockwise for image.
-                size: ({n_batch},)
-            axis (bt.Tensor or np.numpy): the rotation axises, normalized vectors, None for 2D. 
-                size: ({n_batch}, [n_dim])
-            translation (bt.Tensor or np.numpy): the translations after the rotation, zeros by default. 
-                size: ({n_batch}, [n_dim])
-            center (bt.Tensor or np.numpy): the center for the rotations, zeros by default. 
-                size: ({n_batch}, [n_dim])
-            trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
-        
-        Args (usage 2):
-            matrix (bt.Tensor or np.numpy): the affine matrix, it should be orthogonal or will be projected by Procrustes Problem. 
-                size: ({n_batch}, [n_dim + 1, n_dim + 1])
-            trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         angle = bt.to_bttensor(angle)
-        if angle.n_dim <= 0 and not angle.has_batch: angle = angle.unsqueeze({})
-        if angle.n_dim == 1 and not angle.has_batch: angle = angle.with_batchdim(0)
-        if angle.n_dim == 2 and not angle.has_batch: angle = angle.unsqueeze({})
-        if angle.n_dim == 3 and not angle.has_batch and angle.shape[1] == angle.shape[2]: angle.batch_dimension = 0
-        avouch(angle.has_batch, f"Please use batorch tensor of size ({{n_batch}},) for Rigid rotation angles, instead of {angle.shape}. ")
-        n_batch = angle.n_batch
-        n_dim = None
-        if angle.n_dim >= 2:
+        bt.input_shape().usage(
+            angle = "({n_batch},)", 
+            axis = "({n_batch}, [n_dim]) [optional]", 
+            translation = "({n_batch}, [n_dim])", 
+            center = "({n_batch}, [n_dim])"
+        ).usage(angle = "({n_batch}, [n_dim + 1, n_dim + 1])")
+        if usage == 2:
             matrix = angle
-            n_dim = matrix.size(-1) - 1
             center = bt.zeros({n_batch}, [n_dim])
             translation = matrix[..., :-1, -1].with_channeldim(1)
             A = matrix[..., :-1, :-1]
             avouch(bt.norm(A.T @ A - bt.eye(A)).sum() < 1e-4, "Please make sure that matrix input for Rigid is orthogonal. Use Affine instead if it is not. ")
-            # I = bt.eye(A)
-            # Z_left = (A - I)[..., :-1] # ({n_batch}, n_dim, n_dim-1)
-            # Z_right = (A - I)[..., -1] # ({n_batch}, n_dim)
-            # ZTZ = Z_left.T @ Z_left
-            # if n_dim == 2:
-            #     axis = None
-            #     angle = bt.where(bt.abs(bt.det(ZTZ)) < 1e-6, bt.zeros({n_batch}), bt.acos(1 - ZTZ / 2).squeeze(-1, -1))
-            # elif n_dim == 3:
-            #     invZTZ = bt.inv(bt.where(bt.abs(bt.det(ZTZ)).unsqueeze(-1, -1) < 1e-6, bt.eye(ZTZ), ZTZ))
-            #     vector = bt.cat(- invZTZ @ Z_left.T @ Z_right, bt.ones({n_batch}, 1), 1).with_channeldim(1)
-            #     angle = bt.where(bt.abs(bt.det(ZTZ)) < 1e-6, bt.zeros({n_batch}), vector.norm())
-            #     axis = bt.where((bt.abs(bt.det(ZTZ)) < 1e-6).duplicate(n_dim, []), bt.channel_tensor(bt.one_hot(0, n_dim)).duplicate(n_batch, {}), vector / angle)
             if n_dim == 2:
                 axis = None
                 angle = bt.acos(A[..., 0, 0]) * bt.sign(A[..., 0, 1])
             elif n_dim == 3:
                 anti_sym = (A - A.T) / 2
                 sym = (A + A.T) / 2 - bt.eye(A)
                 angle = bt.acos(((anti_sym @ anti_sym) / sym).mean() - 1)
                 axis = bt.uncross_matrix(anti_sym)
                 axis /= bt.sin(angle)
             else:
                 raise Error("NotImplemented")(f"Rigid transformation in micomputing does not support [n_dim] dimensional transforms (2 & 3D only). " + 
                                             "Please contact the developers if there are feasible algorithms (Error Code: T333). Thank you. ")
-
-        if translation is not None:
-            translation = bt.to_bttensor(translation)
-            if translation.n_dim <= 1 and not translation.has_batch: translation = translation.unsqueeze({})
-            if translation.n_dim == 2 and not translation.has_batch: translation = translation.with_batchdim((1 - translation.channel_dimension) if translation.has_channel else 0)
-            if translation.n_dim == 2 and not translation.has_channel: translation = translation.with_channeldim(1 - translation.batch_dimension)
-            avouch(translation.has_batch and translation.has_channel, f"Please use batorch tensor of size ({{n_batch}}, [n_dim]) for Rigid translation, instead of {translation.shape}. ")
-            if n_batch == 1 and translation.n_batch > 1: n_batch = translation.n_batch
-            if n_dim is None: n_dim = translation.n_channel
-            else: avouch(n_dim == translation.n_channel, "Systematic error. Please contact the developers for details (Error Code: T332). ")
-            n_dim = translation.n_channel
-        if center is not None:
-            center = bt.to_bttensor(center)
-            if center.n_dim <= 1 and not center.has_batch: center = center.unsqueeze({})
-            if center.n_dim == 2 and not center.has_batch: center = center.with_batchdim((1 - center.channel_dimension) if center.has_channel else 0)
-            if center.n_dim == 2 and not center.has_channel: center = center.with_channeldim(1 - center.batch_dimension)
-            avouch(center.has_batch and center.has_channel, f"Please use batorch tensor of size ({{n_batch}}, [n_dim]) for Rigid center, instead of {center.shape}. ")
-            if n_batch == 1 and center.n_batch > 1: n_batch = center.n_batch
-            if n_dim is None: n_dim = center.n_channel
-            else: avouch(n_dim == center.n_channel, f"Center({center.n_channel}D) and translation([n_dim]D) in trans.Rigid should have the same dimension. ")
-            n_dim = center.n_channel
-        if axis is not None:
-            axis = bt.to_bttensor(axis)
-            if axis.n_dim <= 1 and not axis.has_batch: axis = axis.unsqueeze({})
-            if axis.n_dim == 2 and not axis.has_batch: axis = axis.with_batchdim((1 - axis.channel_dimension) if axis.has_channel else 0)
-            if axis.n_dim == 2 and not axis.has_channel: axis = axis.with_channeldim(1 - axis.batch_dimension)
-            avouch(axis.has_batch and axis.has_channel, f"Please use batorch tensor of size ({{n_batch}}, [n_dim]) for Rigid axises, instead of {axis.shape}. ")
-            if ((axis.norm() - 1) ** 2).sum().sum() >= 1e-2:
-                print("warning: param. axises for 'Rigid' transformation should be norm-1 vectors, auto-normalization would be performed. Please contact the developers if it is necessary to be non-unit vectors (Error Code: T331). ")
-                axis = axis / axis.norm()
-            if n_batch == 1 and axis.n_batch > 1: n_batch = axis.n_batch
-            if n_dim is None: n_dim = axis.n_channel
-            else: avouch(n_dim == axis.n_channel, f"Translation({n_dim}D) and axises({axis.n_channel}D)) in trans.Rigid should have the same dimension. ")
-        if n_dim is None: n_dim = 2 if axis is None else 3
-        if translation is None: translation = bt.zeros({n_batch}, [n_dim])
-        if center is None: center = bt.zeros({n_batch}, [n_dim])
+        
+        # if angle.n_dim <= 0 and not angle.has_batch: angle = angle.unsqueeze({})
+        # if angle.n_dim == 1 and not angle.has_batch: angle = angle.with_batchdim(0)
+        # if angle.n_dim == 2 and not angle.has_batch: angle = angle.unsqueeze({})
+        # if angle.n_dim == 3 and not angle.has_batch and angle.shape[1] == angle.shape[2]: angle.batch_dimension = 0
+        # avouch(angle.has_batch, f"Please use batorch tensor of size ({{n_batch}},) for Rigid rotation angles, instead of {angle.shape}. ")
+        # n_batch = angle.n_batch
+        # n_dim = None
+        # if angle.n_dim >= 2:
+        #     matrix = angle
+        #     n_dim = matrix.size(-1) - 1
+        #     center = bt.zeros({n_batch}, [n_dim])
+        #     translation = matrix[..., :-1, -1].with_channeldim(1)
+        #     A = matrix[..., :-1, :-1]
+        #     avouch(bt.norm(A.T @ A - bt.eye(A)).sum() < 1e-4, "Please make sure that matrix input for Rigid is orthogonal. Use Affine instead if it is not. ")
+        #     # I = bt.eye(A)
+        #     # Z_left = (A - I)[..., :-1] # ({n_batch}, n_dim, n_dim-1)
+        #     # Z_right = (A - I)[..., -1] # ({n_batch}, n_dim)
+        #     # ZTZ = Z_left.T @ Z_left
+        #     # if n_dim == 2:
+        #     #     axis = None
+        #     #     angle = bt.where(bt.abs(bt.det(ZTZ)) < 1e-6, bt.zeros({n_batch}), bt.acos(1 - ZTZ / 2).squeeze(-1, -1))
+        #     # elif n_dim == 3:
+        #     #     invZTZ = bt.inv(bt.where(bt.abs(bt.det(ZTZ)).unsqueeze(-1, -1) < 1e-6, bt.eye(ZTZ), ZTZ))
+        #     #     vector = bt.cat(- invZTZ @ Z_left.T @ Z_right, bt.ones({n_batch}, 1), 1).with_channeldim(1)
+        #     #     angle = bt.where(bt.abs(bt.det(ZTZ)) < 1e-6, bt.zeros({n_batch}), vector.norm())
+        #     #     axis = bt.where((bt.abs(bt.det(ZTZ)) < 1e-6).duplicate(n_dim, []), bt.channel_tensor(bt.one_hot(0, n_dim)).duplicate(n_batch, {}), vector / angle)
+        #     if n_dim == 2:
+        #         axis = None
+        #         angle = bt.acos(A[..., 0, 0]) * bt.sign(A[..., 0, 1])
+        #     elif n_dim == 3:
+        #         anti_sym = (A - A.T) / 2
+        #         sym = (A + A.T) / 2 - bt.eye(A)
+        #         angle = bt.acos(((anti_sym @ anti_sym) / sym).mean() - 1)
+        #         axis = bt.uncross_matrix(anti_sym)
+        #         axis /= bt.sin(angle)
+        #     else:
+        #         raise Error("NotImplemented")(f"Rigid transformation in micomputing does not support [n_dim] dimensional transforms (2 & 3D only). " + 
+        #                                     "Please contact the developers if there are feasible algorithms (Error Code: T333). Thank you. ")
+
+        # if translation is not None:
+        #     translation = bt.to_bttensor(translation)
+        #     if translation.n_dim <= 1 and not translation.has_batch: translation = translation.unsqueeze({})
+        #     if translation.n_dim == 2 and not translation.has_batch: translation = translation.with_batchdim((1 - translation.channel_dimension) if translation.has_channel else 0)
+        #     if translation.n_dim == 2 and not translation.has_channel: translation = translation.with_channeldim(1 - translation.batch_dimension)
+        #     avouch(translation.has_batch and translation.has_channel, f"Please use batorch tensor of size ({{n_batch}}, [n_dim]) for Rigid translation, instead of {translation.shape}. ")
+        #     if n_batch == 1 and translation.n_batch > 1: n_batch = translation.n_batch
+        #     if n_dim is None: n_dim = translation.n_channel
+        #     else: avouch(n_dim == translation.n_channel, "Systematic error. Please contact the developers for details (Error Code: T332). ")
+        #     n_dim = translation.n_channel
+        # if center is not None:
+        #     center = bt.to_bttensor(center)
+        #     if center.n_dim <= 1 and not center.has_batch: center = center.unsqueeze({})
+        #     if center.n_dim == 2 and not center.has_batch: center = center.with_batchdim((1 - center.channel_dimension) if center.has_channel else 0)
+        #     if center.n_dim == 2 and not center.has_channel: center = center.with_channeldim(1 - center.batch_dimension)
+        #     avouch(center.has_batch and center.has_channel, f"Please use batorch tensor of size ({{n_batch}}, [n_dim]) for Rigid center, instead of {center.shape}. ")
+        #     if n_batch == 1 and center.n_batch > 1: n_batch = center.n_batch
+        #     if n_dim is None: n_dim = center.n_channel
+        #     else: avouch(n_dim == center.n_channel, f"Center({center.n_channel}D) and translation([n_dim]D) in trans.Rigid should have the same dimension. ")
+        #     n_dim = center.n_channel
+        # if axis is not None:
+        #     axis = bt.to_bttensor(axis)
+        #     if axis.n_dim <= 1 and not axis.has_batch: axis = axis.unsqueeze({})
+        #     if axis.n_dim == 2 and not axis.has_batch: axis = axis.with_batchdim((1 - axis.channel_dimension) if axis.has_channel else 0)
+        #     if axis.n_dim == 2 and not axis.has_channel: axis = axis.with_channeldim(1 - axis.batch_dimension)
+        #     avouch(axis.has_batch and axis.has_channel, f"Please use batorch tensor of size ({{n_batch}}, [n_dim]) for Rigid axises, instead of {axis.shape}. ")
+        #     if ((axis.norm() - 1) ** 2).sum().sum() >= 1e-2:
+        #         print("warning: param. axises for 'Rigid' transformation should be norm-1 vectors, auto-normalization would be performed. Please contact the developers if it is necessary to be non-unit vectors (Error Code: T331). ")
+        #         axis = axis / axis.norm()
+        #     if n_batch == 1 and axis.n_batch > 1: n_batch = axis.n_batch
+        #     if n_dim is None: n_dim = axis.n_channel
+        #     else: avouch(n_dim == axis.n_channel, f"Translation({n_dim}D) and axises({axis.n_channel}D)) in trans.Rigid should have the same dimension. ")
+        # if n_dim is None: n_dim = 2 if axis is None else 3
+        # if translation is None: translation = bt.zeros({n_batch}, [n_dim])
+        # if center is None: center = bt.zeros({n_batch}, [n_dim])
         
         # Now we create the matrix
         angle = angle.float()
         center = center.float()
         translation = translation.float()
         if n_dim == 2:
             A = bt.stack(bt.cos(angle), bt.sin(angle), -bt.sin(angle), bt.cos(angle), -1).splitdim(-1, [2, 2])
@@ -1627,41 +1678,37 @@
 
 @alias("rand_Rig")
 def rand_Rigidity(image, std=1e-1, trans_std=5, **kwargs):
     return Rigid(*Rigid.random_init_params(*image.space, n_batch=image.n_batch, std=std, trans_std=trans_std), **kwargs)
 
 @alias("Aff")
 class Affine(Transformation):
+    """
+    Affine transformation with respect to transformation matrix.
+    
+    Args:
+        matrix (bt.Tensor or np.numpy): the affine matrix. 
+            size: ({n_batch}, [n_dim + 1, n_dim + 1])
+        trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
+        domain (str: 'image-space'|'physical-space'): the coordinate domain that the transformation is in. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, matrix, trans_stretch=None, **kwargs):
-        """
-        Affine transformation with respect to transformation matrix.
-        
-        Args:
-            matrix (bt.Tensor or np.numpy): the affine matrix. 
-                size: ({n_batch}, [n_dim + 1, n_dim + 1])
-            trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
-            domain (str: 'image-space'|'physical-space'): the coordinate domain that the transformation is in. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         matrix = bt.to_bttensor(matrix)
-        n_dim = matrix.size(-1) - 1
-        if matrix.n_dim <= 2: matrix = matrix.unsqueeze({})
-        if not matrix.has_batch: matrix.with_batchdim(0)
-        if matrix.n_dim == 3: matrix.with_n_feature_dim(2)
-        avouch(matrix.n_dim == 3 and matrix.has_batch and matrix.n_feature_dim == 2,
-               f"Please use batorch tensor of size ({{n_batch}}, [n_dim + 1, n_dim + 1]) for Affine parameters, instead of {matrix.shape}. ")
+        bt.input_shape().set(matrix = "({n_batch}, [n_dim + 1, n_dim + 1])")
         if trans_stretch is not None: matrix[..., :n_dim, -1] *= trans_stretch
         super().__init__(matrix, trans_stretch=trans_stretch, **kwargs)
 
-        self.n_dim = matrix.size(-1) - 1
+        self.n_dim = n_dim
         self.trans_stretch = trans_stretch
         self.matrix = matrix
         self.batch_param.append('matrix')
 
     def __call_image_space__(self, X):
         matrix = self.matrix.float()
         n_dim = self.n_dim
@@ -1695,55 +1742,61 @@
 
 @alias("rand_Aff")
 def rand_Affinity(image, std=1e-1, trans_std=5, **kwargs):
     return Affine(*Affine.random_init_params(*image.space, n_batch=image.n_batch, std=std, trans_std=trans_std), **kwargs)
 
 @alias("logEu", "logEuclidean")
 class PolyAffine(Transformation):
-    def __init__(self, dmatrices, masks, order=2, level=4, is_inv=False, trans_stretch=None, **kwargs):
-        """
-        Poly affine transformation with respect to transformation matrices [1].
-        Note that dmatrices for this tranformation IS NOT the actual affine matrices, but IS a differentiation instead.
-        
-        Args:
-            dmatrices (bt.Tensor or np.numpy): One affine matrix for each region. 
-                size: ({n_batch}, [n_region], [n_dim + 1, n_dim + 1])
-            masks (bt.Tensor or np.numpy): One 0-1 mask for each region. 
-                size: ({n_batch}, [n_region], n_1, n_2, ..., n_r) [r=n_dim]
-            order (int): the order of interpolation coefficient. The influence of an affine decays at a rate of 1 / distanceᵒʳᵈᵉʳ. Defaults to 2. 
-            level (int): the level of velocity integration. The dmatrix is regarded as 1 / 2ˡᵉᵛᵉˡ of true matrix. Defaults to 4. 
-            trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    Poly affine transformation with respect to transformation matrices [1].
+    Note that dmatrices for this tranformation IS NOT the actual affine matrices, but IS a differentiation instead.
+    
+    Args:
+        dmatrices (bt.Tensor or np.numpy): One affine matrix for each region. 
+            size: ({n_batch}, [n_region], [n_dim + 1, n_dim + 1])
+        masks (bt.Tensor or np.numpy): One 0-1 mask for each region. 
+            size: ({n_batch}, [n_region], n_1, n_2, ..., n_r) [r=n_dim]
+        order (int): the order of interpolation coefficient. The influence of an affine decays at a rate of 1 / distanceᵒʳᵈᵉʳ. Defaults to 2. 
+        level (int): the level of velocity integration. The dmatrix is regarded as 1 / 2ˡᵉᵛᵉˡ of true matrix. Defaults to 4. 
+        trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
 
-        [1] Arsigny V , Commowick O , Ayache N , et al. A Fast and Log-Euclidean Polyaffine Framework for Locally 
-            Linear Registration[J]. Journal of Mathematical Imaging & Vision, 2009, 33(2):222-238.
-        """
+    [1] Arsigny V , Commowick O , Ayache N , et al. A Fast and Log-Euclidean Polyaffine Framework for Locally 
+        Linear Registration[J]. Journal of Mathematical Imaging & Vision, 2009, 33(2):222-238.
+    """
+    
+    def __init__(self, dmatrices, masks, order=2, level=4, is_inv=False, trans_stretch=None, **kwargs):
         from .funcs import distance_map
         dmatrices = bt.to_bttensor(dmatrices)
-        if dmatrices.n_dim <= 3 and not dmatrices.has_batch: dmatrices = dmatrices.unsqueeze({})
-        if dmatrices.n_feature_dim < 3 and not dmatrices.has_feature: dmatrices = dmatrices.unsqueeze([1])
-        if dmatrices.n_dim == 4 and dmatrices.shape[2] == dmatrices.shape[3]:
-            if not dmatrices.has_batch: dmatrices.batch_dimension = 0
-            if not dmatrices.has_feature: dmatrices.n_feature_dim = 3
-        avouch(dmatrices.has_batch and dmatrices.n_feature_dim == 3, "Please use batorch tensor of size ({n_batch}, [n_region]," +
-               f"[n_dim + 1, n_dim + 1]) for PolyAffine parameters, instead of {dmatrices.shape}. ")
-        n_dim = dmatrices.size(-1) - 1
-        if trans_stretch is not None: dmatrices[..., :n_dim, -1] *= trans_stretch
-        masks = bt.to_bttensor(masks)
-        if masks.n_dim <= n_dim + 1 and not masks.has_batch: masks = masks.unsqueeze({})
-        if masks.n_dim <= n_dim + 1 and not masks.has_channel: masks = masks.unsqueeze([])
-        if masks.n_dim == n_dim + 2 and not masks.has_batch: masks.batch_dimension = 0
-        if masks.n_dim == n_dim + 2 and not masks.has_channel: masks.channel_dimension = 1
-        avouch(masks.has_batch and masks.has_channel, "Please use batorch tensor of size ({n_batch}, [n_region]," +
-               f"n_1, n_2, ..., n_r) [r=n_dim] for PolyAffine parameters, instead of {masks.shape}. ")
+        masks = bt.to_bttensor(masks).int()
+        bt.input_shape().set(
+            dmatrices = "({n_batch}, [n_region], [n_dim + 1, n_dim + 1])", 
+            masks = "({n_batch}, [n_region], n_1, ..., n_r) [r=n_dim]"
+        )
+        # if dmatrices.n_dim <= 3 and not dmatrices.has_batch: dmatrices = dmatrices.unsqueeze({})
+        # if dmatrices.n_feature_dim < 3 and not dmatrices.has_feature: dmatrices = dmatrices.unsqueeze([1])
+        # if dmatrices.n_dim == 4 and dmatrices.shape[2] == dmatrices.shape[3]:
+        #     if not dmatrices.has_batch: dmatrices.batch_dimension = 0
+        #     if not dmatrices.has_feature: dmatrices.n_feature_dim = 3
+        # avouch(dmatrices.has_batch and dmatrices.n_feature_dim == 3, "Please use batorch tensor of size ({n_batch}, [n_region]," +
+        #        f"[n_dim + 1, n_dim + 1]) for PolyAffine parameters, instead of {dmatrices.shape}. ")
+        # n_dim = dmatrices.size(-1) - 1
+        # if trans_stretch is not None: dmatrices[..., :n_dim, -1] *= trans_stretch
+        # masks = bt.to_bttensor(masks)
+        # if masks.n_dim <= n_dim + 1 and not masks.has_batch: masks = masks.unsqueeze({})
+        # if masks.n_dim <= n_dim + 1 and not masks.has_channel: masks = masks.unsqueeze([])
+        # if masks.n_dim == n_dim + 2 and not masks.has_batch: masks.batch_dimension = 0
+        # if masks.n_dim == n_dim + 2 and not masks.has_channel: masks.channel_dimension = 1
+        # avouch(masks.has_batch and masks.has_channel, "Please use batorch tensor of size ({n_batch}, [n_region]," +
+        #        f"n_1, n_2, ..., n_r) [r=n_dim] for PolyAffine parameters, instead of {masks.shape}. ")
 
         # preprocess masks ({n_batch}, [n_region], n_1, n_2, ..., n_r) [r=n_dim]
         n_batch = masks.n_batch
         n_region = masks.n_channel
         dis = distance_map(masks)
         dis = (dis + 1).clamp(0)
         # import micomputing.plot as plt
@@ -1833,53 +1886,59 @@
         
 @alias("rand_logEu", "rand_logEuclidean")
 def rand_PolyAffine(image, n_region=3, std=1e-2, trans_std=1, **kwargs):
     return PolyAffine(*PolyAffine.random_init_params(*image.space, n_batch=image.n_batch, n_region=n_region, std=std, trans_std=trans_std), **kwargs)
 
 @alias("LARM")
 class LocallyAffine(Transformation):
-    def __init__(self, matrices, masks, order=2, trans_stretch=None, avoid_conflict=True, **kwargs):
-        """
-        Locally affine transformation with respect to transformation matrices [1].
-        
-        Args:
-            matrices (bt.Tensor or np.numpy): One affine matrix for each region. 
-                size: ({n_batch}, [n_region], [n_dim + 1, n_dim + 1])
-            masks (bt.Tensor or np.numpy): One 0-1 mask for each region. 
-                size: ({n_batch}, [n_region], n_1, n_2, ..., n_r) [r=n_dim]
-            order (int): the order of interpolation coefficient. The influence of an affine decays at a rate of 1 / distance^order.
-            trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    Locally affine transformation with respect to transformation matrices [1].
+    
+    Args:
+        matrices (bt.Tensor or np.numpy): One affine matrix for each region. 
+            size: ({n_batch}, [n_region], [n_dim + 1, n_dim + 1])
+        masks (bt.Tensor or np.numpy): One 0-1 mask for each region. 
+            size: ({n_batch}, [n_region], n_1, n_2, ..., n_r) [r=n_dim]
+        order (int): the order of interpolation coefficient. The influence of an affine decays at a rate of 1 / distance^order.
+        trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
 
-        [1] Zhuang X , Rhode K , Arridge S , et al. An Atlas-Based Segmentation Propagation Framework Using Locally Affine 
-            Registration - Application to Automatic Whole Heart Segmentation[J]. Springer, Berlin, Heidelberg, 2008.
-        """
+    [1] Zhuang X , Rhode K , Arridge S , et al. An Atlas-Based Segmentation Propagation Framework Using Locally Affine 
+        Registration - Application to Automatic Whole Heart Segmentation[J]. Springer, Berlin, Heidelberg, 2008.
+    """
+    
+    def __init__(self, matrices, masks, order=2, trans_stretch=None, avoid_conflict=True, **kwargs):
         from .funcs import dilate, distance_map
         matrices = bt.to_bttensor(matrices)
-        if matrices.n_dim <= 3 and not matrices.has_batch: matrices = matrices.unsqueeze({})
-        if matrices.n_dim <= 3 and not matrices.has_channel: matrices = matrices.unsqueeze([1])
-        if matrices.n_dim == 4 and matrices.shape[2] == matrices.shape[3]:
-            if not matrices.has_batch: matrices.batch_dimension = 0
-            if not matrices.has_feature: matrices.n_feature_dim = 3
-        avouch(matrices.has_batch and matrices.n_feature_dim == 3, "Please use batorch tensor of size ({n_batch}, [n_region]," +
-               f"[n_dim + 1, n_dim + 1]) for LocallyAffine parameters, instead of {matrices.shape}. ")
-        n_dim = matrices.size(-1) - 1
-        if trans_stretch is not None: matrices[..., :n_dim, -1] *= trans_stretch
         masks = bt.to_bttensor(masks).int()
-        if masks.n_dim <= n_dim + 1 and not masks.has_batch: masks = masks.unsqueeze({})
-        if masks.n_dim <= n_dim + 1 and not masks.has_channel: masks = masks.unsqueeze([])
-        if masks.n_dim == n_dim + 2 and not masks.has_batch: masks.batch_dimension = 0
-        if masks.n_dim == n_dim + 2 and not masks.has_channel: masks.channel_dimension = 1
-        avouch(masks.has_batch and masks.has_channel, "Please use batorch tensor of size ({n_batch}, [n_region]," + 
-               f"n_1, n_2, ..., n_r) [r=n_dim] for LocallyAffine parameters, instead of {masks.shape}. ")
+        bt.input_shape().set(
+            matrices = "({n_batch}, [n_region], [n_dim + 1, n_dim + 1])", 
+            masks = "({n_batch}, [n_region], n_1, ..., n_r) [r=n_dim]"
+        )
+        # if matrices.n_dim <= 3 and not matrices.has_batch: matrices = matrices.unsqueeze({})
+        # if matrices.n_dim <= 3 and not matrices.has_channel: matrices = matrices.unsqueeze([1])
+        # if matrices.n_dim == 4 and matrices.shape[2] == matrices.shape[3]:
+        #     if not matrices.has_batch: matrices.batch_dimension = 0
+        #     if not matrices.has_feature: matrices.n_feature_dim = 3
+        # avouch(matrices.has_batch and matrices.n_feature_dim == 3, "Please use batorch tensor of size ({n_batch}, [n_region]," +
+        #        f"[n_dim + 1, n_dim + 1]) for LocallyAffine parameters, instead of {matrices.shape}. ")
+        # n_dim = matrices.size(-1) - 1
+        # if trans_stretch is not None: matrices[..., :n_dim, -1] *= trans_stretch
+        # masks = bt.to_bttensor(masks).int()
+        # if masks.n_dim <= n_dim + 1 and not masks.has_batch: masks = masks.unsqueeze({})
+        # if masks.n_dim <= n_dim + 1 and not masks.has_channel: masks = masks.unsqueeze([])
+        # if masks.n_dim == n_dim + 2 and not masks.has_batch: masks.batch_dimension = 0
+        # if masks.n_dim == n_dim + 2 and not masks.has_channel: masks.channel_dimension = 1
+        # avouch(masks.has_batch and masks.has_channel, "Please use batorch tensor of size ({n_batch}, [n_region]," + 
+        #        f"n_1, n_2, ..., n_r) [r=n_dim] for LocallyAffine parameters, instead of {masks.shape}. ")
 
         # preprocess masks
         n_batch = matrices.n_batch
         n_region = matrices.size(1)
         if avoid_conflict:
             Gi = Affine(matrices.mergedims([0], {}))
             GiVi = interpolation(masks.mergedims([], {}), Gi.inv(), method='Nearest').splitdim({}, {n_batch}, [n_region]) # ({n_batch}, [n_region], n_1, n_2, ..., n_r) [r=n_dim]
@@ -1958,52 +2017,53 @@
     
 @alias("rand_LARM")
 def rand_LocallyAffine(image, n_region=3, std=1e-1, trans_std=5, **kwargs):
     return LocallyAffine(*LocallyAffine.random_init_params(*image.space, n_batch=image.n_batch, n_region=n_region, std=std, trans_std=trans_std), **kwargs)
 
 @alias("FFD")
 class FreeFormDeformation(Transformation):
+    """
+    Free Form Deformation (FFD) transformation [1].
+    
+    Args:
+        offsets (bt.Tensor): the FFD offsets. 
+            size: ({n_batch}, [n_dim], m_1, m_2, ..., m_r) [r=n_dim]
+            for m_1 x m_2 x ... x m_r grid of Δcontrol points
+        spacing (int or tuple): FFD spacing; spacing between FFD control points, in px. Defaults to 1px. 
+        origin (int or tuple): FFD origin; coordinate for the (0, 0, 0) control point. Defaults to (0, 0, 0). 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+            
+    [1] Rueckert D , Sonoda L I , Hayes C , et al. Nonrigid registration using free-form deformations: 
+        application to breast MR images[J]. IEEE Transactions on Medical Imaging, 1999(8).
+    """
 
     def __init__(self, offsets, spacing=1, origin=0, **kwargs):
-        """
-        Free Form Deformation (FFD) transformation [1].
-        
-        Args:
-            offsets (bt.Tensor): the FFD offsets. 
-                size: ({n_batch}, [n_dim], m_1, m_2, ..., m_r) [r=n_dim]
-                for m_1 x m_2 x ... x m_r grid of Δcontrol points
-            spacing (int or tuple): FFD spacing; spacing between FFD control points, in px. Defaults to 1px. 
-            origin (int or tuple): FFD origin; coordinate for the (0, 0, 0) control point. Defaults to (0, 0, 0). 
-            
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-                
-        [1] Rueckert D , Sonoda L I , Hayes C , et al. Nonrigid registration using free-form deformations: 
-            application to breast MR images[J]. IEEE Transactions on Medical Imaging, 1999(8).
-        """
         offsets = bt.to_bttensor(offsets)
-        if not offsets.has_channel:
-            if offsets.size(0) == offsets.n_dim - 1:
-                n_dim = offsets.size(0)
-                offsets.channel_dimension = 0
-                offsets = offsets.unsqueeze({})
-            elif offsets.size(1) == offsets.n_dim - 2:
-                n_dim = offsets.size(1)
-                offsets.channel_dimension = 1
-            else: raise TypeError(f"FFD parameters with size {offsets.shape} donot match ({{n_batch}}, [n_dim], m_1, m_2, ..., m_r) [r=n_dim]. ")
-        if not offsets.has_batch:
-            n_dim = offsets.n_channel
-            if offsets.n_dim <= n_dim + 1: offsets = offsets.unsqueeze({})
-            else: offsets.batch_dimension = 0
-        avouch(offsets.has_batch and offsets.has_channel, f"Please use batorch tensor of size \
-            ({{n_batch}}, [n_dim], m_1, m_2, ..., m_r) [r=n_dim] for FFD parameters, instead of {offsets.shape}. ")
-        n_dim = offsets.n_channel
+        bt.input_shape().set(offsets = "({n_batch}, [n_dim], m_1, ..., m_r) [r=n_dim]")
+        # if not offsets.has_channel:
+        #     if offsets.size(0) == offsets.n_dim - 1:
+        #         n_dim = offsets.size(0)
+        #         offsets.channel_dimension = 0
+        #         offsets = offsets.unsqueeze({})
+        #     elif offsets.size(1) == offsets.n_dim - 2:
+        #         n_dim = offsets.size(1)
+        #         offsets.channel_dimension = 1
+        #     else: raise TypeError(f"FFD parameters with size {offsets.shape} donot match ({{n_batch}}, [n_dim], m_1, m_2, ..., m_r) [r=n_dim]. ")
+        # if not offsets.has_batch:
+        #     n_dim = offsets.n_channel
+        #     if offsets.n_dim <= n_dim + 1: offsets = offsets.unsqueeze({})
+        #     else: offsets.batch_dimension = 0
+        # avouch(offsets.has_batch and offsets.has_channel, f"Please use batorch tensor of size \
+        #     ({{n_batch}}, [n_dim], m_1, m_2, ..., m_r) [r=n_dim] for FFD parameters, instead of {offsets.shape}. ")
+        # n_dim = offsets.n_channel
         spacing = to_tuple(spacing)
         origin = to_tuple(origin)
         if len(spacing) == 1: spacing *= n_dim
         if len(origin) == 1: origin *= n_dim
         super().__init__(offsets, spacing=spacing, origin=origin, **kwargs)
 
         self.n_dim = n_dim
@@ -2075,48 +2135,50 @@
 @alias("rand_FFD")
 def rand_FreeFormDeformation(image, spacing=None, std=10, **kwargs):
     if spacing is None: spacing = 1 << (int(math.log2(min(image.space))) - 3)
     return FreeFormDeformation(*FreeFormDeformation.random_init_params(*image.space, spacing=spacing, n_batch=image.n_batch, std=std), spacing=spacing, **kwargs)
 
 @alias("DDF")
 class DenseDisplacementField(Transformation):
+    """
+    Dense Displacement Field (DDF) transformation.
+    
+    Args:
+        displacements (bt.Tensor): the displacement of each voxel (or pixel). 
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        shape (bt.Size or tuple): the shape of displacement (needed if input displacement is a transformation). 
+        interpolate (bool): Whether to force interpolation in apply. 
+
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, displacements, shape=None, interpolate=False, **kwargs):
-        """
-        Dense Displacement Field (DDF) transformation.
-        
-        Args:
-            displacements (bt.Tensor): the displacement of each voxel (or pixel). 
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            shape (bt.Size or tuple): the shape of displacement (needed if input displacement is a transformation). 
-            interpolate (bool): Whether to force interpolation in apply. 
-
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         if isinstance(displacements, Transformation): displacements = displacements.toDDF(shape)
-        displacements = bt.to_bttensor(displacements)
-        if not displacements.has_channel:
-            if displacements.size(0) == displacements.n_dim - 1:
-                n_dim = displacements.size(0)
-                displacements.channel_dimension = 0
-                displacements = displacements.unsqueeze({})
-            elif displacements.size(1) == displacements.n_dim - 2:
-                n_dim = displacements.size(1)
-                displacements.channel_dimension = 1
-            else: raise TypeError(f"DDF parameters with size {displacements.shape} donot match ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]. ")
-        if not displacements.has_batch:
-            n_dim = displacements.n_channel
-            if displacements.n_dim <= n_dim + 1: displacements = displacements.unsqueeze({})
-            else: displacements.batch_dimension = 0
-        displacements = displacements.float()
-        avouch(displacements.has_batch and displacements.has_channel, f"Please use batorch tensor of size \
-            ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim] for DDF parameters, instead of {displacements.shape}. ")
+        displacements = bt.to_bttensor(displacements).float()
+        bt.input_shape().set(displacements = "({n_batch}, [n_dim], n_1, ..., n_r) [r=n_dim]")
+        # if not displacements.has_channel:
+        #     if displacements.size(0) == displacements.n_dim - 1:
+        #         n_dim = displacements.size(0)
+        #         displacements.channel_dimension = 0
+        #         displacements = displacements.unsqueeze({})
+        #     elif displacements.size(1) == displacements.n_dim - 2:
+        #         n_dim = displacements.size(1)
+        #         displacements.channel_dimension = 1
+        #     else: raise TypeError(f"DDF parameters with size {displacements.shape} donot match ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]. ")
+        # if not displacements.has_batch:
+        #     n_dim = displacements.n_channel
+        #     if displacements.n_dim <= n_dim + 1: displacements = displacements.unsqueeze({})
+        #     else: displacements.batch_dimension = 0
+        # displacements = displacements.float()
+        # avouch(displacements.has_batch and displacements.has_channel, f"Please use batorch tensor of size \
+        #     ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim] for DDF parameters, instead of {displacements.shape}. ")
         super().__init__(displacements, shape=shape, interpolate=interpolate, **kwargs)
         self.n_dim = displacements.n_channel
         self.displacements = displacements
         self.interpolate = interpolate
         self.batch_param.append('displacements')
 
     # parameter alias
@@ -2144,50 +2206,52 @@
 
 @alias("rand_DDF")
 def rand_DenseDisplacementField(image, std=1, **kwargs):
     return DenseDisplacementField(*DenseDisplacementField.random_init_params(*image.space, n_batch=image.n_batch, std=std), **kwargs)
 
 @alias("VF")
 class VelocityField(Transformation):
+    """
+    Velocity Field (VF) transformation.
+    
+    Args:
+        scaled_velocities (bt.Tensor): the velocity at each voxel (or pixel), scaled to displacement level. 
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        shape (bt.Size or tuple): the shape of velocity (needed if input is a transformation). 
+        interpolate (bool): Whether to force interpolation in apply. 
+        level (int): the level of velocity, the transformation in delta time 1 / 2ˡᵉᵛᵉˡ is,
+            dT = V / 2ˡᵉᵛᵉˡ. Therefore, the total transformation is dT∘ ⋯ ∘dT for 2ˡᵉᵛᵉˡ times.
+
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+    
     def __init__(self, scaled_velocities, shape=None, interpolate=False, level=4, **kwargs):
-        """
-        Velocity Field (VF) transformation.
-        
-        Args:
-            scaled_velocities (bt.Tensor): the velocity at each voxel (or pixel), scaled to displacement level. 
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            shape (bt.Size or tuple): the shape of velocity (needed if input is a transformation). 
-            interpolate (bool): Whether to force interpolation in apply. 
-            level (int): the level of velocity, the transformation in delta time 1 / 2ˡᵉᵛᵉˡ is,
-                dT = V / 2ˡᵉᵛᵉˡ. Therefore, the total transformation is dT∘ ⋯ ∘dT for 2ˡᵉᵛᵉˡ times.
-
-        Args for __call__:
-            X (bt.Tensor): Coordinates to be transformed.
-                size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed coordinates.
-                size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-        """
         if isinstance(scaled_velocities, Transformation): scaled_velocities = scaled_velocities.toDDF(shape)
-        scaled_velocities = bt.to_bttensor(scaled_velocities)
-        if not scaled_velocities.has_channel:
-            if scaled_velocities.size(0) == scaled_velocities.n_dim - 1:
-                n_dim = scaled_velocities.size(0)
-                scaled_velocities.channel_dimension = 0
-                scaled_velocities = scaled_velocities.unsqueeze({})
-            elif scaled_velocities.size(1) == scaled_velocities.n_dim - 2:
-                n_dim = scaled_velocities.size(1)
-                scaled_velocities.channel_dimension = 1
-            else: raise TypeError(f"DDF parameters with size {scaled_velocities.shape} donot match ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]. ")
-        if not scaled_velocities.has_batch:
-            n_dim = scaled_velocities.n_channel
-            if scaled_velocities.n_dim <= n_dim + 1: scaled_velocities = scaled_velocities.unsqueeze({})
-            else: scaled_velocities.batch_dimension = 0
-        scaled_velocities = scaled_velocities.float()
-        avouch(scaled_velocities.has_batch and scaled_velocities.has_channel, f"Please use batorch tensor of size \
-            ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim] for DDF parameters, instead of {scaled_velocities.shape}. ")
+        scaled_velocities = bt.to_bttensor(scaled_velocities).float()
+        bt.input_shape().set(scaled_velocities = "({n_batch}, [n_dim], n_1, ..., n_r) [r=n_dim]")
+        # if not scaled_velocities.has_channel:
+        #     if scaled_velocities.size(0) == scaled_velocities.n_dim - 1:
+        #         n_dim = scaled_velocities.size(0)
+        #         scaled_velocities.channel_dimension = 0
+        #         scaled_velocities = scaled_velocities.unsqueeze({})
+        #     elif scaled_velocities.size(1) == scaled_velocities.n_dim - 2:
+        #         n_dim = scaled_velocities.size(1)
+        #         scaled_velocities.channel_dimension = 1
+        #     else: raise TypeError(f"DDF parameters with size {scaled_velocities.shape} donot match ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]. ")
+        # if not scaled_velocities.has_batch:
+        #     n_dim = scaled_velocities.n_channel
+        #     if scaled_velocities.n_dim <= n_dim + 1: scaled_velocities = scaled_velocities.unsqueeze({})
+        #     else: scaled_velocities.batch_dimension = 0
+        # scaled_velocities = scaled_velocities.float()
+        # avouch(scaled_velocities.has_batch and scaled_velocities.has_channel, f"Please use batorch tensor of size \
+        #     ({{n_batch}}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim] for DDF parameters, instead of {scaled_velocities.shape}. ")
         super().__init__(scaled_velocities, shape=shape, interpolate=interpolate, level=level, **kwargs)
         self.n_dim = scaled_velocities.n_channel
         self.scaled_velocities = scaled_velocities
         self.interpolate = interpolate
         self.level = level
         self.batch_param.append('scaled_velocities')
     
@@ -2214,87 +2278,97 @@
         if not self.interpolate and X.space == displacements.space and X.n_channel == displacements.n_channel: return X + displacements
         else: return X + interpolation(displacements, target_space=X)
 
 @alias("rand_VF")
 def rand_VelocityField(image, std=10, level=4, **kwargs):
     return VelocityField(*VelocityField.random_init_params(*image.space, n_batch=image.n_batch, std=std), level=level, **kwargs)
 
-# @alias("MLP")
-# class MultiLayerPerception(Transformation):
-#     def __init__(self, weights, hidden_layers=[], active_function=None, trans_stretch=1, residual=True):
-#         """
-#         A transformation defined by a MLP. 
-        
-#         Args:
-#             weights (bt.Tensor): the weights for the perception network. 
-#                 size: ({n_batch}, n_dim * n_hl_1 + n_hl_1 + sum(i=1..k-1){n_hl_i * n_hl_{i+1} + n_hl_{i+1}} + n_hl_k * n_dim + n_dim)
-#                 where k is the number of hidden layers and n_hl_i is the length of the i-th hidden layer. 
-#             hidden_layers (list of int): the lengths for the hidden layers, i.e. [n_hl_1, n_hl_2, ..., n_hl_k]
-#                 It is by default '[]' so that the default MLP is an affine transformation. 
-#             active_function (class): the active_function. 
-#             trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
-            
-#         Args for __call__:
-#             X (bt.Tensor): Coordinates to be transformed.
-#                 size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-#             Returns (bt.Tensor): The transformed coordinates.
-#                 size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
-#         """
-#         self.hidden_layers = hidden_layers
-#         if not weights.has_batch:
-#             if weights.n_dim == 2: weights.batch_dim = 0
-#             else: weights = weights.unsqueeze([])
-#         self.weights = weights
-#         self.trans_stretch = trans_stretch
-#         super().__init__(weights, hidden_layers = hidden_layers, trans_stretch = trans_stretch, residual = residual)
-#         dim_const = weights.size(-1) - sum(hidden_layers) - sum(x * y for x, y in zip(hidden_layers[:-1], hidden_layers[1:]))
-#         dim_coeff = hidden_layers[0] + hidden_layers[-1] + 1
-#         avouch(dim_const % dim_coeff == 0, f"Wrong weight length for hidden layers of sizes {hidden_layers}, {dim_coeff} x n_dim + {dim_const} expected, but got {weights.size(-1)}.")
-#         self.n_dim = dim_const // dim_coeff
-#         self.n_batch = weights.n_batch
-#         self.layers = []
-#         p = 0
-#         for i in range(len(hidden_layers) + 1):
-#             in_features = self.n_dim if i == 0 else hidden_layers[i - 1]
-#             out_features = self.n_dim if i == len(hidden_layers) else hidden_layers[i]
-#             layer_weights = weights[..., p:p+out_features*in_features].view([self.n_batch], out_features, in_features)
-#             p += out_features * in_features
-#             layer_bias = weights[..., p:p+out_features].view([self.n_batch], out_features)
-#             p += out_features
-#             self.layers.append((layer_weights, layer_bias))
-#         self.active_function = active_function
-#         self.residual = residual
-#         if self.active_function is None: self.active_function = bt.nn.ReLU
+@alias("MLP")
+class MultiLayerPerception(Transformation):
+    """
+    A transformation defined by a MLP. 
     
-#     @classmethod
-#     def get_weight_length(cls, n_dim, *hidden_layers):
-#         hidden_layers = arg_tuple(hidden_layers)
-#         return n_dim * (hidden_layers[0] + hidden_layers[-1] + 1) \
-#             + sum(hidden_layers) + sum(x * y for x, y in zip(hidden_layers[:-1], hidden_layers[1:]))
+    Args:
+        weights (bt.Tensor): the weights for the perception network. 
+            size: ({n_batch}, n_dim * n_hl_1 + n_hl_1 + sum(i=1..k-1){n_hl_i * n_hl_{i+1} + n_hl_{i+1}} + n_hl_k * n_dim + n_dim)
+            where k is the number of hidden layers and n_hl_i is the length of the i-th hidden layer. 
+        hidden_layers (list of int): the lengths for the hidden layers, i.e. [n_hl_1, n_hl_2, ..., n_hl_k]
+            It is by default '[]' so that the default MLP is an affine transformation. 
+        active_function (class): the active_function. 
+        trans_stretch (float): scaling of translation movement, commonly needed in iterative parameter training, 1 by default. 5 seems to be a good choice. 
+        
+    Args for __call__:
+        X (bt.Tensor): Coordinates to be transformed.
+            size: ({n_batch: optional}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed coordinates.
+            size: ({n_batch}, [n_dim], n_1, n_2, ..., n_r) [r=n_dim]
+    """
     
-#     @property
-#     def n_weight_length(self):
-#         return MultiLayerPerception.get_weight_length(self.n_dim, self.hidden_layers)
+    def __init__(self, weights, hidden_layers=[], active_function=None, trans_stretch=1, residual=True):
+        self.hidden_layers = hidden_layers
+        n_hl = sum(x * y for x, y in zip(hidden_layers[:-1], hidden_layers[1:])) + sum(hidden_layers)
+        n_hl_1 = hidden_layers[0]
+        n_hl_k = hidden_layers[-1]
+        bt.input_shape(n_hl=n_hl, n_hl_1=n_hl_1, n_hl_k=n_hl_k).set(weights = "({n_batch}, n_dim * n_hl_1 + n_hl + n_hl_k * n_dim + n_dim)")
+        # if not weights.has_batch:
+        #     if weights.n_dim == 2: weights.batch_dim = 0
+        #     else: weights = weights.unsqueeze([])
+        self.weights = weights
+        self.trans_stretch = trans_stretch
+        super().__init__(weights, hidden_layers = hidden_layers, trans_stretch = trans_stretch, residual = residual)
+        dim_const = weights.size(-1) - n_hl
+        dim_coeff = n_hl_1 + n_hl_k + 1
+        avouch(dim_const % dim_coeff == 0, f"Wrong weight length for hidden layers of sizes {hidden_layers}, {dim_coeff} x n_dim + {dim_const} expected, but got {weights.size(-1)}.")
+        self.n_dim = dim_const // dim_coeff
+        self.n_batch = weights.n_batch
+        self.layers = []
+        p = 0
+        for i in range(len(hidden_layers) + 1):
+            in_features = self.n_dim if i == 0 else hidden_layers[i - 1]
+            out_features = self.n_dim if i == len(hidden_layers) else hidden_layers[i]
+            layer_weights = weights[..., p:p+out_features*in_features].view({self.n_batch}, out_features, in_features)
+            p += out_features * in_features
+            layer_bias = weights[..., p:p+out_features].view({self.n_batch}, out_features)
+            p += out_features
+            self.layers.append((layer_weights, layer_bias))
+        self.active_function = active_function
+        self.residual = residual
+        if self.active_function is None: self.active_function = bt.nn.ReLU
     
-#     @classmethod
-#     def random_init_params(cls, n_dim, *hidden_layers, n_batch=1, std=1e-4):
-#         hidden_layers = arg_tuple(hidden_layers)
-#         n_length = MultiLayerPerception.get_weight_length(n_dim, hidden_layers)
-#         return std * bt.randn({n_batch}, n_length)
+    @classmethod
+    def get_weight_length(cls, n_dim, *hidden_layers):
+        hidden_layers = arg_tuple(hidden_layers)
+        return n_dim * (hidden_layers[0] + hidden_layers[-1] + 1) \
+            + sum(hidden_layers) + sum(x * y for x, y in zip(hidden_layers[:-1], hidden_layers[1:]))
     
-#     def __call__(self, X):
-#         if not X.has_space: X = X.unsqueeze(-1)
-#         Y = X.flatten(...).channel_dim_(None)
-#         for i, (weights, bias) in enumerate(self.layers):
-#             Y = weights @ Y
-#             if i < len(self.layers) - 1: Y = self.active_function()(Y + bias.unsqueeze(-1))
-#             else: Y += self.trans_stretch * bias.unsqueeze(-1)
-#         if self.residual:
-#             return X + Y.view_as(X).channel_dimension_(1)
-#         else: return Y.view_as(X).channel_dimension_(1)
+    @property
+    def n_weight_length(self):
+        return MultiLayerPerception.get_weight_length(self.n_dim, self.hidden_layers)
+    
+    @classmethod
+    def random_init_params(cls, n_dim, *hidden_layers, n_batch=1, std=1e-4):
+        hidden_layers = arg_tuple(hidden_layers)
+        n_length = MultiLayerPerception.get_weight_length(n_dim, hidden_layers)
+        return std * bt.randn({n_batch}, n_length)
+    
+    def __call__(self, X):
+        if not X.has_space: X = X.unsqueeze(-1)
+        Y = X.flatten(...).with_feature_dim(None)
+        for i, (weights, bias) in enumerate(self.layers):
+            Y = weights @ Y
+            if i < len(self.layers) - 1: Y = self.active_function()(Y + bias.unsqueeze(-1))
+            else: Y += self.trans_stretch * bias.unsqueeze(-1)
+        if self.residual:
+            return X + Y.view_as(X)
+        else: return Y.view_as(X)
+
+@alias("rand_MLP")
+def rand_MultiLayerPerception(image, std=10, level=4, **kwargs):
+    hl = [40, 40]
+    return MultiLayerPerception(*MultiLayerPerception.random_init_params(image.n_dim, *hl, n_batch=image.n_batch, std=std), hidden_layers=hl, **kwargs)
 
 # @alias("SAT")
 # class SelfAttentionTransformation(Transformation):
 #     def __init__(self, weights, hidden_layers=[], active_function=None, trans_stretch=1, residual=True):
 #         """
 #         A transformation defined by a Network with self-attention structure. 
         
@@ -2676,28 +2750,29 @@
 #                 if not X.has_channel: X.channel_dimension = 0 if X._batch_dimension > 0 else 1
 #         avouch(X.has_batch and X.has_channel, f"Please use batorch tensor of size \
 #             ({{n_batch}}, [n_channel/n_feature:optional], m_1, m_2, ..., m_r) [r=n_dim] for \
 #                 {self.__name__}, instead of {X.shape}. ")
 #         return X.clone()
 
 class Normalize(Transformation):
-    def __init__(self, *_range):
-        """
-        Normalize the intensity of an image.
+    """
+    Normalize the intensity of an image.
+    
+    Args:
+        _range = (low, high) (int or float or bt.Tensor): The lowest (and highest) intensity. 
+            size: length(2) or ({n_batch:optional}, [n_channel:optional], (2))
         
-        Args:
-            _range = (low, high) (int or float or bt.Tensor): The lowest (and highest) intensity. 
-                size: length(2) or ({n_batch:optional}, [n_channel:optional], (2))
-            
-        Args for __call__:
-            X (bt.Tensor): Image to be transformed.
-                size: ({n_batch:optional}, [n_channel:optional], n_1, n_2, ..., n_r) [r=n_dim]
-            Returns (bt.Tensor): The transformed image.
-                size: ({n_batch}, [n_channel], n_1, n_2, ..., n_r) [r=n_dim]
-        """
+    Args for __call__:
+        X (bt.Tensor): Image to be transformed.
+            size: ({n_batch:optional}, [n_channel:optional], n_1, n_2, ..., n_r) [r=n_dim]
+        Returns (bt.Tensor): The transformed image.
+            size: ({n_batch}, [n_channel], n_1, n_2, ..., n_r) [r=n_dim]
+    """
+
+    def __init__(self, *_range):
         if len(_range) == 0: _range = None
         elif len(_range) == 1 and isinstance(_range[0], (list, tuple)): _range = bt.tensor(list(_range[0])).with_funcdim(True)
         elif len(_range) == 1 and isinstance(_range[0], bt.Tensor): _range = _range[0]
         elif len(_range) == 1 and isinstance(_range[0], int): _range = bt.tensor((0, _range)).with_funcdim(True)
         elif len(_range) == 2 and all(isinstance(r, int) for r in _range): _range = bt.channel_tensor(_range).with_funcdim(True)
         else: raise TypeError(f"Invalid range for Normalize: {_range}. ")
         if _range is None: pass
@@ -2708,14 +2783,15 @@
             if not _range.has_batch: _range.unsqueeze_({})
             if not _range.has_feature: _range.unsqueeze_([])
             avouch(_range.has_batch and _range.has_channel and _range.has_func and _range.func_size == 2, f"Please use batorch tensor of size \
                 ({{n_batch:optional}}, [n_channel:optional], (2)) for Normalizing parameters, instead of {_range.shape}. ")
         super().__init__(_range)
         self.range = _range
         self._range = None
+        self.domain = 'non-spatial'
 
     def __call_non_spatial__(self, X):
         _range = self.range
         if _range is None:
             _range = bt.quantile(X.flatten(...).float(), bt.to_bttensor([0.025, 0.975]), -1).movedim(0, -1)
             self._range = _range
         return ((X - _range[..., 0]) / (_range[..., 1] - _range[..., 0])).clamp(0., 1.)
@@ -2723,14 +2799,32 @@
     def __inv__(self):
         if self.range is not None: _range = self.range
         elif self._range is not None: _range = self._range
         else: return Normalize(None)
         den = _range[..., 1] - _range[..., 0]
         _range = bt.stack(-_range[..., 0], 1-_range[..., 0], [-1]) / den
         return Normalize(_range)
+    
+class Cropping(Transformation):
+    """
+    Cropping transformation.
+        
+    Args for __call__:
+        Img (bt.Tensor): Image to be cropped.
+            size: ({n_batch:optional}, [n_channel:optional], n_1, n_2, ..., n_r)
+        Returns (bt.Tensor): The transformed coordinates. 
+            size: ({n_batch}, [n_channel:optional], n_1, n_2, ..., n_r)
+    """
+    def __init__(self, shape, **kwargs):
+        super().__init__(shape=shape, **kwargs)
+        self.reshape = [shape]
+        self.domain = 'non-spatial'
+        
+    def __call_non_spatial__(self, X):
+        return bt.crop_as(X, self.shape)
 
 # ############# Supporting Functions ############
 
 def Bspline(i, U):
     """
     Cubic B-spline function. 
     Note: As long as i and U have the same size, any shape of tensors would do.
```

### Comparing `micomputing-1.1.47/micomputing/zxhtools/TRS.py` & `micomputing-1.1.48/micomputing/zxhtools/TRS.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc` & `micomputing-1.1.48/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc` & `micomputing-1.1.48/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/__pycache__/TRS.cpython-311.pyc` & `micomputing-1.1.48/micomputing/zxhtools/__pycache__/TRS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc` & `micomputing-1.1.48/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc` & `micomputing-1.1.48/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/__pycache__/exec.cpython-311.pyc` & `micomputing-1.1.48/micomputing/zxhtools/__pycache__/exec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/exec.py` & `micomputing-1.1.48/micomputing/zxhtools/exec.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing/zxhtools/image2.FFD` & `micomputing-1.1.48/micomputing/zxhtools/image2.FFD`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/micomputing.egg-info/SOURCES.txt` & `micomputing-1.1.48/micomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.47/setup_micomputing.py` & `micomputing-1.1.48/setup_micomputing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'micomputing',
-	version = '1.1.47',
+	version = '1.1.48',
 	keywords = ['pip', 'pymyc', 'micomputing', 'medical image', 'image registration', 'image similarities'],
 	description = "'micomputing' is a package for medical image computing. ",
 	long_description = None,
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/micomputing',
 	author = 'Yuncheng Zhou',
```

