# Comparing `tmp/dipcoatimage-finitedepth-2.0.2.tar.gz` & `tmp/dipcoatimage_finitedepth-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipcoatimage-finitedepth-2.0.2.tar", last modified: Fri Mar  8 17:45:21 2024, max compression
+gzip compressed data, was "dipcoatimage_finitedepth-2.0.3.tar", last modified: Wed May 22 09:41:10 2024, max compression
```

## Comparing `dipcoatimage-finitedepth-2.0.2.tar` & `dipcoatimage_finitedepth-2.0.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:21.030579 dipcoatimage-finitedepth-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-08 17:45:21.000000 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-08 17:45:21.000000 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:45:21.000000 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-08 17:45:21.000000 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-08 17:45:21.000000 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-08 17:45:21.000000 dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/src/finitedepth/
--rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    39053 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/coatinglayer.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/
--rw-r--r--   0 runner    (1001) docker     (127)   118422 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/coat.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   106139 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/coat.png
--rw-r--r--   0 runner    (1001) docker     (127)    98920 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/ref.png
--rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/src/finitedepth/substrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:21.034579 dipcoatimage-finitedepth-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-08 17:45:17.000000 dipcoatimage-finitedepth-2.0.2/tests/test_analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:41:10.376432 dipcoatimage_finitedepth-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-22 09:41:10.000000 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-22 09:41:10.000000 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:41:10.000000 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-22 09:41:10.000000 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 09:41:10.000000 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 09:41:10.000000 dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/src/finitedepth/
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36448 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/coatinglayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)   118422 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/coat.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   106139 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/coat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98920 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/ref.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/src/finitedepth/substrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:41:10.380432 dipcoatimage_finitedepth-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-22 09:41:06.000000 dipcoatimage_finitedepth-2.0.3/tests/test_analyzers.py
```

### Comparing `dipcoatimage-finitedepth-2.0.2/LICENSE` & `dipcoatimage_finitedepth-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/PKG-INFO` & `dipcoatimage_finitedepth-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipcoatimage-finitedepth
-Version: 2.0.2
+Version: 2.0.3
 Summary: Image analysis for finite depth dip coating process
 Author-email: Jisoo Song <jeesoo9595@snu.ac.kr>
 License: BSD 2-Clause License
         
         Copyright 2024, Jisoo Song
         
         Redistribution and use in source and binary forms, with or without
@@ -46,27 +46,28 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: shapely
 Requires-Dist: numba
+Requires-Dist: shapely>=2.0
+Requires-Dist: curvesimilarities>=0.1.1
 Requires-Dist: PyYAML
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinx-autoapi; extra == "doc"
+Requires-Dist: sphinx-autoapi!=3.1.0; extra == "doc"
 Requires-Dist: sphinx-tabs>=3.4.5; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `dipcoatimage-finitedepth-2.0.2/README.md` & `dipcoatimage_finitedepth-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/pyproject.toml` & `dipcoatimage_finitedepth-2.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dipcoatimage-finitedepth"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
     {name = "Jisoo Song", email = "jeesoo9595@snu.ac.kr"}
 ]
 description = "Image analysis for finite depth dip coating process"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
@@ -26,16 +26,23 @@
     "Topic :: Scientific/Engineering :: Physics",
     "Typing :: Typed",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
 ]
-dynamic = [
-    "dependencies",
+dependencies = [
+    "opencv-python-headless",
+    "numpy",
+    "scipy",
+    "numba",
+    "shapely >= 2.0",
+    "curvesimilarities >= 0.1.1",
+    "PyYAML",
+    "tqdm",
 ]
 
 [project.urls]
 homepage = "https://github.com/dipcoat-image/finitedepth"
 source = "https://github.com/dipcoat-image/finitedepth"
 documentation = "https://dipcoatimage-finitedepth.readthedocs.io"
 
@@ -45,15 +52,15 @@
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 doc = [
     "furo",
     "sphinx",
-    "sphinx-autoapi",
+    "sphinx-autoapi != 3.1.0",
     "sphinx-tabs >= 3.4.5",
     "matplotlib",
 ]
 dev = [
     "flake8",
     "flake8-docstrings",
     "black",
@@ -76,17 +83,14 @@
 Substrate = "finitedepth.substrate:Substrate"
 RectSubstrate = "finitedepth.substrate:RectSubstrate"
 
 [project.entry-points."finitedepth.coatinglayers"]
 CoatingLayer = "finitedepth.coatinglayer:CoatingLayer"
 RectLayerShape = "finitedepth.coatinglayer:RectLayerShape"
 
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
-
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.isort]
 profile = "black"
 
 [tool.docformatter]
```

