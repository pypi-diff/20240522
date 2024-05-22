# Comparing `tmp/motile-0.2.0.tar.gz` & `tmp/motile-0.2.1.tar.gz`

## Comparing `motile-0.2.0.tar` & `motile-0.2.1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 motile-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 motile-0.2.0/Makefile
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 motile-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 motile-0.2.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 motile-0.2.0/.github/workflows/deploy.yaml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 motile-0.2.0/.github/workflows/publish-docs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 motile-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 motile-0.2.0/docs/make.bat
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/api.rst
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0    12605 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/extending.rst
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/install.rst
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/learning.rst
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/quickstart.rst
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/_static/css/custom.css
--rw-r--r--   0        0        0    26455 2020-02-02 00:00:00.000000 motile-0.2.0/docs/source/img/motile.svg
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 motile-0.2.0/motile/__init__.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 motile-0.2.0/motile/_types.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 motile-0.2.0/motile/data.py
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 motile-0.2.0/motile/plot.py
--rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 motile-0.2.0/motile/solver.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 motile-0.2.0/motile/ssvm.py
--rw-r--r--   0        0        0     8717 2020-02-02 00:00:00.000000 motile-0.2.0/motile/track_graph.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/constraint.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/expression.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/max_children.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/max_parents.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/pin.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 motile-0.2.0/motile/constraints/select_edge_nodes.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/__init__.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/appear.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/costs.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/disappear.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/edge_distance.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/edge_selection.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/features.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/node_selection.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/split.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/weight.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 motile-0.2.0/motile/costs/weights.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/edge_selected.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/node_appear.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/node_disappear.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/node_selected.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/node_split.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 motile-0.2.0/motile/variables/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 motile-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 motile-0.2.0/tests/test_api.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 motile-0.2.0/tests/test_constraints.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 motile-0.2.0/tests/test_costs.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 motile-0.2.0/tests/test_plot.py
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 motile-0.2.0/tests/test_structsvm.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 motile-0.2.0/tests/test_variables.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 motile-0.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 motile-0.2.0/LICENSE
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 motile-0.2.0/README.md
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 motile-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 motile-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 motile-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 motile-0.2.1/Makefile
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 motile-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 motile-0.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 motile-0.2.1/.github/workflows/deploy.yaml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 motile-0.2.1/.github/workflows/publish-docs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 motile-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 motile-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0    12605 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/extending.rst
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/install.rst
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/learning.rst
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/quickstart.rst
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/_static/css/custom.css
+-rw-r--r--   0        0        0    26455 2020-02-02 00:00:00.000000 motile-0.2.1/docs/source/img/motile.svg
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 motile-0.2.1/motile/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 motile-0.2.1/motile/_types.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 motile-0.2.1/motile/data.py
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 motile-0.2.1/motile/plot.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 motile-0.2.1/motile/solver.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 motile-0.2.1/motile/ssvm.py
+-rw-r--r--   0        0        0     8717 2020-02-02 00:00:00.000000 motile-0.2.1/motile/track_graph.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/constraint.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/exclusive_nodes.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/expression.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/max_children.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/max_parents.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/pin.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 motile-0.2.1/motile/constraints/select_edge_nodes.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/appear.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/costs.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/disappear.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/edge_distance.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/edge_selection.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/features.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/node_selection.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/split.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/weight.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 motile-0.2.1/motile/costs/weights.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/edge_selected.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/node_appear.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/node_disappear.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/node_selected.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/node_split.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 motile-0.2.1/motile/variables/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 motile-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 motile-0.2.1/tests/test_api.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 motile-0.2.1/tests/test_constraints.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 motile-0.2.1/tests/test_costs.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 motile-0.2.1/tests/test_plot.py
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 motile-0.2.1/tests/test_structsvm.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 motile-0.2.1/tests/test_variables.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 motile-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 motile-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 motile-0.2.1/README.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 motile-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 motile-0.2.1/PKG-INFO
```

### Comparing `motile-0.2.0/Makefile` & `motile-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/.github/workflows/ci.yaml` & `motile-0.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/.github/workflows/deploy.yaml` & `motile-0.2.1/.github/workflows/deploy.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,10 +20,10 @@
           python -m pip install build
           python -m build
       - name: Publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-      - uses: softprops/action-gh-release@v1
+      - uses: softprops/action-gh-release@v2
         with:
           generate_release_notes: true
