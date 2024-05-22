# Comparing `tmp/fknni-1.1.0.tar.gz` & `tmp/fknni-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fknni-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fknni-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fknni-1.1.0.tar` & `fknni-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      289 2024-04-23 19:36:04.020086 fknni-1.1.0/.codecov.yaml
--rw-r--r--   0        0        0      937 2024-04-23 20:01:11.452795 fknni-1.1.0/.cruft.json
--rw-r--r--   0        0        0      241 2024-04-23 19:36:04.020086 fknni-1.1.0/.editorconfig
--rw-r--r--   0        0        0     3080 2024-04-23 19:36:04.050086 fknni-1.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0       27 2024-04-24 13:16:19.127409 fknni-1.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      389 2024-04-23 20:02:59.097036 fknni-1.1.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2024-04-24 11:23:22.038420 fknni-1.1.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      763 2024-04-24 11:23:22.011753 fknni-1.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1546 2024-04-24 11:23:22.055087 fknni-1.1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      289 2024-04-23 19:39:14.425024 fknni-1.1.0/.gitignore
--rw-r--r--   0        0        0     1352 2024-04-23 19:41:51.476348 fknni-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      325 2024-04-23 21:45:01.535357 fknni-1.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      405 2024-04-24 11:32:08.916359 fknni-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    10798 2024-04-23 19:38:26.364619 fknni-1.1.0/LICENSE
--rw-r--r--   0        0        0     1609 2024-04-24 15:07:20.818527 fknni-1.1.0/README.md
--rw-r--r--   0        0        0      634 2024-04-23 19:36:04.060086 fknni-1.1.0/docs/Makefile
--rw-r--r--   0        0        0        0 2024-04-23 19:36:04.090086 fknni-1.1.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2024-04-23 19:36:04.090086 fknni-1.1.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0        0 2024-04-23 19:36:04.093420 fknni-1.1.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2024-04-23 19:36:04.093420 fknni-1.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      150 2024-04-23 21:45:01.538690 fknni-1.1.0/docs/api.md
--rw-r--r--   0        0        0       34 2024-04-23 19:36:04.060086 fknni-1.1.0/docs/changelog.md
--rw-r--r--   0        0        0     3734 2024-04-23 21:45:01.538690 fknni-1.1.0/docs/conf.py
--rw-r--r--   0        0        0     7199 2024-04-23 20:03:19.820544 fknni-1.1.0/docs/contributing.md
--rw-r--r--   0        0        0     1028 2024-04-23 19:36:04.096753 fknni-1.1.0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      144 2024-04-24 11:07:56.997960 fknni-1.1.0/docs/index.md
--rw-r--r--   0        0        0    34788 2024-04-25 16:10:00.897320 fknni-1.1.0/docs/notebooks/faiss.ipynb
--rw-r--r--   0        0        0     1046 2024-04-23 19:36:04.083420 fknni-1.1.0/docs/references.bib
--rw-r--r--   0        0        0       44 2024-04-23 19:36:04.083420 fknni-1.1.0/docs/references.md
--rw-r--r--   0        0        0     3197 2024-04-25 16:10:00.897320 fknni-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-04-24 07:30:01.767795 fknni-1.1.0/src/fknni/__init__.py
--rw-r--r--   0        0        0       32 2024-04-23 20:40:28.600844 fknni-1.1.0/src/fknni/faiss/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-25 16:10:00.897320 fknni-1.1.0/src/fknni/faiss/faiss.py
--rw-r--r--   0        0        0     1169 2024-04-23 20:54:35.393725 fknni-1.1.0/tests/test_faiss_imputation.py
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 fknni-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-04-23 19:36:04.020086 fknni-1.1.1/.codecov.yaml
+-rw-r--r--   0        0        0      937 2024-04-23 20:01:11.452795 fknni-1.1.1/.cruft.json
+-rw-r--r--   0        0        0      241 2024-04-23 19:36:04.020086 fknni-1.1.1/.editorconfig
+-rw-r--r--   0        0        0     3080 2024-04-23 19:36:04.050086 fknni-1.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0       27 2024-04-24 13:16:19.127409 fknni-1.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      389 2024-04-23 20:02:59.097036 fknni-1.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2024-04-24 11:23:22.038420 fknni-1.1.1/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      763 2024-04-24 11:23:22.011753 fknni-1.1.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1546 2024-04-24 11:23:22.055087 fknni-1.1.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      289 2024-04-23 19:39:14.425024 fknni-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1352 2024-04-23 19:41:51.476348 fknni-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2024-04-23 21:45:01.535357 fknni-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      486 2024-05-22 07:46:37.628173 fknni-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    10798 2024-04-23 19:38:26.364619 fknni-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1609 2024-04-24 15:07:20.818527 fknni-1.1.1/README.md
+-rw-r--r--   0        0        0      634 2024-04-23 19:36:04.060086 fknni-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0        0 2024-04-23 19:36:04.090086 fknni-1.1.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2024-04-23 19:36:04.090086 fknni-1.1.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0        0 2024-04-23 19:36:04.093420 fknni-1.1.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2024-04-23 19:36:04.093420 fknni-1.1.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      150 2024-04-23 21:45:01.538690 fknni-1.1.1/docs/api.md
+-rw-r--r--   0        0        0       34 2024-04-23 19:36:04.060086 fknni-1.1.1/docs/changelog.md
+-rw-r--r--   0        0        0     3734 2024-04-23 21:45:01.538690 fknni-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0     7199 2024-04-23 20:03:19.820544 fknni-1.1.1/docs/contributing.md
+-rw-r--r--   0        0        0     1028 2024-04-23 19:36:04.096753 fknni-1.1.1/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      144 2024-04-24 11:07:56.997960 fknni-1.1.1/docs/index.md
+-rw-r--r--   0        0        0    34788 2024-04-25 16:10:00.897320 fknni-1.1.1/docs/notebooks/faiss.ipynb
+-rw-r--r--   0        0        0     1046 2024-04-23 19:36:04.083420 fknni-1.1.1/docs/references.bib
+-rw-r--r--   0        0        0       44 2024-04-23 19:36:04.083420 fknni-1.1.1/docs/references.md
+-rw-r--r--   0        0        0     3197 2024-05-22 07:47:30.974792 fknni-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-04-24 07:30:01.767795 fknni-1.1.1/src/fknni/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-23 20:40:28.600844 fknni-1.1.1/src/fknni/faiss/__init__.py
+-rw-r--r--   0        0        0     4973 2024-05-22 07:48:57.461331 fknni-1.1.1/src/fknni/faiss/faiss.py
+-rw-r--r--   0        0        0     1169 2024-04-23 20:54:35.393725 fknni-1.1.1/tests/test_faiss_imputation.py
+-rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 fknni-1.1.1/PKG-INFO
```

### Comparing `fknni-1.1.0/.cruft.json` & `fknni-1.1.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `fknni-1.1.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/.github/workflows/build.yaml` & `fknni-1.1.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/.github/workflows/release.yaml` & `fknni-1.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/.github/workflows/test.yaml` & `fknni-1.1.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/.pre-commit-config.yaml` & `fknni-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/LICENSE` & `fknni-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/README.md` & `fknni-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/Makefile` & `fknni-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/_templates/autosummary/class.rst` & `fknni-1.1.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/conf.py` & `fknni-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/contributing.md` & `fknni-1.1.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/extensions/typed_returns.py` & `fknni-1.1.1/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/notebooks/faiss.ipynb` & `fknni-1.1.1/docs/notebooks/faiss.ipynb`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/docs/references.bib` & `fknni-1.1.1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/pyproject.toml` & `fknni-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "fknni"
-version = "1.1.0"
+version = "1.1.1"
 description = "Fast implementations of KNN imputation."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Lukas Heumos"},
 ]
