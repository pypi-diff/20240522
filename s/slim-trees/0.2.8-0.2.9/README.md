# Comparing `tmp/slim_trees-0.2.8.tar.gz` & `tmp/slim_trees-0.2.9.tar.gz`

## Comparing `slim_trees-0.2.8.tar` & `slim_trees-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/compression_utils.py
--rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/lgbm_booster.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/pickling.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/sklearn_tree.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/utils.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 slim_trees-0.2.8/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.8/LICENSE
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 slim_trees-0.2.8/README.md
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 slim_trees-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 slim_trees-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/__init__.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/compression_utils.py
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/lgbm_booster.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/pickling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/py.typed
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/sklearn_tree.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.9/slim_trees/utils.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 slim_trees-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 slim_trees-0.2.9/README.md
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 slim_trees-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 slim_trees-0.2.9/PKG-INFO
```

### Comparing `slim_trees-0.2.8/slim_trees/__init__.py` & `slim_trees-0.2.9/slim_trees/__init__.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.8/slim_trees/compression_utils.py` & `slim_trees-0.2.9/slim_trees/compression_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+from typing import Dict
+
 import numpy as np
+from numpy.typing import DTypeLike, NDArray
 
 
-def safe_cast(arr: np.array, dtype):
+def safe_cast(arr: NDArray, dtype: DTypeLike) -> NDArray:
     if np.can_cast(arr.max(), dtype) and np.can_cast(arr.min(), dtype):
         return arr.astype(dtype)
     raise ValueError(f"Cannot cast array to {dtype}.")
 
 
-def _is_in_neighborhood_of_int(arr, iinfo, eps=1e-12):
+def _is_in_neighborhood_of_int(arr: NDArray, iinfo: np.iinfo, eps: float = 1e-12):
     """
     Checks if the numbers are around an integer.
     np.abs(arr % 1 - 1) < eps checks if the number is in an epsilon neighborhood on the right side
     of the next int and arr % 1 < eps checks if the number is in an epsilon neighborhood on the left
     side of the next int.
     """
     return (
         (np.minimum(np.abs(arr % 1 - 1), arr % 1) < eps)
         & (arr >= iinfo.min)
         & (arr <= iinfo.max)
     )
 
 
