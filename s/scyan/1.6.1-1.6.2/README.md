# Comparing `tmp/scyan-1.6.1.tar.gz` & `tmp/scyan-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scyan-1.6.1.tar", max compression
+gzip compressed data, was "scyan-1.6.2.tar", max compression
```

## Comparing `scyan-1.6.1.tar` & `scyan-1.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1523 2024-04-08 13:39:37.807866 scyan-1.6.1/LICENSE
--rw-r--r--   0        0        0     4841 2024-04-08 13:39:37.807866 scyan-1.6.1/README.md
--rw-r--r--   0        0        0     2591 2024-04-08 13:39:37.851867 scyan-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      428 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/__init__.py
--rw-r--r--   0        0        0     8267 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/_io.py
--rw-r--r--   0        0        0     4972 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/baseline.py
--rw-r--r--   0        0        0      105 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/data/__init__.py
--rw-r--r--   0        0        0    10800 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/data/datasets.py
--rw-r--r--   0        0        0     2247 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/data/tensors.py
--rw-r--r--   0        0        0    24386 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/model.py
--rw-r--r--   0        0        0      154 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/module/__init__.py
--rw-r--r--   0        0        0     3026 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/module/coupling_layer.py
--rw-r--r--   0        0        0     4505 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/module/distribution.py
--rw-r--r--   0        0        0     2295 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/module/real_nvp.py
--rw-r--r--   0        0        0     6263 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/module/scyan_module.py
--rw-r--r--   0        0        0      334 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/__init__.py
--rw-r--r--   0        0        0      277 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/_scanpy_plot/README.md
--rw-r--r--   0        0        0       80 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/_scanpy_plot/__init__.py
--rw-r--r--   0        0        0     5600 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/_scanpy_plot/palettes.py
--rw-r--r--   0        0        0     2082 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/_scanpy_plot/plot_settings.py
--rw-r--r--   0        0        0    32523 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/_scanpy_plot/umap.py
--rw-r--r--   0        0        0     3755 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/density.py
--rw-r--r--   0        0        0     5369 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/dot.py
--rw-r--r--   0        0        0     5886 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/expressions.py
--rw-r--r--   0        0        0     2093 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/graph.py
--rw-r--r--   0        0        0     1930 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/heatmap.py
--rw-r--r--   0        0        0     5794 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/ratios.py
--rw-r--r--   0        0        0     5116 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/plot/utils.py
--rw-r--r--   0        0        0     9562 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/preprocess.py
--rw-r--r--   0        0        0      206 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/tools/__init__.py
--rw-r--r--   0        0        0     5554 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/tools/biomarkers.py
--rw-r--r--   0        0        0     3717 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/tools/colors.py
--rw-r--r--   0        0        0     6992 2024-04-08 13:39:37.851867 scyan-1.6.1/scyan/tools/gating.py
--rw-r--r--   0        0        0     7756 2024-04-08 13:39:37.855867 scyan-1.6.1/scyan/tools/representation.py
--rw-r--r--   0        0        0     9855 2024-04-08 13:39:37.855867 scyan-1.6.1/scyan/utils.py
--rw-r--r--   0        0        0     6967 1970-01-01 00:00:00.000000 scyan-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1523 2024-05-22 15:36:28.920913 scyan-1.6.2/LICENSE
+-rw-r--r--   0        0        0     4841 2024-05-22 15:36:28.920913 scyan-1.6.2/README.md
+-rw-r--r--   0        0        0     2591 2024-05-22 15:36:28.964913 scyan-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/__init__.py
+-rw-r--r--   0        0        0     8267 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/_io.py
+-rw-r--r--   0        0        0     4972 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/baseline.py
+-rw-r--r--   0        0        0      105 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/data/__init__.py
+-rw-r--r--   0        0        0    10800 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/data/datasets.py
+-rw-r--r--   0        0        0     2247 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/data/tensors.py
+-rw-r--r--   0        0        0    24386 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/model.py
+-rw-r--r--   0        0        0      154 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/module/__init__.py
+-rw-r--r--   0        0        0     3026 2024-05-22 15:36:28.964913 scyan-1.6.2/scyan/module/coupling_layer.py
+-rw-r--r--   0        0        0     4505 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/module/distribution.py
+-rw-r--r--   0        0        0     2295 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/module/real_nvp.py
+-rw-r--r--   0        0        0     6263 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/module/scyan_module.py
+-rw-r--r--   0        0        0      334 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/_scanpy_plot/README.md
+-rw-r--r--   0        0        0       80 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/_scanpy_plot/__init__.py
+-rw-r--r--   0        0        0     5600 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/_scanpy_plot/palettes.py
+-rw-r--r--   0        0        0     2082 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/_scanpy_plot/plot_settings.py
+-rw-r--r--   0        0        0    32491 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/_scanpy_plot/umap.py
+-rw-r--r--   0        0        0     3755 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/density.py
+-rw-r--r--   0        0        0     5369 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/dot.py
+-rw-r--r--   0        0        0     5886 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/expressions.py
+-rw-r--r--   0        0        0     2093 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/graph.py
+-rw-r--r--   0        0        0     1930 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/heatmap.py
+-rw-r--r--   0        0        0     5794 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/ratios.py
+-rw-r--r--   0        0        0     5116 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/plot/utils.py
+-rw-r--r--   0        0        0     9562 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/preprocess.py
+-rw-r--r--   0        0        0      206 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/tools/__init__.py
+-rw-r--r--   0        0        0     5554 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/tools/biomarkers.py
+-rw-r--r--   0        0        0     3717 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/tools/colors.py
+-rw-r--r--   0        0        0     6992 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/tools/gating.py
+-rw-r--r--   0        0        0     7756 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/tools/representation.py
+-rw-r--r--   0        0        0     9855 2024-05-22 15:36:28.968913 scyan-1.6.2/scyan/utils.py
+-rw-r--r--   0        0        0     6967 1970-01-01 00:00:00.000000 scyan-1.6.2/PKG-INFO
```

### Comparing `scyan-1.6.1/LICENSE` & `scyan-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/README.md` & `scyan-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/pyproject.toml` & `scyan-1.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scyan"
-version = "1.6.1"
+version = "1.6.2"
 description = "Single-cell Cytometry Annotation Network"
 documentation = "https://mics-lab.github.io/scyan/"
 homepage = "https://mics-lab.github.io/scyan/"
 repository = "https://github.com/MICS-Lab/scyan"
 authors = ["Blampey Quentin <quentin.blampey@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `scyan-1.6.1/scyan/_io.py` & `scyan-1.6.2/scyan/_io.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/baseline.py` & `scyan-1.6.2/scyan/baseline.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/data/datasets.py` & `scyan-1.6.2/scyan/data/datasets.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/data/tensors.py` & `scyan-1.6.2/scyan/data/tensors.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/model.py` & `scyan-1.6.2/scyan/model.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/module/coupling_layer.py` & `scyan-1.6.2/scyan/module/coupling_layer.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/module/distribution.py` & `scyan-1.6.2/scyan/module/distribution.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/module/real_nvp.py` & `scyan-1.6.2/scyan/module/real_nvp.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/module/scyan_module.py` & `scyan-1.6.2/scyan/module/scyan_module.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/_scanpy_plot/palettes.py` & `scyan-1.6.2/scyan/plot/_scanpy_plot/palettes.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/_scanpy_plot/plot_settings.py` & `scyan-1.6.2/scyan/plot/_scanpy_plot/plot_settings.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/_scanpy_plot/umap.py` & `scyan-1.6.2/scyan/plot/_scanpy_plot/umap.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import pandas as pd
 from anndata import AnnData
 from cycler import Cycler, cycler
 from matplotlib import colors, patheffects
 from matplotlib import pyplot as pl
 from matplotlib import rcParams
 from matplotlib.axes import Axes
-from matplotlib.cm import get_cmap
 from matplotlib.collections import PatchCollection
 from matplotlib.colors import Colormap, Normalize, is_color_like
 from matplotlib.figure import Figure
 from matplotlib.patches import Circle
 from pandas.api.types import is_categorical_dtype
 
 from . import palettes
@@ -319,15 +318,15 @@
 
     # Color map
     if color_map is not None:
         if cmap is not None:
             raise ValueError("Cannot specify both `color_map` and `cmap`.")
         else:
             cmap = color_map
-    cmap = copy(get_cmap(cmap))
+    cmap = copy(pl.get_cmap(cmap))
     cmap.set_bad(na_color)
     kwargs["cmap"] = cmap
     # Prevents warnings during legend creation
     na_color = colors.to_hex(na_color, keep_alpha=True)
 
     if "edgecolor" not in kwargs:
         # by default turn off edge color. Otherwise, for
```

### Comparing `scyan-1.6.1/scyan/plot/density.py` & `scyan-1.6.2/scyan/plot/density.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/dot.py` & `scyan-1.6.2/scyan/plot/dot.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/expressions.py` & `scyan-1.6.2/scyan/plot/expressions.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/graph.py` & `scyan-1.6.2/scyan/plot/graph.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/heatmap.py` & `scyan-1.6.2/scyan/plot/heatmap.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/ratios.py` & `scyan-1.6.2/scyan/plot/ratios.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/plot/utils.py` & `scyan-1.6.2/scyan/plot/utils.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/preprocess.py` & `scyan-1.6.2/scyan/preprocess.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/tools/biomarkers.py` & `scyan-1.6.2/scyan/tools/biomarkers.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/tools/colors.py` & `scyan-1.6.2/scyan/tools/colors.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/tools/gating.py` & `scyan-1.6.2/scyan/tools/gating.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/tools/representation.py` & `scyan-1.6.2/scyan/tools/representation.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/scyan/utils.py` & `scyan-1.6.2/scyan/utils.py`

 * *Files identical despite different names*

### Comparing `scyan-1.6.1/PKG-INFO` & `scyan-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scyan
-Version: 1.6.1
+Version: 1.6.2
 Summary: Single-cell Cytometry Annotation Network
 Home-page: https://mics-lab.github.io/scyan/
 License: BSD-3-Clause
 Author: Blampey Quentin
 Author-email: quentin.blampey@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: BSD License
```

