# Comparing `tmp/mljar-supervised-1.1.7.tar.gz` & `tmp/mljar-supervised-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mljar-supervised-1.1.7.tar", last modified: Wed Apr 10 12:39:36 2024, max compression
+gzip compressed data, was "mljar-supervised-1.1.8.tar", last modified: Wed May 22 12:58:33 2024, max compression
```

## Comparing `mljar-supervised-1.1.7.tar` & `mljar-supervised-1.1.8.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.1.7/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26122 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    25334 2024-01-08 08:57:51.000000 mljar-supervised-1.1.7/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/mljar_supervised.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26122 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3493 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-04-10 12:35:04.000000 mljar-supervised-1.1.7/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       33 2023-09-21 12:45:57.000000 mljar-supervised-1.1.7/requirements_dev.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1506 2024-04-10 12:38:52.000000 mljar-supervised-1.1.7/setup.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2024-04-10 12:39:15.000000 mljar-supervised-1.1.7/supervised/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/algorithms/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/algorithms/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4174 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/algorithms/algorithm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2475 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/baseline.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    14679 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9190 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/decision_tree.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5161 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-12-01 11:37:16.000000 mljar-supervised-1.1.7/supervised/algorithms/factory.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3710 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12349 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5833 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/linear.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4842 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5282 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-04 09:46:14.000000 mljar-supervised-1.1.7/supervised/algorithms/registry.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6245 2023-12-01 11:37:16.000000 mljar-supervised-1.1.7/supervised/algorithms/sklearn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12532 2024-03-04 13:30:52.000000 mljar-supervised-1.1.7/supervised/algorithms/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26170 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/automl.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    99509 2024-03-08 09:41:43.000000 mljar-supervised-1.1.7/supervised/base_automl.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/callbacks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/callbacks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/callbacks/callback.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/callbacks/callback_list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9018 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/callbacks/early_stopping.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1701 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/callbacks/learner_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      568 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/callbacks/max_iters_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1847 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/callbacks/metric_logger.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      933 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/callbacks/terminate_on_nan.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3353 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/callbacks/total_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    22911 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/ensemble.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      547 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/exceptions.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/fairness/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.1.7/supervised/fairness/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26141 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/fairness/metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15001 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/fairness/optimization.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.1.7/supervised/fairness/plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4975 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/fairness/report.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.1.7/supervised/fairness/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    29288 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/model_framework.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/preprocessing/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/preprocessing/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3535 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/datetime_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12603 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/eda.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2023-12-01 11:37:16.000000 mljar-supervised-1.1.7/supervised/preprocessing/encoding_selector.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1488 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/exclude_missing_target.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10807 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/goldenfeatures_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3819 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/kmeans_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2446 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/label_binarizer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1793 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/label_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1555 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/loo_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26388 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4616 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_categorical.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_missing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3646 2024-03-04 12:03:16.000000 mljar-supervised-1.1.7/supervised/preprocessing/scale.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2557 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/text_transformer.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/tuner/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/tuner/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2361 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/data_info.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/hill_climbing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    59416 2024-03-04 11:50:15.000000 mljar-supervised-1.1.7/supervised/tuner/mljar_tuner.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/tuner/optuna/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5539 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2510 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1910 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5896 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2122 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2511 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11606 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4727 2024-03-04 13:31:00.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6273 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/preprocessing_tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/tuner/random_parameters.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8944 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/time_controller.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/utils/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      259 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    37054 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/additional_metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8148 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/additional_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5352 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/automl_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/utils/common.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2023-09-21 12:19:11.000000 mljar-supervised-1.1.7/supervised/utils/config.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/utils/constants.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.1.7/supervised/utils/data_validation.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3015 2024-03-04 10:30:50.000000 mljar-supervised-1.1.7/supervised/utils/importance.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      823 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/jsonencoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4951 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/utils/leaderboard_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4972 2024-03-04 12:16:25.000000 mljar-supervised-1.1.7/supervised/utils/learning_curves.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    13465 2024-03-04 11:46:43.000000 mljar-supervised-1.1.7/supervised/utils/metric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12128 2024-03-04 11:50:51.000000 mljar-supervised-1.1.7/supervised/utils/shap.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      424 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/subsample.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      589 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/validation/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/validation/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1210 2023-09-20 06:26:41.000000 mljar-supervised-1.1.7/supervised/validation/validation_step.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/validation/validator_base.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4075 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/validation/validator_custom.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5505 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/validation/validator_kfold.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4708 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/validation/validator_split.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.169940 mljar-supervised-1.1.8/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.1.8/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26633 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    25845 2024-05-22 12:37:47.000000 mljar-supervised-1.1.8/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/mljar_supervised.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26633 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3493 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-05-22 12:58:33.000000 mljar-supervised-1.1.8/mljar_supervised.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-04-10 12:35:04.000000 mljar-supervised-1.1.8/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       33 2023-09-21 12:45:57.000000 mljar-supervised-1.1.8/requirements_dev.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-05-22 12:58:33.169940 mljar-supervised-1.1.8/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1506 2024-05-22 12:57:56.000000 mljar-supervised-1.1.8/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/supervised/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2024-05-22 12:58:01.000000 mljar-supervised-1.1.8/supervised/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/supervised/algorithms/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/algorithms/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4174 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/algorithms/algorithm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2475 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/baseline.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    14679 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9190 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/decision_tree.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5161 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-12-01 11:37:16.000000 mljar-supervised-1.1.8/supervised/algorithms/factory.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3710 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12349 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5833 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/linear.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4842 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5282 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/algorithms/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-04 09:46:14.000000 mljar-supervised-1.1.8/supervised/algorithms/registry.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6245 2023-12-01 11:37:16.000000 mljar-supervised-1.1.8/supervised/algorithms/sklearn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12532 2024-03-04 13:30:52.000000 mljar-supervised-1.1.8/supervised/algorithms/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26170 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/automl.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    99573 2024-05-22 12:50:25.000000 mljar-supervised-1.1.8/supervised/base_automl.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.161940 mljar-supervised-1.1.8/supervised/callbacks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/callbacks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/callbacks/callback.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/callbacks/callback_list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9018 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/callbacks/early_stopping.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1701 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/callbacks/learner_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      568 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/callbacks/max_iters_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1847 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/callbacks/metric_logger.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      933 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/callbacks/terminate_on_nan.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3353 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/callbacks/total_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    22911 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/ensemble.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      547 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/exceptions.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/fairness/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.1.8/supervised/fairness/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26141 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/fairness/metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15001 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/fairness/optimization.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.1.8/supervised/fairness/plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4975 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/fairness/report.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.1.8/supervised/fairness/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29288 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/model_framework.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/preprocessing/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/preprocessing/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3535 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/datetime_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12603 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/eda.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2023-12-01 11:37:16.000000 mljar-supervised-1.1.8/supervised/preprocessing/encoding_selector.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1488 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/exclude_missing_target.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10807 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/goldenfeatures_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3819 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/kmeans_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2446 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/label_binarizer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1793 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/label_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1555 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/loo_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26388 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4616 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_categorical.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_missing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3646 2024-03-04 12:03:16.000000 mljar-supervised-1.1.8/supervised/preprocessing/scale.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2557 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/preprocessing/text_transformer.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/tuner/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/tuner/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2361 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/data_info.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/hill_climbing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    59416 2024-03-04 11:50:15.000000 mljar-supervised-1.1.8/supervised/tuner/mljar_tuner.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/tuner/optuna/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5539 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2510 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1910 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5896 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2122 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2511 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11606 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4727 2024-03-04 13:31:00.000000 mljar-supervised-1.1.8/supervised/tuner/optuna/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6273 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/preprocessing_tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/tuner/random_parameters.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8944 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/tuner/time_controller.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/utils/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      259 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    37054 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/additional_metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8148 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/additional_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5352 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/automl_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/utils/common.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2023-09-21 12:19:11.000000 mljar-supervised-1.1.8/supervised/utils/config.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/utils/constants.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.1.8/supervised/utils/data_validation.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3015 2024-03-04 10:30:50.000000 mljar-supervised-1.1.8/supervised/utils/importance.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      823 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/jsonencoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4951 2023-09-20 06:26:40.000000 mljar-supervised-1.1.8/supervised/utils/leaderboard_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4972 2024-03-04 12:16:25.000000 mljar-supervised-1.1.8/supervised/utils/learning_curves.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    13465 2024-03-04 11:46:43.000000 mljar-supervised-1.1.8/supervised/utils/metric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12128 2024-03-04 11:50:51.000000 mljar-supervised-1.1.8/supervised/utils/shap.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      424 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/subsample.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      589 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/utils/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-22 12:58:33.165940 mljar-supervised-1.1.8/supervised/validation/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/validation/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1210 2023-09-20 06:26:41.000000 mljar-supervised-1.1.8/supervised/validation/validation_step.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.1.8/supervised/validation/validator_base.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4075 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/validation/validator_custom.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5505 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/validation/validator_kfold.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4708 2024-03-01 11:22:55.000000 mljar-supervised-1.1.8/supervised/validation/validator_split.py
```

### Comparing `mljar-supervised-1.1.7/LICENSE` & `mljar-supervised-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/PKG-INFO` & `mljar-supervised-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.1.7
+Version: 1.1.8
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar,random forest,decision tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features selection,features engineering
 Classifier: Programming Language :: Python
