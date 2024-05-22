# Comparing `tmp/attpc_spyral-0.6.1.tar.gz` & `tmp/attpc_spyral-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attpc_spyral-0.6.1.tar", last modified: Mon May 13 18:51:10 2024, max compression
+gzip compressed data, was "attpc_spyral-0.7.0.tar", last modified: Wed May 22 17:59:50 2024, max compression
```

## Comparing `attpc_spyral-0.6.1.tar` & `attpc_spyral-0.7.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2024-05-13 18:50:53.980942 attpc_spyral-0.6.1/LICENSE
--rw-r--r--   0        0        0     5985 2024-05-13 18:50:53.980942 attpc_spyral-0.6.1/README.md
--rw-r--r--   0        0        0      820 2024-05-13 18:51:10.405008 attpc_spyral-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      759 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/__init__.py
--rw-r--r--   0        0        0     6686 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/cluster.py
--rw-r--r--   0        0        0     9635 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/clusterize.py
--rw-r--r--   0        0        0     8335 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/config.py
--rw-r--r--   0        0        0     2241 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/constants.py
--rw-r--r--   0        0        0    11097 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/estimator.py
--rw-r--r--   0        0        0     2202 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/hardware_id.py
--rw-r--r--   0        0        0     1353 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/legacy_beam_pads.py
--rw-r--r--   0        0        0     8708 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/pad_map.py
--rw-r--r--   0        0        0     7456 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/phase.py
--rw-r--r--   0        0        0    10012 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/pipeline.py
--rw-r--r--   0        0        0     7040 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/point_cloud.py
--rw-r--r--   0        0        0     4316 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/run_stacks.py
--rw-r--r--   0        0        0     4575 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/spy_log.py
--rw-r--r--   0        0        0      537 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/status_message.py
--rw-r--r--   0        0        0    20110 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/core/track_generator.py
--rw-r--r--   0        0        0      128 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/correction/__init__.py
--rw-r--r--   0        0        0     2579 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/correction/electron_corrector.py
--rw-r--r--   0        0        0     4367 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/correction/generate.py
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/data/__init__.py
--rw-r--r--   0        0        0   151675 2024-05-13 18:50:53.984942 attpc_spyral-0.6.1/src/spyral/data/pad_electronics.csv
--rw-r--r--   0        0        0   140922 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/data/pad_electronics_legacy.csv
--rw-r--r--   0        0        0    28681 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/data/pad_gain_map.csv
--rw-r--r--   0        0        0    47110 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/data/pad_scale.csv
--rw-r--r--   0        0        0    94283 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/data/pad_time_correction.csv
--rw-r--r--   0        0        0   213104 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/data/padxy.csv
--rw-r--r--   0        0        0   213104 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/data/padxy_legacy.csv
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/geometry/__init__.py
--rw-r--r--   0        0        0     2477 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/geometry/circle.py
--rw-r--r--   0        0        0       89 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/interpolate/__init__.py
--rw-r--r--   0        0        0     9011 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/interpolate/bilinear.py
--rw-r--r--   0        0        0     3474 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/interpolate/linear.py
--rw-r--r--   0        0        0    13187 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/interpolate/track_interpolator.py
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/__init__.py
--rw-r--r--   0        0        0     5675 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/cluster_phase.py
--rw-r--r--   0        0        0     6301 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/estimation_phase.py
--rw-r--r--   0        0        0    11540 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/interp_solver_phase.py
--rw-r--r--   0        0        0     7803 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/pointcloud_legacy_phase.py
--rw-r--r--   0        0        0    12078 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/pointcloud_phase.py
--rw-r--r--   0        0        0     1226 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/phases/schema.py
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/solvers/__init__.py
--rw-r--r--   0        0        0     1591 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/solvers/guess.py
--rw-r--r--   0        0        0    10600 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/solvers/solver_interp.py
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/__init__.py
--rw-r--r--   0        0        0    11463 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/frib_event.py
--rw-r--r--   0        0        0     4827 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/frib_scalers.py
--rw-r--r--   0        0        0     3993 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/frib_trace.py
--rw-r--r--   0        0        0     4542 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/get_event.py
--rw-r--r--   0        0        0     5752 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/get_legacy_event.py
--rw-r--r--   0        0        0     6140 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/get_trace.py
--rw-r--r--   0        0        0      899 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/src/spyral/trace/peak.py
--rw-r--r--   0        0        0        0 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0       67 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/run_0000.h5
--rw-r--r--   0        0        0      121 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/run_0001.h5
--rw-r--r--   0        0        0      396 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/test_circle.py
--rw-r--r--   0        0        0     4007 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/test_default_pipeline.py
--rw-r--r--   0        0        0     1573 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/test_pad.py
--rw-r--r--   0        0        0     1172 2024-05-13 18:50:53.988942 attpc_spyral-0.6.1/tests/test_runs.py
--rw-r--r--   0        0        0     6527 1970-01-01 00:00:00.000000 attpc_spyral-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 17:59:36.450208 attpc_spyral-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6290 2024-05-22 17:59:36.450208 attpc_spyral-0.7.0/README.md
+-rw-r--r--   0        0        0      820 2024-05-22 17:59:50.238369 attpc_spyral-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      759 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/__init__.py
+-rw-r--r--   0        0        0     7509 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/cluster.py
+-rw-r--r--   0        0        0    11603 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/clusterize.py
+-rw-r--r--   0        0        0     8107 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/config.py
+-rw-r--r--   0        0        0     2241 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/constants.py
+-rw-r--r--   0        0        0    10702 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/estimator.py
+-rw-r--r--   0        0        0     2202 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/hardware_id.py
+-rw-r--r--   0        0        0     1353 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/legacy_beam_pads.py
+-rw-r--r--   0        0        0     8708 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/pad_map.py
+-rw-r--r--   0        0        0     7456 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/phase.py
+-rw-r--r--   0        0        0    10125 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/pipeline.py
+-rw-r--r--   0        0        0     7040 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/point_cloud.py
+-rw-r--r--   0        0        0     4316 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/run_stacks.py
+-rw-r--r--   0        0        0     4575 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/spy_log.py
+-rw-r--r--   0        0        0      537 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/status_message.py
+-rw-r--r--   0        0        0    20110 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/track_generator.py
+-rw-r--r--   0        0        0      128 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/correction/__init__.py
+-rw-r--r--   0        0        0     2579 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/correction/electron_corrector.py
+-rw-r--r--   0        0        0     4367 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/correction/generate.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/data/__init__.py
+-rw-r--r--   0        0        0   151675 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_electronics.csv
+-rw-r--r--   0        0        0   140922 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_electronics_legacy.csv
+-rw-r--r--   0        0        0    28681 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_gain_map.csv
+-rw-r--r--   0        0        0    47110 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_scale.csv
+-rw-r--r--   0        0        0    94283 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_time_correction.csv
+-rw-r--r--   0        0        0   213104 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/padxy.csv
+-rw-r--r--   0        0        0   213104 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/padxy_legacy.csv
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/geometry/__init__.py
+-rw-r--r--   0        0        0     2477 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/geometry/circle.py
+-rw-r--r--   0        0        0       89 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/__init__.py
+-rw-r--r--   0        0        0     9011 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/bilinear.py
+-rw-r--r--   0        0        0     3474 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/linear.py
+-rw-r--r--   0        0        0    13187 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/track_interpolator.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/__init__.py
+-rw-r--r--   0        0        0     5819 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/cluster_phase.py
+-rw-r--r--   0        0        0     6305 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/estimation_phase.py
+-rw-r--r--   0        0        0    11667 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/interp_solver_phase.py
+-rw-r--r--   0        0        0     7750 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/pointcloud_legacy_phase.py
+-rw-r--r--   0        0        0    12121 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/pointcloud_phase.py
+-rw-r--r--   0        0        0     1226 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/schema.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/solvers/__init__.py
+-rw-r--r--   0        0        0     1591 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/solvers/guess.py
+-rw-r--r--   0        0        0    10600 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/solvers/solver_interp.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/trace/__init__.py
+-rw-r--r--   0        0        0    11463 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/frib_event.py
+-rw-r--r--   0        0        0     4827 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/frib_scalers.py
+-rw-r--r--   0        0        0     3993 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/frib_trace.py
+-rw-r--r--   0        0        0     4542 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/get_event.py
+-rw-r--r--   0        0        0     5737 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/get_legacy_event.py
+-rw-r--r--   0        0        0     6140 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/get_trace.py
+-rw-r--r--   0        0        0      899 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/peak.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/run_0000.h5
+-rw-r--r--   0        0        0      121 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/run_0001.h5
+-rw-r--r--   0        0        0      396 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_circle.py
+-rw-r--r--   0        0        0     3970 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_default_pipeline.py
+-rw-r--r--   0        0        0     1573 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_pad.py
+-rw-r--r--   0        0        0     1172 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_runs.py
+-rw-r--r--   0        0        0     6832 1970-01-01 00:00:00.000000 attpc_spyral-0.7.0/PKG-INFO
```

### Comparing `attpc_spyral-0.6.1/LICENSE` & `attpc_spyral-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/README.md` & `attpc_spyral-0.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Spyral
 
