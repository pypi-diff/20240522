# Comparing `tmp/pyatf-0.0.3.tar.gz` & `tmp/pyatf-0.0.4.tar.gz`

## Comparing `pyatf-0.0.3.tar` & `pyatf-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.3/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/feature_demonstration/result_check/result_check.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
--rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/cuda__saxpy/cuda__saxpy.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/opencl__saxpy/opencl__saxpy.py
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/opencl__sgemm/cltune_gemm.cl
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.3/examples/full_examples/opencl__sgemm/opencl__sgemm.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/range.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/result_check.py
--rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_space.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/tp.py
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/tuner.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/tuning_data.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/__init__.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/abort_condition.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/cost.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/duration.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/evaluations.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/fraction.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/abort_conditions/speedup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/__init__.py
--rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/cuda.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/generic.py
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/opencl.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/cost_functions/python.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/__init__.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/auc_bandit.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/differential_evolution.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/exhaustive.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/opentuner.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/pattern_search.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/random.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/round_robin.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/search_technique.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/search_technique_1d.py
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/simulated_annealing.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pyatf-0.0.3/src/pyatf/search_techniques/torczon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/test_range.py
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/test_search_space.py
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 pyatf-0.0.3/tests/test_tuning_data.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.3/LICENSE
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.3/PyPI/README.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.4/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/feature_demonstration/result_check/result_check.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
+-rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/cuda__saxpy/cuda__saxpy.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/opencl__saxpy/opencl__saxpy.py
+-rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/opencl__sgemm/cltune_gemm.cl
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/opencl__sgemm/opencl__sgemm.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/range.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/result_check.py
+-rw-r--r--   0        0        0    26798 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_space.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/tp.py
+-rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/tuner.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/tuning_data.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/__init__.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/abort_condition.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/cost.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/duration.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/evaluations.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/fraction.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/speedup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/__init__.py
+-rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/cuda.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/generic.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/opencl.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/python.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/__init__.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/auc_bandit.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/differential_evolution.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/exhaustive.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/opentuner.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/pattern_search.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/random.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/round_robin.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/search_technique.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/search_technique_1d.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/simulated_annealing.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/torczon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_range.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_search_space.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_tp.py
+-rw-r--r--   0        0        0    14546 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_tuning_data.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.4/LICENSE
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.4/PyPI/README.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.4/PKG-INFO
```

### Comparing `pyatf-0.0.3/README.md` & `pyatf-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py` & `pyatf-0.0.4/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/feature_demonstration/result_check/result_check.py` & `pyatf-0.0.4/examples/feature_demonstration/result_check/result_check.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py` & `pyatf-0.0.4/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp` & `pyatf-0.0.4/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py` & `pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp` & `pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/cuda__saxpy/cuda__saxpy.py` & `pyatf-0.0.4/examples/full_examples/cuda__saxpy/cuda__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/opencl__saxpy/opencl__saxpy.py` & `pyatf-0.0.4/examples/full_examples/opencl__saxpy/opencl__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/opencl__sgemm/cltune_gemm.cl` & `pyatf-0.0.4/examples/full_examples/opencl__sgemm/cltune_gemm.cl`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/examples/full_examples/opencl__sgemm/opencl__sgemm.py` & `pyatf-0.0.4/examples/full_examples/opencl__sgemm/opencl__sgemm.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/range.py` & `pyatf-0.0.4/src/pyatf/range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_space.py` & `pyatf-0.0.4/src/pyatf/search_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         self._cot_layer_to_tp_name: List[str] = []
         self._constrained_size: int = 1 if independent_tp_groups else 0
         self._unconstrained_size: int = 1 if independent_tp_groups else 0
         for tp_group in independent_tp_groups:
             for tp in tp_group:
                 self._cot_layer_to_tp_name.append(tp.name)
                 self._unconstrained_size *= len(tp.values)
-        self._partial_leaf_configs: List[List[Tuple[any, ...]]] = []
+        self._partial_leaf_configs: List[List[Tuple[any, ...]]] = []  # stores config values along the path of each leaf
         self._num_leafs: List[int] = []
         total_iterations = 0
         tp_to_range_size: List[List[int]] = []
         finished_iterations = 0
         if enable_1d_access:
             if not silent:
                 # enable 1D access, with progress prints
@@ -227,15 +227,15 @@
                         tp_iter(0, tp_group[0], tp_to_parameter_names[tp_group[0]], tp_group[1:], tree.root)
                     tree.root.num_leafs = num_leafs
                     last_progress_print_ns = None  # force print
                     progress_printer(finished_iterations / total_iterations)
                     self._cot.append(tree)
                     self._constrained_size *= num_leafs
                     self._num_leafs.append(num_leafs)
-                print('\n')
+                print('')
             else:
                 # enable 1D access, no progress prints
                 for tp_group_idx, tp_group in enumerate(independent_tp_groups):
                     self._partial_leaf_configs.append([])
 
                     if len(tp_group) == 1 and tp_group[0].constraint is None:
                         # for TP groups with a single TP without constraints, conserve storage by storing
@@ -356,15 +356,15 @@
                         tree = ChainedTree()
                         tp_iter(0, tp_group[0], tp_to_parameter_names[tp_group[0]], tp_group[1:], tree.root)
                     tree.root.num_leafs = num_leafs
                     last_progress_print_ns = None  # force print
                     progress_printer(finished_iterations / total_iterations)
                     self._cot.append(tree)
                     self._constrained_size *= num_leafs
-                print('\n')
+                print('')
             else:
                 # no 1D access, no progress prints
                 for tp_group_idx, tp_group in enumerate(independent_tp_groups):
                     if len(tp_group) == 1 and tp_group[0].constraint is None:
                         # for TP groups with a single TP without constraints, conserve storage by storing
                         # the TP range in a single child node instead of generating one node per range value.
                         num_leafs = len(tp_group[0].values)
@@ -466,14 +466,17 @@
                     config[self._cot_layer_to_tp_name[layer]] = node.data[leaf_index]
                     layer += 1
                 else:
                     # TP values are represented as child nodes
                     for leaf_value in partial_leaf_configs[leaf_index]:
                         config[self._cot_layer_to_tp_name[layer]] = leaf_value
                         layer += 1
+                    # go to next tree
+                    if layer < self._num_tps:
+                        node = next(trees).root
 
             return config
         else:
             coordinates = coordinates_or_index
             if self._constrained_size == 0:
                 raise ValueError('search space does not contain any configurations')
             if len(coordinates) != self._num_tps:
```