-def compress_half_int_float_array(a, compression_dtype="int8"):
+def compress_half_int_float_array(
+    a: NDArray, compression_dtype: DTypeLike = "int8"
+) -> Dict:
     """Compress small integer and half-integer floats in a lossless fashion
 
     Idea:
         If most values in array <a> are small integers or half-integers, we can
         store them as float16, while keeping the rest as float64.
 
     Technical details:
@@ -44,15 +49,15 @@
         "a2_compressible": a2_compressible,
         "a_incompressible": a_incompressible,
     }
 
     return state
 
 
-def decompress_half_int_float_array(state):
+def decompress_half_int_float_array(state: Dict) -> NDArray:
     n_thresholds = len(state["a2_compressible"]) + len(state["a_incompressible"])
     is_compressible = np.unpackbits(
         state["is_compressible"], count=n_thresholds
     ).astype("bool")
     a = np.zeros(len(is_compressible), dtype="float64")
     a[is_compressible] = state["a2_compressible"] / 2.0
     a[~is_compressible] = state["a_incompressible"]
```

### Comparing `slim_trees-0.2.8/slim_trees/lgbm_booster.py` & `slim_trees-0.2.9/slim_trees/lgbm_booster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import copyreg
 import io
 import os
 import pickle
 import re
 import sys
-from typing import Any, BinaryIO, List, Tuple
+from typing import Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
 import numpy as np
+from numpy.typing import DTypeLike, NDArray
 from packaging.version import Version
 
 from slim_trees import __version__ as slim_trees_version
 from slim_trees.compression_utils import (
     compress_half_int_float_array,
     decompress_half_int_float_array,
     safe_cast,
@@ -38,15 +39,15 @@
     bytes_io = io.BytesIO()
     dump(model, bytes_io)
     return bytes_io.getvalue()
 
 
 def _booster_pickle(booster: Booster):
     assert isinstance(booster, Booster)
-    reconstructor, args, state = booster.__reduce__()
+    reconstructor, args, state = booster.__reduce__()  # type: ignore
     compressed_state = _compress_booster_state(state)
     return _booster_unpickle, (
         reconstructor,
         args,
         (slim_trees_version, compressed_state),
     )
 
@@ -121,17 +122,17 @@
     assert len(feats_map["right_child"]) == num_leaves - 1
 
     # features on leaf-level
     num_leaves = int(feats_map["num_leaves"][0])
     assert len(feats_map["leaf_value"]) == num_leaves
 
 
-def parse(str_list, dtype):
+def parse(str_list: Union[List[str], List[Optional[str]]], dtype: DTypeLike):
     if np.can_cast(dtype, np.int64):
-        int64_array = np.array(str_list, dtype=np.int64)
+        int64_array: NDArray = np.array(str_list, dtype=np.int64)
         return safe_cast(int64_array, dtype)
     assert np.can_cast(dtype, np.float64)
     return np.array(str_list, dtype=dtype)
 
 
 def _compress_booster_handle(model_string: str) -> Tuple[str, List[dict], str]:
     if not model_string.startswith(f"tree\nversion=v{lightgbm_version.major}"):
@@ -155,16 +156,16 @@
     trees: List[dict] = []
     for i, tree_match in enumerate(tree_matches):
         tree_name, features_list = tree_match
         _, tree_idx = tree_name.replace("\n", "").split("=")
         assert int(tree_idx) == i
 
         # extract features -- filter out empty ones
-        features = [f for f in features_list.split("\n") if "=" in f]
-        feats_map = dict(_extract_feature(fl) for fl in features)
+        features: List[str] = [f for f in features_list.split("\n") if "=" in f]
+        feats_map: Dict[str, List[str]] = dict(_extract_feature(fl) for fl in features)
         _validate_feature_lengths(feats_map)
 
         tree_values = {
             "num_leaves": int(feats_map["num_leaves"][0]),
             "num_cat": int(feats_map["num_cat"][0]),
             "split_feature": parse(feats_map["split_feature"], SPLIT_FEATURE_DTYPE),
             "threshold": compress_half_int_float_array(
@@ -181,15 +182,15 @@
         # if tree is linear, add additional features
         if int(feats_map["is_linear"][0]):
             # attributes: leaf_features, leaf_coeff, leaf_const, num_features
             # TODO: not all of these attributes might be needed.
             tree_values["num_features"] = parse(feats_map["num_features"], np.int32)
             tree_values["leaf_const"] = parse(feats_map["leaf_const"], LEAF_VALUE_DTYPE)
             tree_values["leaf_features"] = parse(
-                [s if s else -1 for s in feats_map["leaf_features"]],
+                [s if s else "-1" for s in feats_map["leaf_features"]],
                 np.int16,
             )
             tree_values["leaf_coeff"] = parse(
                 [s if s else None for s in feats_map["leaf_coeff"]], np.float64
             )
 
         # at last
```

### Comparing `slim_trees-0.2.8/slim_trees/pickling.py` & `slim_trees-0.2.9/slim_trees/pickling.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.8/slim_trees/sklearn_tree.py` & `slim_trees-0.2.9/slim_trees/sklearn_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     sklearn_version_ge_130 = sklearn_version >= Version("1.3")
 except ImportError:
     print("scikit-learn does not seem to be installed.")
     sys.exit(os.EX_CONFIG)
 
 import copyreg
 import pickle
-from typing import Any, BinaryIO
+from typing import Any, BinaryIO, Dict
 
 import numpy as np
+from numpy.typing import NDArray
 
 
 def dump(model: Any, file: BinaryIO):
     p = pickle.Pickler(file)
     p.dispatch_table = copyreg.dispatch_table.copy()
     p.dispatch_table[Tree] = _tree_pickle
     p.dump(model)
@@ -38,15 +39,15 @@
 
 def dumps(model: Any) -> bytes:
     bytes_io = io.BytesIO()
     dump(model, bytes_io)
     return bytes_io.getvalue()
 
 
-def _tree_pickle(tree):
+def _tree_pickle(tree: Tree):
     assert isinstance(tree, Tree)
     reconstructor, args, state = tree.__reduce__()
     compressed_state = _compress_tree_state(state)
     return _tree_unpickle, (reconstructor, args, (slim_trees_version, compressed_state))
 
 
 def _tree_unpickle(reconstructor, args, compressed_state):
@@ -55,15 +56,15 @@
 
     tree = reconstructor(*args)
     decompressed_state = _decompress_tree_state(state)
     tree.__setstate__(decompressed_state)
     return tree
 
 
-def _compress_tree_state(state: dict):
+def _compress_tree_state(state: Dict) -> Dict:
     """
     Compresses a Tree state.
     :param state: dictionary with 'max_depth', 'node_count', 'nodes', 'values' as keys.
     :return: dictionary with compressed tree state, only with data that is relevant for prediction.
     """
     assert isinstance(state, dict)
     assert state.keys() == {"max_depth", "node_count", "nodes", "values"}
@@ -115,15 +116,15 @@
             {"missing_go_to_left": np.packbits(missing_go_to_left)}
             if sklearn_version_ge_130
             else {}
         ),
     }
 
 
-def _decompress_tree_state(state: dict):
+def _decompress_tree_state(state: Dict) -> Dict:
     """
     Decompresses a Tree state.
     :param state: 'children_left', 'children_right', 'features', 'thresholds', 'values' as keys.
                   If the sklearn version is >=1.3.0, also 'missing_go_to_left' is a key.
                   'max_depth' and 'node_count' are passed through.
     :return: dictionary with decompressed tree state.
     """
@@ -144,21 +145,21 @@
     }:
         raise ValueError(
             "Invalid tree structure. Do you use an unsupported scikit-learn version "
             "or try to load a model that was pickled with a different version of scikit-learn?"
         )
     n_nodes = state["node_count"]
 
-    children_left = np.zeros(n_nodes, dtype=np.int64)
-    children_right = np.zeros(n_nodes, dtype=np.int64)
-    features = np.zeros(n_nodes, dtype=np.int64)
-    thresholds = np.zeros(n_nodes, dtype=np.float64)
+    children_left: NDArray = np.zeros(n_nodes, dtype=np.int64)
+    children_right: NDArray = np.zeros(n_nodes, dtype=np.int64)
+    features: NDArray = np.zeros(n_nodes, dtype=np.int64)
+    thresholds: NDArray = np.zeros(n_nodes, dtype=np.float64)
     # same shape as values but with all nodes instead of only the leaves
-    values = np.zeros((n_nodes, *state["values"].shape[1:]), dtype=np.float64)
-    missing_go_to_left = np.zeros(n_nodes, dtype="uint8")
+    values: NDArray = np.zeros((n_nodes, *state["values"].shape[1:]), dtype=np.float64)
+    missing_go_to_left: NDArray = np.zeros(n_nodes, dtype="uint8")
 
     is_leaf = np.unpackbits(state["is_leaf"], count=n_nodes).astype("bool")
     children_left[~is_leaf] = state["children_left"]
     children_left[is_leaf] = -1
     children_right[~is_leaf] = state["children_right"]
     children_right[is_leaf] = -1
     features[~is_leaf] = state["features"]
```

### Comparing `slim_trees-0.2.8/.gitignore` & `slim_trees-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.8/LICENSE` & `slim_trees-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.8/README.md` & `slim_trees-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.8/pyproject.toml` & `slim_trees-0.2.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "slim-trees"
 description = "A python package for efficient pickling of ML models."
-version = "0.2.8"
+version = "0.2.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 authors = [
     { name = "Pavel Zwerschke", email = "pavel.zwerschke@quantco.com" },
 ]
 classifiers = [
@@ -81,10 +81,14 @@
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 
 [tool.mypy]
 python_version = "3.8"
-ignore_missing_imports = true
 no_implicit_optional = true
 check_untyped_defs = true
+
+[[tool.mypy.overrides]]
+# https://github.com/scikit-learn/scikit-learn/issues/16705
+module = ["sklearn.*"]
+ignore_missing_imports = true
```

### Comparing `slim_trees-0.2.8/PKG-INFO` & `slim_trees-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: slim-trees
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python package for efficient pickling of ML models.
 Project-URL: Homepage, https://github.com/quantco/slim-trees
 Author-email: Pavel Zwerschke <pavel.zwerschke@quantco.com>
 License: MIT License
         
         Copyright (c) 2023 Pavel Zwerschke, Yasin Tatar and Jonas Haag
```