```

### Comparing `motile-0.2.0/.github/workflows/publish-docs.yaml` & `motile-0.2.1/.github/workflows/publish-docs.yaml`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/Makefile` & `motile-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/make.bat` & `motile-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/api.rst` & `motile-0.2.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/conf.py` & `motile-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/extending.rst` & `motile-0.2.1/docs/source/extending.rst`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/index.rst` & `motile-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/install.rst` & `motile-0.2.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/learning.rst` & `motile-0.2.1/docs/source/learning.rst`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/quickstart.rst` & `motile-0.2.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/_static/css/custom.css` & `motile-0.2.1/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/docs/source/img/motile.svg` & `motile-0.2.1/docs/source/img/motile.svg`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/_types.py` & `motile-0.2.1/motile/_types.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/data.py` & `motile-0.2.1/motile/data.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/plot.py` & `motile-0.2.1/motile/plot.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/solver.py` & `motile-0.2.1/motile/solver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, TypeVar, cast
+import warnings
+from typing import TYPE_CHECKING, Callable, Mapping, TypeVar, cast
 
 import ilpy
 import numpy as np
 
 from .constraints import SelectEdgeNodes
 from .constraints.constraint import Constraint
 from .costs import Features, Weight, Weights
 from .ssvm import fit_weights
+from .track_graph import TrackGraph
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from motile.costs import Costs
-    from motile.track_graph import TrackGraph
     from motile.variables import Variable
 
     V = TypeVar("V", bound=Variable)
 
 
 class Solver:
     """Create a solver for a given track graph.
@@ -33,14 +34,28 @@
             constraints that ensure consistencies between selected nodes and
             edges are added.
     """
 
     def __init__(
         self, track_graph: TrackGraph, skip_core_constraints: bool = False
     ) -> None:
+        if not isinstance(track_graph, TrackGraph):
+            import networkx as nx
+
+            if isinstance(track_graph, nx.Graph):
+                warnings.warn(
+                    "Coercing networkx graph to TrackGraph with frame_attribute='t'. "
+                    "To silence this warning, please pass a motile.TrackGraph instance."
+                )
+                track_graph = TrackGraph(track_graph)
+            else:  # pragma: no cover
+                raise ValueError(
+                    f"Expected a TrackGraph or networkx.Graph, got {type(track_graph)}"
+                )
+
         self.graph = track_graph
         self.variables: dict[type[Variable], Variable] = {}
         self.variable_types: dict[int, ilpy.VariableType] = {}
 
         self.weights = Weights()
         self.weights.register_modify_callback(self._on_weights_modified)
         self._weights_changed = True
@@ -101,25 +116,40 @@
                 The :class:`~motile.constraints.Constraint` to add.
         """
         logger.info("Adding %s constraints...", type(constraints).__name__)
 
         for constraint in constraints.instantiate(self):
             self.constraints.add(constraint)
 
-    def solve(self, timeout: float = 0.0, num_threads: int = 1) -> ilpy.Solution:
+    def solve(
+        self,
+        timeout: float = 0.0,
+        num_threads: int = 1,
+        verbose: bool = False,
+        backend: ilpy.Preference = ilpy.Preference.Any,
+        on_event: Callable[[Mapping], None] | None = None,
+    ) -> ilpy.Solution:
         """Solve the global optimization problem.
 
         Args:
             timeout:
                 The timeout for the ILP solver, in seconds. Default (0.0) is no
                 timeout. If the solver times out, the best solution encountered
                 so far is returned (if any has been found at all).
-
             num_threads:
                 The number of threads the ILP solver uses.