### Comparing `pyatf-0.0.3/src/pyatf/tuner.py` & `pyatf-0.0.4/src/pyatf/tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
             # generate search space
             search_space_generation_start = time.perf_counter_ns()
             self._search_space = SearchSpace(*tps,
                                              enable_1d_access=isinstance(self._search_technique, SearchTechnique1D),
                                              silent=silent)
             search_space_generation_end = time.perf_counter_ns()
             self._search_space_generation_ns = search_space_generation_end - search_space_generation_start
+            if not silent:
+                print(f'search space size: {self._search_space.constrained_size}')
 
             # prepare abort condition
             self._abort_condition: Optional[AbortCondition] = abort_condition
             if self._abort_condition is None:
                 self._abort_condition = Evaluations(len(self._search_space))
 
             # tuning data
```

### Comparing `pyatf-0.0.3/src/pyatf/tuning_data.py` & `pyatf-0.0.4/src/pyatf/tuning_data.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/abort_conditions/abort_condition.py` & `pyatf-0.0.4/src/pyatf/abort_conditions/abort_condition.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/abort_conditions/duration.py` & `pyatf-0.0.4/src/pyatf/abort_conditions/duration.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/abort_conditions/evaluations.py` & `pyatf-0.0.4/src/pyatf/abort_conditions/evaluations.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/abort_conditions/fraction.py` & `pyatf-0.0.4/src/pyatf/abort_conditions/fraction.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/abort_conditions/speedup.py` & `pyatf-0.0.4/src/pyatf/abort_conditions/speedup.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/cost_functions/cuda.py` & `pyatf-0.0.4/src/pyatf/cost_functions/cuda.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/cost_functions/generic.py` & `pyatf-0.0.4/src/pyatf/cost_functions/generic.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/cost_functions/opencl.py` & `pyatf-0.0.4/src/pyatf/cost_functions/opencl.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/cost_functions/python.py` & `pyatf-0.0.4/src/pyatf/cost_functions/python.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/auc_bandit.py` & `pyatf-0.0.4/src/pyatf/search_techniques/auc_bandit.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/differential_evolution.py` & `pyatf-0.0.4/src/pyatf/search_techniques/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/exhaustive.py` & `pyatf-0.0.4/src/pyatf/search_techniques/exhaustive.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/opentuner.py` & `pyatf-0.0.4/src/pyatf/search_techniques/opentuner.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/pattern_search.py` & `pyatf-0.0.4/src/pyatf/search_techniques/pattern_search.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/random.py` & `pyatf-0.0.4/src/pyatf/search_techniques/random.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/round_robin.py` & `pyatf-0.0.4/src/pyatf/search_techniques/round_robin.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/search_technique.py` & `pyatf-0.0.4/src/pyatf/search_techniques/search_technique.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/search_technique_1d.py` & `pyatf-0.0.4/src/pyatf/search_techniques/search_technique_1d.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/simulated_annealing.py` & `pyatf-0.0.4/src/pyatf/search_techniques/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/src/pyatf/search_techniques/torczon.py` & `pyatf-0.0.4/src/pyatf/search_techniques/torczon.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/tests/test_range.py` & `pyatf-0.0.4/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/tests/test_search_space.py` & `pyatf-0.0.4/tests/test_search_space.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,23 +169,26 @@
                          search_space.get_configuration((0.45454, 0.90000, 1.00000, 0.05001, 0.00001, 0.64537)))
         self.assertEqual({'tp1': 4, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 9, 'tp6': 10},
                          search_space.get_configuration((0.45455, 0.65410, 0.50000, 0.95348, 0.47368, 0.00001)))
         self.assertEqual({'tp1': 4, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 10, 'tp6': 7},
                          search_space.get_configuration((0.45455, 0.65410, 0.50001, 1.00000, 0.47369, 0.68753)))
 
     def test_1d_access(self):
