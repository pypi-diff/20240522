# Comparing `tmp/optima_ml-0.3.3a3.tar.gz` & `tmp/optima_ml-0.3.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optima_ml-0.3.3a3.tar", last modified: Sun Apr 28 13:25:01 2024, max compression
+gzip compressed data, was "optima_ml-0.3.4a1.tar", last modified: Wed May 22 16:24:14 2024, max compression
```

## Comparing `optima_ml-0.3.3a3.tar` & `optima_ml-0.3.4a1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/
--rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.3a3/LICENSE
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/
--rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.3a3/OPTIMA/__main__.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/builtin/
--rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.3a3/OPTIMA/builtin/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/OPTIMA/builtin/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.3a3/OPTIMA/builtin/figures_of_merit.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/builtin/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-17 06:54:34.000000 optima_ml-0.3.3a3/OPTIMA/builtin/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/OPTIMA/builtin/search_space.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/core/
--rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/core/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    86860 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/core/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/core/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-17 06:54:34.000000 optima_ml-0.3.3a3/OPTIMA/core/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    41918 2024-04-28 12:14:59.000000 optima_ml-0.3.3a3/OPTIMA/core/search_space.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/core/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    81175 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/core/training.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    80230 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/core/variable_optimization.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    17991 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/defaults.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/hardware_configs/
--rw-rw-r--   0 erik     (30000) erik     (30003)     2809 2024-04-28 12:14:59.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/Dresden_Taurus.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16754 2024-04-28 12:14:59.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/common.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/helpers.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/helpers/
--rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/helpers/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/helpers/extract_data_from_NTuples.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/helpers/manage_ray_nodes.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/keras/
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/keras/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    28658 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/OPTIMA/keras/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/keras/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/keras/training.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/lightning/
--rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.3a3/OPTIMA/lightning/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/lightning/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/lightning/training.py
--rwxrwxr-x   0 erik     (30000) erik     (30003)   100879 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/optima.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/resources/
--rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.3a3/OPTIMA/resources/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.3a3/OPTIMA/resources/config_verification.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/resources/pbt_with_seed.py
--rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)   120177 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/README.md
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/optima_ml.egg-info/
--rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/entry_points.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/requires.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/top_level.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/setup.cfg
--rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/setup.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/tests/
--rw-rw-r--   0 erik     (30000) erik     (30003)    34780 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/tests/test_builtin.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    25631 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/tests/test_core.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6471 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/tests/test_integration.py
--rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima_ml-0.3.3a3/tests/test_integration_sameMachine.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/tests/test_preprocessing.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.4a1/LICENSE
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.716290 optima_ml-0.3.4a1/OPTIMA/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.4a1/OPTIMA/__main__.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/builtin/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.4a1/OPTIMA/builtin/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/builtin/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.4a1/OPTIMA/builtin/figures_of_merit.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/builtin/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/builtin/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/builtin/search_space.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/core/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/core/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    90299 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/core/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    12282 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    41918 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/core/search_space.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/core/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    78638 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/training.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    80431 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/variable_optimization.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    17991 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/defaults.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/hardware_configs/
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2809 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/Dresden_Taurus.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16754 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/common.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/helpers.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/helpers/
+-rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/helpers/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/helpers/extract_data_from_NTuples.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/helpers/manage_ray_nodes.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/keras/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/keras/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    28658 2024-05-08 11:48:13.000000 optima_ml-0.3.4a1/OPTIMA/keras/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/keras/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-05-14 12:20:45.000000 optima_ml-0.3.4a1/OPTIMA/keras/training.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/lightning/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.4a1/OPTIMA/lightning/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/lightning/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/lightning/training.py
+-rwxrwxr-x   0 erik     (30000) erik     (30003)   109000 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/optima.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/OPTIMA/resources/
+-rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.4a1/OPTIMA/resources/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.4a1/OPTIMA/resources/config_verification.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/resources/pbt_with_seed.py
+-rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)   120177 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/README.md
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/optima_ml.egg-info/
+-rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/requires.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/top_level.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/setup.cfg
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/setup.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/tests/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    34780 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/tests/test_builtin.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    25661 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/tests/test_core.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     9011 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/tests/test_integration.py
+-rw-rw-rw-   0 erik     (30000) erik     (30003)     6579 2024-05-14 09:15:25.000000 optima_ml-0.3.4a1/tests/test_integration_sameMachine.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/tests/test_preprocessing.py
```

### Comparing `optima_ml-0.3.3a3/LICENSE` & `optima_ml-0.3.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/builtin/evaluation.py` & `optima_ml-0.3.4a1/OPTIMA/builtin/evaluation.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/builtin/figures_of_merit.py` & `optima_ml-0.3.4a1/OPTIMA/builtin/figures_of_merit.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/builtin/inputs.py` & `optima_ml-0.3.4a1/OPTIMA/builtin/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/builtin/search_space.py` & `optima_ml-0.3.4a1/OPTIMA/builtin/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/evaluation.py` & `optima_ml-0.3.4a1/OPTIMA/core/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     gpus_per_model: int = 0,
     overtraining_conditions: Optional[list] = None,
     write_results: bool = True,
     return_results_str: bool = False,
     return_unfilled: bool = False,
     return_crossval_models: bool = False,
     PBT: bool = False,
-    PBT_replay_getter: Optional[Callable] = None,
+    PBT_mutation_handler: Optional[OPTIMA.core.training.PBTMutationHandler] = None,
     seed: Optional[int] = None,
 ) -> Union[
     tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame],
     tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, str],
     tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, str, list],
     tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, dict, dict],
     tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, str, dict, dict],
@@ -94,16 +94,20 @@
     - `best fit`: the evolution of all metrics of each trial is fitted (see ``evaluation.get_best_trials_from_fit``
       for details). The best trial is given by the best target metric fit function value that passed all overfitting
       conditions. The overfitting conditions are evaluated using the fit function values of all necessary metrics at
       each epoch (if ``run_config.check_overtraining_with_fit`` is ``True``) or using the reported values (if
       ``run_config.check_overtraining_with_fit`` is ``False``).
 
     For both methods, the hyperparameters corresponding to the best trial and the number of epochs to reach the best
-    target metric value are extracted. Both are given to the ``perform_crossvalidation``-function to perform the k-fold
-    crossvalidation, resulting in `k` trained models per method.
+    target metric value are extracted. If ``PBT`` is ``False``, the hyperparameters correspond to the config provided by
+    Tune via ``analysis.get_all_configs()``. If ``PBT`` is ``True``, the ``get_policy()``-function of the provided
+    ``PBT_mutation_handler`` is called to check if a hyperparameter schedule is available for the best trial. If this is
+    the case, this policy is used. If not, the config provided by Tune is used. Both the hyperparameters and the number
+    of epochs are given to the ``perform_crossvalidation``-function to perform the k-fold crossvalidation, resulting in
+    `k` trained models per method.
 
     The ``evaluate``-function is called for the 2*k models trained during the crossvalidation. After the evaluation, the
     mean and standard deviation of the `k` values for each metric provided by the evaluation is calculated for both sets
     of hyperparameters. The results are printed to console.
 
     If ``write_results`` is True, the results and a summary of the experiment (the used input variables as given by the
     provided ``input_handler``-instance, the shape of the training, validation and (if used) testing dataset as well as
@@ -169,18 +173,17 @@
     return_crossval_models : bool
         If ``True``, a dictionary containing file names of the saved crossvalidation models, the corresponding indices
         denoting which of the `k` crossvalidation-splittings was used for the training, the model config and a dictionary
         containing the training, validation and (if used) testing datasets for each splitting are returned. (Default value = False)
     PBT : bool
         Signifies if this is the evaluation of the Population Based Training step. This is given to ``perform_crossvalidation``
         and used to skip the fit evaluation. (Default value = False)
-    PBT_replay_getter : Optional[Callable]
-        A callable that returns a fully configured ``tune.Tuner``-instance to be able to replay a PBT trial (using a
-        ``PopulationBasedTrainingReplay``-scheduler). This is given to ``perform_crossvalidation`` and is only necessary
-        for the Population Based Training step. (Default value = None)
+    PBT_mutation_handler : Optional[OPTIMA.core.training.PBTMutationHandler]
+        An instance of the ``OPTIMA.core.training.PBTMutationHandler``-class that helps to handle the PBT mutation
+        policies. Only used of ``PBT`` is ``True`` (Default value = None)
     seed : Optional[int]
         Seed given to ``perform_crossvalidation``. (Default value = None)
 
     Returns
     -------
     Union[
         tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame],
@@ -317,22 +320,24 @@
                 optimization_results_string += tabulate.tabulate(
                     best_trials_fit,
                     headers=[best_trials_fit.index.name] + list(best_trials_fit.columns),
                     tablefmt="fancy_grid",
                 )
 
         # go through results by iterating over the best trials for each target metric, print the corresponding configs,
-        # copy best checkpoints to results folder and save output paths for later evaluation
+        # and save output paths for later evaluation
         # first prepare the dataframe that will contain the best configs, meaning the hyperparameters of the best trials
         # for each target metric, once determined using the best value and once using the fit. Since the first
         # checkpointing epoch and the checkpointing frequency are not relevant hyperparameters, skip those entries.
         optimize_name_list = optimize_name if isinstance(optimize_name, list) else [optimize_name]
         hps_names = list(search_space.keys())
         hps_names.remove("first_checkpoint_epoch")
         hps_names.remove("checkpoint_frequency")
+        if PBT:
+            hps_names.remove("seed")
         model_configs_df = pd.DataFrame(
             index=hps_names + ["epochs", "seed"],
             columns=list(*zip(optimize_name_list, [f"{metric} fit" for metric in optimize_name_list]))
             if not skip_fit_evaluation
             else optimize_name_list,
         )
         model_configs_df.index.name = "Hyperparameter"
@@ -352,35 +357,108 @@
 
         # start with results from the best metric values
         dirs_to_evaluate = (
             []
         )  # will contain the paths to the directories containing the models to evaluate (best model from optimization + crossvalidation models)
         model_configs_to_evaluate = []  # will contain the configs of the best models
         for metric, best_trial, best_epoch in zip(best_trials.index, best_trials["trial"], best_trials["best epoch"]):
-            # get the config of this trial, add the best epoch and save it to the model_configs_to_evaluate list; this is
-            # later given to the crossvalidation function to train multiple models for each config
-            model_config_to_evaluate = all_model_configs[best_trial].copy()
-            model_config_to_evaluate["epochs"] = int(best_epoch)
+            # get the config of this trial
+            model_config_to_evaluate = {}
+            config = all_model_configs[best_trial].copy()
+
+            # get the trial id
             for trial_id in trial_ids:
                 if trial_id in best_trial:
                     model_config_to_evaluate[
                         "trial_id"
-                    ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
+                    ] = trial_id  # best_trial is full path to the optimization folder while trails in trial_list as only the names
                     break
+
+            # when evaluating the PBT step, check if there is a policy available for this trial. If yes, use a different
+            # structure for the model_config_to_evaluate
+            if PBT and PBT_mutation_handler.get_policy(model_config_to_evaluate["trial_id"]) is not None:
+                # get the policy
+                policy = PBT_mutation_handler.get_policy(model_config_to_evaluate["trial_id"])
+
+                # since first_checkpoint_epoch, checkpoint_frequency, max_epochs and seed are constants, they will be
+                # the same for every config in the policy. Thus, move them outside of the hyperparameter schedule
+                constants = {
+                    "first_checkpoint_epoch": policy[0][1]["first_checkpoint_epoch"],
+                    "checkpoint_frequency": policy[0][1]["checkpoint_frequency"],
+                    "max_epochs": policy[0][1]["max_epochs"],
+                    "seed": policy[0][1]["seed"],
+                }
+
+                # since the constant entries as well as "first_checkpoint_epoch" and "checkpoint_frequency" are not
+                # needed in the schedule, remove the corresponding entries from each config in the policy
+                for _, model_config in policy:
+                    del model_config["max_epochs"]
+                    del model_config["seed"]
+                    del model_config["first_checkpoint_epoch"]
+                    del model_config["checkpoint_frequency"]
+
+                # add the policy and the constants to the model config to evaluate
+                model_config_to_evaluate["hp_schedule"] = policy
+                model_config_to_evaluate.update(constants)
+            else:
+                if PBT:
+                    print(
+                        f"Did not find a hyperparameter mutation policy for trial "
+                        f"{model_config_to_evaluate['trial_id']}. Using fixed hyperparameters: {config}"
+                    )
+                model_config_to_evaluate = config
+
+            # add the best epoch and save it to the model_configs_to_evaluate list; this is later given to the
+            # crossvalidation function to train multiple models for each config
+            model_config_to_evaluate["epochs"] = int(best_epoch)
             model_configs_to_evaluate.append(model_config_to_evaluate)
 
-            # Add the hyperparameters to the dataframe containing the configs of the best trials. For hierarchical
-            # search spaces, not all hyperparameters must have a value, so insert "-" for those. Since the checkpointing
-            # frequency and the first checkpoint epoch are not relevant hyperparameters, skip those entries.
-            model_config = model_configs_to_evaluate[-1]
-            for hp in model_configs_df.index:
-                if hp in ["first_checkpoint_epoch", "checkpoint_frequency"]:
-                    continue
-                hp_value = model_config.get(hp)
-                model_configs_df.loc[hp, metric] = hp_value if hp_value is not None else "-"
+            # Add the hyperparameters to the dataframe containing the configs of the best trials. For PBT with an
+            # available policy, indicate the mutations. For hierarchical search spaces, not all hyperparameters must
+            # have a value, so insert "-" for those. Since the checkpointing frequency and the first checkpoint epoch
+            # are not relevant hyperparameters, skip those entries.
+            if "hp_schedule" in model_config_to_evaluate.keys():
+                # grab the hyperparameter schedule
+                policy = model_config_to_evaluate["hp_schedule"]
+                for hp in model_configs_df.index:
+                    if hp in ["first_checkpoint_epoch", "checkpoint_frequency"]:
+                        continue
+                    elif hp == "epochs":
+                        model_configs_df.loc[hp, metric] = model_config_to_evaluate["epochs"]
+                    elif hp == "seed":
+                        model_configs_df.loc[hp, metric] = model_config_to_evaluate["seed"]
+                    else:
+                        # build the string of mutations by iterating through this hp's schedule
+                        hp_string = ""
+                        previous_hp_value = None
+                        for start_epoch, model_config in policy:
+                            # get the hp value for this schedule step
+                            hp_value = model_config[hp] if hp in model_config.keys() else "-"
+
+                            # check if the value has changed, otherwise we can skip this step
+                            if hp_value == previous_hp_value:
+                                continue
+
+                            # add this step's hp value to the string
+                            if hp_string == "":
+                                hp_string = str(hp_value)
+                            else:
+                                hp_string += f"\nepoch {start_epoch} --> {hp_value}"
+
+                            # update the previous value
+                            previous_hp_value = hp_value
+
+                        # write the config entry
+                        model_configs_df.loc[hp, metric] = hp_string
+            else:
+                for hp in model_configs_df.index:
+                    if hp in ["first_checkpoint_epoch", "checkpoint_frequency"]:
+                        continue
+                    hp_value = model_config_to_evaluate.get(hp)
+                    model_configs_df.loc[hp, metric] = hp_value if hp_value is not None else "-"
 
             # create the target folder for the following crossvalidation
             target_folder = os.path.join(results_dir, metric if len(best_trials.index) > 1 else "", "best_value")
             dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
             if not os.path.exists(target_folder):
                 os.makedirs(target_folder, exist_ok=True)
 
@@ -429,16 +507,14 @@
             input_handler,
             cpus_per_model,
             gpus_per_model,
             custom_metrics,
             composite_metrics,
             native_metrics,
             weighted_native_metrics,
-            PBT=PBT,
-            PBT_replay_getter=PBT_replay_getter,
             seed=seed,
         )
         print("Cross-validation finished!")
 
         # reload best models from the optimization and the corresponding crossvalidation models and do the evaluation
         evaluation_string = "Evaluation:"
         print("\nReloading the cross-validation models for evaluation...")
