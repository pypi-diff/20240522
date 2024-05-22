# Comparing `tmp/funcnodes_plotly-0.1.3.tar.gz` & `tmp/funcnodes_plotly-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_plotly-0.1.3.tar", max compression
+gzip compressed data, was "funcnodes_plotly-0.1.4.tar", max compression
```

## Comparing `funcnodes_plotly-0.1.3.tar` & `funcnodes_plotly-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1029 2024-05-12 06:11:10.862513 funcnodes_plotly-0.1.3/funcnodes_plotly/__init__.py
--rw-r--r--   0        0        0     2036 2024-05-11 18:57:12.461959 funcnodes_plotly-0.1.3/funcnodes_plotly/colors.py
--rw-r--r--   0        0        0    22308 2024-05-12 05:39:41.608486 funcnodes_plotly-0.1.3/funcnodes_plotly/express.py
--rw-r--r--   0        0        0     1911 2024-05-11 17:47:59.451810 funcnodes_plotly-0.1.3/funcnodes_plotly/figure.py
--rw-r--r--   0        0        0      936 2024-05-11 18:16:57.007455 funcnodes_plotly-0.1.3/funcnodes_plotly/layout.py
--rw-r--r--   0        0        0     4360 2024-05-11 17:34:26.149742 funcnodes_plotly-0.1.3/funcnodes_plotly/plots.py
--rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.3/funcnodes_plotly/utils.py
--rw-r--r--   0        0        0      471 2024-05-12 06:11:17.756419 funcnodes_plotly-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.3/README.md
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1159 2024-05-22 11:16:07.539415 funcnodes_plotly-0.1.4/funcnodes_plotly/__init__.py
+-rw-r--r--   0        0        0     2036 2024-05-11 18:57:12.461959 funcnodes_plotly-0.1.4/funcnodes_plotly/colors.py
+-rw-r--r--   0        0        0    22326 2024-05-16 12:03:05.783638 funcnodes_plotly-0.1.4/funcnodes_plotly/express.py
+-rw-r--r--   0        0        0     1911 2024-05-11 17:47:59.451810 funcnodes_plotly-0.1.4/funcnodes_plotly/figure.py
+-rw-r--r--   0        0        0      936 2024-05-11 18:16:57.007455 funcnodes_plotly-0.1.4/funcnodes_plotly/layout.py
+-rw-r--r--   0        0        0     4360 2024-05-11 17:34:26.149742 funcnodes_plotly-0.1.4/funcnodes_plotly/plots.py
+-rw-r--r--   0        0        0  7251402 2024-05-22 11:19:55.998218 funcnodes_plotly-0.1.4/funcnodes_plotly/react_plugin/js/main.js
+-rw-r--r--   0        0        0     1503 2024-05-17 12:35:53.670685 funcnodes_plotly-0.1.4/funcnodes_plotly/react_plugin/js/main.js.LICENSE.txt
+-rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.4/funcnodes_plotly/utils.py
+-rw-r--r--   0        0        0      476 2024-05-22 11:16:47.061642 funcnodes_plotly-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.4/README.md
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.4/PKG-INFO
```

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/__init__.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Tuple, Any
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseTraceType
 import funcnodes as fn
 from exposedfunctionality.function_parser.types import add_type
 from . import plots, layout, figure, express
+import os
 
 add_type(
     go.Figure,
     "plotly.Figure",
 )
 add_type(
     BaseTraceType,
@@ -44,9 +45,15 @@
         plots.NODE_SHELF,
         layout.NODE_SHELF,
         figure.NODE_SHELF,
         express.NODE_SHELF,
     ],
 )
 
+REACT_PLUGIN = {
+    "js": [
+        os.path.join(os.path.dirname(__file__), "react_plugin", "js", "main.js"),
+    ]
+}
+
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/colors.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/colors.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/express.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/express.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
 ) -> go.Figure:
     """
     Create a scatter matrix.
     """
     if dimensions is not None:
         dimensions_list = [s.strip() for s in dimensions.split(",")]
     else:
-        dimensions_list = data.columns
+        dimensions_list = list(data.columns)
 
     if color is not None:
         if color in dimensions_list:
             dimensions_list.remove(color)
 
     return px.scatter_matrix(
         data,
@@ -729,15 +729,15 @@
 ) -> go.Figure:
     """
     Create a parallel coordinates plot.
     """
     if dimensions is not None:
         dimensions_list = [s.strip() for s in dimensions.split(",")]
     else:
-        dimensions_list = data.columns
+        dimensions_list = list(data.columns)
 
     color_continuous_scale = ContinousColorScales.v(color_continuous_scale)
 
     return px.parallel_coordinates(
         data,
         color=color,
         dimensions=dimensions_list,
@@ -764,15 +764,15 @@
 ) -> go.Figure:
     """
     Create a parallel categories plot.
     """
     if dimensions is not None:
         dimensions_list = [s.strip() for s in dimensions.split(",")]
     else:
-        dimensions_list = data.columns
+        dimensions_list = list(data.columns)
 
     color_continuous_scale = ContinousColorScales.v(color_continuous_scale)
 
     return px.parallel_categories(
         data,
         dimensions=dimensions_list,
         color=color,
```

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/figure.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/figure.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/layout.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/layout.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/plots.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/plots.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.3/funcnodes_plotly/utils.py` & `funcnodes_plotly-0.1.4/funcnodes_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.3/PKG-INFO` & `funcnodes_plotly-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: funcnodes-plotly
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/JulianKimmig/funcnodes_plotly
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.2.6)
-Requires-Dist: plotly (>=5.21,<6.0)
+Requires-Dist: funcnodes (>=0.2.16)
+Requires-Dist: plotly (>=5.22.0,<6.0.0)
 Project-URL: Repository, https://github.com/JulianKimmig/funcnodes_plotly
 Description-Content-Type: text/markdown
```

