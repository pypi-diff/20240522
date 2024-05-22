# Comparing `tmp/sarus-0.9.7.dev0.tar.gz` & `tmp/sarus-0.9.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.9.7.dev0.tar", last modified: Fri Apr 26 12:32:20 2024, max compression
+gzip compressed data, was "sarus-0.9.7.dev1.tar", last modified: Mon May 13 13:17:11 2024, max compression
```

## Comparing `sarus-0.9.7.dev0.tar` & `sarus-0.9.7.dev1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.432237 sarus-0.9.7.dev0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1606 2024-04-26 12:32:20.432237 sarus-0.9.7.dev0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.416236 sarus-0.9.7.dev0/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      842 2024-04-26 12:31:02.000000 sarus-0.9.7.dev0/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    32593 2024-03-06 13:56:13.000000 sarus-0.9.7.dev0/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.416236 sarus-0.9.7.dev0/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3314 2024-04-26 12:31:02.000000 sarus-0.9.7.dev0/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      323 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    19168 2024-04-15 15:03:56.000000 sarus-0.9.7.dev0/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      757 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.416236 sarus-0.9.7.dev0/sarus/federated_analytics/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       87 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/federated_analytics/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13063 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/federated_analytics/lib.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.416236 sarus-0.9.7.dev0/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      567 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.416236 sarus-0.9.7.dev0/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.420236 sarus-0.9.7.dev0/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.420236 sarus-0.9.7.dev0/sarus/llm/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       70 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/llm/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3647 2024-04-02 12:36:43.000000 sarus-0.9.7.dev0/sarus/llm/pretrained.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.420236 sarus-0.9.7.dev0/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5642 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1981 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1289 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3865 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9892 2024-04-26 12:31:02.000000 sarus-0.9.7.dev0/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.420236 sarus-0.9.7.dev0/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      672 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3481 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    28593 2024-04-26 12:31:02.000000 sarus-0.9.7.dev0/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2633 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4725 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1826 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.420236 sarus-0.9.7.dev0/sarus/matplotlib/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2024-03-06 13:56:13.000000 sarus-0.9.7.dev0/sarus/matplotlib/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-03-06 13:56:13.000000 sarus-0.9.7.dev0/sarus/matplotlib/pyplot.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.420236 sarus-0.9.7.dev0/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      371 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.424236 sarus-0.9.7.dev0/sarus/optbinning/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      215 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/optbinning/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4761 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/optbinning/binning.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      133 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/optbinning/scorecard.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.424236 sarus-0.9.7.dev0/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      212 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8006 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.424236 sarus-0.9.7.dev0/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      375 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.424236 sarus-0.9.7.dev0/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      165 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      152 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    49337 2024-04-26 12:31:02.000000 sarus-0.9.7.dev0/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.424236 sarus-0.9.7.dev0/sarus/scipy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/scipy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7931 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/scipy/sparse.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.424236 sarus-0.9.7.dev0/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4561 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/scripts/generate_op_list.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3003 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/serialization.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.428237 sarus-0.9.7.dev0/sarus/shap/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1584 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/shap/Explanation.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1181 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/shap/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12871 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/shap/explainers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3881 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/shap/maskers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      413 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/shap/plots.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      140 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/shap/utils.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.428237 sarus-0.9.7.dev0/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      719 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6580 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      789 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      803 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11426 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      589 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      191 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1266 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      188 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1708 2024-03-06 13:56:13.000000 sarus-0.9.7.dev0/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      581 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1565 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.428237 sarus-0.9.7.dev0/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      279 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      943 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.428237 sarus-0.9.7.dev0/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      169 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.428237 sarus-0.9.7.dev0/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3177 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    23032 2024-04-26 12:31:02.000000 sarus-0.9.7.dev0/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2344 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.432237 sarus-0.9.7.dev0/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1205 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.416236 sarus-0.9.7.dev0/sarus.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1606 2024-04-26 12:32:20.000000 sarus-0.9.7.dev0/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2430 2024-04-26 12:32:20.000000 sarus-0.9.7.dev0/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-04-26 12:32:20.000000 sarus-0.9.7.dev0/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-01-22 14:06:25.000000 sarus-0.9.7.dev0/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      436 2024-04-26 12:32:20.000000 sarus-0.9.7.dev0/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2024-04-26 12:32:20.000000 sarus-0.9.7.dev0/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1446 2024-04-26 12:32:20.432237 sarus-0.9.7.dev0/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2024-04-26 12:32:01.000000 sarus-0.9.7.dev0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-26 12:32:20.432237 sarus-0.9.7.dev0/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2024-02-16 15:21:05.000000 sarus-0.9.7.dev0/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.485994 sarus-0.9.7.dev1/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1606 2024-05-13 13:17:11.485994 sarus-0.9.7.dev1/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      728 2024-05-06 06:58:19.000000 sarus-0.9.7.dev1/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    32593 2024-03-06 13:56:13.000000 sarus-0.9.7.dev1/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2024-04-26 20:27:14.000000 sarus-0.9.7.dev1/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      323 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    19168 2024-04-15 15:03:56.000000 sarus-0.9.7.dev1/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      757 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/federated_analytics/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       87 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/federated_analytics/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13063 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/federated_analytics/lib.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      567 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus/llm/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       70 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/llm/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3647 2024-04-02 12:36:43.000000 sarus-0.9.7.dev1/sarus/llm/pretrained.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5642 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1981 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1289 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3865 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9496 2024-04-26 20:27:14.000000 sarus-0.9.7.dev1/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      672 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3481 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    28479 2024-05-13 13:08:08.000000 sarus-0.9.7.dev1/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2633 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4725 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1826 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/matplotlib/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2024-03-06 13:56:13.000000 sarus-0.9.7.dev1/sarus/matplotlib/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-03-06 13:56:13.000000 sarus-0.9.7.dev1/sarus/matplotlib/pyplot.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      371 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/optbinning/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      215 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/optbinning/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4761 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/optbinning/binning.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      133 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/optbinning/scorecard.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      212 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8006 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      375 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      165 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      152 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    45522 2024-05-13 13:08:08.000000 sarus-0.9.7.dev1/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/scipy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/scipy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7931 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/scipy/sparse.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4561 2024-05-13 13:08:08.000000 sarus-0.9.7.dev1/sarus/scripts/generate_op_list.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3003 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/serialization.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.477994 sarus-0.9.7.dev1/sarus/shap/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1584 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/shap/Explanation.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1181 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/shap/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12871 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/shap/explainers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3881 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/shap/maskers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      413 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/shap/plots.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      140 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/shap/utils.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.481994 sarus-0.9.7.dev1/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      719 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6580 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      789 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      803 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11426 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      589 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      191 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1266 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      188 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1708 2024-03-06 13:56:13.000000 sarus-0.9.7.dev1/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      581 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1565 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.481994 sarus-0.9.7.dev1/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      279 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      943 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.481994 sarus-0.9.7.dev1/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      169 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.481994 sarus-0.9.7.dev1/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3177 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18706 2024-04-26 20:27:14.000000 sarus-0.9.7.dev1/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2344 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.485994 sarus-0.9.7.dev1/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1205 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.473994 sarus-0.9.7.dev1/sarus.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1606 2024-05-13 13:17:11.000000 sarus-0.9.7.dev1/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2430 2024-05-13 13:17:11.000000 sarus-0.9.7.dev1/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-05-13 13:17:11.000000 sarus-0.9.7.dev1/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-01-22 14:06:25.000000 sarus-0.9.7.dev1/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      436 2024-05-13 13:17:11.000000 sarus-0.9.7.dev1/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2024-05-13 13:17:11.000000 sarus-0.9.7.dev1/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1446 2024-05-13 13:17:11.485994 sarus-0.9.7.dev1/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2024-05-13 13:17:08.000000 sarus-0.9.7.dev1/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-13 13:17:11.485994 sarus-0.9.7.dev1/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2024-02-16 15:21:05.000000 sarus-0.9.7.dev1/tests/test_sanity.py
```

### Comparing `sarus-0.9.7.dev0/PKG-INFO` & `sarus-0.9.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.9.7.dev0
+Version: 0.9.7.dev1
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.9.7.dev0/README.rst` & `sarus-0.9.7.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/__init__.py` & `sarus-0.9.7.dev1/sarus/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,25 +25,21 @@
     from .utils import (
         eval,
         eval_perturbation,
         eval_policy,
         floating,
         integer,
         length,
-        push_to_table,
-        check_push_to_table_status,
     )
 
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_perturbation",
     "eval_policy",
     "config",
     "floating",
     "integer",