@@ -12,14 +12,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+# New way for visual programming!
+
+We are working on new way for visual programming. We developed desktop application called [MLJAR Studio](https://mljar.com). 
+It is a notebook based development environment with interactive code recipes and managed Python environment. All running locally on your machine. We are waiting for your feedback.
+
+<p align="center">
+  <img 
+    alt="mljar AutoML"
+    src="https://raw.githubusercontent.com/pplonski/pplonski/main/media/piece-of-code.png" width="88%" />  
+</p>
+
+---
+
 # MLJAR Automated Machine Learning for Humans
 
 [![Tests status](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
 
@@ -27,20 +41,20 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-supervised)
 
 <p align="center">
   <img 
     alt="mljar AutoML"
-    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_white.png#gh-light-mode-only" width="100%" />  
+    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_white.png#gh-light-mode-only" width="50%" />  
 </p>
 <p align="center">
   <img 
     alt="mljar AutoML"
-    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_black.png#gh-dark-mode-only" width="100%" />  
+    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_black.png#gh-dark-mode-only" width="50%" />  
 </p>
 
 ---
 
 **Documentation**: <a href="https://supervised.mljar.com/" target="_blank">https://supervised.mljar.com/</a>
 
 **Source Code**: <a href="https://github.com/mljar/mljar-supervised" target="_blank">https://github.com/mljar/mljar-supervised</a>
@@ -48,16 +62,14 @@
 **Looking for commercial support**: Please contact us by [email](https://mljar.com/contact/) for details
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/pipeline_AutoML.png" width="100%" />
 </p>
 
-
-
 ---
 
 ## Table of Contents
 
  - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
  - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
  - [AutoML Web App with GUI](https://github.com/mljar/mljar-supervised#automl-web-app-with-user-interface)
@@ -72,14 +84,17 @@
  - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
  - [Cite](https://github.com/mljar/mljar-supervised#cite)
  - [License](https://github.com/mljar/mljar-supervised#license)
  - [Commercial support](https://github.com/mljar/mljar-supervised#commercial-support)
  - [MLJAR](https://github.com/mljar/mljar-supervised#mljar)
  
 
+
+
+
 # Automated Machine Learning 
 
 The `mljar-supervised` is an Automated Machine Learning Python package that works with tabular data. It is designed to save time for a data scientist. It abstracts the common way to preprocess the data, construct the machine learning models, and perform hyper-parameters tuning to find the best model :trophy:. It is no black box, as you can see exactly how the ML pipeline is constructed (with a detailed Markdown report for each ML model). 
 
 The `mljar-supervised` will help you with:
  - explaining and understanding your data (Automatic Exploratory Data Analysis),
  - trying many different machine learning models (Algorithm Selection and Hyper-Parameters tuning),
```

#### html2text {}

```diff
@@ -1,32 +1,38 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.7 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.8 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Keywords: automated machine learning,automl,machine learning,data
 science,data mining,mljar,random forest,decision
 tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features
 selection,features engineering Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # MLJAR Automated
-Machine Learning for Humans [![Tests status](https://github.com/mljar/mljar-
-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/
-mljar/mljar-supervised/actions/workflows/run-tests.yml) [![PyPI version](https:
-//badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-
-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-
-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-
-supervised) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-
-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/) [![Anaconda-
-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/
-platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised) [![Anaconda-
-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/
-license.svg)](https://anaconda.org/conda-forge/mljar-supervised) [![Downloads]
-(https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-
-supervised)
+Description-Content-Type: text/markdown License-File: LICENSE # New way for
+visual programming! We are working on new way for visual programming. We
+developed desktop application called [MLJAR Studio](https://mljar.com). It is a
+notebook based development environment with interactive code recipes and
+managed Python environment. All running locally on your machine. We are waiting
+for your feedback.
+                                [mljar AutoML]
+--- # MLJAR Automated Machine Learning for Humans [![Tests status](https://
+github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)]
+(https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml) [!
+[PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://
+badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
+anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://
+anaconda.org/conda-forge/mljar-supervised) [![PyPI pyversions](https://
+img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/
+pypi/mljar-supervised/) [![Anaconda-Server Badge](https://anaconda.org/conda-
+forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/
+mljar-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
+mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-
+supervised) [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://
+pepy.tech/project/mljar-supervised)
                                 [mljar AutoML]
                                 [mljar AutoML]
 --- **Documentation**: _h_t_t_p_s_:_/_/_s_u_p_e_r_v_i_s_e_d_._m_l_j_a_r_._c_o_m_/ **Source Code**: _h_t_t_p_s_:_/_/
 _g_i_t_h_u_b_._c_o_m_/_m_l_j_a_r_/_m_l_j_a_r_-_s_u_p_e_r_v_i_s_e_d **Looking for commercial support**: Please
 contact us by [email](https://mljar.com/contact/) for details
      [https://raw.githubusercontent.com/mljar/mljar-examples/master/media/
                              pipeline_AutoML.png]
```

### Comparing `mljar-supervised-1.1.7/README.md` & `mljar-supervised-1.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+
+# New way for visual programming!
+
+We are working on new way for visual programming. We developed desktop application called [MLJAR Studio](https://mljar.com). 
+It is a notebook based development environment with interactive code recipes and managed Python environment. All running locally on your machine. We are waiting for your feedback.
+
+<p align="center">
+  <img 
+    alt="mljar AutoML"
+    src="https://raw.githubusercontent.com/pplonski/pplonski/main/media/piece-of-code.png" width="88%" />  
+</p>
+
+---
+
 # MLJAR Automated Machine Learning for Humans
 
 [![Tests status](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
 
@@ -9,20 +23,20 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-supervised)
 
 <p align="center">
   <img 
     alt="mljar AutoML"
-    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_white.png#gh-light-mode-only" width="100%" />  
+    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_white.png#gh-light-mode-only" width="50%" />  
 </p>
 <p align="center">
   <img 
     alt="mljar AutoML"
-    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_black.png#gh-dark-mode-only" width="100%" />  
+    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_black.png#gh-dark-mode-only" width="50%" />  
 </p>
 
 ---
 
 **Documentation**: <a href="https://supervised.mljar.com/" target="_blank">https://supervised.mljar.com/</a>
 
 **Source Code**: <a href="https://github.com/mljar/mljar-supervised" target="_blank">https://github.com/mljar/mljar-supervised</a>
@@ -30,16 +44,14 @@
 **Looking for commercial support**: Please contact us by [email](https://mljar.com/contact/) for details
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/pipeline_AutoML.png" width="100%" />
 </p>
 
-
-
 ---
 
 ## Table of Contents
 
  - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
  - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
  - [AutoML Web App with GUI](https://github.com/mljar/mljar-supervised#automl-web-app-with-user-interface)
@@ -54,14 +66,17 @@
  - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
  - [Cite](https://github.com/mljar/mljar-supervised#cite)
  - [License](https://github.com/mljar/mljar-supervised#license)
  - [Commercial support](https://github.com/mljar/mljar-supervised#commercial-support)
  - [MLJAR](https://github.com/mljar/mljar-supervised#mljar)
  
 
+
+
+
 # Automated Machine Learning 
 
 The `mljar-supervised` is an Automated Machine Learning Python package that works with tabular data. It is designed to save time for a data scientist. It abstracts the common way to preprocess the data, construct the machine learning models, and perform hyper-parameters tuning to find the best model :trophy:. It is no black box, as you can see exactly how the ML pipeline is constructed (with a detailed Markdown report for each ML model). 
 
 The `mljar-supervised` will help you with:
  - explaining and understanding your data (Automatic Exploratory Data Analysis),
  - trying many different machine learning models (Algorithm Selection and Hyper-Parameters tuning),
```

#### html2text {}

```diff
@@ -1,8 +1,14 @@
-# MLJAR Automated Machine Learning for Humans [![Tests status](https://
+# New way for visual programming! We are working on new way for visual
+programming. We developed desktop application called [MLJAR Studio](https://
+mljar.com). It is a notebook based development environment with interactive
+code recipes and managed Python environment. All running locally on your
+machine. We are waiting for your feedback.
+                                [mljar AutoML]
+--- # MLJAR Automated Machine Learning for Humans [![Tests status](https://
 github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)]
 (https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml) [!
 [PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://
 badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
 anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://
 anaconda.org/conda-forge/mljar-supervised) [![PyPI pyversions](https://
 img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/
```

### Comparing `mljar-supervised-1.1.7/mljar_supervised.egg-info/PKG-INFO` & `mljar-supervised-1.1.8/mljar_supervised.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.1.7
+Version: 1.1.8
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar,random forest,decision tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features selection,features engineering
 Classifier: Programming Language :: Python
@@ -12,14 +12,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+# New way for visual programming!
+
+We are working on new way for visual programming. We developed desktop application called [MLJAR Studio](https://mljar.com). 
+It is a notebook based development environment with interactive code recipes and managed Python environment. All running locally on your machine. We are waiting for your feedback.
+
+<p align="center">
+  <img 
+    alt="mljar AutoML"
+    src="https://raw.githubusercontent.com/pplonski/pplonski/main/media/piece-of-code.png" width="88%" />  
+</p>
+
+---
+
 # MLJAR Automated Machine Learning for Humans
 
 [![Tests status](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
 
@@ -27,20 +41,20 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-supervised)
 
 <p align="center">
   <img 
     alt="mljar AutoML"
-    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_white.png#gh-light-mode-only" width="100%" />  
+    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_white.png#gh-light-mode-only" width="50%" />  
 </p>
 <p align="center">
   <img 
     alt="mljar AutoML"
-    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_black.png#gh-dark-mode-only" width="100%" />  
+    src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_black.png#gh-dark-mode-only" width="50%" />  
 </p>
 
 ---
 
 **Documentation**: <a href="https://supervised.mljar.com/" target="_blank">https://supervised.mljar.com/</a>
 
 **Source Code**: <a href="https://github.com/mljar/mljar-supervised" target="_blank">https://github.com/mljar/mljar-supervised</a>
@@ -48,16 +62,14 @@
 **Looking for commercial support**: Please contact us by [email](https://mljar.com/contact/) for details
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/pipeline_AutoML.png" width="100%" />
 </p>
 
-
-
 ---
 
 ## Table of Contents
 
  - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
  - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
  - [AutoML Web App with GUI](https://github.com/mljar/mljar-supervised#automl-web-app-with-user-interface)
@@ -72,14 +84,17 @@
  - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
  - [Cite](https://github.com/mljar/mljar-supervised#cite)
  - [License](https://github.com/mljar/mljar-supervised#license)
  - [Commercial support](https://github.com/mljar/mljar-supervised#commercial-support)
  - [MLJAR](https://github.com/mljar/mljar-supervised#mljar)
  
 
+
+
+
 # Automated Machine Learning 
 
 The `mljar-supervised` is an Automated Machine Learning Python package that works with tabular data. It is designed to save time for a data scientist. It abstracts the common way to preprocess the data, construct the machine learning models, and perform hyper-parameters tuning to find the best model :trophy:. It is no black box, as you can see exactly how the ML pipeline is constructed (with a detailed Markdown report for each ML model). 
 
 The `mljar-supervised` will help you with:
  - explaining and understanding your data (Automatic Exploratory Data Analysis),
  - trying many different machine learning models (Algorithm Selection and Hyper-Parameters tuning),
```

#### html2text {}

```diff
@@ -1,32 +1,38 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.7 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.8 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Keywords: automated machine learning,automl,machine learning,data
 science,data mining,mljar,random forest,decision
 tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features
 selection,features engineering Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # MLJAR Automated
-Machine Learning for Humans [![Tests status](https://github.com/mljar/mljar-
-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/
-mljar/mljar-supervised/actions/workflows/run-tests.yml) [![PyPI version](https:
-//badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-
-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-
-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-
-supervised) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-
-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/) [![Anaconda-
-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/
-platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised) [![Anaconda-
-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/
-license.svg)](https://anaconda.org/conda-forge/mljar-supervised) [![Downloads]
-(https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-
-supervised)
+Description-Content-Type: text/markdown License-File: LICENSE # New way for
+visual programming! We are working on new way for visual programming. We
+developed desktop application called [MLJAR Studio](https://mljar.com). It is a
+notebook based development environment with interactive code recipes and
+managed Python environment. All running locally on your machine. We are waiting
+for your feedback.
+                                [mljar AutoML]
+--- # MLJAR Automated Machine Learning for Humans [![Tests status](https://
+github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)]
+(https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml) [!
+[PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://
+badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
+anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://
+anaconda.org/conda-forge/mljar-supervised) [![PyPI pyversions](https://
+img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/
+pypi/mljar-supervised/) [![Anaconda-Server Badge](https://anaconda.org/conda-
+forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/
+mljar-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
+mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-
+supervised) [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://
+pepy.tech/project/mljar-supervised)
                                 [mljar AutoML]
                                 [mljar AutoML]
 --- **Documentation**: _h_t_t_p_s_:_/_/_s_u_p_e_r_v_i_s_e_d_._m_l_j_a_r_._c_o_m_/ **Source Code**: _h_t_t_p_s_:_/_/
 _g_i_t_h_u_b_._c_o_m_/_m_l_j_a_r_/_m_l_j_a_r_-_s_u_p_e_r_v_i_s_e_d **Looking for commercial support**: Please
 contact us by [email](https://mljar.com/contact/) for details
      [https://raw.githubusercontent.com/mljar/mljar-examples/master/media/
                              pipeline_AutoML.png]
```

### Comparing `mljar-supervised-1.1.7/mljar_supervised.egg-info/SOURCES.txt` & `mljar-supervised-1.1.8/mljar_supervised.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/setup.py` & `mljar-supervised-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mljar-supervised",
-    version="1.1.7",
+    version="1.1.8",
     description="Automated Machine Learning for Humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mljar/mljar-supervised",
     author="MLJAR, Sp. z o.o.",
     author_email="contact@mljar.com",
     license="MIT",
```

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/algorithm.py` & `mljar-supervised-1.1.8/supervised/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/baseline.py` & `mljar-supervised-1.1.8/supervised/algorithms/baseline.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/catboost.py` & `mljar-supervised-1.1.8/supervised/algorithms/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/decision_tree.py` & `mljar-supervised-1.1.8/supervised/algorithms/decision_tree.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/extra_trees.py` & `mljar-supervised-1.1.8/supervised/algorithms/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/factory.py` & `mljar-supervised-1.1.8/supervised/algorithms/factory.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/knn.py` & `mljar-supervised-1.1.8/supervised/algorithms/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/lightgbm.py` & `mljar-supervised-1.1.8/supervised/algorithms/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/linear.py` & `mljar-supervised-1.1.8/supervised/algorithms/linear.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/nn.py` & `mljar-supervised-1.1.8/supervised/algorithms/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/random_forest.py` & `mljar-supervised-1.1.8/supervised/algorithms/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/registry.py` & `mljar-supervised-1.1.8/supervised/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/sklearn.py` & `mljar-supervised-1.1.8/supervised/algorithms/sklearn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/algorithms/xgboost.py` & `mljar-supervised-1.1.8/supervised/algorithms/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/automl.py` & `mljar-supervised-1.1.8/supervised/automl.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/base_automl.py` & `mljar-supervised-1.1.8/supervised/base_automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2286,18 +2286,18 @@
     padding-top: 6px;
     padding-bottom: 6px;
     text-align: left;
     background-color: #0099cc;
     color: white;
 }}
 
-body {{
+.mljar-automl-report {{
     font-family: ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
     background-color: rgba(236, 243, 249, 0.15);
-}}
+
 
 h1 {{
     color: #004666;
     border-bottom: 1px solid rgba(0,70,102,0.3)
 }}
 h2 {{
     color: #004666;
@@ -2323,15 +2323,15 @@
     color: #004666;
 }}
 
 a:hover {{
     cursor: pointer;
     color: #0099CC;
 }}
-
+}}
 
 """
 
     def _md_to_html(self, md_fname, page_type, dir_path, me=None):
         import base64
 
         import markdown
@@ -2455,15 +2455,17 @@
 <html>
 <head>
     <style>
     {self.report_style}
     </style>
 </head>
 <body>
+    <div class="mljar-automl-report">
     {body}
+    <div>
 </body>
 </html>
 """
         with open(main_readme_html, "w") as fout:
             fout.write(report_content)
 
         return self._show_report(main_readme_html, width, height)
```

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/callback.py` & `mljar-supervised-1.1.8/supervised/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/callback_list.py` & `mljar-supervised-1.1.8/supervised/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/early_stopping.py` & `mljar-supervised-1.1.8/supervised/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/learner_time_constraint.py` & `mljar-supervised-1.1.8/supervised/callbacks/learner_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/max_iters_constraint.py` & `mljar-supervised-1.1.8/supervised/callbacks/max_iters_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/metric_logger.py` & `mljar-supervised-1.1.8/supervised/callbacks/metric_logger.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/terminate_on_nan.py` & `mljar-supervised-1.1.8/supervised/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/callbacks/total_time_constraint.py` & `mljar-supervised-1.1.8/supervised/callbacks/total_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/ensemble.py` & `mljar-supervised-1.1.8/supervised/ensemble.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/exceptions.py` & `mljar-supervised-1.1.8/supervised/exceptions.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/fairness/metrics.py` & `mljar-supervised-1.1.8/supervised/fairness/metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/fairness/optimization.py` & `mljar-supervised-1.1.8/supervised/fairness/optimization.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/fairness/plots.py` & `mljar-supervised-1.1.8/supervised/fairness/plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/fairness/report.py` & `mljar-supervised-1.1.8/supervised/fairness/report.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/fairness/utils.py` & `mljar-supervised-1.1.8/supervised/fairness/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/model_framework.py` & `mljar-supervised-1.1.8/supervised/model_framework.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/datetime_transformer.py` & `mljar-supervised-1.1.8/supervised/preprocessing/datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/eda.py` & `mljar-supervised-1.1.8/supervised/preprocessing/eda.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/encoding_selector.py` & `mljar-supervised-1.1.8/supervised/preprocessing/encoding_selector.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/exclude_missing_target.py` & `mljar-supervised-1.1.8/supervised/preprocessing/exclude_missing_target.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/goldenfeatures_transformer.py` & `mljar-supervised-1.1.8/supervised/preprocessing/goldenfeatures_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/kmeans_transformer.py` & `mljar-supervised-1.1.8/supervised/preprocessing/kmeans_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/label_binarizer.py` & `mljar-supervised-1.1.8/supervised/preprocessing/label_binarizer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/label_encoder.py` & `mljar-supervised-1.1.8/supervised/preprocessing/label_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/loo_encoder.py` & `mljar-supervised-1.1.8/supervised/preprocessing/loo_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing.py` & `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_categorical.py` & `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_categorical.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_missing.py` & `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_missing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_utils.py` & `mljar-supervised-1.1.8/supervised/preprocessing/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/scale.py` & `mljar-supervised-1.1.8/supervised/preprocessing/scale.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/preprocessing/text_transformer.py` & `mljar-supervised-1.1.8/supervised/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/data_info.py` & `mljar-supervised-1.1.8/supervised/tuner/data_info.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/hill_climbing.py` & `mljar-supervised-1.1.8/supervised/tuner/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/mljar_tuner.py` & `mljar-supervised-1.1.8/supervised/tuner/mljar_tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/catboost.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/extra_trees.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/knn.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/lightgbm.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/nn.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/random_forest.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/tuner.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/optuna/xgboost.py` & `mljar-supervised-1.1.8/supervised/tuner/optuna/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/preprocessing_tuner.py` & `mljar-supervised-1.1.8/supervised/tuner/preprocessing_tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/random_parameters.py` & `mljar-supervised-1.1.8/supervised/tuner/random_parameters.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/tuner/time_controller.py` & `mljar-supervised-1.1.8/supervised/tuner/time_controller.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/additional_metrics.py` & `mljar-supervised-1.1.8/supervised/utils/additional_metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/additional_plots.py` & `mljar-supervised-1.1.8/supervised/utils/additional_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/automl_plots.py` & `mljar-supervised-1.1.8/supervised/utils/automl_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/common.py` & `mljar-supervised-1.1.8/supervised/utils/common.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/config.py` & `mljar-supervised-1.1.8/supervised/utils/config.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/data_validation.py` & `mljar-supervised-1.1.8/supervised/utils/data_validation.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/importance.py` & `mljar-supervised-1.1.8/supervised/utils/importance.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/jsonencoder.py` & `mljar-supervised-1.1.8/supervised/utils/jsonencoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/leaderboard_plots.py` & `mljar-supervised-1.1.8/supervised/utils/leaderboard_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/learning_curves.py` & `mljar-supervised-1.1.8/supervised/utils/learning_curves.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/metric.py` & `mljar-supervised-1.1.8/supervised/utils/metric.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/shap.py` & `mljar-supervised-1.1.8/supervised/utils/shap.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/utils/utils.py` & `mljar-supervised-1.1.8/supervised/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/validation/validation_step.py` & `mljar-supervised-1.1.8/supervised/validation/validation_step.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/validation/validator_custom.py` & `mljar-supervised-1.1.8/supervised/validation/validator_custom.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/validation/validator_kfold.py` & `mljar-supervised-1.1.8/supervised/validation/validator_kfold.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.7/supervised/validation/validator_split.py` & `mljar-supervised-1.1.8/supervised/validation/validator_split.py`

 * *Files identical despite different names*