+![CI](https://github.com/ATTPC/Spyral/actions/workflows/ci.yml/badge.svg)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/attpc_spyral.svg)](https://pypi.python.org/pypi/attpc_spyral/)
+[![PyPI license](https://img.shields.io/pypi/l/attpc_spyral.svg)](https://pypi.python.org/pypi/attpc_spyral/)
+
 Spyral is an analysis library for data from the Active Target Time Projection Chamber (AT-TPC). Spyral provides a flexible analysis pipeline, transforming the raw trace data into physical observables over several tunable steps. The analysis pipeline is also extensible, supporting a diverse array of datasets. Sypral can process multiple data files in parallel, allowing for scalable performance over larger experiment datasets.
 
 ## Installation
 
 Install using pip:
 
 ```bash
@@ -95,36 +99,36 @@
 )
 
 cluster_params = ClusterParameters(
     min_cloud_size=50,
     min_points=3,
     min_size_scale_factor=0.05,
     min_size_lower_cutoff=10,
-    cluster_selection_epsilon=0.3,
+    cluster_selection_epsilon=10.0,
     circle_overlap_ratio=0.5,
     fractional_charge_threshold=0.8,
     outlier_scale_factor=0.05,
 )
 
 estimate_params = EstimateParameters(
     min_total_trajectory_points=30, smoothing_factor=100.0
 )
 
 solver_params = SolverParameters(
     gas_data_path=Path("/path/to/some/gas/data.json"),
     particle_id_filename=Path("/path/to/some/particle/id.json"),
     ic_min_val=900.0,
     ic_max_val=1350.0,
-    n_time_steps=10000,
-    interp_ke_min=0.05,
+    n_time_steps=1000,
+    interp_ke_min=0.1,
     interp_ke_max=70.0,
-    interp_ke_bins=400,
+    interp_ke_bins=350,
     interp_polar_min=2.0,
     interp_polar_max=88.0,
-    interp_polar_bins=170,
+    interp_polar_bins=166,
 )
 
 pipe = Pipeline(
     [
         PointcloudPhase(
             get_params,
             frib_params,
```

### Comparing `attpc_spyral-0.6.1/pyproject.toml` & `attpc_spyral-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "attpc_spyral"
-version = "0.6.1"
+version = "0.7.0"
 description = "AT-TPC analysis pipeline"
 authors = [
     { name = "gwm17", email = "gordonmccann215@gmail.com" },
 ]
 dependencies = [
-    "spyral-utils>=0.3.0",
+    "spyral-utils>=1.0.0",
     "black>=24.4.0",
     "contourpy>=1.2.1",
     "h5py>=3.11.0",
     "lmfit>=1.3.0",
     "numba>=0.59.1",
     "scikit-learn>=1.4.2",
     "tqdm>=4.66.2",
```

### Comparing `attpc_spyral-0.6.1/src/spyral/__init__.py` & `attpc_spyral-0.7.0/src/spyral/__init__.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/clusterize.py` & `attpc_spyral-0.7.0/src/spyral/core/clusterize.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,109 @@
 from .point_cloud import PointCloud
 from .cluster import LabeledCloud, Cluster, convert_labeled_to_cluster
 from .config import ClusterParameters
 from ..geometry.circle import least_squares_circle
 
 import sklearn.cluster as skcluster
-from sklearn.preprocessing import RobustScaler
 import numpy as np
 
+NOISE_LABEL: int = -1
+
 
 def join_clusters(
-    clusters: list[LabeledCloud], params: ClusterParameters
-) -> list[LabeledCloud]:
+    clusters: list[LabeledCloud], params: ClusterParameters, labels: np.ndarray
+) -> tuple[list[LabeledCloud], np.ndarray]:
     """Join clusters until either only one cluster is left or no clusters meet the criteria to be joined together.
 
     Parameters
     ----------
     clusters: list[LabeledCloud]
         the set of clusters to examine
     params: ClusterParameters
         contains parameters controlling the joining algorithm
+    labels: numpy.ndarray
+        The cluster label for each point in the original point cloud
 
     Returns
     -------
-    list[LabeledCloud]
-        the set of joined clusters
+    tuple[list[LabeledCloud], numpy.ndarray]
+        A two element tuple, the first the list of joined clusters,
+        the second being an updated list of labels for each point in
+        the point cloud
     """
     jclusters = clusters.copy()
     before = len(jclusters)
     after = 0
     while before != after and len(jclusters) > 1:
         before = len(jclusters)
-        jclusters = join_clusters_step(jclusters, params)
+        jclusters, labels = join_clusters_step(jclusters, params, labels)
         after = len(jclusters)
-    return jclusters
+    return (jclusters, labels)
 
 
 def join_clusters_step(
-    clusters: list[LabeledCloud], params: ClusterParameters
-) -> list[LabeledCloud]:
+    clusters: list[LabeledCloud], params: ClusterParameters, labels: np.ndarray
+) -> tuple[list[LabeledCloud], np.ndarray]:
     """A single step of joining clusters
 
     Combine clusters based on the center around which they orbit. This is necessary because often times tracks are
     fractured or contain regions of varying density which causes clustering algorithms to separate them.
 
     Parameters
     ----------
     clusters: list[LabeledCloud]
         the set of clusters to examine
     params: ClusterParameters
         contains the parameters controlling the joining algorithm (max_center_distance)
+    labels: numpy.ndarray
+        The cluster label for each point in the original point cloud
 
     Returns
     -------
-    list[LabeledCloud]
-        the set of joined clusters
+    tuple[list[LabeledCloud], numpy.ndarray]
+        A two element tuple, the first the list of joined clusters,
+        the second being an updated list of labels for each point in
+        the point cloud
     """
     # Can't join 1 or 0 clusters
     if len(clusters) < 2:
-        return clusters
+        return (clusters, labels)
 
     event_number = clusters[0].point_cloud.event_number
 
     # Fit the clusters with circles
     centers = np.zeros((len(clusters), 3))
     for idx, cluster in enumerate(clusters):
         centers[idx, 0], centers[idx, 1], centers[idx, 2], _ = least_squares_circle(
             cluster.point_cloud.cloud[:, 0], cluster.point_cloud.cloud[:, 1]
         )
 
-    # Make a dictionary of center groups
+    # Make a dictionary of center groups, label groups
     # First everyone is in their own group
-    groups: dict[int, list[int]] = {}
+    groups_index: dict[int, list[int]] = {}  # Regroup the actual cluster data
+    groups_label: dict[int, list[int]] = {}  # Regroup the label array
     for idx, cluster in enumerate(clusters):
-        groups[cluster.label] = [idx]
+        groups_index[cluster.label] = [idx]  # Use indicies for data
+        groups_label[cluster.label] = [cluster.label]  # Use labels for ... labels
 
     # Now regroup, searching for clusters whose circles mostly overlap
     for idx, center in enumerate(centers):
         cluster = clusters[idx]
         # Reject noise
-        if cluster.label == -1 or np.isnan(center[0]) or center[2] < 10.0:
+        if cluster.label == NOISE_LABEL or np.isnan(center[0]) or center[2] < 10.0:
             continue
         radius = center[2]
         area = np.pi * radius**2.0
 
         for cidx, comp_cluster in enumerate(clusters):
             comp_center = centers[cidx]
             comp_radius = comp_center[2]
             comp_area = np.pi * comp_radius**2.0
             if (
-                comp_cluster.label == -1
+                comp_cluster.label == NOISE_LABEL
                 or np.isnan(comp_center[0])
                 or center[2] < 10.0
                 or cidx == idx
             ):
                 continue
 
             # Calculate area of overlap between the two circles
@@ -128,75 +139,95 @@
                 term2 = min(1.0, max(-1.0, term2))
                 area_overlap = (
                     radius**2.0 * np.arccos(term1)
                     + comp_radius**2.0 * np.arccos(term2)
                     - 0.5 * np.sqrt(term3)
                 )
 
+            # Apply the condition
             smaller_area = min(area, comp_area)
-            comp_mean_charge = np.mean(comp_cluster.point_cloud.cloud[:, 4], axis=0)
-            mean_charge = np.mean(cluster.point_cloud.cloud[:, 4], axis=0)
-            charge_diff = np.abs(mean_charge - comp_mean_charge)
-            threshold = params.fractional_charge_threshold * np.max(
-                [comp_mean_charge, mean_charge]
-            )
-            if (
-                (area_overlap > params.circle_overlap_ratio * smaller_area)
-                and (cidx not in groups[cluster.label])
-                and (charge_diff < threshold)
+            if (area_overlap > params.circle_overlap_ratio * smaller_area) and (
+                cidx not in groups_index[cluster.label]
             ):
-                comp_group = groups.pop(comp_cluster.label)
-                for subs in comp_group:
+                comp_indicies = groups_index.pop(comp_cluster.label)
+                comp_labels = groups_label.pop(comp_cluster.label)
+                for subs in comp_indicies:
                     clusters[subs].label = cluster.label
-                groups[cluster.label].extend(comp_group)
+                groups_index[cluster.label].extend(comp_indicies)
+                groups_label[cluster.label].extend(comp_labels)
 
     # Now reform the clouds such that there is one cloud per group
     new_clusters: list[LabeledCloud] = []
-    for g in groups.keys():
-        if g == -1:
+    for g in groups_index.keys():
+        if g == NOISE_LABEL:
             continue
 
         new_cluster = LabeledCloud(g, PointCloud())
         new_cluster.point_cloud.event_number = event_number
         new_cluster.point_cloud.cloud = np.zeros((0, 8))
-        for idx in groups[g]:
+        for idx in groups_index[g]:
             new_cluster.point_cloud.cloud = np.concatenate(
                 (new_cluster.point_cloud.cloud, clusters[idx].point_cloud.cloud), axis=0
             )
+            # Merge the indicies
+            new_cluster.parent_indicies = np.concatenate(
+                (new_cluster.parent_indicies, clusters[idx].parent_indicies)
+            )
         new_clusters.append(new_cluster)
 
-    return new_clusters
+    # Now replace the labels in the label array with the joined
+    # values
+    new_labels = labels
+    for g in groups_label.keys():
+        if g == NOISE_LABEL:
+            continue
+        for label in groups_label[g]:
+            new_labels[labels == label] = g
+
+    return (new_clusters, new_labels)
 
 
 def cleanup_clusters(
-    clusters: list[LabeledCloud], params: ClusterParameters
-) -> list[Cluster]:
-    """Converts the LabeledClouds to Clusters and bins the data in z
+    clusters: list[LabeledCloud], params: ClusterParameters, labels: np.ndarray
+) -> tuple[list[Cluster], np.ndarray]:
+    """Converts the LabeledClouds to Clusters
 
     Parameters
     ----------
     clusters: list[LabeledCloud]
         clusters to clean
     params: ClusterParameters
         Configuration parameters controlling the clustering algorithms
+    labels: numpy.ndarray
+        The cluster label for each point in the original point cloud
 
     Returns
     -------
-    list[Cluster]
-        The cleaned clusters
+    tuple[list[Cluster], numpy.ndarray]
+        A two element tuple, the first the list of cleaned clusters,
+        the second being an updated list of labels for each point in
+        the point cloud
     """
-    # Cluster must have more than two points to have outlier test applied
-    return [
-        convert_labeled_to_cluster(cluster, params)
-        for cluster in clusters
-        if cluster.label != -1 and len(cluster.point_cloud.cloud) > 2
-    ]
+    cleaned = []
+    for cluster in clusters:
+        # Cluster must have more than two points to have outlier test applied
+        if cluster.label == NOISE_LABEL or len(cluster.point_cloud.cloud) < 2:
+            continue
+        cleaned_cluster, outliers = convert_labeled_to_cluster(cluster, params)
+        cleaned.append(cleaned_cluster)
+        if len(outliers) == 0:
+            continue
+        orig_indicies = (cluster.parent_indicies[outliers]).astype(dtype=np.int32)
+        labels[orig_indicies] = NOISE_LABEL
+    return (cleaned, labels)
 
 
-def form_clusters(pc: PointCloud, params: ClusterParameters) -> list[LabeledCloud]:
+def form_clusters(
+    pc: PointCloud, params: ClusterParameters
+) -> tuple[list[LabeledCloud], np.ndarray]:
     """Apply the HDBSCAN clustering algorithm to a PointCloud
 
     Analyze a point cloud, and group the points into clusters which in principle should correspond to particle trajectories. This analysis contains several steps,
     and revolves around the HDBSCAN clustering algorithm implemented in scikit-learn (see [their description](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.HDBSCAN.html) for details)
     First the point cloud is smoothed by averaging over nearest neighbors (defined by the smoothing_neighbor_distance parameter) to remove small deviations.
     The data is then scaled where each coordinate (x,y,z,int) is centered to its mean and then scaled to its std deviation using the scikit-learn StandardScaler. This data is then
     clustered by HDBSCAN and the clusters are returned.
@@ -206,22 +237,24 @@
     pc: PointCloud
         The point cloud to be clustered
     params: ClusterParameters
         Configuration parameters controlling the clustering algorithms
 
     Returns
     --------
-    list[LabeledCloud]
-        List of clusters found by the algorithm with labels
+    tuple[list[LabeledCloud], numpy.ndarray]
+        Two element tuple, the first being a ist of clusters found by the algorithm with labels
+        the second being an array of length of the point cloud with each element conatining
+        that point's label.
     """
 
     # Smooth out the point cloud by averaging over neighboring points within a distance, droping any duplicate points
     pc.remove_illegal_points()
     if len(pc.cloud) < params.min_cloud_size:
-        return []
+        return ([], np.empty(0))
 
     n_points = len(pc.cloud)
     min_size = int(params.min_size_scale_factor * n_points)
     if min_size < params.min_size_lower_cutoff:
         min_size = params.min_size_lower_cutoff
 
     # Use spatial dimensions and integrated charge
@@ -245,8 +278,9 @@
     clusters: list[LabeledCloud] = []
     for idx, label in enumerate(labels):
         clusters.append(LabeledCloud(label, PointCloud(), np.empty(0)))
         mask = fitted_clusters.labels_ == label
         clusters[idx].point_cloud.cloud = pc.cloud[mask]
         clusters[idx].point_cloud.event_number = pc.event_number
         clusters[idx].clustered_data = cluster_data[mask]
-    return clusters
+        clusters[idx].parent_indicies = np.flatnonzero(mask)
+    return (clusters, fitted_clusters.labels_)
```

### Comparing `attpc_spyral-0.6.1/src/spyral/core/config.py` & `attpc_spyral-0.7.0/src/spyral/core/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,29 +177,25 @@
         min_cluster_size parameter in scikit-learn's HDBSCAN algorithm for events where n_points * min_size_scale_factor
         are less than this value.
     cluster_selection_epsilon: float
         cluster_selection_epsilon parameter in scikit-learn's HDBSCAN algorithm. Clusters less than this distance apart
         are merged in the hierarchy
     circle_overlap_ratio: float
         minimum overlap ratio between two circles in the cluster joining algorithm
-    fractional_charge_threshold: float
-        The maximum allowed difference between two clusters mean charge (relative to the larger mean charge of the two)
-        for them to be joined
     outlier_scale_factor: float
         Factor which is multiplied by the number of points in a trajectory to set the number of neighbors parameter
         for scikit-learns LocalOutlierFactor test
     """
 
     min_cloud_size: int
     min_points: int
     min_size_scale_factor: float
     min_size_lower_cutoff: int
     cluster_selection_epsilon: float
     circle_overlap_ratio: float
-    fractional_charge_threshold: float
     outlier_scale_factor: float
 
 
 @dataclass
 class EstimateParameters:
     """Parameters for physics estimation
```

### Comparing `attpc_spyral-0.6.1/src/spyral/core/constants.py` & `attpc_spyral-0.7.0/src/spyral/core/constants.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/estimator.py` & `attpc_spyral-0.7.0/src/spyral/core/estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,25 +175,14 @@
     results: dict[str, int]
         Dictionary to store estimation results in
     chosen_direction: Direction, default=Direction.NONE
         Optional direction for the trajectory. Default
         estimates the direction.
 
     """
-    # Do some cleanup, reject clusters which have too many beam region points
-    beam_region_fraction = float(
-        len(
-            cluster.data[
-                np.linalg.norm(cluster.data[:, :2], axis=1)
-                < detector_params.beam_region_radius
-            ]
-        )
-    ) / float(len(cluster.data))
-    if beam_region_fraction > 0.9:
-        return (False, Direction.NONE)
 
     direction = chosen_direction
     vertex = np.array([0.0, 0.0, 0.0])  # reaction vertex
     center = np.array([0.0, 0.0, 0.0])  # spiral center
     # copy the data so we can modify it without worrying about side-effects
     cluster_data = cluster.data.copy()
```

### Comparing `attpc_spyral-0.6.1/src/spyral/core/hardware_id.py` & `attpc_spyral-0.7.0/src/spyral/core/hardware_id.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/legacy_beam_pads.py` & `attpc_spyral-0.7.0/src/spyral/core/legacy_beam_pads.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/pad_map.py` & `attpc_spyral-0.7.0/src/spyral/core/pad_map.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/phase.py` & `attpc_spyral-0.7.0/src/spyral/core/phase.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/pipeline.py` & `attpc_spyral-0.7.0/src/spyral/core/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,18 @@
         This should be called before running the pipeline.
 
         Returns
         -------
         bool
             True if all phases were successful, False otherwise
         """
-        for phase in self.phases:
+        for idx, phase in enumerate(self.phases):
+            # Skip inactive phases
+            if not self.active[idx]:
+                continue
             if not phase.create_assets(self.workspace):
                 return False
         return True
 
     def validate(self) -> dict[str, bool]:
         """Validate the pipeline by comparing the schema of the phases.
```

### Comparing `attpc_spyral-0.6.1/src/spyral/core/point_cloud.py` & `attpc_spyral-0.7.0/src/spyral/core/point_cloud.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/run_stacks.py` & `attpc_spyral-0.7.0/src/spyral/core/run_stacks.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/spy_log.py` & `attpc_spyral-0.7.0/src/spyral/core/spy_log.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/status_message.py` & `attpc_spyral-0.7.0/src/spyral/core/status_message.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/core/track_generator.py` & `attpc_spyral-0.7.0/src/spyral/core/track_generator.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/correction/electron_corrector.py` & `attpc_spyral-0.7.0/src/spyral/correction/electron_corrector.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/correction/generate.py` & `attpc_spyral-0.7.0/src/spyral/correction/generate.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/data/pad_electronics.csv` & `attpc_spyral-0.7.0/src/spyral/data/pad_electronics.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/data/pad_electronics_legacy.csv` & `attpc_spyral-0.7.0/src/spyral/data/pad_electronics_legacy.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/data/pad_time_correction.csv` & `attpc_spyral-0.7.0/src/spyral/data/pad_time_correction.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/data/padxy.csv` & `attpc_spyral-0.7.0/src/spyral/data/padxy.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/data/padxy_legacy.csv` & `attpc_spyral-0.7.0/src/spyral/data/padxy_legacy.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/geometry/circle.py` & `attpc_spyral-0.7.0/src/spyral/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/interpolate/bilinear.py` & `attpc_spyral-0.7.0/src/spyral/interpolate/bilinear.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/interpolate/linear.py` & `attpc_spyral-0.7.0/src/spyral/interpolate/linear.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/interpolate/track_interpolator.py` & `attpc_spyral-0.7.0/src/spyral/interpolate/track_interpolator.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/phases/cluster_phase.py` & `attpc_spyral-0.7.0/src/spyral/phases/cluster_phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         min_event: int = cloud_group.attrs["min_event"]  # type: ignore
         max_event: int = cloud_group.attrs["max_event"]  # type: ignore
         cluster_group: h5.Group = cluster_file.create_group("cluster")
         cluster_group.attrs["min_event"] = min_event
         cluster_group.attrs["max_event"] = max_event
 
-        nevents = max_event - min_event
+        nevents = max_event - min_event + 1
         total: int
         flush_val: int
         if nevents < 100:
             total = nevents
             flush_val = 0
         else:
             flush_percent = 0.01
@@ -127,17 +127,19 @@
 
             if cloud_data is None:
                 continue
 
             cloud = PointCloud()
             cloud.load_cloud_from_hdf5_data(cloud_data[:].copy(), idx)
 
-            clusters = form_clusters(cloud, self.cluster_params)
-            joined = join_clusters(clusters, self.cluster_params)
-            cleaned = cleanup_clusters(joined, self.cluster_params)
+            # Here we don't need to use the labels array.
+            # We just pass it along as needed.
+            clusters, labels = form_clusters(cloud, self.cluster_params)
+            joined, labels = join_clusters(clusters, self.cluster_params, labels)
+            cleaned, _ = cleanup_clusters(joined, self.cluster_params, labels)
 
             # Each event can contain many clusters
             cluster_event_group = cluster_group.create_group(f"event_{idx}")
             cluster_event_group.attrs["nclusters"] = len(cleaned)
             cluster_event_group.attrs["ic_amplitude"] = cloud_data.attrs["ic_amplitude"]
             cluster_event_group.attrs["ic_centroid"] = cloud_data.attrs["ic_centroid"]
             cluster_event_group.attrs["ic_integral"] = cloud_data.attrs["ic_integral"]
```

### Comparing `attpc_spyral-0.6.1/src/spyral/phases/estimation_phase.py` & `attpc_spyral-0.7.0/src/spyral/phases/estimation_phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 __name__, f"Cluster group not present for run {payload.run_number}!"
             )
             return PhaseResult.invalid_result(payload.run_number)
 
         min_event: int = cluster_group.attrs["min_event"]  # type: ignore
         max_event: int = cluster_group.attrs["max_event"]  # type: ignore
 
-        nevents = max_event - min_event
+        nevents = max_event - min_event + 1
         total: int
         flush_val: int
         if nevents < 100:
             total = nevents
             flush_val = 0
         else:
             flush_percent = 0.01
```

### Comparing `attpc_spyral-0.6.1/src/spyral/phases/interp_solver_phase.py` & `attpc_spyral-0.7.0/src/spyral/phases/interp_solver_phase.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,23 +129,31 @@
             generate_track_mesh(mesh_params, self.track_path, meta_path)
             print("Done.")
         return True
 
     def construct_artifact(
         self, payload: PhaseResult, workspace_path: Path
     ) -> PhaseResult:
+        if not self.solver_params.particle_id_filename.exists():
+            spyral_warn(
+                __name__,
+                f"Particle ID {self.solver_params.particle_id_filename} does not exist, Solver will not run!",
+            )
+            return PhaseResult.invalid_result(payload.run_number)
+
         pid: ParticleID | None = deserialize_particle_id(
             Path(self.solver_params.particle_id_filename), self.nuclear_map
         )
         if pid is None:
             spyral_warn(
                 __name__,
-                f"Particle ID {self.solver_params.particle_id_filename} does not exist, Solver will not run!",
+                f"Particle ID {self.solver_params.particle_id_filename} is not valid, Solver will not run!",
             )
             return PhaseResult.invalid_result(payload.run_number)
+
         result = PhaseResult(
             artifact_path=self.get_artifact_path(workspace_path)
             / form_physics_file_name(payload.run_number, pid),
             successful=True,
             run_number=payload.run_number,
         )
         return result
@@ -198,23 +206,20 @@
             spyral_error(
                 __name__,
                 f"Cluster group does not eixst for run {payload.run_number} at phase 4!",
             )
             return PhaseResult(Path("null"), False, payload.run_number)
 
         # Select the particle group data, beam region of ic, convert to dictionary for row-wise operations
-        # Select only the largest polar angle for a given event to avoid beam-like particles
         estimates_gated = (
             estimate_df.filter(
                 pl.struct(["dEdx", "brho"]).map_batches(pid.cut.is_cols_inside)
                 & (pl.col("ic_amplitude") > self.solver_params.ic_min_val)
                 & (pl.col("ic_amplitude") < self.solver_params.ic_max_val)
             )
-            .sort("polar", descending=True)
-            .unique("event", keep="first")
             .collect()
             .to_dict()
         )
 
         # Check that data actually exists for given PID
         if len(estimates_gated["event"]) == 0:
             msg_queue.put(StatusMessage("Waiting", 0, 0, payload.run_number))
```

### Comparing `attpc_spyral-0.6.1/src/spyral/phases/pointcloud_legacy_phase.py` & `attpc_spyral-0.7.0/src/spyral/phases/pointcloud_legacy_phase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ..core.phase import PhaseLike, PhaseResult
 from ..core.run_stacks import form_run_string
 from ..core.status_message import StatusMessage
 from ..core.config import (
-    FribParameters,
     GetParameters,
     DetectorParameters,
     PadParameters,
 )
 from ..correction import (
     generate_electron_correction,
     create_electron_corrector,
@@ -52,63 +51,63 @@
     removal and scipy.signal.find_peaks to extract signals from the traces. PointcloudLegacyPhase
     is expected to be the first phase in the Pipeline.
 
     Parameters
     ----------
     get_params: GetParameters
         Parameters controlling the GET-DAQ signal analysis
-    frib_params: FribParameters
-        Parameters repurposed in legacy to analyze auxilary detectors (IC, Si, etc)
+    ic_params: GetParameters
+        Parameters in legacy to analyze auxilary detectors (IC, Si, etc)
     detector_params: DetectorParameters
         Parameters describing the detector
     pad_params: PadParameters
         Parameters describing the pad plane mapping
 
     Attributes
     ----------
     get_params: GetParameters
         Parameters controlling the GET-DAQ signal analysis
-    frib_params: FribParameters
-        Parameters repurposed in legacy to analyze auxilary detectors (IC, Si, etc)
+    ic_params: GetParameters
+        Parameters in legacy to analyze auxilary detectors (IC, Si, etc)
     det_params: DetectorParameters
         Parameters describing the detector
     pad_map: PadMap
         Map which converts trace ID to pad ID
 
     """
 
     def __init__(
         self,
         get_params: GetParameters,
-        frib_params: FribParameters,
+        ic_params: GetParameters,
         detector_params: DetectorParameters,
         pad_params: PadParameters,
     ):
         super().__init__(
             "PointcloudLegacy",
             incoming_schema=TRACE_SCHEMA,
             outgoing_schema=POINTCLOUD_SCHEMA,
         )
         self.get_params = get_params
-        self.frib_params = frib_params
+        self.ic_params = ic_params
         self.det_params = detector_params
         self.pad_map = PadMap(pad_params)
 
     def create_assets(self, workspace_path: Path) -> bool:
         asset_path = self.get_asset_storage_path(workspace_path)
         garf_path = Path(self.det_params.garfield_file_path)
         self.electron_correction_path = asset_path / f"{garf_path.stem}.npy"
 
         if (
             not self.electron_correction_path.exists()
             and self.det_params.do_garfield_correction
         ):
             generate_electron_correction(
-                self.electron_correction_path,
                 garf_path,
+                self.electron_correction_path,
                 self.det_params,
             )
         return True
 
     def construct_artifact(
         self, payload: PhaseResult, workspace_path: Path
     ) -> PhaseResult:
@@ -156,15 +155,15 @@
             )
             return PhaseResult.invalid_result(payload.run_number)
 
         cloud_group = point_file.create_group("cloud")
         cloud_group.attrs["min_event"] = min_event
         cloud_group.attrs["max_event"] = max_event
 
-        nevents = max_event - min_event
+        nevents = max_event - min_event + 1
         total: int
         flush_val: int
         if nevents < 100:
             total = nevents
             flush_val = 0
         else:
             flush_percent = 0.01
@@ -185,15 +184,15 @@
             event_data: h5.Dataset
             try:
                 event_data = event_group[f"evt{idx}_data"]  # type: ignore
             except Exception:
                 continue
 
             event = GetLegacyEvent(
-                event_data, idx, self.get_params, self.frib_params, rng
+                event_data, idx, self.get_params, self.ic_params, rng
             )
 
             pc = PointCloud()
             pc.load_cloud_from_get_event(event, self.pad_map)
             pc.calibrate_z_position(
                 self.det_params.micromegas_time_bucket,
                 self.det_params.window_time_bucket,
```

### Comparing `attpc_spyral-0.6.1/src/spyral/phases/pointcloud_phase.py` & `attpc_spyral-0.7.0/src/spyral/phases/pointcloud_phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,28 +182,30 @@
                 f"FRIB scaler data group does not exist in run {payload.run_number}. Spyral will continue, but scalers will not exist.",
             )
             frib_scaler_group = None
         cloud_group = point_file.create_group("cloud")
         cloud_group.attrs["min_event"] = min_event
         cloud_group.attrs["max_event"] = max_event
 
-        nevents = max_event - min_event
+        nevents = max_event - min_event + 1
         total: int
         flush_val: int
         if nevents < 100:
             total = nevents
             flush_val = 0
         else:
             flush_percent = 0.01
             flush_val = int(flush_percent * (max_event - min_event))
             total = 100
 
         count = 0
 
-        msg = StatusMessage(self.name, 1, total, 1)  # We always increment by 1
+        msg = StatusMessage(
+            self.name, 1, total, payload.run_number
+        )  # We always increment by 1
 
         # Process the data
         for idx in range(min_event, max_event + 1):
             count += 1
             if count > flush_val:
                 count = 0
                 msg_queue.put(msg)
```

### Comparing `attpc_spyral-0.6.1/src/spyral/phases/schema.py` & `attpc_spyral-0.7.0/src/spyral/phases/schema.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/solvers/guess.py` & `attpc_spyral-0.7.0/src/spyral/solvers/guess.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/solvers/solver_interp.py` & `attpc_spyral-0.7.0/src/spyral/solvers/solver_interp.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/frib_event.py` & `attpc_spyral-0.7.0/src/spyral/trace/frib_event.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/frib_scalers.py` & `attpc_spyral-0.7.0/src/spyral/trace/frib_scalers.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/frib_trace.py` & `attpc_spyral-0.7.0/src/spyral/trace/frib_trace.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/get_event.py` & `attpc_spyral-0.7.0/src/spyral/trace/get_event.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/get_legacy_event.py` & `attpc_spyral-0.7.0/src/spyral/trace/get_legacy_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .get_trace import GetTrace
-from ..core.config import GetParameters, FribParameters
+from ..core.config import GetParameters
 from ..core.constants import INVALID_EVENT_NAME, INVALID_EVENT_NUMBER
 from ..core.hardware_id import hardware_id_from_array
 
 import numpy as np
 import h5py as h5
 from numba import njit
 
@@ -22,15 +22,15 @@
     ----------
     raw_data: h5py.Dataset
         The hdf5 Dataset that contains trace data
     event_number: int
         The event number
     get_params: GetParameters
         Configuration parameters controlling the GET signal analysis
-    ic_params: FribParameters
+    ic_params: GetParameters
         Configuration parameters controlling the ion chamber signal analysis
     rng: numpy.random.Generator
         A random number generator for use in the signal analysis
 
     Attributes
     ----------
     traces: list[GetTrace]
@@ -53,42 +53,42 @@
     """
 
     def __init__(
         self,
         raw_data: h5.Dataset,
         event_number: int,
         get_params: GetParameters,
-        ic_params: FribParameters,
+        ic_params: GetParameters,
         rng: np.random.Generator,
     ):
         self.traces: list[GetTrace] = []
         self.ic_trace: GetTrace | None = None
         self.name: str = INVALID_EVENT_NAME
         self.number: int = INVALID_EVENT_NUMBER
         self.load_traces(raw_data, event_number, get_params, ic_params, rng)
 
     def load_traces(
         self,
         raw_data: h5.Dataset,
         event_number: int,
         get_params: GetParameters,
-        ic_params: FribParameters,
+        ic_params: GetParameters,
         rng: np.random.Generator,
     ):
         """Process the traces
 
         Parameters
         ----------
         raw_data: h5py.Dataset
             The hdf5 Dataset that contains trace data
         event_number: int
             The event number
         get_params: GetParameters
             Configuration parameters controlling the GET signal analysis
-        ic_params: FribParameters
+        ic_params: GetParameters
             Configuration parameters controlling the ion chamber signal analysis
         rng: numpy.random.Generator
             A random number generator for use in the signal analysis
         """
         self.name = str(raw_data.name)
         self.number = event_number
         trace_matrix = preprocess_traces(
@@ -106,15 +106,15 @@
             # Extract IC
             if (
                 trace.hw_id.cobo_id == 10
                 and trace.hw_id.aget_id == 1
                 and trace.hw_id.aget_channel == 0
             ):
                 self.ic_trace = trace
-                self.ic_trace.find_peaks(ic_params, rel_height=0.8)  # type: ignore
+                self.ic_trace.find_peaks(ic_params, rng, rel_height=0.8)  # type: ignore
                 break
         # Remove CoBo 10 from our normal traces
         self.traces = [trace for trace in self.traces if trace.hw_id.cobo_id != 10]
 
     def is_valid(self) -> bool:
         return self.name != INVALID_EVENT_NAME and self.number != INVALID_EVENT_NUMBER
```

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/get_trace.py` & `attpc_spyral-0.7.0/src/spyral/trace/get_trace.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/src/spyral/trace/peak.py` & `attpc_spyral-0.7.0/src/spyral/trace/peak.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/tests/test_default_pipeline.py` & `attpc_spyral-0.7.0/tests/test_default_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 cluster_params = ClusterParameters(
     min_cloud_size=50,
     min_points=3,
     min_size_scale_factor=0.05,
     min_size_lower_cutoff=10,
     cluster_selection_epsilon=0.3,
     circle_overlap_ratio=0.5,
-    fractional_charge_threshold=0.8,
     outlier_scale_factor=0.05,
 )
 estimate_params = EstimateParameters(
     min_total_trajectory_points=30, smoothing_factor=100.0
 )
 solver_params = SolverParameters(
     gas_data_path=Path("/path/to/some/gas/data.json"),
```

### Comparing `attpc_spyral-0.6.1/tests/test_pad.py` & `attpc_spyral-0.7.0/tests/test_pad.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/tests/test_runs.py` & `attpc_spyral-0.7.0/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.6.1/PKG-INFO` & `attpc_spyral-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: attpc_spyral
-Version: 0.6.1
+Version: 0.7.0
 Summary: AT-TPC analysis pipeline
 Author-Email: gwm17 <gordonmccann215@gmail.com>
 License: GPL-3
 Requires-Python: <3.13,>=3.10
-Requires-Dist: spyral-utils>=0.3.0
+Requires-Dist: spyral-utils>=1.0.0
 Requires-Dist: black>=24.4.0
 Requires-Dist: contourpy>=1.2.1
 Requires-Dist: h5py>=3.11.0
 Requires-Dist: lmfit>=1.3.0
 Requires-Dist: numba>=0.59.1
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: rocket-fft>=0.2.5
 Requires-Dist: typing-extensions>=4.11.0
 Description-Content-Type: text/markdown
 
 # Spyral
 
+![CI](https://github.com/ATTPC/Spyral/actions/workflows/ci.yml/badge.svg)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/attpc_spyral.svg)](https://pypi.python.org/pypi/attpc_spyral/)
+[![PyPI license](https://img.shields.io/pypi/l/attpc_spyral.svg)](https://pypi.python.org/pypi/attpc_spyral/)
+
 Spyral is an analysis library for data from the Active Target Time Projection Chamber (AT-TPC). Spyral provides a flexible analysis pipeline, transforming the raw trace data into physical observables over several tunable steps. The analysis pipeline is also extensible, supporting a diverse array of datasets. Sypral can process multiple data files in parallel, allowing for scalable performance over larger experiment datasets.
 
 ## Installation
 
 Install using pip:
 
 ```bash
@@ -114,36 +118,36 @@
 )
 
 cluster_params = ClusterParameters(
     min_cloud_size=50,
     min_points=3,
     min_size_scale_factor=0.05,
     min_size_lower_cutoff=10,
-    cluster_selection_epsilon=0.3,
+    cluster_selection_epsilon=10.0,
     circle_overlap_ratio=0.5,
     fractional_charge_threshold=0.8,
     outlier_scale_factor=0.05,
 )
 
 estimate_params = EstimateParameters(
     min_total_trajectory_points=30, smoothing_factor=100.0
 )
 
 solver_params = SolverParameters(
     gas_data_path=Path("/path/to/some/gas/data.json"),
     particle_id_filename=Path("/path/to/some/particle/id.json"),
     ic_min_val=900.0,
     ic_max_val=1350.0,
-    n_time_steps=10000,
-    interp_ke_min=0.05,
+    n_time_steps=1000,
+    interp_ke_min=0.1,
     interp_ke_max=70.0,
-    interp_ke_bins=400,
+    interp_ke_bins=350,
     interp_polar_min=2.0,
     interp_polar_max=88.0,
-    interp_polar_bins=170,
+    interp_polar_bins=166,
 )
 
 pipe = Pipeline(
     [
         PointcloudPhase(
             get_params,
             frib_params,
```

