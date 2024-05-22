# Comparing `tmp/causy-0.0.9.tar.gz` & `tmp/causy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causy-0.0.9.tar", max compression
+gzip compressed data, was "causy-0.1.0.tar", max compression
```

## Comparing `causy-0.0.9.tar` & `causy-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,56 @@
--rw-r--r--   0        0        0     1202 2023-10-22 12:24:06.291515 causy-0.0.9/README.md
--rw-r--r--   0        0        0        1 2023-10-22 12:24:06.292007 causy-0.0.9/causy/__init__.py
--rw-r--r--   0        0        0     2789 2023-10-22 12:24:06.292377 causy-0.0.9/causy/algorithms.py
--rw-r--r--   0        0        0     4285 2023-10-22 12:24:06.292726 causy-0.0.9/causy/cli.py
--rw-r--r--   0        0        0      798 2023-10-22 12:24:06.293066 causy-0.0.9/causy/exit_conditions.py
--rw-r--r--   0        0        0     6072 2023-10-22 12:24:06.293405 causy-0.0.9/causy/generators.py
--rw-r--r--   0        0        0    19508 2023-10-22 12:24:06.293831 causy-0.0.9/causy/graph.py
--rw-r--r--   0        0        0    10748 2023-10-22 12:24:06.294233 causy-0.0.9/causy/independence_tests.py
--rw-r--r--   0        0        0     6778 2023-10-22 12:24:06.294595 causy-0.0.9/causy/interfaces.py
--rw-r--r--   0        0        0    11462 2023-10-22 12:24:06.295032 causy-0.0.9/causy/orientation_tests.py
--rw-r--r--   0        0        0     4926 2023-10-22 12:24:06.295413 causy-0.0.9/causy/utils.py
--rw-r--r--   0        0        0      725 2023-10-22 12:24:06.296713 causy-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 causy-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-22 20:20:14.159964 causy-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6185 2024-05-22 20:20:14.159964 causy-0.1.0/README.md
+-rw-r--r--   0        0        0      374 2024-05-22 20:20:14.159964 causy-0.1.0/causy/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/algorithms/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/algorithms/fci.py
+-rw-r--r--   0        0        0     6510 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/algorithms/pc.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/independence_tests/__init__.py
+-rw-r--r--   0        0        0    10875 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/independence_tests/common.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/orientation_rules/__init__.py
+-rw-r--r--   0        0        0     3932 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/orientation_rules/fci.py
+-rw-r--r--   0        0        0    13744 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_discovery/constraint/orientation_rules/pc.py
+-rw-r--r--   0        0        0     2339 2024-05-22 20:20:14.159964 causy-0.1.0/causy/causal_effect_estimation/multivariate_regression.py
+-rw-r--r--   0        0        0     3037 2024-05-22 20:20:14.159964 causy-0.1.0/causy/cli.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:14.159964 causy-0.1.0/causy/common_pipeline_steps/__init__.py
+-rw-r--r--   0        0        0     1596 2024-05-22 20:20:14.159964 causy-0.1.0/causy/common_pipeline_steps/calculation.py
+-rw-r--r--   0        0        0      806 2024-05-22 20:20:14.159964 causy-0.1.0/causy/common_pipeline_steps/exit_conditions.py
+-rw-r--r--   0        0        0     2981 2024-05-22 20:20:14.159964 causy-0.1.0/causy/common_pipeline_steps/logic.py
+-rw-r--r--   0        0        0     1567 2024-05-22 20:20:14.159964 causy-0.1.0/causy/common_pipeline_steps/placeholder.py
+-rw-r--r--   0        0        0     1264 2024-05-22 20:20:14.159964 causy-0.1.0/causy/contrib/graph_ui.py
+-rw-r--r--   0        0        0     3948 2024-05-22 20:20:14.159964 causy-0.1.0/causy/data_loader.py
+-rw-r--r--   0        0        0     2994 2024-05-22 20:20:14.159964 causy-0.1.0/causy/edge_types.py
+-rw-r--r--   0        0        0     8374 2024-05-22 20:20:14.159964 causy-0.1.0/causy/generators.py
+-rw-r--r--   0        0        0    22204 2024-05-22 20:20:14.159964 causy-0.1.0/causy/graph.py
+-rw-r--r--   0        0        0    15716 2024-05-22 20:20:14.159964 causy-0.1.0/causy/graph_model.py
+-rw-r--r--   0        0        0     1608 2024-05-22 20:20:14.159964 causy-0.1.0/causy/graph_utils.py
+-rw-r--r--   0        0        0    10486 2024-05-22 20:20:14.159964 causy-0.1.0/causy/interfaces.py
+-rw-r--r--   0        0        0      698 2024-05-22 20:20:14.159964 causy-0.1.0/causy/math_utils.py
+-rw-r--r--   0        0        0     2738 2024-05-22 20:20:14.159964 causy-0.1.0/causy/models.py
+-rw-r--r--   0        0        0    15747 2024-05-22 20:20:14.163964 causy-0.1.0/causy/sample_generator.py
+-rw-r--r--   0        0        0     3591 2024-05-22 20:20:14.163964 causy-0.1.0/causy/serialization.py
+-rw-r--r--   0        0        0     9316 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    39587 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0     8407 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/apple-touch-icon.png
+-rw-r--r--   0        0        0     7633 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/assets/index-4c14e422.css
+-rw-r--r--   0        0        0  2785907 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/assets/index-eacbaea2.js
+-rw-r--r--   0        0        0     3442 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/assets/style-8961fb08.css
+-rw-r--r--   0        0        0     2695 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/assets/vueflow-3647b393.css
+-rw-r--r--   0        0        0    26265 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/causy-500.png
+-rw-r--r--   0        0        0      399 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/favicon-16x16.png
+-rw-r--r--   0        0        0      838 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/favicon.ico
+-rw-r--r--   0        0        0      657 2024-05-22 20:18:23.000000 causy-0.1.0/causy/static/index.html
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:14.163964 causy-0.1.0/causy/ui/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-22 20:20:14.163964 causy-0.1.0/causy/ui/cli.py
+-rw-r--r--   0        0        0      672 2024-05-22 20:20:14.163964 causy-0.1.0/causy/ui/models.py
+-rw-r--r--   0        0        0     6643 2024-05-22 20:20:14.163964 causy-0.1.0/causy/ui/server.py
+-rw-r--r--   0        0        0     7503 2024-05-22 20:20:14.163964 causy-0.1.0/causy/variables.py
+-rw-r--r--   0        0        0      929 2024-05-22 20:20:14.163964 causy-0.1.0/causy/workspaces/__init__.py
+-rw-r--r--   0        0        0    29335 2024-05-22 20:20:14.163964 causy-0.1.0/causy/workspaces/cli.py
+-rw-r--r--   0        0        0      683 2024-05-22 20:20:14.163964 causy-0.1.0/causy/workspaces/models.py
+-rw-r--r--   0        0        0      708 2024-05-22 20:20:14.163964 causy-0.1.0/causy/workspaces/templates/dataloader.py.tpl
+-rw-r--r--   0        0        0      271 2024-05-22 20:20:14.163964 causy-0.1.0/causy/workspaces/templates/pipeline.py.tpl
+-rw-r--r--   0        0        0     1008 2024-05-22 20:20:14.163964 causy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7113 1970-01-01 00:00:00.000000 causy-0.1.0/PKG-INFO
```

### Comparing `causy-0.0.9/causy/exit_conditions.py` & `causy-0.1.0/causy/common_pipeline_steps/exit_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from causy.interfaces import ExitConditionInterface
 
 
 class ExitOnNoActions(ExitConditionInterface):
