# Comparing `tmp/labo1-1.0.0.tar.gz` & `tmp/labo1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labo1-1.0.0.tar", last modified: Fri May 10 02:58:26 2024, max compression
+gzip compressed data, was "labo1-1.1.0.tar", last modified: Wed May 22 21:12:45 2024, max compression
```

## Comparing `labo1-1.0.0.tar` & `labo1-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.673005 labo1-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 02:58:20.000000 labo1-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.669005 labo1-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.669005 labo1-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-10 02:58:20.000000 labo1-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 02:58:20.000000 labo1-1.0.0/.github/workflows/test-pre-releases.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 02:58:20.000000 labo1-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 02:58:20.000000 labo1-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 02:58:20.000000 labo1-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-10 02:58:26.673005 labo1-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 02:58:20.000000 labo1-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.673005 labo1-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-10 02:58:20.000000 labo1-1.0.0/docs/API.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.673005 labo1-1.0.0/docs/ajustes/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-10 02:58:20.000000 labo1-1.0.0/docs/ajustes/basico.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-10 02:58:20.000000 labo1-1.0.0/docs/ajustes/graficos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-10 02:58:20.000000 labo1-1.0.0/docs/ajustes/no-lineal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-10 02:58:20.000000 labo1-1.0.0/docs/ajustes/ponderado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-10 02:58:20.000000 labo1-1.0.0/docs/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-10 02:58:20.000000 labo1-1.0.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 02:58:20.000000 labo1-1.0.0/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 02:58:20.000000 labo1-1.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-10 02:58:20.000000 labo1-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 02:58:20.000000 labo1-1.0.0/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 02:58:20.000000 labo1-1.0.0/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 02:58:20.000000 labo1-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:58:26.673005 labo1-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.669005 labo1-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.673005 labo1-1.0.0/src/labo1/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-10 02:58:20.000000 labo1-1.0.0/src/labo1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-10 02:58:20.000000 labo1-1.0.0/src/labo1/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-10 02:58:20.000000 labo1-1.0.0/src/labo1/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-10 02:58:20.000000 labo1-1.0.0/src/labo1/round.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.673005 labo1-1.0.0/src/labo1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-10 02:58:20.000000 labo1-1.0.0/src/labo1/tests/test_round.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:58:26.673005 labo1-1.0.0/src/labo1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-10 02:58:26.000000 labo1-1.0.0/src/labo1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 02:58:26.000000 labo1-1.0.0/src/labo1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:58:26.000000 labo1-1.0.0/src/labo1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 02:58:26.000000 labo1-1.0.0/src/labo1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 02:58:26.000000 labo1-1.0.0/src/labo1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-10 02:58:20.000000 labo1-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.363056 labo1-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 21:12:33.000000 labo1-1.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.359056 labo1-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.359056 labo1-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-22 21:12:33.000000 labo1-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 21:12:33.000000 labo1-1.1.0/.github/workflows/test-pre-releases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 21:12:33.000000 labo1-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-22 21:12:33.000000 labo1-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 21:12:33.000000 labo1-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 21:12:45.363056 labo1-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 21:12:33.000000 labo1-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.359056 labo1-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 21:12:33.000000 labo1-1.1.0/docs/API.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.363056 labo1-1.1.0/docs/ajustes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-22 21:12:33.000000 labo1-1.1.0/docs/ajustes/basico.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-22 21:12:33.000000 labo1-1.1.0/docs/ajustes/graficos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-22 21:12:33.000000 labo1-1.1.0/docs/ajustes/no-lineal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 21:12:33.000000 labo1-1.1.0/docs/ajustes/ponderado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-22 21:12:33.000000 labo1-1.1.0/docs/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-22 21:12:33.000000 labo1-1.1.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 21:12:33.000000 labo1-1.1.0/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-22 21:12:33.000000 labo1-1.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 21:12:33.000000 labo1-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 21:12:33.000000 labo1-1.1.0/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 21:12:33.000000 labo1-1.1.0/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 21:12:33.000000 labo1-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:12:45.363056 labo1-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.359056 labo1-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.363056 labo1-1.1.0/src/labo1/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-22 21:12:33.000000 labo1-1.1.0/src/labo1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-22 21:12:33.000000 labo1-1.1.0/src/labo1/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-22 21:12:33.000000 labo1-1.1.0/src/labo1/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 21:12:33.000000 labo1-1.1.0/src/labo1/round.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.363056 labo1-1.1.0/src/labo1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-22 21:12:33.000000 labo1-1.1.0/src/labo1/tests/test_round.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:45.363056 labo1-1.1.0/src/labo1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 21:12:45.000000 labo1-1.1.0/src/labo1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 21:12:45.000000 labo1-1.1.0/src/labo1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:12:45.000000 labo1-1.1.0/src/labo1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 21:12:45.000000 labo1-1.1.0/src/labo1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 21:12:45.000000 labo1-1.1.0/src/labo1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-22 21:12:33.000000 labo1-1.1.0/tox.ini
```

### Comparing `labo1-1.0.0/.github/workflows/ci.yml` & `labo1-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/.github/workflows/test-pre-releases.yml` & `labo1-1.1.0/.github/workflows/test-pre-releases.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     - cron: '0 7 * * 1'  # every Monday at 7 AM UTC
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
```

### Comparing `labo1-1.0.0/.pre-commit-config.yaml` & `labo1-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/LICENSE` & `labo1-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/PKG-INFO` & `labo1-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labo1
-Version: 1.0.0
+Version: 1.1.0
 Author-email: Mauro Silberberg <maurosilber@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Mauro Silberberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `labo1-1.0.0/docs/ajustes/basico.py` & `labo1-1.1.0/docs/ajustes/basico.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/docs/ajustes/graficos.py` & `labo1-1.1.0/docs/ajustes/graficos.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/docs/ajustes/no-lineal.py` & `labo1-1.1.0/docs/ajustes/no-lineal.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/docs/ajustes/ponderado.py` & `labo1-1.1.0/docs/ajustes/ponderado.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/docs/index.py` & `labo1-1.1.0/docs/index.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/mkdocs.yml` & `labo1-1.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/pyproject.toml` & `labo1-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/src/labo1/fit.py` & `labo1-1.1.0/src/labo1/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Callable, Mapping, Sequence
 from warnings import warn
 
 import numpy as np
 import scipy.optimize
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure, SubFigure
+from numpy.typing import ArrayLike
 
 from .plot import with_errorbars, with_residuals
 from .round import to_significant_figures
 
 
 @dataclass(frozen=True)
 class Result:
@@ -129,17 +130,17 @@
     def __repr__(self):
         return f"{self.__class__.__name__}({self})"
 
 
 def curve_fit(
     func: Callable[..., np.ndarray],
     /,
-    x: np.ndarray,
-    y: np.ndarray,
-    y_err: np.ndarray | None = None,
+    x: ArrayLike,
+    y: ArrayLike,
+    y_err: ArrayLike | None = None,
     *,
     initial_params: Sequence[float] | Mapping[str, float] | None = None,
     rescale_errors: bool = True,
     **kwargs,
 ):
     """Use non-linear least squares to fit a function to data.
 
@@ -161,14 +162,22 @@
         ...     return a * x + b
         ...
         >>> x = np.array([0.0, 1.0, 2.0])
         >>> y = np.array([0.0, 0.9, 2.1])
         >>> curve_fit(f, x, y)
         Result(a=1.050 ± 0.087, b=-0.05 ± 0.11)
     """
+    # accept ArrayLike
+    x = np.asarray(x)
+    y = np.asarray(y)
+    if y_err is None:
+        y_err = np.ones_like(y)  # assume equal errors
+    else:
+        y_err = np.asarray(y_err)
+
     if isinstance(initial_params, Mapping):
         names = _get_parameter_names(func)
         unused_params = initial_params.keys() - names
         if len(unused_params) > 0:
             warn(f"unused parameters: {unused_params}")
 
         initial_params = [initial_params.get(name, 1) for name in names]  # type: ignore
```

### Comparing `labo1-1.0.0/src/labo1/plot.py` & `labo1-1.1.0/src/labo1/plot.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/src/labo1/round.py` & `labo1-1.1.0/src/labo1/round.py`

 * *Files identical despite different names*

### Comparing `labo1-1.0.0/src/labo1.egg-info/PKG-INFO` & `labo1-1.1.0/src/labo1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labo1
-Version: 1.0.0
+Version: 1.1.0
 Author-email: Mauro Silberberg <maurosilber@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Mauro Silberberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `labo1-1.0.0/src/labo1.egg-info/SOURCES.txt` & `labo1-1.1.0/src/labo1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