```

### Comparing `fknni-1.1.0/src/fknni/faiss/faiss.py` & `fknni-1.1.1/src/fknni/faiss/faiss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from typing import Literal, Union
+from __future__ import annotations
+
+from typing import Literal
 
 import faiss
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array, check_is_fitted
 
 
 class FaissImputer(BaseEstimator, TransformerMixin):
     """Imputer for completing missing values using Faiss, incorporating weighted averages based on distance."""
 
     def __init__(
         self,
-        missing_values: Union[int, float, str, None] = np.nan,
+        missing_values: int | float | str | None = np.nan,
         n_neighbors: int = 5,
         *,
         metric: Literal["l2", "ip"] = "l2",
         strategy: Literal["mean", "median", "weighted"] = "mean",
         index_factory: str = "Flat",
     ):
         """Initializes FaissImputer with specified parameters that are used for the imputation.
@@ -33,15 +35,15 @@
         super().__init__()
         self.missing_values = missing_values
         self.n_neighbors = n_neighbors
         self.metric = metric
         self.strategy = strategy
         self.index_factory = index_factory
 
-    def fit(self, X: np.ndarray | pd.DataFrame, *, y: np.ndarray | None = None) -> "FaissImputer":
+    def fit(self, X: np.ndarray | pd.DataFrame, *, y: np.ndarray | None = None) -> FaissImputer:
         """Fits the FaissImputer to the provided data.
 
         Args:
             X: Input data with potential missing values.
             y: Ignored, present for compatibility with sklearn's TransformerMixin.
 
         Raises:
```

### Comparing `fknni-1.1.0/tests/test_faiss_imputation.py` & `fknni-1.1.1/tests/test_faiss_imputation.py`

 * *Files identical despite different names*

### Comparing `fknni-1.1.0/PKG-INFO` & `fknni-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fknni
-Version: 1.1.0
+Version: 1.1.1
 Summary: Fast implementations of KNN imputation.
 Author: Lukas Heumos
 Maintainer-email: Lukas Heumos <lukas.heumos@posteo.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: faiss-cpu
```