-    def check(self, graph, graph_model_instance_, actions_taken, iteration):
+    def check(self, graph, graph_model_instance_, actions_taken, iteration) -> bool:
         """
         Check if there are no actions taken in the last iteration and if so, break the loop
         If it is the first iteration, do not break the loop (we need to execute the first step)
         :param graph: the graph
         :param graph_model_instance_: the graph model instance
         :param actions_taken: the actions taken in the last iteration
         :param iteration: iteration number
```

### Comparing `causy-0.0.9/causy/independence_tests.py` & `causy-0.1.0/causy/causal_discovery/constraint/independence_tests/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,101 +1,80 @@
 import itertools
-from typing import Tuple, List, Optional
+from typing import Tuple, List, Optional, Generic
 import logging
 
 import torch
 
 from causy.generators import AllCombinationsGenerator, PairsWithNeighboursGenerator
-from causy.utils import get_t_and_critical_t, get_correlation, pearson_correlation
+from causy.math_utils import get_t_and_critical_t
 from causy.interfaces import (
-    IndependenceTestInterface,
+    PipelineStepInterface,
     BaseGraphInterface,
     NodeInterface,
-    TestResult,
-    TestResultAction,
     AS_MANY_AS_FIELDS,
-    ComparisonSettings,
+    GeneratorInterface,
+    PipelineStepInterfaceType,
 )
+from causy.models import ComparisonSettings, TestResultAction, TestResult
+from causy.variables import IntegerParameter, BoolParameter
 
 logger = logging.getLogger(__name__)
 
 
-class CalculateCorrelations(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+class CorrelationCoefficientTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1
+    parallel: BoolParameter = False
 
-    def test(self, nodes: Tuple[str], graph: BaseGraphInterface) -> TestResult:
-        """
-        Calculate the correlation between each pair of nodes and store it to the respective edge.
-        :param nodes: list of nodes
-        :return: A TestResult with the action to take
-        """
-        x = graph.nodes[nodes[0]]
-        y = graph.nodes[nodes[1]]
-        edge_value = graph.edge_value(graph.nodes[nodes[0]], graph.nodes[nodes[1]])
-        edge_value["correlation"] = pearson_correlation(
-            x.values,
-            y.values,
-        ).item()
-        return TestResult(
-            x=x,
-            y=y,
-            action=TestResultAction.UPDATE_EDGE,
-            data=edge_value,
-        )
-
-
-class CorrelationCoefficientTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
-        comparison_settings=ComparisonSettings(min=2, max=2)
-    )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
-
-    def test(self, nodes: List[str], graph: BaseGraphInterface) -> Optional[TestResult]:
+    def process(
+        self, nodes: List[str], graph: BaseGraphInterface
+    ) -> Optional[TestResult]:
         """