+        tp7 = TP('tp7', Interval(1, 2))
         search_space = SearchSpace(
             TP('tp1', Interval(1, 10)),
             TP('tp2', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0),
             TP('tp3', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0),
 
             TP('tp4', Set(min, max)),
             TP('tp5', Interval(1, 10)),
             TP('tp6', Interval(1, 10), lambda tp6, tp4, tp5: tp4(tp5, tp6) == 10),
 
+            tp7,
+
             enable_1d_access=True
         )
         self._check_cot(search_space.cot, [
             ({
                  2: ({6: ({2: (None, 1)}, 1), 8: ({2: (None, 1)}, 1), 10: ({2: (None, 1)}, 1)}, 3),
                  3: ({6: ({3: (None, 1)}, 1), 9: ({3: (None, 1)}, 1)}, 2),
                  4: ({8: ({2: (None, 1)}, 1)}, 1),
@@ -203,20 +206,31 @@
                         5: ({10: (None, 1)}, 1),
                         6: ({10: (None, 1)}, 1),
                         7: ({10: (None, 1)}, 1),
                         8: ({10: (None, 1)}, 1),
                         9: ({10: (None, 1)}, 1),
                         10: ({1: (None, 1), 2: (None, 1), 3: (None, 1), 4: (None, 1), 5: (None, 1),
                               6: (None, 1), 7: (None, 1), 8: (None, 1), 9: (None, 1), 10: (None, 1)}, 10)}, 19)
-             }, 20)
+             }, 20),
+            ({tp7.values: (None, 1)}, 2)
         ])
-        self.assertEqual(220, len(search_space))
-        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': min, 'tp5': 10, 'tp6': 10},
+        self.assertEqual(440, len(search_space))
+        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': min, 'tp5': 10, 'tp6': 10, 'tp7': 1},
                          search_space.get_configuration(0))