-    "push_to_table",
-    "check_push_to_table_status",
 ]
```

### Comparing `sarus-0.9.7.dev0/sarus/config.yaml` & `sarus-0.9.7.dev1/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/context/local_sdk.py` & `sarus-0.9.7.dev1/sarus/context/local_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.factory import Factory
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import Schema
 from sarus_data_spec.storage.local import Storage
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
-from sarus_data_spec.type import Type
 
 from sarus.dataspec_wrapper import MetaWrapper
 from sarus.manager.sdk_manager import SDKManager, manager
 from sarus.typing import Client
 from sarus.wrapper_factory import DataSpecWrapperFactory
 
 from ..typing import SyncPolicy
@@ -60,19 +59,14 @@
         self.factory().register(
             sp.type_name(sp.VariantConstraint),
             lambda protobuf, store: VariantConstraint(
                 cast(sp.VariantConstraint, protobuf), store
             ),
         )
 
-        self.factory().register(
-            sp.type_name(sp.Type),
-            lambda protobuf: Type(cast(sp.Type, protobuf)),
-        )
-
         self._wrapper_factory = DataSpecWrapperFactory()
         for (
             python_classname,
             sarus_wrapper_class,
         ) in MetaWrapper._wrapper_classes:
             self._wrapper_factory.register(
                 python_classname=python_classname,
```

### Comparing `sarus-0.9.7.dev0/sarus/dataspec_wrapper.py` & `sarus-0.9.7.dev1/sarus/dataspec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/debug.py` & `sarus-0.9.7.dev1/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/federated_analytics/lib.py` & `sarus-0.9.7.dev1/sarus/federated_analytics/lib.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/imblearn/over_sampling.py` & `sarus-0.9.7.dev1/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/imblearn/pipeline.py` & `sarus-0.9.7.dev1/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/imblearn/under_sampling.py` & `sarus-0.9.7.dev1/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/legacy/tensorflow/dataset.py` & `sarus-0.9.7.dev1/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/legacy/tensorflow/model.py` & `sarus-0.9.7.dev1/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/llm/pretrained.py` & `sarus-0.9.7.dev1/sarus/llm/pretrained.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/arrow_local.py` & `sarus-0.9.7.dev1/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/arrow_remote.py` & `sarus-0.9.7.dev1/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/base_remote.py` & `sarus-0.9.7.dev1/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/cache_scalar_local.py` & `sarus-0.9.7.dev1/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/dataspec_api.py` & `sarus-0.9.7.dev1/sarus/manager/dataspec_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,20 +287,7 @@
         return arrow_iterator_from_response()
 
 
 def scalar_result(client: Client, uuid: str) -> t.Any:
     """Return the scalar's value."""
     resp = dataspec_result_response(client, uuid)
     return pkl.loads(resp.content)
-
-
-def push_sql_dataset(client: Client, uuid: str):
-    start = time.perf_counter()
-    resp: Response = client.session().post(
-        f"{client.url()}/dataspecs/{uuid}/push_sql",
-    )
-    end = time.perf_counter()
-    logger.debug(
-        f"GET /dataspecs/{uuid}/push_sql {resp.status_code} {resp.headers.get('Content-Type')} ({end-start:.2f}s)"
-    )
-    raise_response(resp)
-    return resp
```

### Comparing `sarus-0.9.7.dev0/sarus/manager/ops/api.py` & `sarus-0.9.7.dev1/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/parquet_local.py` & `sarus-0.9.7.dev1/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/sdk_manager.py` & `sarus-0.9.7.dev1/sarus/manager/sdk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,17 +209,14 @@
         alt_dataspec = self.storage().referrable(alt_dataspec_uuid)
         return alt_dataspec, privacy_policy
 
     def launch(self, dataspec: st.DataSpec) -> None:
         """Launch a Dataspec's computation on the server."""
         api.launch_dataspec(self.client(), dataspec.uuid())
 
-    def push_sql_dataset(self, dataset: st.Dataset):
-        api.push_sql_dataset(self.client(), dataset.uuid())
-
     def python_type(self, dataspec: st.DataSpec) -> str:
         """Return the Python class name of a DataSpec.
 
         This is used to instantiate the correct DataSpecWrapper class.
         """
         python_type_att = dataspec.attribute(name=PYTHON_TYPE)
         if python_type_att is not None:
```

### Comparing `sarus-0.9.7.dev0/sarus/manager/typing.py` & `sarus-0.9.7.dev1/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/value_local.py` & `sarus-0.9.7.dev1/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/manager/value_remote.py` & `sarus-0.9.7.dev1/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/numpy/scalars.py` & `sarus-0.9.7.dev1/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/optbinning/binning.py` & `sarus-0.9.7.dev1/sarus/optbinning/binning.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/pandas/core.py` & `sarus-0.9.7.dev1/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/pandas/dataframe.py` & `sarus-0.9.7.dev1/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sarus.py` & `sarus-0.9.7.dev1/sarus/sarus.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,14 @@
     try:
         import tensorflow as tf
 
         import sarus.legacy.tensorflow as sltf
     except ModuleNotFoundError:
         pass  # error message in sarus_data_spec.typing
 
-logger = logging.getLogger(__name__)
-
 
 def sdk_excepthook(
     exc_cls: t.Type[BaseException],
     exc: BaseException,
     tb: Optional[TracebackType],
 ) -> Any:
     if isinstance(exc, DataSpecErrorStatus):
@@ -169,69 +167,14 @@
 
     @classmethod
     def _from_dict(cls, data: dict) -> ShallowDataset:
         # `data` is the JSON returned by calling GET /datasets/
         return cls(data.get("id"), data.get("name"))
 
 
-class DataConnectionList(list):
-    """Custom class to lazily fetch a Dataset when indexing."""
-
-    def __init__(self, iterable: t.Iterable[ShallowDataConnection]) -> None:
-        super().__init__(iterable)
-
-    def __setitem__(self, i: int, value: t.Any) -> None:
-        raise NotImplementedError("A DatasetList is immutable.")
-
-    def append(self, value: t.Any) -> None:
-        raise NotImplementedError("A DatasetList is immutable.")
-
-    def insert(self, i: int, value: t.Any) -> None:
-        raise NotImplementedError("A DatasetList is immutable.")
-
-    def extend(self, other: DatasetList) -> None:
-        raise NotImplementedError("A DatasetList is immutable.")
-
-    @classmethod
-    def _from_list(cls, data: list) -> DataConnectionList:
-        # `data` is the JSON returned by calling GET /dataconnection/
-        return cls(
-            [ShallowDataConnection._from_dict(datacon) for datacon in data]
-        )
-
-
-class ShallowDataConnection:
-    """Shallow dataset that is merely used as a placeholder for slugname."""
-
-    def __init__(
-        self,
-        id: int,
-        slugname: str,
-        connector_type: str,
-        table_names: List[str],
-    ):
-        self.id = id
-        self.name = slugname
-        self.connector_type = connector_type
-        self.destination_table_names = table_names
-
-    def __repr__(self) -> str:
-        return f"<Sarus DataConnection name={self.name} id={self.id} connector_type={self.connector_type}, destination_table_names={self.destination_table_names}>>"
-
-    @classmethod
-    def _from_dict(cls, data: dict) -> ShallowDataset:
-        # `data` is the JSON returned by calling GET /dataconnection/
-        return cls(
-            data.get("id"),
-            data.get("name"),
-            data.get("connector_type"),
-            data.get("whitelisted_table_names"),
-        )
-
-
 class Dataset(DataSpecWrapper[t.Iterator[pa.RecordBatch]]):
     """A class representing a Sarus Dataset.
 
     This class is the interface to the protected data. It enables to inspect the
     Sarus dataset metadata, manipulate synthetic data locally, prepare
     processing steps and identify the dataset for executing remote private
     queries.
@@ -437,19 +380,19 @@
             randomize_bigdata_sampling (bool, optional): Determines whether the limited rows should be selected
             randomly or if only the first rows should be used. This is only applicable if sampling is performed.
             Defaults to True.
 
         Returns:
             DataFrame: The Sarus DataFrame wrapper.
         """
-        # attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)   # noqa: E800
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
         dataspec_small_data = transform_to_small_data(
             self._dataspec, None, random_sampling=randomize_bigdata_sampling
         )
-        # assert attributes_ds is not None
+        assert attributes_ds is not None
         return DataFrame.from_dataspec(dataspec_small_data)
 
     def __getitem__(self, item: t.List[str]) -> Dataset:
         return self.table(item)
 
     def table(self, table_name: t.List[str]) -> Dataset:
         """Get a table from the dataset.
@@ -1047,64 +990,14 @@
         ]
         sorted_datasets = sorted(
             unsorted_datasets,
             key=lambda x: x.name,
         )
         return DatasetList(sorted_datasets, self)
 
-    def _dataconnections(self, slugname=None):
-        payload = {"slugname": slugname} if slugname is not None else {}
-        request = self.session().get(
-            f"{self.base_url}/dataconnections",
-            json=payload,
-        )
-        raise_response(request)
-        dataconnections = request.json()
-        return dataconnections
-
-    def list_writable_dataconnections(self, slugname=None):
-        dataconnections = self._dataconnections(slugname)
-        return DataConnectionList._from_list(dataconnections)
-
-    def describe_destination_table(
-        self, data_connection_name: str, table: str
-    ):
-        type_table = self._get_type_destination_table(
-            data_connection_name, table
-        )
-        for column_name in type_table.children().keys():
-            print(
-                f"Column name: {column_name}, Type: {type_table.children()[column_name].name()}"
-            )
-
-    def _get_type_destination_table(
-        self, data_connection_name: str, table: str
-    ):
-        parts = table.split(".")
-        if len(parts) == 2 and all(parts):
-            schema_name = parts[0]
-            table_name = parts[1]
-        else:
-            raise ValueError(
-                "Error: Input must be in the format 'dataconnection_name.table_name' with non-empty Schema and table_name."
-            )
-        start = time.perf_counter()
-        resp = self.session().get(
-            f"{self.url()}/table/{data_connection_name}/{schema_name}/{table_name}/describe",
-        )
-        end = time.perf_counter()
-        logger.debug(
-            f"GET /table/{data_connection_name}/{schema_name}/{table_name}/describe {resp.status_code} {resp.headers.get('Content-Type')} ({end-start:.2f}s)"
-        )
-        raise_response(resp)
-
-        proto = dict_deserialize(resp.json()['table_type'])
-        type_table = self.context().factory().create(proto)
-        return type_table
-
     def dataset(self, slugname: str = None, id: int = None) -> Dataset:
         """Select a dataset from the Sarus Gateway.
 
         Either `slugname` or `id` should be provided. If both are provided, then
         only the `slugname` is considered.
 
         Args:
```

### Comparing `sarus-0.9.7.dev0/sarus/scipy/sparse.py` & `sarus-0.9.7.dev1/sarus/scipy/sparse.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/scripts/generate_op_list.py` & `sarus-0.9.7.dev1/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/serialization.py` & `sarus-0.9.7.dev1/sarus/serialization.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/shap/Explanation.py` & `sarus-0.9.7.dev1/sarus/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/shap/__init__.py` & `sarus-0.9.7.dev1/sarus/shap/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/shap/explainers.py` & `sarus-0.9.7.dev1/sarus/shap/explainers.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/shap/maskers.py` & `sarus-0.9.7.dev1/sarus/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/__init__.py` & `sarus-0.9.7.dev1/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/cluster.py` & `sarus-0.9.7.dev1/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/compose.py` & `sarus-0.9.7.dev1/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/decomposition.py` & `sarus-0.9.7.dev1/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/ensemble.py` & `sarus-0.9.7.dev1/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/impute.py` & `sarus-0.9.7.dev1/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/linear_model.py` & `sarus-0.9.7.dev1/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/model_selection.py` & `sarus-0.9.7.dev1/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/pipeline.py` & `sarus-0.9.7.dev1/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/preprocessing.py` & `sarus-0.9.7.dev1/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/sklearn/svm.py` & `sarus-0.9.7.dev1/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/skopt/searchcv.py` & `sarus-0.9.7.dev1/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/std/types.py` & `sarus-0.9.7.dev1/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/typing.py` & `sarus-0.9.7.dev1/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/utils.py` & `sarus-0.9.7.dev1/sarus/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from functools import partial, wraps
 from typing import Any, Callable, Dict, Optional, Type, Union
 
 import numpy as np
 import pandas as pd
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
-import sarus_data_spec.status as stt
 import yaml
 from sarus_data_spec.context import global_context
 from sarus_data_spec.status import DataSpecErrorStatus
-from sarus_data_spec.transform import external, error_estimation, push_sql
+from sarus_data_spec.transform import (
+    external,
+    error_estimation,
+)
 from sarus_data_spec.dataset import transformed
-from sarus_data_spec.constants import TO_SQL_TASK
-import sarus.manager.dataspec_api as api
 
 from .context.typing import LocalSDKContext
 from .typing import (
     DataSpecVariant,
     DataSpecWrapper,
     FederatedWrapper,
     TracedFunction,
@@ -133,133 +133,14 @@
         return {
             eval_perturbation(k): eval_perturbation(v) for k, v in x.items()
         }
     else:
         return x
 
 
-def find_id_by_name_datacon(dataconnections, datacon_name):
-    for data in dataconnections:
-        if data.get('name') == datacon_name:
-            return data.get('id')
-    return None
-
-
-def push_to_table(
-    wrapper: DataSpecWrapper,
-    data_connection_name: str,
-    table: str,
-    return_uuid=False,
-):
-    """Pushes a dataspec to a specified table within a data connection.
-
-    This method constructs the URI for the dataspec, prepares the dataspec for pushing by removing columns not present in the table, and performs the push
-    operation using the provided wrapper's manager and client API.
-
-    Args:
-        wrapper (DataSpecWrapper): The dataspec wrapper containing the dataspec to be pushed.
-        data_connection_name (str): The name of the data connection where the dataspec will be pushed.
-        table (str): The name of the table where the dataspec will be pushed, in the format 'schema_name.table_name'.
-        return_uuid (bool): If True, the function returns the UUID of the pushed dataspec.
-
-    Returns:
-        str: The UUID of the pushed dataspec, if return_uuid is True.
-
-    Raises:
-        ValueError: If 'table' does not follow the 'schema_name.table_name' format or if it contains empty values, or if the wrapper type is not supported.
-    """
-    manager = wrapper.manager()
-    client = manager.client()
-
-    # get data_connection_name and table_name
-    parts = table.split(".")
-    if len(parts) == 2 and all(parts):
-        schema_name, table_name = parts
-    else:
-        raise ValueError(
-            "Error: Input must be in the format 'dataconnection_name.schema_name.table_name' with non-empty dataconnection_name, schema_name or table_name."
-        )
-
-    dataconnections = client._dataconnections()
-    dataconnection_id = find_id_by_name_datacon(
-        dataconnections, data_connection_name
-    )
-    uri = f"sarus://{dataconnection_id}"
-
-    from sarus.sarus import DataFrame, Dataset
-
-    if isinstance(wrapper, Dataset):
-        wrapper = wrapper.as_pandas()
-    elif isinstance(wrapper, DataFrame):
-        pass
-    else:
-        raise ValueError(
-            "Error: Input must be either a {DataFrame} or a {Dataset}. to be pushed"
-        )
-
-    try:
-        destination_table_columns = (
-            client._get_type_destination_table(data_connection_name, table)
-            .children()
-            .keys()
-        )
-        wrapper_columns = set(eval(wrapper.columns, verbose=0))
-        common_columns = wrapper_columns.intersection(
-            destination_table_columns
-        )
-
-        if not common_columns:
-            raise ValueError(
-                f"No common columns with the destination table '{table}'."
-            )
-
-        difference_columns = wrapper_columns - common_columns
-        if difference_columns:
-            logger.warning(
-                f"Dropping columns {difference_columns} not present in destination table '{table}'."
-            )
-
-        wrapper = wrapper[list(common_columns)]
-    except Exception:
-        pass
-
-    dataspec = wrapper.dataspec()
-    to_be_pushed_dataspec = push_sql(
-        data_connection_name, schema_name, table_name, uri
-    )(dataspec)
-    manager.push(to_be_pushed_dataspec)
-    api.push_sql_dataset(client, to_be_pushed_dataspec.uuid())
-    print(
-        f"Check the evolution of the push to table with sarus.check_push_to_table_status('{to_be_pushed_dataspec.uuid()}')"
-    )
-    if return_uuid:
-        return to_be_pushed_dataspec.uuid()
-
-
-def check_push_to_table_status(uuid: str, return_status=False):
-    """Returns/Prints the status of the computation to sql for the input uuid."""
-    context: LocalSDKContext = global_context()
-    client = context.manager().client()
-
-    status_proto = api.dataspec_status(
-        client=client,
-        uuid=uuid,
-        task_names=[TO_SQL_TASK],
-    )
-    if status_proto is None:
-        return None
-    else:
-        status = stt.Status(protobuf=status_proto, store=False)
-        stage = status.task(TO_SQL_TASK).stage()
-        print(f"The push to table is in stage {stage}")
-        print(status.task(TO_SQL_TASK).properties()["message"])
-        if return_status:
-            return status.task(TO_SQL_TASK)
-
-
 def save(dw: DataSpecWrapper, path: str) -> None:
     """Save a DataSpecWrapper for loading in another notebook."""
     dw.sarus_save(path)
 
 
 def is_standard_type_iterable(iterable) -> bool:
     """Checks if all elements in an iterable are instances of a specific set of standard types.
```

### Comparing `sarus-0.9.7.dev0/sarus/wrapper_factory.py` & `sarus-0.9.7.dev1/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus/xgboost/xgboost.py` & `sarus-0.9.7.dev1/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/sarus.egg-info/PKG-INFO` & `sarus-0.9.7.dev1/sarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.9.7.dev0
+Version: 0.9.7.dev1
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.9.7.dev0/sarus.egg-info/SOURCES.txt` & `sarus-0.9.7.dev1/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.9.7.dev0/setup.cfg` & `sarus-0.9.7.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.11.1.dev0
+	sarus-data-spec-public==3.11.2.dev0
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
 	protobuf >= 3.20.3
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
```