-        Test if x and y are independent and delete edge in graph if they are.
+        Test if u and v are independent and delete edge in graph if they are.
         :param nodes: list of nodes
         :return: A TestResult with the action to take
         """
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        # make t test for independency of x and y
+        # make t test for independency of u and v
         sample_size = len(x.values)
         nb_of_control_vars = 0
         corr = graph.edge_value(x, y)["correlation"]
         t, critical_t = get_t_and_critical_t(
             sample_size, nb_of_control_vars, corr, self.threshold
         )
         if abs(t) < critical_t:
             logger.debug(f"Nodes {x.name} and {y.name} are uncorrelated")
             return TestResult(
-                x=x,
-                y=y,
+                u=x,
+                v=y,
                 action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
                 data={},
             )
 
 
-class PartialCorrelationTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+class PartialCorrelationTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=3, max=3)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1
+    parallel: BoolParameter = False
 
-    def test(
+    def process(
         self, nodes: Tuple[str], graph: BaseGraphInterface
     ) -> Optional[List[TestResult]]:
         """
-        Test if nodes x,y are independent given node z based on a partial correlation test.
+        Test if nodes u,v are independent given node z based on a partial correlation test.
         We use this test for all combinations of 3 nodes because it is faster than the extended test (which supports combinations of n nodes). We can
         use it to remove edges between nodes which are not independent given another node and so reduce the number of combinations for the extended test.
         :param nodes: the nodes to test
         :return: A TestResult with the action to take
 
         TODO: we are testing (C and E given B) and (E and C given B), we just need one of these, remove redundant tests.
         """
@@ -113,132 +92,92 @@
             if not graph.edge_exists(x, y) or (y, x) in already_deleted_edges:
                 continue
 
             try:
                 cor_xy = graph.edge_value(x, y)["correlation"]
                 cor_xz = graph.edge_value(x, z)["correlation"]
                 cor_yz = graph.edge_value(y, z)["correlation"]
-            except KeyError:
+            except (KeyError, TypeError):
                 return
 
             numerator = cor_xy - cor_xz * cor_yz
             denominator = ((1 - cor_xz**2) * (1 - cor_yz**2)) ** 0.5
 
             # Avoid division by zero
             if denominator == 0:
                 return
 
             par_corr = numerator / denominator
 
-            # make t test for independency of x and y given z
+            # make t test for independency of u and v given z
             sample_size = len(x.values)
             nb_of_control_vars = len(nodes) - 2
             t, critical_t = get_t_and_critical_t(
                 sample_size, nb_of_control_vars, par_corr, self.threshold
             )
 
             if abs(t) < critical_t:
                 logger.debug(
                     f"Nodes {x.name} and {y.name} are uncorrelated given {z.name}"
                 )
 
                 results.append(
                     TestResult(
-                        x=x,
-                        y=y,
+                        u=x,
+                        v=y,
                         action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
                         data={"separatedBy": [z]},
                     )
                 )
                 already_deleted_edges.add((x, y))
-        return results
-
-
-class ExtendedPartialCorrelationTestLinearRegression(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
-        comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS)
-    )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1000
-    PARALLEL = True
-
-    def test(
-        self, nodes: List[str], graph: BaseGraphInterface
-    ) -> Optional[List[TestResult]]:
-        """
-        Test if nodes x,y are independent given Z (set of nodes) based on partial correlation using linear regression and a correlation test on the residuals.
-        We use this test for all combinations of more than 3 nodes because it is slower.
-        :param nodes: the nodes to test
-        :return: A TestResult with the action to take
-
-        TODO: Does not run in reasonable time yet.
-        """
-        n = len(nodes)
-        sample_size = len(graph.nodes[nodes[0]].values)
-        nodes_set = set([graph.nodes[n] for n in nodes])
-
-        nb_of_control_vars = n - 2
-        results = []
-        for i in range(n):
-            for j in range(i + 1, n):
-                x = graph.nodes[nodes[i]]
-                y = graph.nodes[nodes[j]]
-                exclude_indices = [i, j]
-                other_nodes = [
-                    graph.nodes[n].values
-                    for idx, n in enumerate(nodes)
-                    if idx not in exclude_indices
-                ]
-                par_corr = get_correlation(x, y, other_nodes)
-                logger.debug(f"par_corr {par_corr}")
-                # make t test for independence of a and y given other nodes
-                t, critical_t = get_t_and_critical_t(
-                    sample_size, nb_of_control_vars, par_corr, self.threshold
-                )
-
-                if abs(t) < critical_t:
-                    results.append(
-                        TestResult(
-                            x=x,
-                            y=y,
-                            action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
-                            data={"separatedBy": list(nodes_set - {x, y})},
-                        )
-                    )
 
         return results
 
 
-class ExtendedPartialCorrelationTestMatrix(IndependenceTestInterface):
-    GENERATOR = PairsWithNeighboursGenerator(
-        comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS)
+class ExtendedPartialCorrelationTestMatrix(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = PairsWithNeighboursGenerator(
+        comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS),
+        shuffle_combinations=False,
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1000
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1000
+    parallel: BoolParameter = False
 
-    def test(self, nodes: List[str], graph: BaseGraphInterface) -> Optional[TestResult]:
+    def process(
+        self, nodes: List[str], graph: BaseGraphInterface
+    ) -> Optional[TestResult]:
         """
