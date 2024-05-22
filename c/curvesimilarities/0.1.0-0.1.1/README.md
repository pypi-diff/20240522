# Comparing `tmp/curvesimilarities-0.1.0.tar.gz` & `tmp/curvesimilarities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvesimilarities-0.1.0.tar", last modified: Sun May 19 09:13:58 2024, max compression
+gzip compressed data, was "curvesimilarities-0.1.1.tar", last modified: Wed May 22 08:10:40 2024, max compression
```

## Comparing `curvesimilarities-0.1.0.tar` & `curvesimilarities-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:13:58.910537 curvesimilarities-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-19 09:13:50.000000 curvesimilarities-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-19 09:13:58.910537 curvesimilarities-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-19 09:13:50.000000 curvesimilarities-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-19 09:13:50.000000 curvesimilarities-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:13:58.910537 curvesimilarities-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:13:58.906537 curvesimilarities-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:13:58.906537 curvesimilarities-0.1.0/src/curvesimilarities/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-19 09:13:50.000000 curvesimilarities-0.1.0/src/curvesimilarities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-19 09:13:50.000000 curvesimilarities-0.1.0/src/curvesimilarities/frechet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:13:58.910537 curvesimilarities-0.1.0/src/curvesimilarities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-19 09:13:58.000000 curvesimilarities-0.1.0/src/curvesimilarities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-19 09:13:58.000000 curvesimilarities-0.1.0/src/curvesimilarities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:13:58.000000 curvesimilarities-0.1.0/src/curvesimilarities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 09:13:58.000000 curvesimilarities-0.1.0/src/curvesimilarities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 09:13:58.000000 curvesimilarities-0.1.0/src/curvesimilarities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:13:58.910537 curvesimilarities-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-19 09:13:50.000000 curvesimilarities-0.1.0/tests/test_fd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:10:40.647740 curvesimilarities-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-22 08:10:40.647740 curvesimilarities-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:10:40.647740 curvesimilarities-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:10:40.643740 curvesimilarities-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:10:40.643740 curvesimilarities-0.1.1/src/curvesimilarities/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/src/curvesimilarities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/src/curvesimilarities/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/src/curvesimilarities/frechet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:10:40.643740 curvesimilarities-0.1.1/src/curvesimilarities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-22 08:10:40.000000 curvesimilarities-0.1.1/src/curvesimilarities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-22 08:10:40.000000 curvesimilarities-0.1.1/src/curvesimilarities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:10:40.000000 curvesimilarities-0.1.1/src/curvesimilarities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-22 08:10:40.000000 curvesimilarities-0.1.1/src/curvesimilarities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 08:10:40.000000 curvesimilarities-0.1.1/src/curvesimilarities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:10:40.643740 curvesimilarities-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 08:10:35.000000 curvesimilarities-0.1.1/tests/test_fd.py
```

### Comparing `curvesimilarities-0.1.0/LICENSE` & `curvesimilarities-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curvesimilarities-0.1.0/PKG-INFO` & `curvesimilarities-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: curvesimilarities
-Version: 0.1.0
+Version: 0.1.1
 Summary: Curve similarity measures
 Author-email: Jisoo Song <jeesoo9595@snu.ac.kr>
 License: Copyright 2024, Jisoo Song
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         
         2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: homepage, https://github.com/JSS95/curvesimilarities
+Project-URL: source, https://github.com/JSS95/curvesimilarities
+Project-URL: documentation, https://curvesimilarities.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -35,14 +38,15 @@
 Requires-Dist: numba
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: pydata_sphinx_theme; extra == "doc"
+Requires-Dist: matplotlib; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: doc8; extra == "dev"
```

### Comparing `curvesimilarities-0.1.0/README.md` & `curvesimilarities-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `curvesimilarities-0.1.0/pyproject.toml` & `curvesimilarities-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "curvesimilarities"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Jisoo Song", email = "jeesoo9595@snu.ac.kr"}
 ]
 description = "Curve similarity measures"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
@@ -29,22 +29,28 @@
 ]
 dependencies = [
   "numpy",
   "scipy",
   "numba",
 ]
 
+[project.urls]
+homepage = "https://github.com/JSS95/curvesimilarities"
+source = "https://github.com/JSS95/curvesimilarities"
+documentation = "https://curvesimilarities.readthedocs.io"
+
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata_sphinx_theme",
+    "matplotlib",
 ]
 dev = [
     "flake8",
     "flake8-docstrings",
     "black",
     "isort",
     "docformatter",
@@ -73,8 +79,8 @@
 
 [tool.pytest.ini_options]
 doctest_optionflags = [
     "NORMALIZE_WHITESPACE",
     "IGNORE_EXCEPTION_DETAIL",
     "ELLIPSIS",
 ]
-addopts = "--doctest-modules"
+addopts = "--doctest-modules --ignore=doc"
```

### Comparing `curvesimilarities-0.1.0/src/curvesimilarities/frechet.py` & `curvesimilarities-0.1.1/src/curvesimilarities/frechet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Fréchet distance and its variants."""
 
-import sys
-
 import numpy as np
 from numba import njit
 from scipy.spatial.distance import cdist
 
 __all__ = [
     "fd",
     "dfd",
 ]
 
 