@@ -598,14 +674,16 @@
                     model_configs_df,
                     optimization_str,
                     optimization_results_string,
                     crossval_model_info,
                     {
                         k: [ray.get(e) for e in v] for k, v in crossval_input_data.items()
                     },  # we want to save the actual data here!
+                    model_configs_to_evaluate,
+                    dirs_to_evaluate,
                     evaluation_string,
                     raw_values_list,
                 ),
                 evaluation_file,
             )
     else:
         print(
@@ -618,61 +696,41 @@
                 best_trials,
                 best_trials_fit,
                 model_configs_df,
                 optimization_str,
                 optimization_results_string,
                 crossval_model_info,
                 crossval_input_data,
+                crossval_model_configs_to_evaluate,
+                crossval_dirs_to_evaluate,
                 evaluation_string,
                 raw_values_list,
             ) = pickle.load(evaluation_file)
 
         # check if the crossvalidation should be done again; could be useful when crossvalidation should be repeated but
         # the optimization folder was already deleted, but should be avoided when possible because the evaluation cannot
         # be redone in that case (because the configs of each trial are saved inside the optimization folder and are
         # thus not available anymore)
         print(
             "Checking if crossvalidation needs to be repeated. Note that the evaluation will not be repeated even when"
             " the crossvalidation is redone! If you want to repeat the evaluation, it's necessary to delete the "
             "'evaluation.pickle' file."
         )