-        Test if nodes x,y are independent given Z (set of nodes) based on partial correlation using the inverted covariance matrix (precision matrix).
+        Test if nodes u,v are independent given Z (set of nodes) based on partial correlation using the inverted covariance matrix (precision matrix).
         https://en.wikipedia.org/wiki/Partial_correlation#Using_matrix_inversion
         We use this test for all combinations of more than 3 nodes because it is slower.
+        If the covariance matrix is ill-conditioned, i.e., its condition number is high, the precision matrix is not reliable.
+        In that case, we throw a warning.
         :param nodes: the nodes to test
         :return: A TestResult with the action to take
         """
 
         if not graph.edge_exists(graph.nodes[nodes[0]], graph.nodes[nodes[1]]):
             return
 
-        other_neighbours = set(graph.edges[nodes[0]])
+        other_neighbours = set(
+            [
+                k
+                for k, value in graph.edges[nodes[0]].items()
+                if graph.directed_edge_exists(k, nodes[0])
+            ]
+        )
         other_neighbours.remove(graph.nodes[nodes[1]].id)
 
         if not set(nodes[2:]).issubset(set([on for on in list(other_neighbours)])):
             return
-
         inverse_cov_matrix = torch.inverse(
             torch.cov(torch.stack([graph.nodes[node].values for node in nodes]))
         )
+
         n = inverse_cov_matrix.size(0)
         diagonal = torch.diag(inverse_cov_matrix)
         diagonal_matrix = torch.zeros((n, n), dtype=torch.float64)
         for i in range(n):
             diagonal_matrix[i, i] = diagonal[i]
 
         helper = torch.mm(torch.sqrt(diagonal_matrix), inverse_cov_matrix)
@@ -259,34 +198,92 @@
 
         if abs(t) < critical_t:
             logger.debug(
                 f"Nodes {graph.nodes[nodes[0]].name} and {graph.nodes[nodes[1]].name} are uncorrelated given nodes {','.join([graph.nodes[on].name for on in other_neighbours])}"
             )
             nodes_set = set([graph.nodes[n] for n in nodes])
             return TestResult(
-                x=graph.nodes[nodes[0]],
-                y=graph.nodes[nodes[1]],
+                u=graph.nodes[nodes[0]],
+                v=graph.nodes[nodes[1]],
                 action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
                 data={
                     "separatedBy": list(
                         nodes_set - {graph.nodes[nodes[0]], graph.nodes[nodes[1]]}
                     )
                 },
             )
 
 
-class PlaceholderTest(IndependenceTestInterface):
-    NUM_OF_COMPARISON_ELEMENTS = 2
-    CHUNK_SIZE_PARALLEL_PROCESSING = 10
-    PARALLEL = False
+def partial_correlation_regression(x, y, z):
+    """
+    Compute the partial correlation coefficient between x and y controlling for other variables in z using linear regression.
+
+    Arguments:
+    x, y : torch.Tensor : Variables for which the partial correlation is computed.
+    z : torch.Tensor : Other variables used to control for in the partial correlation.
+
+    Returns:
+    partial_corr : torch.Tensor : Partial correlation coefficient between x and y.
+    """
+    # Define linear regression model
+    model_x = torch.linalg.lstsq(z.T, x).solution
+    model_y = torch.linalg.lstsq(z.T, y).solution
+
+    residual_x = x - torch.matmul(model_x, z)
+    residual_y = y - torch.matmul(model_y, z)
+
+    # Compute correlation of residuals
+    return torch.dot(residual_x, residual_y) / (
+        torch.norm(residual_x) * torch.norm(residual_y)
+    )
 
-    def test(
-        self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> List[TestResult] | TestResult:
-        """
-        Placeholder test for testing purposes
-        :param nodes:
-        :param graph:
-        :return:
-        """
-        logger.debug(f"PlaceholderTest {nodes}")
-        return TestResult(x=None, y=None, action=TestResultAction.DO_NOTHING, data={})
+
+class ExtendedPartialCorrelationTestLinearRegression(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = PairsWithNeighboursGenerator(
+        comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS),
+        shuffle_combinations=False,
+    )
+    chunk_size_parallel_processing: IntegerParameter = 1000
+    parallel: BoolParameter = False
+
+    def process(
+        self, nodes: List[str], graph: BaseGraphInterface
+    ) -> Optional[TestResult]:
+        if not graph.edge_exists(graph.nodes[nodes[0]], graph.nodes[nodes[1]]):
+            return
+
+        other_neighbours = set(graph.edges[nodes[0]])
+        other_neighbours.remove(graph.nodes[nodes[1]].id)
+
+        partial_correlation = partial_correlation_regression(
+            graph.nodes[nodes[0]].values,
+            graph.nodes[nodes[1]].values,
+            torch.stack([graph.nodes[node].values for node in nodes[2:]]),
+        )
+
+        sample_size = len(graph.nodes[nodes[0]].values)
+        nb_of_control_vars = len(nodes) - 2
+
+        t, critical_t = get_t_and_critical_t(
+            sample_size,
+            nb_of_control_vars,
+            partial_correlation.item(),
+            self.threshold,
+        )
+
+        if abs(t) < critical_t:
+            logger.debug(
+                f"Nodes {graph.nodes[nodes[0]].name} and {graph.nodes[nodes[1]].name} are uncorrelated given nodes {','.join([graph.nodes[on].name for on in other_neighbours])}"
+            )
+            nodes_set = set([graph.nodes[n] for n in nodes])
+            return TestResult(
+                u=graph.nodes[nodes[0]],
+                v=graph.nodes[nodes[1]],
+                action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
+                data={
+                    "separatedBy": list(
+                        nodes_set - {graph.nodes[nodes[0]], graph.nodes[nodes[1]]}
+                    )
+                },
+            )
```

### Comparing `causy-0.0.9/causy/orientation_tests.py` & `causy-0.1.0/causy/causal_discovery/constraint/orientation_rules/pc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,123 @@
-from typing import Tuple, List
+from typing import Tuple, List, Optional, Generic
 import itertools
 
 from causy.generators import AllCombinationsGenerator
 from causy.interfaces import (
     BaseGraphInterface,
-    TestResult,
-    TestResultAction,
-    IndependenceTestInterface,
-    ComparisonSettings,
+    PipelineStepInterface,
+    GeneratorInterface,
+    PipelineStepInterfaceType,
 )
+from causy.models import ComparisonSettings, TestResultAction, TestResult
+from causy.variables import IntegerParameter, BoolParameter
 
-# theory for all orientation rules with pictures: https://hpi.de/fileadmin/user_upload/fachgebiete/plattner/teaching/CausalInference/2019/Introduction_to_Constraint-Based_Causal_Structure_Learning.pdf
 
+# theory for all orientation rules with pictures:
+# https://hpi.de/fileadmin/user_upload/fachgebiete/plattner/teaching/CausalInference/2019/Introduction_to_Constraint-Based_Causal_Structure_Learning.pdf
 
-class ColliderTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+# TODO: refactor ColliderTest -> ColliderRule and move to folder orientation_rules (after checking for duplicates)
+
+
+class ColliderTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1
+    parallel: BoolParameter = False
 
-    def test(
+    def process(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> List[TestResult] | TestResult:
+    ) -> Optional[List[TestResult] | TestResult]:
         """