-EPSILON = np.float_(sys.float_info.epsilon)
+EPSILON = np.finfo(np.float_).eps
+NAN = np.float_(np.nan)
 
 
 def fd(P, Q):
     r"""(Continuous) Fréchet distance between two open polygonal curves.
 
     Let :math:`f: [0, 1] \to \Omega` and :math:`g: [0, 1] \to \Omega` be curves
     where :math:`\Omega` is a metric space. The Fréchet distance between
@@ -65,20 +64,19 @@
     >>> fd([[0, 0], [0.5, 0], [1, 0]], [[0, 1], [1, 1]])
     1.0...
     """
     if len(P) == 0 or len(Q) == 0:
         raise ValueError("Vertices must not be empty.")
     P = np.asarray(P, dtype=np.float_)
     Q = np.asarray(Q, dtype=np.float_)
-    return _fd(P, Q)
+    return np.float_(_fd(P, Q))
 
 
-@njit
+@njit(cache=True)
 def _free_interval(A, B, C, eps):
-    NAN = np.float_(np.nan)
     # resulting interval is always in [0, 1] or is [nan, nan].
     coeff1 = B - A
     coeff2 = A - C
     a = np.dot(coeff1, coeff1)
     c = np.dot(coeff2, coeff2) - eps**2
     if a == 0:  # degenerate case
         if c > 0:
@@ -95,15 +93,15 @@
         end = min((-b + Det**0.5) / 2 / a, np.float_(1))
         if start > 1 or end < 0:
             start = end = NAN
         interval = [start, end]
     return interval
 
 
-@njit
+@njit(cache=True)
 def _decision_problem(P, Q, eps):
     """Algorithm 1 of Alt & Godau (1995)."""
     # Decide reachablilty
     B = np.empty((len(P) - 1, len(Q), 2), dtype=np.float_)
     start, end = _free_interval(P[0], P[1], Q[0], eps)
     if start == 0:
         B[0, 0] = [start, end]
@@ -153,15 +151,15 @@
                 B[i, j + 1] = [max(prevB_start, B_start), B_end]
             else:
                 B[i, j + 1] = [np.nan, np.nan]
 
     return L[-1, -1, 1] == 1 or B[-1, -1, 1] == 1
 
 
-@njit
+@njit(cache=True)
 def _critical_b(A, B, C):
     v = B - A
     w = C - A
     vv = np.dot(v, v)
     if vv == 0:
         return np.linalg.norm(w)
     t = np.dot(v, w) / vv
@@ -170,15 +168,15 @@
     elif t > 1:
         dist = np.linalg.norm(C - B)
     else:
         dist = np.linalg.norm(t * v - w)
     return dist
 
 
-@njit
+@njit(cache=True)
 def _fd(P, Q):
     """Algorithm 3 of Alt & Godau (1995)."""
     crit_a = max(np.linalg.norm(P[0] - Q[0]), np.linalg.norm(P[-1] - Q[-1]))
 
     crit_b = np.empty(2 * len(P) * len(Q) - len(P) - len(Q) + 1, dtype=np.float_)
     count = 0
     for i in range(len(P) - 1):
@@ -204,15 +202,15 @@
         if mid_reachable:
             end = mid
         else:
             start = mid
 
     # parametric search
     e1, e2 = crit_b[start], crit_b[end]
-    tol = max(e1 / 100, EPSILON)
+    tol = EPSILON
     while e2 - e1 > tol:
         mid = (e1 + e2) / 2
         mid_reachable = _decision_problem(P, Q, mid)
         if mid_reachable:
             e2 = mid
         else:
             e1 = mid
@@ -220,24 +218,25 @@
     return e2
 
 
 def dfd(P, Q):
     r"""Discrete Fréchet distance between two open polygonal curves.
 
     Let :math:`\{P_0, P_1, ..., P_n\}` and :math:`\{Q_0, Q_1, ..., Q_m\}` be
-    polyline vertices in metris space. The discrete Fréchet distance between
+    polyline vertices in metric space. The discrete Fréchet distance between
     two polylines is defined as
 
     .. math::
 
         \min_{C} \max_{(i, j) \in C} \lVert P_i - Q_j \rVert
 
     where :math:`C` is a nondecreasing coupling over
     :math:`\{0, ..., n\} \times \{0, ..., m\}`, starting from :math:`(0, 0)` and
-    ending with :math:`(n, m)`.
+    ending with :math:`(n, m)`. :math:`\lVert \cdot \rVert` is the underlying
+    metric, which is the Euclidean metric in this implementation.
 
     Parameters
     ----------
     P : array_like
         An :math:`p` by :math:`n` array of :math:`p` vertices in an
         :math:`n`-dimensional space.
     Q : array_like
@@ -269,15 +268,15 @@
     """
     if len(P) == 0 or len(Q) == 0:
         raise ValueError("Vertices must not be empty.")
     dist = cdist(P, Q)
     return _dfd(dist)[-1, -1]
 
 
-@njit
+@njit(cache=True)
 def _dfd(dist):
     # Eiter, T., & Mannila, H. (1994)
     p, q = dist.shape
     ret = np.empty((p, q), dtype=np.float_)
 
     ret[0, 0] = dist[0, 0]
```

### Comparing `curvesimilarities-0.1.0/src/curvesimilarities.egg-info/PKG-INFO` & `curvesimilarities-0.1.1/src/curvesimilarities.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: curvesimilarities
-Version: 0.1.0
+Version: 0.1.1
 Summary: Curve similarity measures
 Author-email: Jisoo Song <jeesoo9595@snu.ac.kr>
 License: Copyright 2024, Jisoo Song
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         
         2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: homepage, https://github.com/JSS95/curvesimilarities
+Project-URL: source, https://github.com/JSS95/curvesimilarities
+Project-URL: documentation, https://curvesimilarities.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -35,14 +38,15 @@
 Requires-Dist: numba
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: pydata_sphinx_theme; extra == "doc"
+Requires-Dist: matplotlib; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: doc8; extra == "dev"
```