+            verbose:
+                If true, print more information from ILP solver. Defaults to False.
+            backend:
+                The ILP solver backend to use. Defaults to Any.
+            on_event:
+                A callback function that will be called when the solver emits an event.
+                Should accept an event data dict. (see `ilpy.EventData` for typing info
+                which may be imported inside of a TYPE_CHECKING block.)
+                Defaults to None.
 
         Returns:
             :class:`ilpy.Solution`, a vector of variable values. Use
             :func:`get_variables` to find the indices of variables in this
             vector.
         """
         self.objective = ilpy.Objective(self.num_variables)
@@ -128,25 +158,26 @@
             self.objective.set_coefficient(i, c)
 
         # TODO: support other variable types
         self.ilp_solver = ilpy.Solver(
             self.num_variables,
             ilpy.VariableType.Binary,
             variable_types=self.variable_types,
-            preference=ilpy.Preference.Any,
+            preference=backend,
         )
 
         self.ilp_solver.set_objective(self.objective)
         self.ilp_solver.set_constraints(self.constraints)
 
         self.ilp_solver.set_num_threads(num_threads)
         if timeout > 0:
             self.ilp_solver.set_timeout(timeout)
 
-        self.ilp_solver.set_verbose(False)
+        self.ilp_solver.set_verbose(verbose)
+        self.ilp_solver.set_event_callback(on_event)
 
         self.solution = self.ilp_solver.solve()
         if message := self.solution.get_status():
             logger.info("ILP solver returned with: %s", message)
 
         return self.solution
 
@@ -259,7 +290,50 @@
 
     def _on_weights_modified(self, old_value: float | None, new_value: float) -> None:
         if old_value != new_value:
             if not self._weights_changed:
                 logger.info("Weights have changed")
 
             self._weights_changed = True
+
+    def get_selected_subgraph(
+        self, solution: ilpy.Solution | None = None
+    ) -> TrackGraph:
+        """Return TrackGraph with only the selected nodes/edges from the solution.
+
+        Args:
+            solution:
+                The solution to use. If not provided, the last solution is used.
+
+        Returns:
+            A new TrackGraph with only the selected nodes and edges.
+
+        Raises:
+            RuntimeError: If no solution is provided and the solver has not been solved
+            yet.
+        """
+        from motile.variables import EdgeSelected, NodeSelected
+
+        if solution is None:
+            solution = self.solution
+
+        # TODO:
+        # in theory this could be made more efficient by using a nx.DiGraph view
+        # but TrackGraph itself doesn't provide views (and isn't a subclass)
+        if not solution:
+            raise RuntimeError(
+                "No solution available. Run solve() first or manually pass a solution."
+            )
+
+        node_selected = self.get_variables(NodeSelected)
+        edge_selected = self.get_variables(EdgeSelected)
+        selected_graph = TrackGraph()
+
+        for node_id, node in self.graph.nodes.items():
+            if solution[node_selected[node_id]] > 0.5:
+                selected_graph.add_node(node_id, node)
+
+        for edge_id, edge in self.graph.edges.items():
+            if solution[edge_selected[edge_id]] > 0.5:
+                selected_graph.add_edge(edge_id, edge)
+
+        return selected_graph
```

### Comparing `motile-0.2.0/motile/ssvm.py` & `motile-0.2.1/motile/ssvm.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/track_graph.py` & `motile-0.2.1/motile/track_graph.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/constraints/constraint.py` & `motile-0.2.1/motile/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/constraints/expression.py` & `motile-0.2.1/motile/constraints/expression.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/constraints/max_children.py` & `motile-0.2.1/motile/constraints/max_children.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/constraints/max_parents.py` & `motile-0.2.1/motile/constraints/max_parents.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/constraints/pin.py` & `motile-0.2.1/motile/constraints/pin.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/constraints/select_edge_nodes.py` & `motile-0.2.1/motile/constraints/select_edge_nodes.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/appear.py` & `motile-0.2.1/motile/costs/appear.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/costs.py` & `motile-0.2.1/motile/costs/costs.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/disappear.py` & `motile-0.2.1/motile/costs/disappear.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/edge_distance.py` & `motile-0.2.1/motile/costs/node_selection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING
 
-import numpy as np
-
-from ..variables import EdgeSelected
+from ..variables import NodeSelected
 from .costs import Costs
 from .weight import Weight
 
 if TYPE_CHECKING:
     from motile.solver import Solver
 
 
-class EdgeDistance(Costs):
-    """Costs for :class:`~motile.variables.EdgeSelected` variables.
-
-    Costs are based on the spatial distance of the incident nodes.
+class NodeSelection(Costs):
+    """Costs for :class:`~motile.variables.NodeSelected` variables.
 
     Args:
-        position_attributes:
-            The names of the node attributes that correspond to their spatial
-            position, e.g., ``('z', 'y', 'x')``.
-
         weight:
-            The weight to apply to the distance to convert it into a cost.
+            The weight to apply to the cost given by the ``costs`` attribute of
+            each node.
+
+        attribute:
+            The name of the node attribute to use to look up costs. Default is
+            ``'costs'``.
+
+        constant:
+            A constant cost for each selected node. Default is ``0.0``.
     """
 
     def __init__(
-        self, position_attributes: tuple[str, ...], weight: float = 1.0
+        self, weight: float, attribute: str = "costs", constant: float = 0.0
     ) -> None:
-        self.position_attributes = position_attributes
         self.weight = Weight(weight)
+        self.constant = Weight(constant)
+        self.attribute = attribute
 
     def apply(self, solver: Solver) -> None:
-        edge_variables = solver.get_variables(EdgeSelected)
-        for key, index in edge_variables.items():
-            u, v = cast("tuple[int, int]", key)
-            pos_u = np.array(
-                [solver.graph.nodes[u][p] for p in self.position_attributes]
-            )
-            pos_v = np.array(
-                [solver.graph.nodes[v][p] for p in self.position_attributes]
-            )
+        node_variables = solver.get_variables(NodeSelected)
 
-            feature = np.linalg.norm(pos_u - pos_v)
-
-            solver.add_variable_cost(index, feature, self.weight)
+        for node, index in node_variables.items():
+            solver.add_variable_cost(
+                index, solver.graph.nodes[node][self.attribute], self.weight
+            )
+            solver.add_variable_cost(index, 1.0, self.constant)
```

### Comparing `motile-0.2.0/motile/costs/edge_selection.py` & `motile-0.2.1/motile/costs/edge_selection.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/features.py` & `motile-0.2.1/motile/costs/features.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/node_selection.py` & `motile-0.2.1/motile/costs/split.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from ..variables import NodeSelected
+from ..variables import NodeSplit
 from .costs import Costs
 from .weight import Weight
 
 if TYPE_CHECKING:
     from motile.solver import Solver
 
 
-class NodeSelection(Costs):
-    """Costs for :class:`~motile.variables.NodeSelected` variables.
+class Split(Costs):
+    """Costs for :class:`~motile.variables.NodeSplit` variables.
 
     Args:
         weight:
-            The weight to apply to the cost given by the ``costs`` attribute of
-            each node.
+            The weight to apply to the cost of each split.
 
         attribute:
-            The name of the node attribute to use to look up costs. Default is
-            ``'costs'``.
+            The name of the attribute to use to look up costs. Default is
+            ``None``, which means that a constant cost is used.
 
         constant:
-            A constant cost for each selected node. Default is ``0.0``.
+            A constant cost for each node that has more than one selected
+            child.
     """
 
     def __init__(
-        self, weight: float, attribute: str = "costs", constant: float = 0.0
+        self, weight: float = 1, attribute: str | None = None, constant: float = 0
     ) -> None:
         self.weight = Weight(weight)
         self.constant = Weight(constant)
         self.attribute = attribute
 
     def apply(self, solver: Solver) -> None:
-        node_variables = solver.get_variables(NodeSelected)
+        split_indicators = solver.get_variables(NodeSplit)
 
-        for node, index in node_variables.items():
-            solver.add_variable_cost(
-                index, solver.graph.nodes[node][self.attribute], self.weight
-            )
+        for node, index in split_indicators.items():
+            if self.attribute is not None:
+                solver.add_variable_cost(
+                    index, solver.graph.nodes[node][self.attribute], self.weight
+                )
             solver.add_variable_cost(index, 1.0, self.constant)
```

### Comparing `motile-0.2.0/motile/costs/weight.py` & `motile-0.2.1/motile/costs/weight.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/costs/weights.py` & `motile-0.2.1/motile/costs/weights.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/variables/node_appear.py` & `motile-0.2.1/motile/variables/node_appear.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/variables/node_disappear.py` & `motile-0.2.1/motile/variables/node_disappear.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/variables/node_split.py` & `motile-0.2.1/motile/variables/node_split.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/motile/variables/variable.py` & `motile-0.2.1/motile/variables/variable.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/tests/test_api.py` & `motile-0.2.1/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from unittest.mock import Mock
+
 import motile
 from motile.constraints import MaxChildren, MaxParents
 from motile.costs import (
     Appear,
     EdgeDistance,
     EdgeSelection,
     NodeSelection,
@@ -56,20 +58,27 @@
     graph = arlo_graph()
 
     solver = motile.Solver(graph)
     solver.add_costs(NodeSelection(weight=-1.0, attribute="score", constant=-100.0))
     solver.add_costs(
         EdgeSelection(weight=0.5, attribute="prediction_distance", constant=-1.0)
     )
-    solver.add_costs(EdgeDistance(position_attributes=("x",), weight=0.5))
+    solver.add_costs(EdgeDistance(position_attribute=("x",), weight=0.5))
     solver.add_costs(Appear(constant=200.0, attribute="score", weight=-1.0))
     solver.add_costs(Split(constant=100.0, attribute="score", weight=1.0))
 
     solver.add_constraints(MaxParents(1))
     solver.add_constraints(MaxChildren(2))
 
-    solution = solver.solve()
-
-    assert _selected_edges(solver) == [(0, 2), (1, 3), (2, 4), (3, 5)]
-    assert _selected_nodes(solver) == [0, 1, 2, 3, 4, 5]
+    callback = Mock()
+    solution = solver.solve(on_event=callback)
+    assert callback.call_count
+    subgraph = solver.get_selected_subgraph()
+
+    assert (
+        list(subgraph.edges)
+        == _selected_edges(solver)
+        == [(0, 2), (1, 3), (2, 4), (3, 5)]
+    )
+    assert list(subgraph.nodes) == _selected_nodes(solver) == [0, 1, 2, 3, 4, 5]
     cost = solution.get_value()
     assert cost == -206.0, f"{cost=}"
```

### Comparing `motile-0.2.0/tests/test_constraints.py` & `motile-0.2.1/tests/test_constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import motile
 import pytest
-from motile.constraints import ExpressionConstraint, MaxChildren, MaxParents, Pin
-from motile.costs import EdgeSelection, NodeSelection
-from motile.data import arlo_graph
+from motile.constraints import (
+    ExclusiveNodes,
+    ExpressionConstraint,
+    MaxChildren,
+    MaxParents,
+    Pin,
+)
+from motile.costs import Appear, EdgeSelection, NodeSelection
+from motile.data import arlo_graph, arlo_graph_nx
 
 from .test_api import _selected_edges, _selected_nodes
 
 
 @pytest.fixture
 def solver():
     return motile.Solver(arlo_graph())
 
 
+def test_graph_casting() -> None:
+    with pytest.warns(UserWarning, match="Coercing networkx graph to TrackGraph"):
+        motile.Solver(arlo_graph_nx())
+
+
 def test_pin(solver: motile.Solver) -> None:
     # pin the value of two edges:
     solver.graph.edges[(0, 2)]["pin_to"] = False  # type: ignore
     solver.graph.edges[(3, 6)]["pin_to"] = True  # type: ignore
 
     assert _selected_edges(solver) != [(3, 6)], "test invalid"
     solver.add_constraints(Pin("pin_to"))
@@ -49,7 +60,25 @@
         EdgeSelection(weight=1.0, attribute="prediction_distance", constant=-100)
     )
 
     expect = [(0, 2), (1, 3), (2, 4), (3, 5), (3, 6)]
     assert _selected_edges(solver) != expect, "test invalid"
     solver.add_constraints(MaxParents(1))
     assert _selected_edges(solver) == expect
+
+
+def test_exlusive_nodes(solver: motile.Solver) -> None:
+    exclusive_sets = [
+        [0, 1],
+        [2, 3],
+        [4, 5],
+    ]
+
+    solver.add_costs(
+        EdgeSelection(weight=1.0, attribute="prediction_distance", constant=-100)
+    )
+    solver.add_costs(Appear(constant=2.0, attribute="score", weight=0))
+    solver.add_constraints(MaxParents(1))
+    solver.add_constraints(MaxChildren(2))
+    solver.add_constraints(ExclusiveNodes(exclusive_sets))
+
+    assert _selected_nodes(solver) == [1, 3, 5, 6], "test invalid"
```

### Comparing `motile-0.2.0/tests/test_costs.py` & `motile-0.2.1/tests/test_costs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # first solve without ignore attribute:
 
     solver = motile.Solver(graph)
     solver.add_costs(NodeSelection(weight=-1.0, attribute="score", constant=-100.0))
     solver.add_costs(
         EdgeSelection(weight=0.5, attribute="prediction_distance", constant=-1.0)
     )
-    solver.add_costs(EdgeDistance(position_attributes=("x",), weight=0.5))
+    solver.add_costs(EdgeDistance(position_attribute=("x",), weight=0.5))
     solver.add_costs(Appear(constant=200.0, attribute="score", weight=-1.0))
     solver.add_costs(Split(constant=100.0, attribute="score", weight=1.0))
 
     solver.add_constraints(MaxParents(1))
     solver.add_constraints(MaxChildren(2))
 
     solution = solver.solve()
@@ -38,15 +38,15 @@
         graph.nodes[first_node]["ignore_appear_cost"] = True
 
     solver = motile.Solver(graph)
     solver.add_costs(NodeSelection(weight=-1.0, attribute="score", constant=-100.0))
     solver.add_costs(
         EdgeSelection(weight=0.5, attribute="prediction_distance", constant=-1.0)
     )
-    solver.add_costs(EdgeDistance(position_attributes=("x",), weight=0.5))
+    solver.add_costs(EdgeDistance(position_attribute="x", weight=0.5))
     solver.add_costs(
         Appear(
             constant=200.0,
             attribute="score",
             weight=-1.0,
             ignore_attribute="ignore_appear_cost",
         )
```

### Comparing `motile-0.2.0/tests/test_plot.py` & `motile-0.2.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/tests/test_structsvm.py` & `motile-0.2.1/tests/test_structsvm.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/tests/test_variables.py` & `motile-0.2.1/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/LICENSE` & `motile-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/README.md` & `motile-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `motile-0.2.0/pyproject.toml` & `motile-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 name = "motile"
 description = "Multi-Object Tracker using Integer Linear Equations"
 readme = "README.md"
 license = { text = "MIT" }
 authors = [
     { name = 'Jan Funke', email = 'funkej@janelia.hhmi.org' },
     { name = 'Talley Lambert', email = 'talley.lambert@gmail.com' },
+    { name = 'Caroline Malin-Mayor', email = 'malinmayorc@janelia.hhmi.org' },
     { name = 'Benjamin Gallusser', email = 'bgallusser@googlemail.com' },
     { name = 'Florian Jug', email = 'florian.jug@fht.org' },
 ]
 dynamic = ["version"]
-dependencies = ['networkx', 'ilpy>=0.3.1', 'numpy', 'structsvm']
+dependencies = ['networkx', 'ilpy>=0.4.0', 'numpy', 'structsvm']
 
 [project.optional-dependencies]
 dev = ["pre-commit", "pytest", "pytest-cov", "ruff", "twine", "build"]
 test = ["pytest", "pytest-cov", "plotly"]
 docs = [
     "ipykernel",
     "jupyter_sphinx",
@@ -40,35 +41,36 @@
 [tool.hatch.version]
 path = "motile/__init__.py"
 
 # https://beta.ruff.rs/docs
 [tool.ruff]
 target-version = "py38"
 src = ["motile"]
+
+[tool.ruff.lint]
 select = [
     "F",   # pyflakes
     "E",   # pycodestyle
     "I",   # isort
     "UP",  # pyupgrade 
     "RUF", # ruff specific rules
     "D",
 ]
 ignore = [
     "D100", # Missing docstring in public mod
     "D104", # Missing docstring in public package
     "D105", # Missing docstring in magic method
     "D107", # Missing docstring in `__init__`
-
     "D102", # Missing docstring in public method
-    # "D205", # 1 blank line required between summary line and description
-
 ]
-[tool.ruff.pydocstyle]
+
+[tool.ruff.lint.pydocstyle]
 convention = "google"
-[tool.ruff.per-file-ignores]
+
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["D"]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = [
```

### Comparing `motile-0.2.0/PKG-INFO` & `motile-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: motile
-Version: 0.2.0
+Version: 0.2.1
 Summary: Multi-Object Tracker using Integer Linear Equations
 Project-URL: homepage, https://github.com/funkelab/motile
-Author-email: Jan Funke <funkej@janelia.hhmi.org>, Talley Lambert <talley.lambert@gmail.com>, Benjamin Gallusser <bgallusser@googlemail.com>, Florian Jug <florian.jug@fht.org>
+Author-email: Jan Funke <funkej@janelia.hhmi.org>, Talley Lambert <talley.lambert@gmail.com>, Caroline Malin-Mayor <malinmayorc@janelia.hhmi.org>, Benjamin Gallusser <bgallusser@googlemail.com>, Florian Jug <florian.jug@fht.org>
 License: MIT
 License-File: LICENSE
-Requires-Dist: ilpy>=0.3.1
+Requires-Dist: ilpy>=0.4.0
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: structsvm
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
```