-        We call triples x, y, z of nodes v structures if x and y that are NOT adjacent but share an adjacent node z.
-        V structures looks like this in the undirected skeleton: (x - z - y).
+        We call triples u, v, z of nodes v structures if u and v that are NOT adjacent but share an adjacent node z.
+        V structures looks like this in the undirected skeleton: (u - z - v).
         We now check if z is in the separating set.
-        If z is not in the separating set, we know that x and y are uncorrelated given z.
-        So, the edges must be oriented from x to z and from y to z (x -> z <- y).
+        If z is not in the separating set, we know that u and v are uncorrelated given z.
+        So, the edges must be oriented from u to z and from v to z (u -> z <- v).
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
         # https://github.com/pgmpy/pgmpy/blob/1fe10598df5430295a8fc5cdca85cf2d9e1c4330/pgmpy/estimators/PC.py#L416
 
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        # if x and y are adjacent, do nothing
+        # if u and v are adjacent, do nothing
         if graph.undirected_edge_exists(x, y):
-            return TestResult(x=x, y=y, action=TestResultAction.DO_NOTHING, data={})
+            return TestResult(u=x, v=y, action=TestResultAction.DO_NOTHING, data={})
 
-        # if x and y are NOT adjacent, store all shared adjacent nodes
+        # if u and v are NOT adjacent, store all shared adjacent nodes
         potential_zs = set(graph.edges[x.id].keys()).intersection(
             set(graph.edges[y.id].keys())
         )
 