-        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': max, 'tp5': 1, 'tp6': 10},
+        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': min, 'tp5': 10, 'tp6': 10, 'tp7': 2},
                          search_space.get_configuration(1))
-        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': max, 'tp5': 2, 'tp6': 10},
+        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': max, 'tp5': 1, 'tp6': 10, 'tp7': 1},
                          search_space.get_configuration(2))
-        self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2, 'tp4': min, 'tp5': 10, 'tp6': 10},
-                         search_space.get_configuration(20))
-        self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 1, 'tp6': 10},
-                         search_space.get_configuration(21))
+        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': max, 'tp5': 1, 'tp6': 10, 'tp7': 2},
+                         search_space.get_configuration(3))
+        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': max, 'tp5': 2, 'tp6': 10, 'tp7': 1},
+                         search_space.get_configuration(4))
+        self.assertEqual({'tp1': 2, 'tp2': 6, 'tp3': 2, 'tp4': max, 'tp5': 2, 'tp6': 10, 'tp7': 2},
+                         search_space.get_configuration(5))
+        self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2, 'tp4': min, 'tp5': 10, 'tp6': 10, 'tp7': 1},
+                         search_space.get_configuration(40))
+        self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2, 'tp4': min, 'tp5': 10, 'tp6': 10, 'tp7': 2},
+                         search_space.get_configuration(41))
+        self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 1, 'tp6': 10, 'tp7': 1},
+                         search_space.get_configuration(42))
+        self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 1, 'tp6': 10, 'tp7': 2},
+                         search_space.get_configuration(43))
```

### Comparing `pyatf-0.0.3/tests/test_tuning_data.py` & `pyatf-0.0.4/tests/test_tuning_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,17 @@
             Random().to_json(),
             Evaluations(6).to_json()
         )
 
         self.assertEqual([
             {'name': 'tp1', 'range': {'kind': 'Interval', 'start': 1, 'end': 10, 'step': 1}},
             {'name': 'tp2', 'range': {'kind': 'Interval', 'start': 5, 'end': 10, 'step': 1},
-             'constraint': '        tp2 = TP(\'tp2\', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0)\n'},
+             'constraint': 'tp2 = TP(\'tp2\', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0)\n'},
             {'name': 'tp3', 'range': {'kind': 'Interval', 'start': 2, 'end': 3, 'step': 1},
-             'constraint': '        tp3 = TP(\'tp3\', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0)\n'}
+             'constraint': 'tp3 = TP(\'tp3\', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0)\n'}
         ], tuning_data.tuning_parameters)
         self.assertEqual(11, tuning_data.constrained_search_space_size)
         self.assertEqual(120, tuning_data.unconstrained_search_space_size)
         self.assertEqual(search_space_generation_end - search_space_generation_start,
                          tuning_data.search_space_generation_ns)
         self.assertEqual({'kind': 'Random'}, tuning_data.search_technique)
         self.assertEqual({'kind': 'Evaluations', 'evaluations': 6}, tuning_data.abort_condition)
```

### Comparing `pyatf-0.0.3/LICENSE` & `pyatf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/pyproject.toml` & `pyatf-0.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyatf"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Richard Schulze", email="r.schulze@uni-muenster.de" },
     { name="Ari Rasch", email="a.rasch@uni-muenster.de" }
 ]
 description = "Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained"
 readme = "./PyPI/README.md"
 requires-python = ">=3.9"
```

### Comparing `pyatf-0.0.3/PyPI/README.md` & `pyatf-0.0.4/PyPI/README.md`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.3/PKG-INFO` & `pyatf-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained
 Project-URL: Homepage, https://atf-project.org/
 Project-URL: Issues, https://github.com/atf-tuner/pyATF/issues
 Author-email: Richard Schulze <r.schulze@uni-muenster.de>, Ari Rasch <a.rasch@uni-muenster.de>
 License-File: LICENSE
 Keywords: auto-tuning,constraints,optimization,performance,tuning
 Classifier: License :: OSI Approved :: MIT License
```