### Comparing `dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/PKG-INFO` & `dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipcoatimage-finitedepth
-Version: 2.0.2
+Version: 2.0.3
 Summary: Image analysis for finite depth dip coating process
 Author-email: Jisoo Song <jeesoo9595@snu.ac.kr>
 License: BSD 2-Clause License
         
         Copyright 2024, Jisoo Song
         
         Redistribution and use in source and binary forms, with or without
@@ -46,27 +46,28 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: shapely
 Requires-Dist: numba
+Requires-Dist: shapely>=2.0
+Requires-Dist: curvesimilarities>=0.1.1
 Requires-Dist: PyYAML
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinx-autoapi; extra == "doc"
+Requires-Dist: sphinx-autoapi!=3.1.0; extra == "doc"
 Requires-Dist: sphinx-tabs>=3.4.5; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `dipcoatimage-finitedepth-2.0.2/src/dipcoatimage_finitedepth.egg-info/SOURCES.txt` & `dipcoatimage_finitedepth-2.0.3/src/dipcoatimage_finitedepth.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 src/dipcoatimage_finitedepth.egg-info/PKG-INFO
 src/dipcoatimage_finitedepth.egg-info/SOURCES.txt
 src/dipcoatimage_finitedepth.egg-info/dependency_links.txt
 src/dipcoatimage_finitedepth.egg-info/entry_points.txt
 src/dipcoatimage_finitedepth.egg-info/requires.txt
 src/dipcoatimage_finitedepth.egg-info/top_level.txt
 src/finitedepth/__init__.py
```

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/__init__.py` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/cache.py` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/cache.py`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/coatinglayer.py` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/coatinglayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 """Analyze coating layer and similarity measures [#senin]_ [#sim]_.
 
-.. [#senin] P., Senin (2008)
+.. [#senin] Senin, P. (2008).
 .. [#sim] https://pypi.org/project/similaritymeasures/
 """
 
-# TODO: fix docstring formats
-
 import abc
 import dataclasses
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 import cv2
 import numpy as np
 import numpy.typing as npt
-from numba import njit  # type: ignore
+from curvesimilarities import dtw_acm, dtw_owp  # type: ignore
+from scipy.interpolate import splev, splprep  # type: ignore
 from scipy.optimize import root  # type: ignore
 from scipy.spatial.distance import cdist  # type: ignore
-from shapely import LineString, offset_curve  # type: ignore
+from shapely import LineString, get_coordinates, offset_curve  # type: ignore
 
 from .cache import attrcache
 from .substrate import RectSubstrate, SubstrateBase
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 __all__ = [
     "CoatingLayerBase",
     "CoatingLayer",
     "RectLayerShape",
     "images_XOR",
     "images_ANDXOR",
-    "equidistant_interpolate",
+    "sample_polyline",
     "parallel_curve",
-    "acm",
-    "owp",
 ]
 
 
 SubstTypeVar = TypeVar("SubstTypeVar", bound=SubstrateBase)
 """Type variable for the substrate type of :class:`CoatingLayerBase`."""
 DataTypeVar = TypeVar("DataTypeVar", bound="DataclassInstance")
 """Type variable for :attr:`CoatingLayerBase.DataType`."""
@@ -321,16 +318,20 @@
         substrate: Substrate instance.
         opening_ksize: Kernel size for morphological operation.
             Elements must be zero or odd number.
         reconstruct_radius: Radius of the "safe zone" for noise removal.
             Imaginary circles with this radius are drawn on bottom corners of the
             substrate. Connected components not passing these circles are regarded as
             image artifacts.
-        roughness_measure ({`'DTW', 'SDTW'`}): Similarity measure to quantify roughness.
-            `'DTW'` is dynamic time warping and `'SDTW'` is its root mean square.
+        roughness_measure: Similarity measure to quantify roughness.
+
+            `'DTW'`
+                Dynamice time warping.
+            `'SDTW'`
+                Root mean square of dynamic time warping.
         tempmatch: Pre-computed template matching result.
 
     Examples:
         Construct substrate instance first.
 
         .. plot::
             :include-source:
@@ -352,15 +353,15 @@
             :context: close-figs
 
             >>> from finitedepth import RectLayerShape
             >>> img = cv2.imread(get_sample_path("coat.png"), cv2.IMREAD_GRAYSCALE)
             >>> _, bin = cv2.threshold(img, 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
             >>> coat = RectLayerShape(bin, subst, (1, 1), 50, "DTW")
             >>> plt.imshow(
-            ...     coat.draw(conformality_step=10, roughness_step=10)
+            ...     coat.draw(conformality_step=10, roughness_step=1)
             ... ) #doctest: +SKIP
     """
 
     DataType = RectLayerShapeData
     """Return :obj:`RectLayerShapeData`."""
 
     def __init__(
@@ -371,16 +372,15 @@
         reconstruct_radius: int,
         roughness_measure: str,
         *,
         tempmatch: tuple[tuple[int, ...], float] | None = None,
     ):
         """Initialize the instance.
 
-        Check whether kernel size are zero or odd and roughness measure is either
-        `'DTW'` or `'SDTW'`.
+        Check whether kernel size are zero or odd and roughness measure is valid.
         """
         if not all(i == 0 or (i > 0 and i % 2 == 1) for i in opening_ksize):
             raise ValueError("Kernel size must be zero or odd.")
         if roughness_measure not in ["DTW", "SDTW"]:
             raise TypeError(f"Unknown roughness measure: {roughness_measure}")
         super().__init__(image, substrate, tempmatch=tempmatch)
         self._opening_ksize = opening_ksize
@@ -590,66 +590,70 @@
         return (t, parallel_curve(s, t))
 
     @attrcache("_conformality")
     def conformality(self) -> tuple[float, npt.NDArray[np.int32]]:
         """DTW-based conformality of the coating layer.
 
         Returns:
-            Conformality and optimal pairs between substrate surface and layer surface.
+            Conformality between layer surface and substrate surface and its pair of
+            points in curve space.
         """
         if not self.interfaces():
             return (np.nan, np.empty((0, 2), dtype=np.int32))
 
         (i0, i1) = np.sort(np.concatenate(self.interfaces()).flatten())[[0, -1]]
         subst_cnt = self.substrate.contour() + self.substrate_point()
         intf = subst_cnt[i0:i1]
 
         I0, I1 = self.surface()
         surf = self.contour()[I0:I1]
 
         dist = cdist(np.squeeze(surf, axis=1), np.squeeze(intf, axis=1))
-        mat = acm(dist)
-        path = owp(mat)
+        mat = dtw_acm(dist)
+        path = dtw_owp(mat)
         d = dist[path[:, 0], path[:, 1]]
         d_avrg = mat[-1, -1] / len(path)
         C = 1 - np.sum(np.abs(d - d_avrg)) / mat[-1, -1]
-        return (float(C), path)
+        pairs = np.concatenate([surf[path[..., 0]], intf[path[..., 1]]], axis=1)
+        return (float(C), pairs)
 
     @attrcache("_roughness")
-    def roughness(self) -> tuple[float, npt.NDArray[np.int32]]:
-        """DTW-based surface roughness of the coating layer.
+    def roughness(self) -> tuple[float, npt.NDArray[np.float64]]:
+        """Similarity-based surface roughness of the coating layer.
 
         Returns:
-            Roughness and optimal pairs between layer surface and uniform layer.
+            Roughness between layer surface and uniform layer and its pair of points in
+            curve space.
         """
         I0, I1 = self.surface()
         surf = self.contour()[I0:I1]
         _, ul = self.uniform_layer()
 
         if surf.size == 0 or ul.size == 0:
-            return (np.nan, np.empty((0, 2), dtype=np.int32))
+            return (np.nan, np.empty((0, 2), dtype=np.float64))
 
+        ul_len = cv2.arcLength(ul.astype(np.float32), closed=False)
         if self.roughness_measure == "DTW":
-            ul_len = np.ceil(cv2.arcLength(ul.astype(np.float32), closed=False))
-            ul = equidistant_interpolate(ul, int(ul_len))
+            ul = sample_polyline(ul, int(np.ceil(ul_len)))
             dist = cdist(np.squeeze(surf, axis=1), np.squeeze(ul, axis=1))
-            mat = acm(dist)
-            path = owp(mat)
+            mat = dtw_acm(dist)
+            path = dtw_owp(mat)
             roughness = mat[-1, -1] / len(path)
+            pairs = np.concatenate([surf[path[..., 0]], ul[path[..., 1]]], axis=1)
         elif self.roughness_measure == "SDTW":
-            ul_len = np.ceil(cv2.arcLength(ul.astype(np.float32), closed=False))
-            ul = equidistant_interpolate(ul, int(ul_len))
+            ul = sample_polyline(ul, int(np.ceil(ul_len)))
             dist = cdist(np.squeeze(surf, axis=1), np.squeeze(ul, axis=1))
-            mat = acm(dist**2)
-            path = owp(mat)
+            mat = dtw_acm(dist**2)
+            path = dtw_owp(mat)
             roughness = np.sqrt(mat[-1, -1] / len(path))
+            pairs = np.concatenate([surf[path[..., 0]], ul[path[..., 1]]], axis=1)
         else:
-            path = np.empty((0, 2), dtype=np.int32)
-            roughness = -1
-        return (float(roughness), path)
+            roughness = np.nan
+            pairs = np.empty((0, 2), dtype=np.float64)
+        return (float(roughness), pairs)
 
     @attrcache("_max_thickness")
     def max_thickness(self) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
         """Regional maximum thicknesses.
 
         Coating layer is segmented using :meth:`RectSubstrate.sideline_intersections`.
         Points on layer surface and sideline for maximum distance in each region are
@@ -831,43 +835,28 @@
             [points.astype(np.int32)],
             isClosed=False,
             color=uniformlayer_color,
             thickness=uniformlayer_thickness,
         )
 
         if len(self.interfaces()) > 0:
-            I0, I1 = self.surface()
-            surf = self.contour()[I0:I1]
-            (i0, i1) = np.sort(np.concatenate(self.interfaces()).flatten())[[0, -1]]
-            intf = (self.substrate.contour() + self.substrate_point())[i0:i1]
-            _, path = self.conformality()
-            path = path[::conformality_step]
-            lines = np.concatenate([surf[path[..., 0]], intf[path[..., 1]]], axis=1)
+            _, pairs = self.conformality()
             cv2.polylines(
                 image,
-                lines,
+                pairs[::conformality_step],
                 isClosed=False,
                 color=conformality_color,
                 thickness=conformality_thickness,
             )
 
         if len(self.interfaces()) > 0:
-            I0, I1 = self.surface()
-            surf = self.contour()[I0:I1]
-            _, ul = self.uniform_layer()
-            ul_len = np.ceil(cv2.arcLength(ul.astype(np.float32), closed=False))
-            ul = equidistant_interpolate(ul, int(ul_len))
-            _, path = self.roughness()
-            path = path[::roughness_step]
-            lines = np.concatenate(
-                [surf[path[..., 0]], ul[path[..., 1]]], axis=1
-            ).astype(np.int32)
+            _, pairs = self.roughness()
             cv2.polylines(
                 image,
-                lines,
+                pairs.astype(np.int32)[::roughness_step],
                 isClosed=False,
                 color=roughness_color,
                 thickness=roughness_thickness,
             )
 
         return image
 
@@ -917,120 +906,43 @@
     img1_crop = img1[max(y0, 0) : min(y1, H), max(x0, 0) : min(x1, W)]
     img2_crop = img2[max(-y0, 0) : min(H - y0, h), max(-x0, 0) : min(W - x0, w)]
     common = img1_crop & img2_crop
     img1_crop ^= common
     return img1
 
 
-def equidistant_interpolate(points, n) -> npt.NDArray[np.float64]:
-    """Interpolate points with equidistant new points.
+def sample_polyline(vertices: npt.NDArray, n: int) -> npt.NDArray[np.float64]:
+    """Sample *n* points from a polyline which consists of *vertices*.
 
     Arguments:
-        points: Points that are interpolated.
-            The shape must be ``(N, 1, D)`` where ``N`` is the number of points
-            and ``D`` is the dimension.
-        n: Number of new points.
+        vertices
+            An array whose shape is ``(N, 1, D)`` where ``N`` is the number of
+            points and ``D`` is the dimension.
+        n
+            Number of new points to be sampled.
 
     Returns:
-        Interpolated points. If ``N`` is positive number, the shape is ``(n, 1, D)``.
-        If ``N`` is zero, the shape is ``(n, 0, D)``.
+        pts
+            Sampled points of shape ``(n, 1, D)``.
     """
-    # https://stackoverflow.com/a/19122075
-    if points.size == 0:
-        return np.empty((n, 0, points.shape[-1]), dtype=np.float64)
-    vec = np.diff(points, axis=0)
-    dist = np.linalg.norm(vec, axis=-1)
-    u = np.insert(np.cumsum(dist), 0, 0)
-    t = np.linspace(0, u[-1], n)
-    ret = np.column_stack([np.interp(t, u, a) for a in np.squeeze(points, axis=1).T])
-    return ret.reshape((n,) + points.shape[1:])
+    tck, _ = splprep(vertices.squeeze(axis=1).T, s=0)
+    u = np.linspace(0, 1, n)
+    pts = np.stack(splev(u, tck)).T[:, np.newaxis, ...]
+    return pts
 
 
-def parallel_curve(curve: npt.NDArray, dist: float) -> npt.NDArray:
-    """Return parallel curve of *curve* with offset distance *dist*.
+def parallel_curve(vertices: npt.NDArray, dist: float) -> npt.NDArray[np.float64]:
+    """Parallel curve of a polyline of *vertices* with offset distance *dist*.
 
     Arguments:
-        curve: Vertices of a polyline.
-            The shape is ``(V, 1, D)``, where ``V`` is the number of vertices and
-            ``D`` is the dimension.
+        vertices
+            An array whose shape is ``(N, 1, D)`` where ``N`` is the number of
+            points and ``D`` is the dimension.
         dist: offset distance of the parallel curve.
 
     Returns:
-        Round-joint parallel curve of shape ``(V, 1, D)``.
-    """
-    if dist == 0:
-        return curve
-    ret = offset_curve(LineString(np.squeeze(curve, axis=1)), dist, join_style="round")
-    return np.array(ret.coords)[:, np.newaxis]
-
-
-@njit(cache=True)
-def acm(cm: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
-    """Compute accumulated cost matrix from local cost matrix.
-
-    Arguments:
-        cm: Local cost matrix.
-
-    Returns:
-        Accumulated cost matrix. The element at `[-1, -1]` is the total sum along the
-        optimal path. If *cm* is empty, return value is an empty array.
-    """
-    p, q = cm.shape
-    ret = np.zeros((p, q), dtype=np.float64)
-    if p == 0 or q == 0:
-        return ret
-
-    ret[0, 0] = cm[0, 0]
-
-    for i in range(1, p):
-        ret[i, 0] = ret[i - 1, 0] + cm[i, 0]
-
-    for j in range(1, q):
-        ret[0, j] = ret[0, j - 1] + cm[0, j]
-
-    for i in range(1, p):
-        for j in range(1, q):
-            ret[i, j] = min(ret[i - 1, j], ret[i, j - 1], ret[i - 1, j - 1]) + cm[i, j]
-
-    return ret
-
-
-@njit(cache=True)
-def owp(acm: npt.NDArray[np.float64]) -> npt.NDArray[np.int32]:
-    """Compute optimal warping path from accumulated cost matrix.
-
-    Arguments:
-        acm: Accumulated cost matrix.
-
-    Returns:
-        Indices for the two series to get the optimal warping path.
+        Round-joint parallel curve of shape ``(N, 1, D)``.
     """
-    p, q = acm.shape
-    if p == 0 or q == 0:
-        return np.empty((0, 2), dtype=np.int32)
-
-    path = np.zeros((p + q - 1, 2), dtype=np.int32)
-    path_len = np.int32(0)
-
-    i, j = p - 1, q - 1
-    path[path_len] = [i, j]
-    path_len += np.int32(1)
-
-    while i > 0 or j > 0:
-        if i == 0:
-            j -= 1
-        elif j == 0:
-            i -= 1
-        else:
-            d = min(acm[i - 1, j], acm[i, j - 1], acm[i - 1, j - 1])
-            if acm[i - 1, j] == d:
-                i -= 1
-            elif acm[i, j - 1] == d:
-                j -= 1
-            else:
-                i -= 1
-                j -= 1
-
-        path[path_len] = [i, j]
-        path_len += np.int32(1)
-
-    return path[-(len(path) - path_len + 1) :: -1, :]
+    ret = offset_curve(
+        LineString(np.squeeze(vertices, axis=1)), dist, join_style="round"
+    )
+    return get_coordinates(ret)[:, np.newaxis]
```

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/reference.py` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/reference.py`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/coat.mp4` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/coat.mp4`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/coat.png` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/coat.png`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/samples/ref.png` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/samples/ref.png`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/src/finitedepth/substrate.py` & `dipcoatimage_finitedepth-2.0.3/src/finitedepth/substrate.py`

 * *Files identical despite different names*

### Comparing `dipcoatimage-finitedepth-2.0.2/tests/test_analyzers.py` & `dipcoatimage_finitedepth-2.0.3/tests/test_analyzers.py`

 * *Files identical despite different names*