-        # if x and y are not independent given z, safe action: make z a collider
+        actions = graph.retrieve_edge_history(
+            x, y, TestResultAction.REMOVE_EDGE_UNDIRECTED
+        )
+
+        # if u and v are not independent given z, safe action: make z a collider
         results = []
         for z in potential_zs:
             z = graph.nodes[z]
-            actions = graph.retrieve_edge_history(
-                x, y, TestResultAction.REMOVE_EDGE_UNDIRECTED
-            )
 
             separators = []
             for action in actions:
                 if "separatedBy" in action.data:
                     separators += [a.id for a in action.data["separatedBy"]]
 
             if z.id not in separators:
                 results += [
                     TestResult(
-                        x=z,
-                        y=x,
+                        u=z,
+                        v=x,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     ),
                     TestResult(
-                        x=z,
-                        y=y,
+                        u=z,
+                        v=y,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     ),
                 ]
         return results
 
 
-class NonColliderTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+class NonColliderTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1
+    parallel: BoolParameter = False
 
-    def test(
+    def process(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> List[TestResult] | TestResult:
+    ) -> Optional[List[TestResult] | TestResult]:
         """
         Further orientation rule: all v structures that are colliders are already oriented.
         We now orient all v structures that have a single alternative to being a collider.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        # if x and y are adjacent, do nothing
+        # if u and v are adjacent, do nothing
         if graph.edge_exists(x, y):
             return
 
-        # if x and y are NOT adjacent, store all shared adjacent nodes
+        # if u and v are NOT adjacent, store all shared adjacent nodes
         potential_zs = set(graph.edges[x.id].keys()).intersection(
             set(graph.edges[y.id].keys())
         )
         # if one edge has an arrowhead at z, orient the other one pointing away from z.
         # It cannot be a collider because we have already oriented all unshielded triples that contain colliders.
         for z in potential_zs:
             z = graph.nodes[z]
@@ -118,208 +128,251 @@
                 for node in graph.nodes:
                     if graph.only_directed_edge_exists(graph.nodes[node], y):
                         breakflag = True
                         break
                 if breakflag is True:
                     continue
                 return TestResult(
-                    x=y,
-                    y=z,
+                    u=y,
+                    v=z,
                     action=TestResultAction.REMOVE_EDGE_DIRECTED,
                     data={},
                 )
 
             if graph.only_directed_edge_exists(y, z) and graph.undirected_edge_exists(
                 z, x
             ):
                 for node in graph.nodes:
                     if graph.only_directed_edge_exists(graph.nodes[node], x):
                         continue
                 return TestResult(
-                    x=x,
-                    y=z,
+                    u=x,
+                    v=z,
                     action=TestResultAction.REMOVE_EDGE_DIRECTED,
                     data={},
                 )
-        return
 
 
-class FurtherOrientTripleTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+class FurtherOrientTripleTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1
+    parallel: BoolParameter = False
 
-    def test(
+    def process(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> List[TestResult] | TestResult:
+    ) -> Optional[List[TestResult] | TestResult]:
         """
         Further orientation rule.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        potential_zs = set(graph.edges[x.id].keys()).intersection(
-            set(graph.edges[y.id].keys())
-        )
-
         results = []
-        for z in potential_zs:
+        for z in graph.nodes:
             z = graph.nodes[z]
+            # check if it is a potential z
+            if not (graph.edge_exists(y, z) and graph.edge_exists(x, z)):
+                continue
+
             if (
                 graph.undirected_edge_exists(x, y)
                 and graph.only_directed_edge_exists(x, z)
                 and graph.only_directed_edge_exists(z, y)
             ):
                 results.append(
                     TestResult(
-                        x=y,
-                        y=x,
+                        u=y,
+                        v=x,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
             if (
                 graph.undirected_edge_exists(x, y)
                 and graph.only_directed_edge_exists(y, z)
                 and graph.only_directed_edge_exists(z, x)
             ):
                 results.append(
                     TestResult(
-                        x=x,
-                        y=y,
+                        u=x,
+                        v=y,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
         return results
 
 
-class OrientQuadrupleTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+class OrientQuadrupleTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: IntegerParameter = 1
+    parallel: BoolParameter = False
 
-    def test(
+    def process(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> List[TestResult] | TestResult:
+    ) -> Optional[List[TestResult] | TestResult]:
         """
         Further orientation rule.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
-        x = graph.nodes[nodes[0]]
-        y = graph.nodes[nodes[1]]
+        y = graph.nodes[nodes[0]]
+        w = graph.nodes[nodes[1]]
 
-        potential_zs = set(graph.edges[x.id].keys()).intersection(
-            set(graph.edges[y.id].keys())
-        )
+        potential_zs = set()
+
+        # TODO: just iterate over edges
+        for z in graph.nodes:
+            z = graph.nodes[z]
+            if graph.edge_exists(y, z) and graph.edge_exists(z, w):
+                potential_zs.add(z)
 
         results = []
         for zs in itertools.combinations(potential_zs, 2):
-            z = graph.nodes[zs[0]]
-            w = graph.nodes[zs[1]]
+            x, z = zs
             if (
-                not graph.undirected_edge_exists(x, y)
-                and graph.only_directed_edge_exists(x, z)
+                not graph.edge_exists(y, w)
                 and graph.only_directed_edge_exists(y, z)
+                and graph.only_directed_edge_exists(w, z)
+                and graph.undirected_edge_exists(x, y)
                 and graph.undirected_edge_exists(x, w)
-                and graph.undirected_edge_exists(y, w)
-                and graph.undirected_edge_exists(z, w)
+                and graph.undirected_edge_exists(x, z)
             ):
                 results.append(
                     TestResult(
-                        x=z,
-                        y=w,
+                        u=z,
+                        v=x,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
             if (
-                not graph.undirected_edge_exists(x, y)
-                and graph.only_directed_edge_exists(x, w)
-                and graph.only_directed_edge_exists(y, w)
-                and graph.undirected_edge_exists(x, z)
+                not graph.edge_exists(y, w)
+                and graph.only_directed_edge_exists(y, x)
+                and graph.only_directed_edge_exists(w, x)
                 and graph.undirected_edge_exists(y, z)
-                and graph.undirected_edge_exists(z, w)
+                and graph.undirected_edge_exists(w, z)
+                and graph.undirected_edge_exists(x, z)
             ):
                 results.append(
                     TestResult(
-                        x=w,
-                        y=z,
+                        u=x,
+                        v=z,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
         return results
 
 
-class FurtherOrientQuadrupleTest(IndependenceTestInterface):
-    GENERATOR = AllCombinationsGenerator(
+class FurtherOrientQuadrupleTest(
+    PipelineStepInterface[PipelineStepInterfaceType], Generic[PipelineStepInterfaceType]
+):
+    generator: Optional[GeneratorInterface] = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    CHUNK_SIZE_PARALLEL_PROCESSING = 1
-    PARALLEL = False
+    chunk_size_parallel_processing: int = 1
+    parallel: bool = False
 
-    def test(
+    def process(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> List[TestResult] | TestResult:
+    ) -> Optional[List[TestResult] | TestResult]:
         """
         Further orientation rule.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
         x = graph.nodes[nodes[0]]
-        y = graph.nodes[nodes[1]]
+        w = graph.nodes[nodes[1]]
 
-        potential_zs = set(graph.edges[x.id].keys()).intersection(
-            set(graph.edges[y.id].keys())
-        )
+        potential_zs = set()
+
+        # TODO: just iterate over edges
+        for z in graph.nodes:
+            z = graph.nodes[z]
+            if graph.edge_exists(x, z) and graph.edge_exists(z, w):
+                potential_zs.add(z)
 
         results = []
         for zs in itertools.combinations(potential_zs, 2):
-            z = graph.nodes[zs[0]]
-            w = graph.nodes[zs[1]]
+            y, z = zs
             if (
-                not graph.undirected_edge_exists(x, y)
-                and graph.only_directed_edge_exists(x, z)
-                and graph.only_directed_edge_exists(z, y)
-                and graph.undirected_edge_exists(z, w)
+                not graph.edge_exists(y, z)
                 and graph.undirected_edge_exists(x, z)
-                and graph.undirected_edge_exists(y, z)
+                and graph.undirected_edge_exists(x, w)
+                and graph.undirected_edge_exists(x, y)
+                and graph.only_directed_edge_exists(y, w)
+                and graph.only_directed_edge_exists(w, z)
             ):
                 results.append(
                     TestResult(
-                        x=y,
-                        y=z,
+                        u=z,
+                        v=x,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
-            if (
-                not graph.undirected_edge_exists(y, x)
-                and graph.only_directed_edge_exists(y, z)
-                and graph.only_directed_edge_exists(z, x)
-                and graph.undirected_edge_exists(z, w)
+            elif (
+                not graph.edge_exists(z, y)
+                and graph.undirected_edge_exists(x, y)
+                and graph.undirected_edge_exists(x, w)
                 and graph.undirected_edge_exists(x, z)
-                and graph.undirected_edge_exists(y, z)
+                and graph.only_directed_edge_exists(z, w)
+                and graph.only_directed_edge_exists(w, y)
+            ):
+                results.append(
+                    TestResult(
+                        u=y,
+                        v=x,
+                        action=TestResultAction.REMOVE_EDGE_DIRECTED,
+                        data={},
+                    )
+                )
+            elif (
+                not graph.edge_exists(y, z)
+                and graph.undirected_edge_exists(w, z)
+                and graph.undirected_edge_exists(x, w)
+                and graph.undirected_edge_exists(w, y)
+                and graph.only_directed_edge_exists(y, x)
+                and graph.only_directed_edge_exists(x, z)
+            ):
+                results.append(
+                    TestResult(
+                        u=z,
+                        v=w,
+                        action=TestResultAction.REMOVE_EDGE_DIRECTED,
+                        data={},
+                    )
+                )
+            elif (
+                not graph.edge_exists(z, y)
+                and graph.undirected_edge_exists(w, y)
+                and graph.undirected_edge_exists(x, w)
+                and graph.undirected_edge_exists(w, z)
+                and graph.only_directed_edge_exists(z, x)
+                and graph.only_directed_edge_exists(x, y)
             ):
                 results.append(
                     TestResult(
-                        x=x,
-                        y=z,
+                        u=y,
+                        v=w,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
         return results
```