-        model_configs_to_evaluate = []
-        dirs_to_evaluate = []
-        for metric in best_trials.index:
-            model_config = {}
-            model_config_fit = {}
-            for hp in model_configs_df.index:
-                model_config[hp] = model_configs_df.loc[hp, metric]
-                if not skip_fit_evaluation:
-                    model_config_fit[hp] = model_configs_df.loc[hp, f"{metric} fit"]
-            model_configs_to_evaluate.append(model_config)
-            if not skip_fit_evaluation:
-                model_configs_to_evaluate.append(model_config_fit)
-            dirs_to_evaluate.append(
-                os.path.join(results_dir, metric if len(best_trials.index) > 1 else "", "best_value")
-            )
-            if not skip_fit_evaluation:
-                dirs_to_evaluate.append(
-                    os.path.join(results_dir, metric if len(best_trials.index) > 1 else "", "best_fit")
-                )
-
         crossval_model_info, crossval_input_data = OPTIMA.core.training.perform_crossvalidation(
-            model_configs_to_evaluate,
-            dirs_to_evaluate,
+            crossval_model_configs_to_evaluate,
+            crossval_dirs_to_evaluate,
             training_func,
             run_config,
             input_handler,
             cpus_per_model,
             gpus_per_model,
             custom_metrics,
             composite_metrics,
             native_metrics,
             weighted_native_metrics,
-            PBT=PBT,
-            PBT_replay_getter=PBT_replay_getter,
             seed=seed,
         )
 
     print(
         "\nResults:\n"
         + optimization_str
         + "\n"
```

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/inputs.py` & `optima_ml-0.3.4a1/OPTIMA/core/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/model.py` & `optima_ml-0.3.4a1/OPTIMA/core/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # -*- coding: utf-8 -*-
 """A module that provides abstract functionality to interact with models from different libraries."""
 from types import ModuleType
 from typing import Any, Optional, Union
 
+import sys
+
+if sys.platform == "darwin":
+    import multiprocess as mp
+else:
+    import multiprocessing as mp
+
 import numpy as np
 
 import importlib.util
 
 if importlib.util.find_spec("tensorflow") is not None:
     import tensorflow as tf
 
@@ -234,7 +241,66 @@
             devices="auto",
             accelerator="auto",
             enable_progress_bar=False,
             logger=False,  # we don't need logging here
             enable_checkpointing=False,  # also disable checkpointing
         )
         return pl_trainer
+
+
+def is_model(run_config: ModuleType, path: str) -> bool:
+    """Helper function that checks if a path corresponds to a model file.
+
+    The file ending is automatically appended based on the machine learning framework used, i.e. ``'.keras'`` for `Keras`
+    and ``'.ckpt'`` for `Lightning`.
+
+    Parameters
+    ----------
+    run_config : ModuleType
+        Reference to the imported `run-config`-file.
+    path : str
+        Path to the suspected model file.
+
+    Returns
+    -------
+    bool
+        ``True`` if the provided path corresponds to a valid model file, ``False`` otherwise.
+    """
+    # add the file ending
+    if run_config.model_type == "Keras":
+        if path[-6:] != ".keras":
+            path += ".keras"
+    elif run_config.model_type == "Lightning":
+        if path[-5:] != ".ckpt":
+            path += ".ckpt"
+
+    # try to load the model
+    def _check_model_path(run_config: ModuleType, path: str, mp_queue: mp.Queue) -> None:
+        """Helper function that calls the ``load_model`` function.
+
+        It is expected to be executed in a subprocess. The communication to the parent process is done using the provided
+        queue. A queue value of ``True`` indicates the loading was successful, a value of ``False`` indicates the loading
+        failed.
+
+        Parameters
+        ----------
+        run_config : ModuleType
+            Reference to the imported `run-config`-file.
+        path : str
+            Path to the suspected model file.
+        mp_queue : mp.Queue
+            Multiprocessing queue for the communication to the parent process.
+        """
+        try:
+            load_model(run_config, path, cpus=1)
+            mp_queue.put(True)
+        except BaseException:  # noqa: B036
+            # something happened during loading, assume it's not a valid model file
+            mp_queue.put(False)
+
+    # start the subprocess and try to load the model
+    queue = mp.Queue()
+    p = mp.Process(target=_check_model_path, args=(run_config, path, queue))
+    p.daemon = True
+    p.start()
+    success = queue.get()
+    return success
```

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/search_space.py` & `optima_ml-0.3.4a1/OPTIMA/core/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/tools.py` & `optima_ml-0.3.4a1/OPTIMA/core/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/training.py` & `optima_ml-0.3.4a1/OPTIMA/core/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """A module that provides general functionality for the training and crossvalidation."""
-import glob
 import logging
 import os
+import json
 import pickle
 import shutil
 import sys
 import time
 from functools import partial
 
 if sys.platform == "darwin":
@@ -69,14 +69,15 @@
         targets_train: Optional[Any] = None,
         weights_train: Optional[Any] = None,
         inputs_val: Optional[Any] = None,
         targets_val: Optional[Any] = None,
         weights_val: Optional[Any] = None,
         restore_best_weights: bool = False,
         create_checkpoints: bool = True,
+        checkpoint_dir: Optional[str] = None,
         first_checkpoint_epoch: int = 1,
         checkpoint_frequency: int = 1,
         report_event: Optional[Event] = None,
         report_queue: Optional[Queue] = None,
         report_queue_read_event: Optional[Event] = None,
         termination_event: Optional[Event] = None,
         in_tune_session: bool = True,
@@ -136,14 +137,17 @@
             Data structure containing the event weights of the validation dataset. (Default value = None)
         restore_best_weights : bool
             Whether to restore model weights from the epoch with the best value of the target metric. If ``False``, the
             model weights obtained at the last step of training are used. (Default value = False)
         create_checkpoints : bool
             Whether to save a checkpoint of the current and best model and the state of the early stopper at the end of
             each epoch. (Default value = True)
+        checkpoint_dir : Optional[str]
+            An optional path to the directory the model checkpoints should be saved to. If ``None``, a new directory
+            ``'checkpoint_dir'`` is created in the current working directory. (Default value = None)
         first_checkpoint_epoch : int
             The first epoch after which a checkpoint should be saved. (Default value = 1)
         checkpoint_frequency : int
             Controls how often a checkpoint of the model weights and the early stopper state are saved. If the current
             epoch number (when starting to count from 1) minus the ``first_checkpoint_epoch`` is divisible by
             ``checkpoint_frequency``, a checkpoint is created. (Default value = 1)
         report_event : Optional[Event]
@@ -191,14 +195,15 @@
         self.min_delta = min_delta
         self.patience_improvement = patience_improvement
         self.patience_overfitting = patience_overfitting
         self.overfitting_conditions = overfitting_conditions
 
         # various other settings
         self.create_checkpoints = create_checkpoints
+        self.checkpoint_dir = checkpoint_dir if checkpoint_dir is not None else "checkpoint_dir"
         self.first_checkpoint_epoch = first_checkpoint_epoch
         self.checkpoint_frequency = checkpoint_frequency
         self.restore_best_weights = restore_best_weights
         self.verbose = verbose
 
         # status variables to keep track of the current status of the optimization
         self.current_epoch = 0
@@ -280,15 +285,15 @@
           ``self.report_event``, this function waits for up to 600 seconds for the ``self.report_queue_read_event`` to
           be triggered, which is used to signify that the results have been successfully reported to `Tune`. After 120
           seconds of waiting, the status of the parent process is checked in a one-second interval. If the parent process
           is not alive anymore, this process self-terminates. After 600 seconds of waiting, the self-termination is also
           triggered even if the parent process is still alive. Once the ``self.report_queue_read_event`` is triggered,
           it is cleared and the function returns.
         - ``self.report_directly`` is ``True``: Multiprocessing events and queues were not provided, thus a checkpoint is
-          built from the ``'checkpoint_dir'`` directory and the results dictionary and the checkpoint are reported
+          built from the ``self.checkpoint_dir`` directory and the results dictionary and the checkpoint are reported
           directly to `Tune`.
 
         Parameters
         ----------
         epoch : int
             The number of epochs since the start of the training.
         logs : Optional[dict]
@@ -318,23 +323,23 @@
         # the early stopper state is dumped there
         if (
             self.create_checkpoints
             and epoch + 1 >= self.first_checkpoint_epoch
             and (epoch + 1 - self.first_checkpoint_epoch) % self.checkpoint_frequency == 0
         ):
             # save current model
-            os.makedirs("checkpoint_dir", exist_ok=True)
-            self.save_model(output_dir="checkpoint_dir", model_name="model", **kwargs)
+            os.makedirs(self.checkpoint_dir, exist_ok=True)
+            self.save_model(output_dir=self.checkpoint_dir, model_name="model", **kwargs)
 
             # save model again as best model if there was an improvement; TODO: replace this with a copy?
             if is_improvement or epoch + 1 == self.first_checkpoint_epoch:
-                self.save_model(output_dir="checkpoint_dir", model_name="best_model", **kwargs)
+                self.save_model(output_dir=self.checkpoint_dir, model_name="best_model", **kwargs)
 
             # save early stopper state
-            self.save_state(path=os.path.join("checkpoint_dir", "early_stopper"), **kwargs)
+            self.save_state(path=os.path.join(self.checkpoint_dir, "early_stopper"), **kwargs)
 
         # report to Tune if we are in a Tune session
         if self.in_tune_session:
             (
                 current_metrics,
                 current_weighted_metrics,
                 current_custom,
@@ -353,15 +358,15 @@
             if self.report_directly:
                 time_before_report = time.time()
                 if (
                     self.create_checkpoints
                     and epoch + 1 >= self.first_checkpoint_epoch
                     and (epoch + 1 - self.first_checkpoint_epoch) % self.checkpoint_frequency == 0
                 ):
-                    checkpoint = train.Checkpoint.from_directory("checkpoint_dir")
+                    checkpoint = train.Checkpoint.from_directory(self.checkpoint_dir)
                     train.report(results, checkpoint=checkpoint)
                 else:
                     train.report(results)
                 if time.time() - time_before_report > 2:
                     logging.warning(
                         "Reporting results took {} seconds, which may be a performance bottleneck.".format(
                             time.time() - time_before_report
@@ -750,15 +755,15 @@
         if self.wait >= self.patience_improvement and self.verbose > 0:
             print("Epoch {}: Early stopping...".format(self.stopped_epoch + 1))
         elif self.wait_overfitting >= self.patience_overfitting and self.verbose > 0:
             print("Epoch {}: Early stopping due to overfitting...".format(self.stopped_epoch + 1))
 
     state_type = tuple[int, int, int, Union[float, int], dict, dict, dict, dict, Any, int, int, bool, Union[float, int]]
 
-    def _get_state(self, **kwargs: dict) -> state_type:
+    def get_state(self, **kwargs: dict) -> state_type:
         """Returns the values of all attributes needed to restore the state of the early stopper.
 
         This includes the number of epochs since the last improvement (``self.wait``), the number of epochs since the last
         time no `overfitting condition` was violated (``self.wait_overfitting``), the best target metric value seen
         (``self.best``), the dictionaries containing the values of the `native`, `weighted native`, `custom` and
         `composite metrics` after the best epoch (``self.best_metrics``, ``self.best_weighted_metrics``,
         ``self.best_custom_metrics`` and ``self.best_composite_metrics``), the model weights after the best epoch
@@ -789,15 +794,15 @@
             self.best_weights,
             self.best_epoch,
             self.stopped_epoch,
             self.early_stopped,
             self.last_valid,
         )
 
-    def _set_state(self, state: state_type, **kwargs: dict) -> None:
+    def set_state(self, state: state_type, **kwargs: dict) -> None:
         """Restores the state of the early stopper.
 
         Parameters
         ----------
         state : state_type
             Early stopper state to restore from.
         **kwargs : dict
@@ -828,46 +833,49 @@
         checkpoint_dir : str
             Directory to load from.
         **kwargs : dict
             Additional keyword arguments that may be necessary for ML framework specific functionality, e.g. saving the
             model. They are provided to any call of a member function.
         """
         with open(os.path.join(checkpoint_dir, "early_stopper"), "rb") as f:
-            self._set_state(pickle.load(f), **kwargs)
+            self.set_state(pickle.load(f), **kwargs)
 
     def save_state(self, path: str, **kwargs: dict) -> None:
         """Saves the early stopper state to the provided path.
 
         Parameters
         ----------
         path : str
             Path to save the pickle-file to.
         **kwargs : dict
             Additional keyword arguments that may be necessary for ML framework specific functionality, e.g. saving the
             model. They are provided to any call of a member function.
         """
         with open(path, "wb") as f:
-            pickle.dump(self._get_state(**kwargs), f)
+            pickle.dump(self.get_state(**kwargs), f)
 
     def copy_best_model(self, path: str, **kwargs: dict) -> None:
-        """Copies the best model from the provided path to a checkpoint_dir folder in the current working directory.
+        """Copies the best model from the provided path to the ``self.checkpoint_dir`` directory.
 
         This is needed whenever the training is resumed from a checkpoint in order to copy the best model in the checkpoint
         to the working directory.
 
         Parameters
         ----------
         path : str
             Path of the best model in the checkpoint.
         **kwargs : dict
             Additional keyword arguments that may be necessary for ML framework specific functionality, e.g. saving the
             model. They are provided to any call of a member function.
         """
-        os.makedirs("checkpoint_dir", exist_ok=True)
-        shutil.copy2(path, "checkpoint_dir")
+        os.makedirs(self.checkpoint_dir, exist_ok=True)
+        try:
+            shutil.copy2(path, self.checkpoint_dir)
+        except shutil.SameFileError:
+            pass
 
     @abstractmethod
     def get_train_val_metric_names(self, metric: str, **kwargs: dict) -> tuple[str, str]:
         """Returns the training and validation metric name to be used as the key in the ``logs`` dictionary.
 
         Parameters
         ----------
@@ -998,14 +1006,157 @@
         Literal[False]
             Will currently always return ``False``.
         """
         # currently will always be false
         return self.should_stop
 
 
+class PBTMutationHandler:
+    """_summary_.
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+
+    def __init__(self) -> None:
+        """_summary_.
+
+        Returns
+        -------
+        None
+            _description_
+        """
+        self._policies = None
+
+    def load_experiment_state(self, experiment_dir: str) -> None:
+        """_summary_.
+
+        Parameters
+        ----------
+        experiment_dir : str
+            _description_
+
+        Returns
+        -------
+        None
+            _description_
+        """
+        # collect the policies of all trials at the end of the optimization. This does not include any cut-off branches
+        # where under-performing trials were overwritten during the optimization. These can be taken from the
+        # pbt_global.txt file and will be handled in the future.
+        # TODO: handle overwritten trials
+        self._policies = {}
+        for file in os.listdir(experiment_dir):
+            if "pbt_policy_" in file:
+                # strip the file name to get the trial
+                trial = file.replace("pbt_policy_", "").replace(".txt", "")
+
+                # extract the policy
+                policy = self._load_policy(os.path.join(experiment_dir, file))
+
+                # add the policy to the policies dict
+                self._policies[trial] = policy
+
+    def get_policy(self, trial: str) -> Optional[list[tuple[int, dict]]]:
+        """_summary_.
+
+        Parameters
+        ----------
+        trial : str
+            _description_
+
+        Returns
+        -------
+        Optional[list[tuple[int, dict]]]
+            _description_
+        """
+        if self._policies is None:
+            raise RuntimeWarning(
+                "PBTMutation handler has not yet been initialized by loading an experiment via "
+                "`load_experiment_state()` or loading a save state via `load()`."
+            )
+        return self._policies.get(trial)
+
+    def save(self, savefile: str) -> None:
+        """_summary_.
+
+        Parameters
+        ----------
+        savefile : str
+            _description_
+
+        Returns
+        -------
+        None
+            _description_
+        """
+        with open(savefile, "wb") as f:
+            pickle.dump(self._policies, f)
+
+    def load(self, savefile: str) -> None:
+        """_summary_.
+
+        Parameters
+        ----------
+        savefile : str
+            _description_
+
+        Returns
+        -------
+        None
+            _description_
+        """
+        with open(savefile, "rb") as f:
+            self._policies = pickle.load(f)
+
+    def _load_policy(self, policy_file: str) -> list[tuple[int, dict]]:
+        """_summary_.
+
+        Parameters
+        ----------
+        policy_file : str
+            _description_
+
+        Returns
+        -------
+        list[tuple[int, dict]]
+            _description_
+        """
+        raw_policy = []
+        with open(policy_file, "rt") as fp:
+            for row in fp.readlines():
+                try:
+                    parsed_row = json.loads(row)
+                except json.JSONDecodeError:
+                    raise ValueError("Could not read PBT policy file: {}.".format(policy_file)) from None
+                raw_policy.append(tuple(parsed_row))
+
+        # Loop through policy from end to start to obtain changepoints
+        policy = []
+        last_new_tag = None
+        last_old_conf = None
+        for old_tag, new_tag, _old_step, new_step, old_conf, new_conf in reversed(raw_policy):
+            if last_new_tag and old_tag != last_new_tag:
+                # Tag chain ended. This means that previous changes were
+                # overwritten by the last change and should be ignored.
+                break
+            last_new_tag = new_tag
+            last_old_conf = old_conf
+
+            policy.append((new_step, new_conf))
+
+        # Add the initial config to the policy
+        policy.append((0, last_old_conf))
+
+        # return the reversed list
+        return list(reversed(policy))
+
+
 def build_trainable(
     run_config: ModuleType,
     training_func: Callable,
     input_handler: OPTIMA.builtin.inputs.InputHandler,
     inputs_train: Union[np.ndarray, ray.ObjectRef],
     inputs_val: Union[np.ndarray, ray.ObjectRef],
     targets_train: Union[np.ndarray, ray.ObjectRef],
@@ -1160,90 +1311,64 @@
     cpus_per_model: int,
     gpus_per_model: int,
     custom_metrics: Optional[list[tuple[str, Callable]]] = None,
     composite_metrics: Optional[list[tuple[str, tuple[str, str], Callable]]] = None,
     native_metrics: Optional[list] = None,
     weighted_native_metrics: Optional[list] = None,
     return_futures: bool = False,
-    PBT: bool = False,
-    PBT_replay_getter: Optional[Callable] = None,
     verbose: int = 2,
     seed: Optional[int] = None,
 ) -> Union[tuple[dict, dict], tuple[dict, dict, list]]:
     """Performs k-fold crossvalidation for a given list of model-configs.
 
     The ``get_experiment_inputs``-function (either defined in the run-config or the built-in version ``OptimizationTools``) is
     called to load the input data for crossvalidation.
 
     For each fold, the trainable is build by calling ``build_trainable`` in order to save the datasets to Ray's shared
     memory (if needed) and to set constant arguments of the ``training_func``. The following choices are made:
 
     - ``run_config``: the provided ``run_config`` is passed.
-    - ``training_func``: unless ``PBT`` is ``True``, the provided ``training_func`` is wrapped with a
-      ``ray.remote``-decorator, setting ``num_cpus`` to ``cpus_per_model`` and ``num_gpus`` to ``gpus_per_model``, to
-      allow remote execution of the trainable. The ``training_func`` needs to be decorated first before calling
-      ``build_trainable`` as ``ray.remote`` does not accept ``functools.partial``. Since for Population Based Training,
-      a ``PopulationBasedTrainingReplay``-scheduler is used, the trainable must not be decorated for the PBT step.
+    - ``training_func``: the provided ``training_func`` is wrapped with a ``ray.remote``-decorator, setting ``num_cpus``
+      to ``cpus_per_model`` and ``num_gpus`` to ``gpus_per_model``, to allow remote execution of the trainable. The
+      ``training_func`` needs to be decorated first before calling ``build_trainable`` as ``ray.remote`` does not accept
+      ``functools.partial``.
     - ``inputs_train``, ``inputs_val``, ``targets_train``, ``targets_val``, ``normalized_weights_train`` and
       ``normalized_weights_val``: the corresponding arrays for each fold returned by ``get_experiment_inputs`` are passed.
     - ``overtraining_conditions``: default (``None``) if ``run_config.use_OT_conditions_for_crossvalidation`` is ``True``,
       ``[]`` otherwise. This disables the overfitting conditions during crossvalidation if necessary.
     - ``early_stopping_patience``: default (``None``) if ``run_config.use_early_stopping_for_crossvalidation`` is ``True``,
       ``run_config.max_epochs`` otherwise. This (effectively) disables early stopping during crossvalidation if necessary
       while still using the remaining functionality of the ``EarlyStopperForTuning``.
     - ``num_threads``: ``cpus_per_model`` is passed.
-    - ``create_checkpoints``: ``PBT`` is passed. Since the ``PopulationBasedTrainingReplay``-scheduler forcefully
-      terminates the training once done, the fitting function never returns and thus the final model cannot be saved.
-      Instead, the checkpointing is used so that the final checkpoint can be used instead.
+    - ``create_checkpoints``: ``True``.
     - ``custom_metrics``, ``composite_metrics``, ``native_metrics`` and ``weighted_native_metrics``: the corresponding
       arguments of this function are passed.
-    - ``restore_best_weights``: ``True``. For all but the PBT step, the EarlyStopper must restore the best weights if
-      the training is early stopped before saving the model. Since the model weights are not restored if the early
-      stopping is not invoked (i.e. the training terminated for a different reason), a value of ``True`` can also be
-      used for the other cases.
+    - ``restore_best_weights``: ``True``. Since the best weights are only restored if the training is early stopped,
+      this option can always be set to ``True``.
     - ``run_in_subprocess``: ``True``. This is done to ensure all resources reserved by Tensorflow are released when
       training terminates.
     - ``verbose``: ``verbose`` is passed.
 
     With the trainable and the datasets for all `k` folds ready, the training of the `k` models per provided model-config
     is started. While the number of epochs that were found to result in the best target metric by the
     ``evaluate_experiment`` is included in the ``model_config`` with the key ``'epochs'``, this is only used if
     ``run_config.use_early_stopping_for_crossvalidation`` is ``False``, in which case ``model_config["max_epochs"]``
     is overwritten with ``model_config["epochs"]``. For the model corresponding to the `i`-th fold, the output file name
     is set to `model_crossval_i` and path given in ``model_output_dirs[i]`` is used as the output directory. For each
     model, the presence of a `.crossvalidation_done`-file or a file with the target output name is checked. If any of the
-    two files is present, the training for this model is skipped. The training procedure is different for the first two
-    steps and the PBT step and is distinguished by the value of ``PBT``:
-
-    - ``PBT`` is ``False``: the target output path is added to the model-config with key ``'final_model_path'``. The
-      trainable is subsequently called, provided with the model-config, and the returned future (due to the remote
-      execution) is saved to a list.
-    - ``PBT`` is ``True``: the ``PBT_replay_getter`` is called to get the ``tune.Tuner``-instance to perform the replay
-      of the PBT-run. It is provided with:
-
-        - ``trial_id``: the trial-id corresponding to the current model (``model_config["trial_id"]``)
-        - ``trainable``: the ``trainable``
-        - ``max_epochs``: if ``run_config.use_early_stopping_for_crossvalidation`` is ``True``, `-1` is passed to
-          signify that early stopping should be used. Otherwise, ``model_config["max_epochs"]`` is passed and the trial
-          is expected to be terminated after ``model_config["max_epochs"]`` epochs.
-      The ``fit``-function of the returned Tuner is called to replay the PBT-run. Since this is not executed remotely,
-      this is blocking until the training is terminated. Once done, the final checkpoint is copied to the target output
-      path.
-
-      In case a `ValueError` is raised at any point, which happens if no policy-file was found for the trial-id provided
-      to the ``PBT_replay_getter``, a warning message is printed and the training falls back to the same simple training
-      as in the ``PBT == False``-case, including the remote execution. In this case, the training performed during the
-      crossvalidation is still equivalent to the training during the optimization, since the policy-file is only missing
-      if no perturbations were done, i.e. the hyperparameters were kept unchanged.
+    two files is present, the training for this model is skipped. The target output path is added to the model-config
+    with key ``'final_model_path'``. The trainable is subsequently called, provided with the model-config, and the
+    returned future (due to the remote execution) is saved to a list.
 
     If ``return_futures`` is ``False``, the function only returns once all trainings are terminated. To mark the
-    crossvalidation as completed, a `.crossvalidation_done` file is created on each of the directories in
-    ``model_output_dirs``. This allows the crossvalidation to be resumed if interruped at any point, any only the
-    progress of not fully trained models is lost. If ``return_futures`` is ``True``, the list of ``futures`` is returned
-    instead and the function does not block.
+    crossvalidation as completed, a `.crossvalidation_done` file is created in each of the directories in
+    ``model_output_dirs`` and the temporary directory ``'crossval_checkpoints'``containing the training checkpoints is
+    removed. This allows the crossvalidation to be resumed if interruped at any point, and only the progress since the
+    last model checkpoint is lost. If ``return_futures`` is ``True``, the list of ``futures`` is returned instead and
+    the function does not block. The temporary checkpoint directory is subsequently not removed.
 
     Parameters
     ----------
     model_configs : list[model_config_type]
         A list of model configs for which crossvalidation should be performed.
     model_output_dirs : list[str]
         A list of paths to directories, one entry per config in ``model_configs``, to save the trained models in.
@@ -1264,20 +1389,14 @@
     native_metrics : Optional[list]
         A list of native metrics as defined in the run-config. (Default value = None)
     weighted_native_metrics : Optional[list]
         A list of weighted native metrics as defined in the run-config. (Default value = None)
     return_futures : bool
         If True, the list of futures given by `Ray` is returned instead of waiting for the workers to finish.
         (Default value = False)
-    PBT : bool
-        Used to signify if this is the Population Based Training step which requires a different training procedure.
-        (Default value = False)
-    PBT_replay_getter : Optional[Callable]
-        Callable used to get the ``Tune.Tuner``-instance with the ``PopulationBasedTrainingReplay``-scheduler. Only used
-        if ``PBT`` is ``True``. (Default value = None)
     verbose : int
         Verbosity mode. 0 = silent, 1 = info messages and progress bar for training, 2 = info messages and one line per
         epoch. Note that the progress bar is not particularly useful when logged to a file, so verbose=2 is recommended
         when not running interactively (e.g., in a production environment). (Default value = 2)
     seed : Optional[int]
         If provided, the seed is used to set the numpy random state. Only used to generate a new seed for the model
         config if the original seed should not be reused. (Default value = None)
@@ -1316,19 +1435,16 @@
     (
         inputs_split,
         targets_split,
         weights_split,
         normalized_weights_split,
     ) = get_experiment_inputs(run_config, input_handler, inputs_for_crossvalidation=True, disable_printing=verbose == 0)
 
-    if not PBT:
-        # simulate a @ray.remote() decorator on the training function
-        training_func_remote = ray.remote(num_cpus=cpus_per_model, num_gpus=gpus_per_model)(training_func).remote
-    else:
-        training_func_remote = training_func
+    # simulate a @ray.remote() decorator on the training function
+    training_func_remote = ray.remote(num_cpus=cpus_per_model, num_gpus=gpus_per_model)(training_func).remote
 
     # iterate over all input data splits, build the corresponding trainables, and add them to the list
     trainables_list = []
     crossval_input_data = (
         {}
     )  # save the split data and return it together with the names of the trained models for later evaluation
     for k, data_k in enumerate(zip(*inputs_split, *targets_split, *weights_split, *normalized_weights_split)):
@@ -1380,15 +1496,15 @@
                 inputs_train_k,
                 inputs_val_k,
                 targets_train_k,
                 targets_val_k,
                 normalized_weights_train_k,
                 normalized_weights_val_k,
                 num_threads=cpus_per_model,
-                create_checkpoints=PBT,
+                create_checkpoints=True,
                 custom_metrics=custom_metrics,
                 composite_metrics=composite_metrics,
                 native_metrics=native_metrics,
                 weighted_native_metrics=weighted_native_metrics,
                 early_stopping_patience=None
                 if run_config.use_early_stopping_for_crossvalidation
                 else run_config.max_epochs,  # effectively disables early stopping while keeping the custom metric and reporting functionality
@@ -1444,90 +1560,32 @@
                     {"name": output_name, "split": str(k), "config": model_config_k}
                 ]
             else:
                 crossval_model_info[model_output_dir].append(
                     {"name": output_name, "split": str(k), "config": model_config_k}
                 )
             if not skip_training:
-                if os.path.isfile(output_path):
+                if OPTIMA.core.model.is_model(run_config, output_path):
                     if verbose > 0:
                         print(
                             f"The file {output_path} already exists. Assuming this is a fully trained model, not "
                             f"starting the training for this split..."
                         )
                 else:
-                    if not PBT:
-                        # adding the final model path to the model's config, start the training and add the future to the list
-                        model_config_k["final_model_path"] = output_path
-                        futures.append(trainable(model_config_k))
-                    else:
-                        # # with PBT, we simply take the last checkpoint
-                        # futures.append(_pbt_replay.remote(trainable, model_config_k, final_model_path=output_path, max_epochs=max_epochs))
-                        # currently, when running the tuning in a ray task, the evaluation shows (near) perfect agreement between
-                        # training and validation, indicating that the splits are somehow mixed up. When running them
-                        # sequentially, this does not happen. This is possibly due to the problem discussed in
-                        # https://github.com/ray-project/ray/issues/30091, i.e. the trainable would need to be renamed
-                        # for each instance, otherwise Tune mixes up the parameters. TODO: fix this!
-                        try:
-                            tuner = PBT_replay_getter(
-                                model_config_k["trial_id"],
-                                trainable,
-                                max_epochs=-1 if run_config.use_early_stopping_for_crossvalidation else target_epochs,
-                                name=output_path.replace("/", "_"),
-                            )
-                            results_grid = tuner.fit()
-                            analysis = results_grid._experiment_analysis
-                            with analysis.best_checkpoint.as_directory() as checkpoint_path:
-                                # we don't know the extension of the saved model file here, so we look at all files
-                                # with the correct name and grab it. If more than one fits, raise an error.
-                                model_paths = glob.glob(os.path.join(checkpoint_path, "model.*"))
-                                if len(model_paths) > 1:
-                                    raise RuntimeError(f"More than 1 model.* file in {checkpoint_path}!")
-                                extension = os.path.basename(model_paths[0]).split(".")[
-                                    -1
-                                ]  # take filename, split at ".", and take the last
-                                shutil.copy2(model_paths[0], f"{output_path}.{extension}")
-                        except ValueError:
-                            # when the policy file for this trial does not exist (which means no perturbations were done),
-                            # PBT_replay_getter will raise a ValueError. We can simply train manually without the PBT
-                            # scheduler in that case, but need to wrap the trainable in a dummy function because the
-                            # ray.remote decorator can only be used for functions, not partials
-                            @ray.remote(num_cpus=cpus_per_model, num_gpus=gpus_per_model)
-                            def _execute_trainable(trainable: Callable, model_config_k: model_config_type) -> None:
-                                """Small helper function to remotely execute the ``trainable``.
-
-                                Since for ``PBT == True``, the ``training_func`` is not wrapped in a ``ray.remote``
-                                decorator, the ``trainable`` is a ``functools.partial`` at this point. Since these
-                                cannot be wrapped by a ``ray.remote`` decorator anymore, we need to use a dummy function
-                                for that sole purpose.
-
-                                Provided with the ``trainable`` and the model-config, this function simply calls the
-                                ``trainable``. Since this is now a function, it can be decorated again.
-
-                                Parameters
-                                ----------
-                                trainable : Callable
-                                    The trainable to be executed remotely.
-                                model_config_k : model_config_type
-                                    The model-config to be provided to the ``trainable``.
-                                """
-                                trainable(model_config_k)
-
-                            print(
-                                f"Policy file for trial {model_config_k['trial_id']} could not be found, training without"
-                                f" perturbations!"
-                            )
-                            # adding the final model path to the model's config, start the training and add the future to the list
-                            model_config_k["final_model_path"] = output_path
-                            futures.append(_execute_trainable.remote(trainable, model_config_k))
+                    # adding the checkpoint directory and the final model path to the model's config, start the training
+                    # and add the future to the list
+                    model_config_k["checkpoint_dir"] = os.path.join(model_output_dir, "crossval_checkpoints", str(k))
+                    model_config_k["final_model_path"] = output_path
+                    futures.append(trainable(model_config_k))
 
     # this will block until all models are fully trained
     if return_futures:
         return crossval_model_info, crossval_input_data, futures
     else:
         ray.get(futures)
 
-        # when crossvalidation is done, create all the .crossvalidation_done files
+        # when crossvalidation is done, create all the .crossvalidation_done files and remove the temporary checkpoint directory
         for model_output_dir in model_output_dirs:
             open(os.path.join(model_output_dir, ".crossvalidation_done"), "w").close()
+            shutil.rmtree(os.path.join(model_output_dir, "crossval_checkpoints"), ignore_errors=True)
 
         return crossval_model_info, crossval_input_data
```

### Comparing `optima_ml-0.3.3a3/OPTIMA/core/variable_optimization.py` & `optima_ml-0.3.4a1/OPTIMA/core/variable_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,17 @@
                     continue
 
                 # when training for this iteration of this var set is done (otherwise we can't get here), mark the
                 # folder as done so that it could be resumed should the optimization be killed and remove the var
                 # from the list
                 open(os.path.join(crossval_model_path, ".crossvalidation_done"), "w").close()
 
+                # the model checkpoints are also no longer needed, so delete those as well
+                shutil.rmtree(os.path.join(crossval_model_path, "crossval_checkpoints"), ignore_errors=True)
+
             # this is only True if all iterations of this var set are finished
             if var_set_done:
                 var_sets_not_finished.remove(var_set_key)
 
     print("\tAll models trained, starting evaluation...")
 
     # once training is done, iterate over all var sets again to perform the evaluation of the trained models
```

### Comparing `optima_ml-0.3.3a3/OPTIMA/defaults.py` & `optima_ml-0.3.4a1/OPTIMA/defaults.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/hardware_configs/Dresden_Taurus.py` & `optima_ml-0.3.4a1/OPTIMA/hardware_configs/Dresden_Taurus.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/hardware_configs/common.py` & `optima_ml-0.3.4a1/OPTIMA/hardware_configs/common.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/helpers/extract_data_from_NTuples.py` & `optima_ml-0.3.4a1/OPTIMA/helpers/extract_data_from_NTuples.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/helpers/manage_ray_nodes.py` & `optima_ml-0.3.4a1/OPTIMA/helpers/manage_ray_nodes.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/keras/model.py` & `optima_ml-0.3.4a1/OPTIMA/keras/model.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/keras/tools.py` & `optima_ml-0.3.4a1/OPTIMA/keras/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/keras/training.py` & `optima_ml-0.3.4a1/OPTIMA/keras/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/lightning/inputs.py` & `optima_ml-0.3.4a1/OPTIMA/lightning/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/lightning/training.py` & `optima_ml-0.3.4a1/OPTIMA/lightning/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/optima.py` & `optima_ml-0.3.4a1/OPTIMA/optima.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main steering script of OPTIMA."""
 
 __author__ = "E. Bachmann"
 __licence__ = "GPL3"
-__version__ = "0.3.3alpha3"
+__version__ = "0.3.4alpha1"
 __maintainer__ = "E. Bachmann"
 
 import os
 import sys
 import shutil
 import logging
 import argparse
@@ -59,57 +59,351 @@
     import OPTIMA.lightning.inputs
     import OPTIMA.lightning.training
 
 from OPTIMA.hardware_configs.helpers import get_cluster, get_suitable_job
 from OPTIMA.resources.pbt_with_seed import PopulationBasedTraining
 
 
-def train_model(model_config, run_config, input_handler, inputs_train, inputs_val, targets_train, targets_val,
-                normalized_weights_train, normalized_weights_val, monitor=('val_loss', 'min'),
-                custom_metrics=[], composite_metrics=[], native_metrics=[], weighted_native_metrics=[],
-                overtraining_conditions=[], early_stopping_patience=0, overtraining_patience=0, restore_best_weights=False,
-                restore_on_best_checkpoint=False, num_threads=1, create_checkpoints=True, run_in_subprocess=True,
-                verbose=2):
-    def _train_model(checkpoint_com, report_com, termination_event, start_time,
-                     model_config, run_config, input_handler, inputs_train, inputs_val, targets_train, targets_val,
-                     normalized_weights_train, normalized_weights_val, monitor,
-                     custom_metrics, composite_metrics, native_metrics, weighted_native_metrics,
-                     overtraining_conditions, early_stopping_patience, overtraining_patience, restore_best_weights,
-                     restore_on_best_checkpoint, num_threads, create_checkpoints, in_tune_session, runs_in_subprocess,
-                     verbose):
-        # TODO: use abstraction?
+def setup_tensorflow(num_threads):
+    # configure tensorflow to limit its thread usage and its memory usage if a gpu is used
+    from tensorflow import config as tf_config
+    try:
+        # set automatic scaling of the VRAM allocation
+        gpus = tf_config.experimental.list_physical_devices('GPU')
+        for gpu in gpus:
+            tf_config.experimental.set_memory_growth(gpu, True)
+
+        # reduce number of threads
+        tf_config.threading.set_inter_op_parallelism_threads(min(num_threads, 2))
+        tf_config.threading.set_intra_op_parallelism_threads(num_threads)
+    except RuntimeError:
+        pass
+
+
+def set_seeds(run_config, model_config):
+    # fixed global random seeds (if provided) to make training deterministic
+    if model_config.get("seed") is not None:
+        if run_config.model_type == "Keras":
+            import tensorflow as tf
+            max_seeds = OPTIMA.core.tools.get_max_seeds()
+            np.random.seed(model_config["seed"])
+            python_random.seed(np.random.randint(*max_seeds))
+            tf.keras.utils.set_random_seed(np.random.randint(*max_seeds))
+            tf.random.set_seed(np.random.randint(*max_seeds))
+        elif run_config.model_type == "Lightning":
+            import lightning.pytorch as pl
+            pl.seed_everything(model_config["seed"], workers=True)
+
+
+def compile_metrics(run_config, native_metrics, weighted_native_metrics):
+    # compile the metrics (needs to be done here (and not earlier) because tensorflow must not be initialized before setting inter- and intra-op threads)
+    if run_config.model_type == "Keras":
+        compiled_metrics = [metric(name=name, **metric_kwargs) for name, (metric, metric_kwargs) in
+                            native_metrics]
+        compiled_weighted_metrics = [metric(name=name, **metric_kwargs) for name, (metric, metric_kwargs) in
+                                     weighted_native_metrics]
+    elif run_config.model_type == "Lightning":
+        compiled_metrics = [(f"{prefix}_{name}", metric(**metric_kwargs)) for name, (metric, metric_kwargs) in
+                            native_metrics for prefix in ["train", "val"]]
+        compiled_weighted_metrics = [(f"{prefix}_{name}", metric(**metric_kwargs)) for
+                                     name, (metric, metric_kwargs) in
+                                     weighted_native_metrics for prefix in ["train", "val"]]
+    return compiled_metrics, compiled_weighted_metrics
+
+
+def limit_hyperparameters(run_config, model_config):
+    # limit all hyperparameters properly; since only non-conditional hyperparameters can go out of bounds (PBT does
+    # not support conditional hps), we don't need to do any deserialization
+    for hp, hp_search_space in run_config.search_space.items():
+        if isinstance(hp_search_space, dict) and "bounds" in hp_search_space.keys() and hp in model_config.keys():
+            bounds = hp_search_space["bounds"]
+            if (isinstance(bounds[0], int) or isinstance(bounds[0], float)) and model_config[hp] < bounds[0]:
+                model_config[hp] = bounds[0]
+            elif (isinstance(bounds[1], int) or isinstance(bounds[1], float)) and model_config[hp] > bounds[1]:
+                model_config[hp] = bounds[1]
+    return model_config
+
+
+def prepare_data(
+    run_config,
+    input_handler,
+    model_config,
+    inputs_train,
+    targets_train,
+    normalized_weights_train,
+    inputs_val,
+    targets_val,
+    normalized_weights_val
+):
+    # convert the training, validation and testing data to tensorflow datasets or lightning dataloaders
+    if run_config.model_type == "Keras":
+        import tensorflow as tf
+        train_data = tf.data.Dataset.from_tensor_slices((inputs_train, targets_train, normalized_weights_train))
+        val_data = tf.data.Dataset.from_tensor_slices((inputs_val, targets_val, normalized_weights_val))
+
+        # batch the datasets for tensorflow
+        train_data = train_data.batch(model_config["batch_size"])
+        val_data = val_data.batch(model_config["batch_size"])
+        return train_data, val_data
+    elif run_config.model_type == "Lightning":
+        if hasattr(run_config, "DataModule"):
+            DataModule = run_config.DataModule
+        else:
+            DataModule = OPTIMA.lightning.inputs.DefaultDataModule
+        pl_data_module = DataModule(
+            input_handler=input_handler,
+            inputs_train=inputs_train,
+            targets_train=targets_train,
+            weights_train=normalized_weights_train,
+            inputs_val=inputs_val,
+            targets_val=targets_val,
+            weights_val=normalized_weights_val,
+            run_config=run_config,
+            model_config=model_config
+        )
+        return pl_data_module
+
+
+def update_model(run_config, model, model_config, input_handler, inputs_train, targets_train):
+    if hasattr(run_config, 'update_model'):
+        model = run_config.update_model(
+            model,
+            model_config,
+            input_handler=input_handler,
+            inputs_train=inputs_train,
+            targets_train=targets_train,
+        )
+    else:
+        model = OPTIMA.builtin.model.update_model(
+            model,
+            model_config,
+            input_handler=input_handler,
+            inputs_train=inputs_train,
+            targets_train=targets_train,
+        )
+    return model
+
+def reload_from_checkpoint(
+    run_config,
+    input_handler,
+    model_config,
+    early_stopper,
+    inputs_train,
+    targets_train,
+    checkpoint_dir,
+    restore_on_best_checkpoint
+):
+    if run_config.model_type == "Keras":
+        import tensorflow as tf
+        if not restore_on_best_checkpoint:
+            model = tf.keras.models.load_model(os.path.join(checkpoint_dir, "model.keras"))  # reload the model
+        else:
+            model = tf.keras.models.load_model(
+                os.path.join(checkpoint_dir, "best_model.keras"))  # reload the best model
+
+        # since some hyperparameters may have been changed since the save, we need to update the model
+        model = update_model(run_config, model, model_config, input_handler, inputs_train, targets_train)
+    elif run_config.model_type == "Lightning":
+        # update hyperparameters while loading checkpoint
+        if not restore_on_best_checkpoint:
+            model = run_config.LitModel.load_from_checkpoint(os.path.join(checkpoint_dir, "model.ckpt"),
+                                                             model_config=model_config)
+        else:
+            model = run_config.LitModel.load_from_checkpoint(os.path.join(checkpoint_dir, "best_model.ckpt"),
+                                                             model_config=model_config)
+
+    # load current early stopper state, even when restoring on best model checkpoint
+    early_stopper.load_state(checkpoint_dir)
+    if run_config.model_type == "Keras":
+        early_stopper.copy_best_model(os.path.join(checkpoint_dir, "best_model.keras"))
+    elif run_config.model_type == "Lightning":
+        early_stopper.copy_best_model(os.path.join(checkpoint_dir, "best_model.ckpt"))
+
+    return model, early_stopper
+
+
+def build_model(
+    run_config,
+    model_config,
+    input_handler,
+    inputs_train,
+    targets_train,
+    compiled_metrics,
+    compiled_weighted_metrics
+):
+    if hasattr(run_config, 'build_model') and run_config.model_type == "Keras":
+        model = run_config.build_model(
+            model_config,
+            input_handler=input_handler,
+            inputs_train=inputs_train,
+            targets_train=targets_train,
+        )
+    elif hasattr(run_config, 'LitModel') and run_config.model_type == "Lightning":
+        model = run_config.LitModel(
+            model_config,
+            inputs_train.shape,
+            targets_train.shape,
+            compiled_metrics,
+            compiled_weighted_metrics
+        )
+    else:
         if run_config.model_type == "Keras":
-            # configure tensorflow to limit its thread usage and its memory usage if a gpu is used
-            from tensorflow import config as tf_config
-            try:
-                # set automatic scaling of the VRAM allocation
-                gpus = tf_config.experimental.list_physical_devices('GPU')
-                for gpu in gpus:
-                    tf_config.experimental.set_memory_growth(gpu, True)
-
-                # reduce number of threads
-                tf_config.threading.set_inter_op_parallelism_threads(min(num_threads, 2))
-                tf_config.threading.set_intra_op_parallelism_threads(num_threads)
-            except RuntimeError:
-                pass
+            model = OPTIMA.builtin.model.build_model(
+                model_config,
+                input_handler=input_handler,
+                inputs_train=inputs_train,
+                targets_train=targets_train,
+            )
+        elif run_config.model_type == "Lightning":
+            raise NotImplementedError("Lightning models requires a LitModel-class to be present in the run-config.")
+    return model
+
+
+def compile_model(
+    run_config,
+    model,
+    model_config,
+    compiled_metrics,
+    compiled_weighted_metrics,
+    input_handler,
+    inputs_train,
+    targets_train,
+    first_compile
+):
+    if run_config.model_type == "Keras":
+        if hasattr(run_config, 'compile_model'):
+            model = run_config.compile_model(
+                model,
+                model_config,
+                metrics=compiled_metrics,
+                weighted_metrics=compiled_weighted_metrics,
+                input_handler=input_handler,
+                inputs_train=inputs_train,
+                targets_train=targets_train,
+                first_compile=first_compile
+            )
+        else:
+            model = OPTIMA.builtin.model.compile_model(
+                model,
+                model_config,
+                metrics=compiled_metrics,
+                weighted_metrics=compiled_weighted_metrics,
+                input_handler=input_handler,
+                inputs_train=inputs_train,
+                targets_train=targets_train,
+                first_compile=first_compile
+            )
+    elif run_config.model_type == "Lightning":
+        model.prepare(input_handler, inputs_train, targets_train, first_prepare=first_compile)
+
+    return model
 
+
+def fit_model(run_config, model, early_stopper, data, end_epoch, num_threads, verbose):
+    if run_config.model_type == "Keras":
+        train_data, val_data = data
+        model.fit(
+            train_data,
+            validation_data=val_data,
+            epochs=end_epoch,
+            initial_epoch=early_stopper.current_epoch,  # when continuing the training, set the correct epoch number
+            callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
+            verbose=verbose
+        )
+        return model
+    elif run_config.model_type == "Lightning":
+        # set correct number of cpu cores; TODO: this for some reason currently only works with pytorch-gpu and is ignored by pytorch??
+        from torch import get_num_threads, get_num_interop_threads, set_num_threads, set_num_interop_threads
+        if get_num_threads() != num_threads:
+            set_num_threads(num_threads)
+        if get_num_interop_threads() != min(num_threads, 2):
+            set_num_interop_threads(min(num_threads, 2))
+
+        # currently, the device summary cannot be disabled. TODO: check if this has changed
+        import lightning.pytorch as pl
+        trainer = pl.Trainer(
+            max_epochs=end_epoch,
+            callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
+            devices='auto',
+            accelerator='auto',
+            num_sanity_val_steps=0,  # this messes with the reporting to Tune since it calls the Callbacks
+            enable_progress_bar=False,
+            enable_model_summary=False,
+            logger=False,  # logging is done via Tune
+            enable_checkpointing=False,  # checkpointing is done in the early stopper
+        )
+        trainer.fit_loop.epoch_progress.current.processed = early_stopper.current_epoch  # when continuing the training, set the correct epoch number
+        trainer.fit(model, data)
+        return model, trainer
+
+
+def train_model(
+    model_config,
+    run_config,
+    input_handler,
+    inputs_train,
+    inputs_val,
+    targets_train,
+    targets_val,
+    normalized_weights_train,
+    normalized_weights_val,
+    monitor=('val_loss', 'min'),
+    custom_metrics=[],
+    composite_metrics=[],
+    native_metrics=[],
+    weighted_native_metrics=[],
+    overtraining_conditions=[],
+    early_stopping_patience=0,
+    overtraining_patience=0,
+    restore_best_weights=False,
+    restore_on_best_checkpoint=False,
+    num_threads=1,
+    create_checkpoints=True,
+    run_in_subprocess=True,
+    verbose=2
+):
+    def _train_model(
+        checkpoint_com,
+        report_com,
+        termination_event,
+        start_time,
+        model_config,
+        run_config,
+        input_handler,
+        inputs_train,
+        inputs_val,
+        targets_train,
+        targets_val,
+        normalized_weights_train,
+        normalized_weights_val,
+        monitor,
+        custom_metrics,
+        composite_metrics,
+        native_metrics,
+        weighted_native_metrics,
+        overtraining_conditions,
+        early_stopping_patience,
+        overtraining_patience,
+        restore_best_weights,
+        restore_on_best_checkpoint,
+        num_threads,
+        create_checkpoints,
+        in_tune_session,
+        runs_in_subprocess,
+        verbose
+    ):
+        # setup the environment
+        if run_config.model_type == "Keras":
+            setup_tensorflow(num_threads)
             import tensorflow as tf
         elif run_config.model_type == "Lightning":
             import lightning.pytorch as pl
 
-        # fixed global random seeds (if provided) to make training deterministic
-        if model_config.get("seed") is not None:
-            if run_config.model_type == "Keras":
-                max_seeds = OPTIMA.core.tools.get_max_seeds()
-                np.random.seed(model_config["seed"])
-                python_random.seed(np.random.randint(*max_seeds))
-                tf.keras.utils.set_random_seed(np.random.randint(*max_seeds))
-                tf.random.set_seed(np.random.randint(*max_seeds))
-            elif run_config.model_type == "Lightning":
-                pl.seed_everything(model_config["seed"], workers=True)
+        # set the seeds
+        set_seeds(run_config, model_config)
 
         # check if training data is given as ray.ObjectReference; if yes, get the objects from Ray's shared memory
         if isinstance(inputs_train, ray.ObjectRef):
             inputs_train, inputs_val, targets_train, targets_val, normalized_weights_train, normalized_weights_val = ray.get([
                 inputs_train, inputs_val, targets_train, targets_val, normalized_weights_train, normalized_weights_val
             ])
 
@@ -117,262 +411,205 @@
         # - checkpoint_event and checkpoint_queue are used when checking if the trainable should reload from a checkpoint
         # - report_event and report_queue are used to report back results
         # - report_queue_read_event signifies that the main process has finished the report and the subprocess can continue training
         # - termination_event is set when the training terminates internally via EarlyStopping to tell the main process to return
         checkpoint_event, checkpoint_queue = checkpoint_com
         report_event, report_queue, report_queue_read_event = report_com
 
-        # limit all hyperparameters properly; since only non-conditional hyperparameters can go out of bounds (PBT does
-        # not support conditional hps), we don't need to do any deserialization
-        for hp, hp_search_space in run_config.search_space.items():
-            if isinstance(hp_search_space, dict) and "bounds" in hp_search_space.keys() and hp in model_config.keys():
-                bounds = hp_search_space["bounds"]
-                if (isinstance(bounds[0], int) or isinstance(bounds[0], float)) and model_config[hp] < bounds[0]:
-                    model_config[hp] = bounds[0]
-                elif (isinstance(bounds[1], int) or isinstance(bounds[1], float)) and model_config[hp] > bounds[1]:
-                    model_config[hp] = bounds[1]
-
-        # convert the training, validation and testing data to tensorflow datasets or lighning dataloaders
-        if run_config.model_type == "Keras":
-            train_data = tf.data.Dataset.from_tensor_slices((inputs_train, targets_train, normalized_weights_train))
-            val_data = tf.data.Dataset.from_tensor_slices((inputs_val, targets_val, normalized_weights_val))
-
-            # batch the datasets for tensorflow
-            train_data = train_data.batch(model_config["batch_size"])
-            val_data = val_data.batch(model_config["batch_size"])
-        elif run_config.model_type == "Lightning":
-            if hasattr(run_config, "DataModule"):
-                DataModule = run_config.DataModule
-            else:
-                DataModule = OPTIMA.lightning.inputs.DefaultDataModule
-            pl_data_module = DataModule(
-                input_handler=input_handler,
-                inputs_train=inputs_train,
-                targets_train=targets_train,
-                weights_train=normalized_weights_train,
-                inputs_val=inputs_val,
-                targets_val=targets_val,
-                weights_val=normalized_weights_val,
-                run_config=run_config,
-                model_config=model_config
-            )
-
-        # get the input and output shapes (incl. batch dimension)
-        output_shape = targets_train.shape
+        # compile the metrics
+        compiled_metrics, compiled_weighted_metrics = compile_metrics(run_config, native_metrics, weighted_native_metrics)
 
-        # compile the metrics (needs to be done here (and not earlier) because tensorflow must not be initialized before setting inter- and intra-op threads)
-        if run_config.model_type == "Keras":
-            compiled_metrics = [metric(name=name, **metric_kwargs) for name, (metric, metric_kwargs) in native_metrics]
-            compiled_weighted_metrics = [metric(name=name, **metric_kwargs) for name, (metric, metric_kwargs) in
-                                         weighted_native_metrics]
-        elif run_config.model_type == "Lightning":
-            compiled_metrics = [(f"{prefix}_{name}", metric(**metric_kwargs)) for name, (metric, metric_kwargs) in
-                                native_metrics for prefix in ["train", "val"]]
-            compiled_weighted_metrics = [(f"{prefix}_{name}", metric(**metric_kwargs)) for name, (metric, metric_kwargs) in
-                                         weighted_native_metrics for prefix in ["train", "val"]]
+        # check if we have fixed hyperparameters or a hyperparameter schedule and build a list of hyperparameters in the
+        # form [(start_epoch, end_epoch, model_config_iteration), ...] where the training should stop before end_epoch
+        # when counting from start_epoch
+        if "hp_schedule" in model_config:
+            policy = model_config["hp_schedule"]
+            hp_list = []
+            for i, (start_epoch, model_config_iteration) in enumerate(policy):
+                if i + 1 < len(policy):
+                    end_epoch = policy[i+1][0]
+                else:
+                    end_epoch = model_config["max_epochs"]
+                hp_list.append((start_epoch, end_epoch, model_config_iteration))
+        else:
+            hp_list = [(0, model_config["max_epochs"], model_config)]
 
-        # create the EarlyStopper instance
-        if run_config.model_type == "Keras":
-            early_stopper = OPTIMA.keras.training.EarlyStopperForKerasTuning(
-                monitor=monitor,
-                metrics=[metric_name for metric_name, _ in native_metrics],
-                weighted_metrics=[metric_name for metric_name, _ in weighted_native_metrics],
-                custom_metrics=custom_metrics,
-                composite_metrics=composite_metrics,
-                overfitting_conditions=overtraining_conditions,
-                patience_improvement=early_stopping_patience,
-                patience_overfitting=overtraining_patience,
-                inputs_train=train_data,
-                inputs_val=val_data,
-                targets_train=targets_train,
-                targets_val=targets_val,
-                weights_train=normalized_weights_train,
-                weights_val=normalized_weights_val,
-                restore_best_weights=restore_best_weights,
-                verbose=verbose,
-                create_checkpoints=create_checkpoints,
-                first_checkpoint_epoch=model_config["first_checkpoint_epoch"],
-                checkpoint_frequency=model_config["checkpoint_frequency"],
-                report_event=report_event,
-                report_queue=report_queue,
-                report_queue_read_event=report_queue_read_event,
-                termination_event=termination_event,
-                in_tune_session=in_tune_session
-            )
-        elif run_config.model_type == "Lightning":
-            early_stopper = OPTIMA.lightning.training.EarlyStopperForLightningTuning(
-                run_config=run_config,
-                model_config=model_config,
-                monitor=monitor,
-                metrics=[metric_name for metric_name, _ in native_metrics],
-                weighted_metrics=[metric_name for metric_name, _ in weighted_native_metrics],
-                custom_metrics=custom_metrics,
-                composite_metrics=composite_metrics,
-                overfitting_conditions=overtraining_conditions,
-                patience_improvement=early_stopping_patience,
-                patience_overfitting=overtraining_patience,
-                inputs_train=inputs_train,
-                inputs_val=inputs_val,
-                targets_train=targets_train,
-                targets_val=targets_val,
-                weights_train=normalized_weights_train,
-                weights_val=normalized_weights_val,
-                restore_best_weights=restore_best_weights,
-                verbose=verbose,
-                create_checkpoints=create_checkpoints,
-                first_checkpoint_epoch=model_config["first_checkpoint_epoch"],
-                checkpoint_frequency=model_config["checkpoint_frequency"],
-                report_event=report_event,
-                report_queue=report_queue,
-                report_queue_read_event=report_queue_read_event,
-                termination_event=termination_event,
-                in_tune_session=in_tune_session
-            )
+        # save the early stopper state when performing hyperparameter schedule
+        early_stopper_state = None
 
+        # check if we need to reload from a checkpoint
         if in_tune_session:
+            # check for Tune-managed checkpoint loading
             if runs_in_subprocess:
                 # activate checkpoint event, then wait until queue is filled
                 checkpoint_event.set()
                 checkpoint = checkpoint_queue.get()
             else:
                 # fetch checkpoint directly
                 checkpoint = train.get_checkpoint()
+
+            # convert checkpoint to directory path
+            if checkpoint is not None:
+                checkpoint = checkpoint.to_directory()
+        elif "checkpoint_dir" in model_config.keys() and os.path.exists(model_config["checkpoint_dir"]) and \
+                os.path.exists(os.path.join(model_config["checkpoint_dir"], "early_stopper")):
+            # check for manual checkpoint
+            checkpoint = model_config["checkpoint_dir"]
         else:
             checkpoint = None
 
-        # if checkpoint is not None, we are reloading a checkpoint
-        if checkpoint is not None:
-            checkpoint_dir = checkpoint.to_directory()
-            if run_config.model_type == "Keras":
-                if not restore_on_best_checkpoint:
-                    model = tf.keras.models.load_model(os.path.join(checkpoint_dir, "model.keras"))  # reload the model
-                else:
-                    model = tf.keras.models.load_model(os.path.join(checkpoint_dir, "best_model.keras"))  # reload the best model
+        # iterate over hyperparameter list
+        for hp_schedule_iteration, (start_epoch, end_epoch, model_config_iteration) in enumerate(hp_list):
+            # limit all hyperparameters
+            model_config_iteration = limit_hyperparameters(run_config, model_config_iteration)
 
-                # since some hyperparameters may have been changed since the save, we need to update the model
-                if hasattr(run_config, 'update_model'):
-                    model = run_config.update_model(
-                        model,
-                        model_config,
-                        input_handler=input_handler,
-                        inputs_train=inputs_train,
-                        targets_train=targets_train,
-                    )
-                else:
-                    model = OPTIMA.builtin.model.update_model(
-                        model,
-                        model_config,
-                        input_handler=input_handler,
-                        inputs_train=inputs_train,
-                        targets_train=targets_train,
-                    )
+            # convert the training and validation data to tensorflow datasets or lightning dataloaders
+            data = prepare_data(
+                run_config,
+                input_handler,
+                model_config_iteration,
+                inputs_train,
+                targets_train,
+                normalized_weights_train,
+                inputs_val,
+                targets_val,
+                normalized_weights_val
+            )
+            if run_config.model_type == "Keras":
+                train_data, val_data = data
             elif run_config.model_type == "Lightning":
-                # update hyperparameters while loading checkpoint
-                if not restore_on_best_checkpoint:
-                    model = run_config.LitModel.load_from_checkpoint(os.path.join(checkpoint_dir, "model.ckpt"), model_config=model_config)
-                else:
-                    model = run_config.LitModel.load_from_checkpoint(os.path.join(checkpoint_dir, "best_model.ckpt"), model_config=model_config)
+                pl_data_module = data
 
-            # load current early stopper state, even when restoring on best model checkpoint
-            early_stopper.load_state(checkpoint_dir)
+            # create the EarlyStopper instance
             if run_config.model_type == "Keras":
-                early_stopper.copy_best_model(os.path.join(checkpoint_dir, "best_model.keras"))
+                early_stopper = OPTIMA.keras.training.EarlyStopperForKerasTuning(
+                    monitor=monitor,
+                    metrics=[metric_name for metric_name, _ in native_metrics],
+                    weighted_metrics=[metric_name for metric_name, _ in weighted_native_metrics],
+                    custom_metrics=custom_metrics,
+                    composite_metrics=composite_metrics,
+                    overfitting_conditions=overtraining_conditions,
+                    patience_improvement=early_stopping_patience,
+                    patience_overfitting=overtraining_patience,
+                    inputs_train=train_data,
+                    inputs_val=val_data,
+                    targets_train=targets_train,
+                    targets_val=targets_val,
+                    weights_train=normalized_weights_train,
+                    weights_val=normalized_weights_val,
+                    restore_best_weights=restore_best_weights,
+                    verbose=verbose,
+                    create_checkpoints=create_checkpoints,
+                    checkpoint_dir=model_config.get('checkpoint_dir'),
+                    first_checkpoint_epoch=model_config["first_checkpoint_epoch"] if create_checkpoints else -1,
+                    checkpoint_frequency=model_config["checkpoint_frequency"] if create_checkpoints else -1,
+                    report_event=report_event,
+                    report_queue=report_queue,
+                    report_queue_read_event=report_queue_read_event,
+                    termination_event=termination_event,
+                    in_tune_session=in_tune_session
+                )
             elif run_config.model_type == "Lightning":
-                early_stopper.copy_best_model(os.path.join(checkpoint_dir, "best_model.ckpt"))
-        else:
-            # build model if it should not be reloaded from a checkpoint
-            if hasattr(run_config, 'build_model') and run_config.model_type == "Keras":
-                model = run_config.build_model(
-                    model_config,
-                    input_handler=input_handler,
+                early_stopper = OPTIMA.lightning.training.EarlyStopperForLightningTuning(
+                    run_config=run_config,
+                    model_config=model_config_iteration,
+                    monitor=monitor,
+                    metrics=[metric_name for metric_name, _ in native_metrics],
+                    weighted_metrics=[metric_name for metric_name, _ in weighted_native_metrics],
+                    custom_metrics=custom_metrics,
+                    composite_metrics=composite_metrics,
+                    overfitting_conditions=overtraining_conditions,
+                    patience_improvement=early_stopping_patience,
+                    patience_overfitting=overtraining_patience,
                     inputs_train=inputs_train,
+                    inputs_val=inputs_val,
                     targets_train=targets_train,
-                )#, seed=model_config["seed"])
-            elif hasattr(run_config, 'LitModel') and run_config.model_type == "Lightning":
-                model = run_config.LitModel(model_config, inputs_train.shape, output_shape, compiled_metrics, compiled_weighted_metrics)#, seed=model_config["seed"]
-            else:
-                if run_config.model_type == "Keras":
-                    model = OPTIMA.builtin.model.build_model(
-                        model_config,
-                        input_handler=input_handler,
-                        inputs_train=inputs_train,
-                        targets_train=targets_train,
-                    )#, seed=model_config["seed"])
-                elif run_config.model_type == "Lightning":
-                    raise NotImplementedError("Lightning models requires a LitModel-class to be present in the run-config.")
-
-        # delete the numpy arrays of the validation data, as they are no longer needed
-        del inputs_val
-        del targets_val
+                    targets_val=targets_val,
+                    weights_train=normalized_weights_train,
+                    weights_val=normalized_weights_val,
+                    restore_best_weights=restore_best_weights,
+                    verbose=verbose,
+                    create_checkpoints=create_checkpoints,
+                    checkpoint_dir=model_config.get('checkpoint_dir'),
+                    first_checkpoint_epoch=model_config["first_checkpoint_epoch"] if create_checkpoints else -1,
+                    checkpoint_frequency=model_config["checkpoint_frequency"] if create_checkpoints else -1,
+                    report_event=report_event,
+                    report_queue=report_queue,
+                    report_queue_read_event=report_queue_read_event,
+                    termination_event=termination_event,
+                    in_tune_session=in_tune_session
+                )
 
-        # in any case, the model needs to be compiled / prepared (this is also necessary if only the regularizers have been updated!)
-        if run_config.model_type == "Keras":
-            if hasattr(run_config, 'compile_model'):
-                model = run_config.compile_model(
-                    model,
-                    model_config,
-                    metrics=compiled_metrics,
-                    weighted_metrics=compiled_weighted_metrics,
-                    input_handler=input_handler,
-                    inputs_train=inputs_train,
-                    targets_train=targets_train,
-                    first_compile=checkpoint is None
+            # apply the checkpoint if available
+            if checkpoint is not None:
+                # load the model and the early stopper state from the checkpoint
+                model, early_stopper = reload_from_checkpoint(
+                    run_config,
+                    input_handler,
+                    model_config_iteration,
+                    early_stopper,
+                    inputs_train,
+                    targets_train,
+                    checkpoint,
+                    restore_on_best_checkpoint
                 )
+            elif hp_schedule_iteration > 0:
+                # we are running a hyperparameter schedule, so we need to update the model and set the early stopper
+                # state
+                if run_config.model_type == "Keras":
+                    model = update_model(
+                        run_config,
+                        model,
+                        model_config_iteration,
+                        input_handler,
+                        inputs_train,
+                        targets_train
+                    )
+                else:
+                    # TODO: manually save and reload the model here?
+                    raise NotImplementedError("Updating the hyperparameters of a Lightning model requires a checkpoint "
+                                              "to load from, which could not be found!")
+                early_stopper.set_state(early_stopper_state)
             else:
-                model = OPTIMA.builtin.model.compile_model(
-                    model,
-                    model_config,
-                    metrics=compiled_metrics,
-                    weighted_metrics=compiled_weighted_metrics,
-                    input_handler=input_handler,
-                    inputs_train=inputs_train,
-                    targets_train=targets_train,
-                    first_compile=checkpoint is None
+                # build model if it should not be reloaded from a checkpoint
+                model = build_model(
+                    run_config,
+                    model_config_iteration,
+                    input_handler,
+                    inputs_train,
+                    targets_train,
+                    compiled_metrics,
+                    compiled_weighted_metrics
                 )
-        elif run_config.model_type == "Lightning":
-            model.prepare(input_handler, inputs_train, targets_train, first_prepare=checkpoint is None)
 
-        # delete the numpy arrays of the training data, as they are no longer needed
-        del inputs_train
-        del targets_train
+            # in any case, the model needs to be compiled / prepared (this is also necessary if only the regularizers have been updated!)
+            model = compile_model(
+                        run_config,
+                        model,
+                        model_config_iteration,
+                        compiled_metrics,
+                        compiled_weighted_metrics,
+                        input_handler,
+                        inputs_train,
+                        targets_train,
+                        first_compile=checkpoint is None and hp_schedule_iteration == 0
+                    )
 
-        if time.time() - start_time > 2:
-            logging.warning(f"Starting the subprocess and prepare training took {time.time()-start_time}s which may be a performance bottleneck.")
+            if time.time() - start_time > 2 and hp_schedule_iteration == 0:
+                logging.warning(f"Starting the subprocess and prepare training took {time.time()-start_time}s which may "
+                                f"be a performance bottleneck.")
 
-        if run_config.model_type == "Keras":
-            model.fit(
-                train_data,
-                validation_data=val_data,
-                epochs=model_config["max_epochs"],
-                initial_epoch=early_stopper.current_epoch,  # when continuing the training, set the correct epoch number
-                callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
-                verbose=verbose
-            )
-        elif run_config.model_type == "Lightning":
-            # set correct number of cpu cores; TODO: this for some reason currently only works with pytorch-gpu and is ignored by pytorch??
-            from torch import get_num_threads, get_num_interop_threads, set_num_threads, set_num_interop_threads
-            if get_num_threads() != num_threads:
-                set_num_threads(num_threads)
-            if get_num_interop_threads() != min(num_threads, 2):
-                set_num_interop_threads(min(num_threads, 2))
-
-            # currently, the device summary cannot be disabled. TODO: check if this has changed
-            trainer = pl.Trainer(
-                max_epochs=model_config["max_epochs"],
-                callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
-                devices='auto',
-                accelerator='auto',
-                num_sanity_val_steps=0,  # this messes with the reporting to Tune since it calls the Callbacks
-                enable_progress_bar=False,
-                enable_model_summary=False,
-                logger=False,  # logging is done via Tune
-                enable_checkpointing=False,  # checkpointing is done in the early stopper
-            )
-            trainer.fit_loop.epoch_progress.current.processed = early_stopper.current_epoch  # when continuing the training, set the correct epoch number
-            trainer.fit(model, pl_data_module)
+            # fit the model
+            if run_config.model_type == "Keras":
+                model = fit_model(run_config, model, early_stopper, (train_data, val_data), end_epoch, num_threads, verbose)
+            elif run_config.model_type == "Lightning":
+                model, trainer = fit_model(run_config, model, early_stopper, pl_data_module, end_epoch, num_threads, verbose)
+
+            # save the early stopper state
+            early_stopper_state = early_stopper.get_state()
 
         # if requested, save the final model
         if "final_model_path" in model_config.keys():
             if not os.path.exists(os.path.dirname(model_config["final_model_path"])):
                 os.makedirs(os.path.dirname(model_config["final_model_path"]), exist_ok=True)
             if run_config.model_type == "Keras":
                 out_path = model_config["final_model_path"] + ".keras"
@@ -1071,14 +1308,18 @@
                   f"frequency to {run_config.perturbation_interval} epochs.")
             search_space_PBT["checkpoint_frequency"] = run_config.perturbation_interval
 
         # print the updated search space
         print("Updated search space:")
         print(search_space_PBT)
 
+        # Print the hyperparameters to mutate
+        print("Hyperparameters to mutate:")
+        print(hyperparams_to_mutate)
+
         # since the search algorithm is completely ignored when using PBT, we cannot do the same trick to include the
         # random seed as for Optuna. Fortunately, PBT only optimizes hyperparameters provided in hyperparams_to_mutate,
         # so we can simply add a new search space entry for the seed. Unfortunately, the only way to make the sampling
         # from Tune search space entries reproducible is to set the numpy global random state.
         np.random.seed(rng_PBT.randint(*max_seeds))
         search_space_PBT["seed"] = tune.randint(*max_seeds)
 
@@ -1129,30 +1370,61 @@
                     num_samples=run_config.num_samples_PBT if not replay else 1,
                     reuse_actors=True,
                 ),
             )
             return tuner
 
         if not os.path.isfile(os.path.join(results_dir_PBT, "analysis.pickle")):
-            # configure population based training
-            pbt = PopulationBasedTraining(
-                time_attr="training_iteration",
-                perturbation_interval=run_config.perturbation_interval,
-                burn_in_period=run_config.burn_in_period,
-                hyperparam_mutations=hyperparams_to_mutate,
-                seed=rng_PBT.randint(*max_seeds)
-            )
-
             if resume_experiment and tune.Tuner.can_restore(os.path.abspath(optimization_dir_PBT)):
                 # currently, restore does not handle relative paths; TODO: still true?
                 tuner = tune.Tuner.restore(os.path.abspath(optimization_dir_PBT), trainable=trainable, resume_errored=True)
             else:
-                tuner = _get_PBT_tuner(trainable, pbt, stopper,
-                                       name=os.path.basename(optimization_dir_PBT),
-                                       storage_path=os.path.dirname(optimization_dir_PBT),)
+                # configure population based training
+                pbt = PopulationBasedTraining(
+                    time_attr="training_iteration",
+                    perturbation_interval=run_config.perturbation_interval,
+                    burn_in_period=run_config.burn_in_period,
+                    hyperparam_mutations=hyperparams_to_mutate,
+                    seed=rng_PBT.randint(*max_seeds)
+                )
+
+                # get the Tuner
+                tuner = tune.Tuner(
+                    tune.with_resources(
+                        trainable,
+                        resources=tune.PlacementGroupFactory(
+                            [{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
+                        # resources={"cpu": cpus_per_trial, "gpu": args.gpus_per_trial, "memory": memory_per_trial},
+                    ),
+                    param_space=search_space_PBT,
+                    run_config=train.RunConfig(
+                        name=os.path.basename(optimization_dir_PBT),
+                        storage_path=os.path.abspath(os.path.dirname(optimization_dir_PBT)),
+                        # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
+                        stop=stopper,
+                        checkpoint_config=train.CheckpointConfig(
+                            num_to_keep=None,
+                            # checkpoint_score_attribute=optimize_name,
+                            # checkpoint_score_order=optimize_op
+                        ),
+                        failure_config=train.FailureConfig(
+                            max_failures=-1,
+                        ),
+                        # callbacks=[JsonLoggerCallback(), CSVLoggerCallback()],
+                        verbose=1,
+                    ),
+                    tune_config=tune.TuneConfig(
+                        # search_alg=BasicVariantGenerator(random_state=rng_PBT.randint(*max_seeds)) if not replay else None,
+                        scheduler=pbt,
+                        metric=optimize_name,
+                        mode=optimize_op,
+                        num_samples=run_config.num_samples_PBT,
+                        reuse_actors=True,
+                    ),
+                )
 
             results_grid = tuner.fit()
             analysis = results_grid._experiment_analysis
 
             # check if the experiment finished or was aborted (e.g. by KeyboardInterrupt)
             success_str = "\nPBT run finished!"
             failure_str = "Experiment did not finish. This indicates that either an error occured or the execution was interrupted " \
@@ -1163,31 +1435,28 @@
             with open(os.path.join(results_dir_PBT, "analysis.pickle"), "wb") as file:
                 pickle.dump(analysis, file)
         else:
             print("Finished experiment found, reloading the analysis.pickle file...")
             with open(os.path.join(results_dir_PBT, "analysis.pickle"), "rb") as file:
                 analysis = pickle.load(file)
 
-        # evaluate optimization results
-        def _get_PBT_replay_tuner(trial_id, trainable, name, max_epochs=-1):
-            policy_path = os.path.join(optimization_dir_PBT, f"pbt_policy_{trial_id}.txt")
+        # prepare the mutation handler
+        if os.path.exists(os.path.join(results_dir_PBT, "PBT_mutation_policies.pickle")):
+            # load from the save state
+            pbt_mutation_handler = OPTIMA.core.training.PBTMutationHandler()
+            pbt_mutation_handler.load(os.path.join(results_dir_PBT, "PBT_mutation_policies.pickle"))
+        else:
+            # prepare the PBT mutation handler and load from the experiment state
+            pbt_mutation_handler = OPTIMA.core.training.PBTMutationHandler()
+            pbt_mutation_handler.load_experiment_state(optimization_dir_PBT)
 
-            # make sure the policy file exists (e.g. when best trial did not have any perturbations, no policy file
-            # is generated
-            if not os.path.exists(policy_path):
-                raise ValueError
-
-            pbt_replay = PopulationBasedTrainingReplay(policy_path)
-
-            # use termination based on early stopping when max_epochs is not provided
-            stop = stopper if max_epochs == -1 else {"training_iteration": max_epochs}
-            return _get_PBT_tuner(trainable, pbt_replay, stop, name,
-                                  os.path.join(os.path.dirname(optimization_dir_PBT), "PBT_replay"),
-                                  verbose=0, replay=True)
+            # save the mutation policies to the results directory
+            pbt_mutation_handler.save(os.path.join(results_dir_PBT, "PBT_mutation_policies.pickle"))
 
+        # evaluate optimization results
         best_trials, best_trials_fit, configs_df = \
             OPTIMA.core.evaluation.evaluate_experiment(analysis,
                                                        train_model,
                                                        run_config,
                                                        run_config.monitor_name,
                                                        run_config.monitor_op,
                                                        search_space_PBT,
@@ -1201,15 +1470,15 @@
                                                        composite_metrics=composite_metrics,
                                                        native_metrics=native_metrics,
                                                        weighted_native_metrics=weighted_native_metrics,
                                                        cpus_per_model=args.cpus_per_trial,
                                                        gpus_per_model=args.gpus_per_trial,
                                                        overtraining_conditions=run_config.overtraining_conditions,
                                                        PBT=True,
-                                                       PBT_replay_getter=_get_PBT_replay_tuner,
+                                                       PBT_mutation_handler=pbt_mutation_handler,
                                                        seed=rng_PBT.randint(*max_seeds))
 
 def initialize(args, run_config, cluster, custom_cluster_config=None):
     # get the cluster and configure the job
     if custom_cluster_config is not None and hasattr(custom_cluster_config, "ClusterJob"):
         job = custom_cluster_config.ClusterJob
     else:
```

### Comparing `optima_ml-0.3.3a3/OPTIMA/resources/config_verification.py` & `optima_ml-0.3.4a1/OPTIMA/resources/config_verification.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/OPTIMA/resources/pbt_with_seed.py` & `optima_ml-0.3.4a1/OPTIMA/resources/pbt_with_seed.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/PKG-INFO` & `optima_ml-0.3.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.3a3
+Version: 0.3.4a1
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
```

### Comparing `optima_ml-0.3.3a3/README.md` & `optima_ml-0.3.4a1/README.md`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/optima_ml.egg-info/PKG-INFO` & `optima_ml-0.3.4a1/optima_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.3a3
+Version: 0.3.4a1
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
```

### Comparing `optima_ml-0.3.3a3/optima_ml.egg-info/SOURCES.txt` & `optima_ml-0.3.4a1/optima_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/setup.py` & `optima_ml-0.3.4a1/setup.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/tests/test_builtin.py` & `optima_ml-0.3.4a1/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a3/tests/test_core.py` & `optima_ml-0.3.4a1/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,14 +441,16 @@
             best_trials,
             best_trials_fit,
             configs_df,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string,
             raw_metric_values
         ) = pickle.load(evaluation_file)
 
     # we assume that the results of the optimization are identical, and the results of the evaluation are close (but need
     # not be identical due to numerical differences on different systems arising during the crossvalidation)
     assert best_trials.equals(best_trials_test)
```

### Comparing `optima_ml-0.3.3a3/tests/test_integration.py` & `optima_ml-0.3.4a1/tests/test_integration_sameMachine.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,116 +26,128 @@
             best_trials,
             best_trials_fit,
             configs_df,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string,
             raw_metric_values
         ) = pickle.load(evaluation_file)
     with open("tests/temp_integration_test/test_optimization/results/variable_optimization/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials_reference,
             best_trials_fit_reference,
             configs_df_reference,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string_reference,
             raw_metric_values_reference
         ) = pickle.load(evaluation_file)
 
     # we assume that the results of the optimization are identical, and the results of the evaluation are close (but need
     # not be identical due to numerical differences on different systems arising during the crossvalidation). The path
     # to the trial of cause is expected to be different.
-    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-2
-    assert (2 * (best_trials_fit.drop(columns="trial") - best_trials_fit_reference.drop(columns="trial")) / (best_trials_fit.drop(columns="trial") + best_trials_fit_reference.drop(columns="trial"))).abs().max().max() < 1e-2
+    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-8
+    assert (2 * (best_trials_fit.drop(columns="trial") - best_trials_fit_reference.drop(columns="trial")) / (best_trials_fit.drop(columns="trial") + best_trials_fit_reference.drop(columns="trial"))).abs().max().max() < 1e-8
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
-            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 0.1
+            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 1e-8
 
     # check the variable optimization
     with open("tests/test_optimization/results/variable_optimization/optimized_vars.pickle", "rb") as f:
         optimized_vars = pickle.load(f)
     with open("tests/test_optimization/results/variable_optimization/variable_optimization.pickle", "rb") as f:
         var_opt_baseline, var_opt_results = pickle.load(f)
     with open("tests/temp_integration_test/test_optimization/results/variable_optimization/optimized_vars.pickle", "rb") as f:
         optimized_vars_reference = pickle.load(f)
     with open("tests/temp_integration_test/test_optimization/results/variable_optimization/variable_optimization.pickle", "rb") as f:
         var_opt_baseline_reference, var_opt_results_reference = pickle.load(f)
 
     assert optimized_vars == optimized_vars_reference
-    assert np.max(np.abs(var_opt_baseline - var_opt_baseline_reference)) < 1e-4
+    assert np.max(np.abs(var_opt_baseline - var_opt_baseline_reference)) < 1e-8
     for it in range(len(var_opt_results_reference)):
         for var_set in var_opt_results_reference[it].keys():
-            assert np.max(np.abs(np.array(var_opt_results[it][var_set]) - np.array(var_opt_results_reference[it][var_set]))) < 1e-3
+            assert np.max(np.abs(np.array(var_opt_results[it][var_set]) - np.array(var_opt_results_reference[it][var_set]))) < 1e-8
 
     # check the main optimization step
     with open("tests/test_optimization/results/optuna+ASHA/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials,
             best_trials_fit,
             configs_df,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string,
             raw_metric_values
         ) = pickle.load(evaluation_file)
     with open("tests/temp_integration_test/test_optimization/results/optuna+ASHA/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials_reference,
             best_trials_fit_reference,
             configs_df_reference,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string_reference,
             raw_metric_values_reference
         ) = pickle.load(evaluation_file)
-    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-2
-    assert (2 * (best_trials_fit.drop(columns="trial") - best_trials_fit_reference.drop(columns="trial")) / (best_trials_fit.drop(columns="trial") + best_trials_fit_reference.drop(columns="trial"))).abs().max().max() < 1e-2
+    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-8
+    assert (2 * (best_trials_fit.drop(columns="trial") - best_trials_fit_reference.drop(columns="trial")) / (best_trials_fit.drop(columns="trial") + best_trials_fit_reference.drop(columns="trial"))).abs().max().max() < 1e-8
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
-            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 0.1
+            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 1e-8
 
     # check the PBT step
     with open("tests/test_optimization/results/PBT/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials,
             _,
             configs_df,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string,
             raw_metric_values
         ) = pickle.load(evaluation_file)
     with open("tests/temp_integration_test/test_optimization/results/PBT/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials_reference,
             _,
             configs_df_reference,
             _,
             _,
             _,
             _,
+            _,
+            _,
             evaluation_string_reference,
             raw_metric_values_reference
         ) = pickle.load(evaluation_file)
-    assert (2 * (best_trials.drop(columns=["trial", "best index"]) - best_trials_reference.drop(columns=["trial", "best index"]))
-            / (best_trials.drop(columns=["trial", "best index"]) + best_trials_reference.drop(columns=["trial", "best index"]))).abs().max().max() < 1e-2
+    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-8
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
-            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 0.1
+            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 1e-8
 
     # cleanup
     shutil.rmtree("tests/test_optimization")
     shutil.rmtree("tests/temp_integration_test")
+
```

### Comparing `optima_ml-0.3.3a3/tests/test_preprocessing.py` & `optima_ml-0.3.4a1/tests/test_preprocessing.py`

 * *Files identical despite different names*

