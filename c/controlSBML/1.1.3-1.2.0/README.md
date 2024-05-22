# Comparing `tmp/controlSBML-1.1.3.tar.gz` & `tmp/controlsbml-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlSBML-1.1.3.tar", last modified: Sat Jan 20 18:11:39 2024, max compression
+gzip compressed data, was "controlsbml-1.2.0.tar", last modified: Wed May 22 21:42:48 2024, max compression
```

## Comparing `controlSBML-1.1.3.tar` & `controlsbml-1.2.0.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.485090 controlSBML-1.1.3/
--rw-r--r--   0 jlheller   (501) staff       (20)     1075 2022-03-18 16:48:50.000000 controlSBML-1.1.3/LICENSE
--rw-r--r--   0 jlheller   (501) staff       (20)     8351 2024-01-20 18:11:39.484923 controlSBML-1.1.3/PKG-INFO
--rw-r--r--   0 jlheller   (501) staff       (20)     6353 2024-01-20 17:50:18.000000 controlSBML-1.1.3/README.md
--rw-r--r--   0 jlheller   (501) staff       (20)      793 2023-12-27 21:34:45.000000 controlSBML-1.1.3/pyproject.toml
--rw-r--r--   0 jlheller   (501) staff       (20)      119 2024-01-20 18:11:39.485851 controlSBML-1.1.3/setup.cfg
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.365921 controlSBML-1.1.3/src/
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.393644 controlSBML-1.1.3/src/controlSBML/
--rw-r--r--   0 jlheller   (501) staff       (20)      421 2024-01-16 20:27:15.000000 controlSBML-1.1.3/src/controlSBML/__init__.py
--rw-r--r--   0 jlheller   (501) staff       (20)      325 2023-12-27 21:34:01.000000 controlSBML-1.1.3/src/controlSBML/_version.py
--rw-r--r--   0 jlheller   (501) staff       (20)    18655 2024-01-10 21:25:56.000000 controlSBML-1.1.3/src/controlSBML/antimony_builder.py
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.429917 controlSBML-1.1.3/src/controlSBML/archive/
--rw-r--r--   0 jlheller   (501) staff       (20)     1872 2023-10-05 00:19:08.000000 controlSBML-1.1.3/src/controlSBML/archive/__init__.py
--rw-r--r--   0 jlheller   (501) staff       (20)     5347 2023-08-12 23:21:53.000000 controlSBML-1.1.3/src/controlSBML/archive/control_analysis.py
--rw-r--r--   0 jlheller   (501) staff       (20)    12704 2023-08-29 16:47:26.000000 controlSBML-1.1.3/src/controlSBML/archive/control_base.py
--rw-r--r--   0 jlheller   (501) staff       (20)     7868 2023-08-13 00:07:22.000000 controlSBML-1.1.3/src/controlSBML/archive/control_plot.py
--rw-r--r--   0 jlheller   (501) staff       (20)    12874 2023-09-04 17:43:23.000000 controlSBML-1.1.3/src/controlSBML/archive/control_sbml.py
--rw-r--r--   0 jlheller   (501) staff       (20)     2490 2023-12-15 06:19:54.000000 controlSBML-1.1.3/src/controlSBML/archive/history.py
--rw-r--r--   0 jlheller   (501) staff       (20)    23900 2023-09-19 21:32:07.000000 controlSBML-1.1.3/src/controlSBML/archive/iosystem_factory.py
--rw-r--r--   0 jlheller   (501) staff       (20)     4299 2023-08-29 22:42:51.000000 controlSBML-1.1.3/src/controlSBML/archive/logger.py
--rw-r--r--   0 jlheller   (501) staff       (20)     8717 2023-10-25 22:28:04.000000 controlSBML-1.1.3/src/controlSBML/archive/mimo_transfer_function_builder.py
--rw-r--r--   0 jlheller   (501) staff       (20)     8879 2023-09-11 19:52:33.000000 controlSBML-1.1.3/src/controlSBML/archive/nonlinear_io_system.py
--rw-r--r--   0 jlheller   (501) staff       (20)     3129 2022-03-18 16:48:50.000000 controlSBML-1.1.3/src/controlSBML/archive/sequential_model.py
--rw-r--r--   0 jlheller   (501) staff       (20)     3474 2023-09-11 18:47:38.000000 controlSBML-1.1.3/src/controlSBML/archive/simulate_system.py
--rw-r--r--   0 jlheller   (501) staff       (20)    12943 2024-01-19 19:27:40.000000 controlSBML-1.1.3/src/controlSBML/archive/siso_closed_loop_designer.py
--rw-r--r--   0 jlheller   (501) staff       (20)    21362 2023-09-19 21:50:01.000000 controlSBML-1.1.3/src/controlSBML/archive/siso_closed_loop_system.py
--rw-r--r--   0 jlheller   (501) staff       (20)    10243 2023-12-12 21:33:04.000000 controlSBML-1.1.3/src/controlSBML/archive/siso_design_evaluator.py
--rw-r--r--   0 jlheller   (501) staff       (20)    16127 2023-10-04 20:32:45.000000 controlSBML-1.1.3/src/controlSBML/archive/siso_transfer_function_builder.py
--rw-r--r--   0 jlheller   (501) staff       (20)     4067 2023-09-19 00:18:27.000000 controlSBML-1.1.3/src/controlSBML/archive/temporal_series.py
--rw-r--r--   0 jlheller   (501) staff       (20)     7464 2024-01-19 20:24:21.000000 controlSBML-1.1.3/src/controlSBML/constants.py
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.431840 controlSBML-1.1.3/src/controlSBML/control_extensions/
--rw-r--r--   0 jlheller   (501) staff       (20)        0 2022-03-18 16:48:50.000000 controlSBML-1.1.3/src/controlSBML/control_extensions/__init__.py
--rw-r--r--   0 jlheller   (501) staff       (20)     5298 2022-03-18 16:48:50.000000 controlSBML-1.1.3/src/controlSBML/control_extensions/state_space_tf.py
--rw-r--r--   0 jlheller   (501) staff       (20)    31029 2024-01-20 06:50:26.000000 controlSBML-1.1.3/src/controlSBML/control_sbml.py
--rw-r--r--   0 jlheller   (501) staff       (20)     4878 2023-12-14 15:54:14.000000 controlSBML-1.1.3/src/controlSBML/dict_array.py
--rw-r--r--   0 jlheller   (501) staff       (20)    11107 2023-12-06 22:14:38.000000 controlSBML-1.1.3/src/controlSBML/grid.py
--rw-r--r--   0 jlheller   (501) staff       (20)     2364 2023-10-12 02:01:23.000000 controlSBML-1.1.3/src/controlSBML/iterate_biomodels.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1285 2022-03-18 16:48:50.000000 controlSBML-1.1.3/src/controlSBML/make_roadrunner.py
--rw-r--r--   0 jlheller   (501) staff       (20)      276 2023-10-01 01:32:07.000000 controlSBML-1.1.3/src/controlSBML/msgs.py
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.435120 controlSBML-1.1.3/src/controlSBML/option_management/
--rw-r--r--   0 jlheller   (501) staff       (20)        0 2022-03-18 16:48:50.000000 controlSBML-1.1.3/src/controlSBML/option_management/__init__.py
--rw-r--r--   0 jlheller   (501) staff       (20)     5770 2023-08-15 18:21:51.000000 controlSBML-1.1.3/src/controlSBML/option_management/option_manager.py
--rw-r--r--   0 jlheller   (501) staff       (20)     3116 2023-07-31 18:29:51.000000 controlSBML-1.1.3/src/controlSBML/option_management/options.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1513 2023-11-27 20:55:20.000000 controlSBML-1.1.3/src/controlSBML/option_set.py
--rw-r--r--   0 jlheller   (501) staff       (20)     6754 2023-12-16 01:24:16.000000 controlSBML-1.1.3/src/controlSBML/parallel_search.py
--rw-r--r--   0 jlheller   (501) staff       (20)     5510 2024-01-20 06:50:55.000000 controlSBML-1.1.3/src/controlSBML/point_evaluator.py
--rw-r--r--   0 jlheller   (501) staff       (20)    21777 2024-01-20 01:11:04.000000 controlSBML-1.1.3/src/controlSBML/sbml_system.py
--rw-r--r--   0 jlheller   (501) staff       (20)    18682 2024-01-20 00:19:17.000000 controlSBML-1.1.3/src/controlSBML/siso_closed_loop_designer.py
--rw-r--r--   0 jlheller   (501) staff       (20)     6202 2024-01-20 01:11:27.000000 controlSBML-1.1.3/src/controlSBML/siso_maker.py
--rw-r--r--   0 jlheller   (501) staff       (20)    17784 2024-01-20 01:12:05.000000 controlSBML-1.1.3/src/controlSBML/siso_transfer_function_builder.py
--rw-r--r--   0 jlheller   (501) staff       (20)     3547 2023-12-16 14:51:38.000000 controlSBML-1.1.3/src/controlSBML/staircase.py
--rw-r--r--   0 jlheller   (501) staff       (20)     7802 2023-10-29 20:18:43.000000 controlSBML-1.1.3/src/controlSBML/timeseries.py
--rw-r--r--   0 jlheller   (501) staff       (20)    19101 2024-01-19 19:53:14.000000 controlSBML-1.1.3/src/controlSBML/util.py
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.484414 controlSBML-1.1.3/src/controlSBML.egg-info/
--rw-r--r--   0 jlheller   (501) staff       (20)     8351 2024-01-20 18:11:39.000000 controlSBML-1.1.3/src/controlSBML.egg-info/PKG-INFO
--rw-r--r--   0 jlheller   (501) staff       (20)     2341 2024-01-20 18:11:39.000000 controlSBML-1.1.3/src/controlSBML.egg-info/SOURCES.txt
--rw-r--r--   0 jlheller   (501) staff       (20)        1 2024-01-20 18:11:39.000000 controlSBML-1.1.3/src/controlSBML.egg-info/dependency_links.txt
--rw-r--r--   0 jlheller   (501) staff       (20)        1 2022-12-26 19:09:32.000000 controlSBML-1.1.3/src/controlSBML.egg-info/not-zip-safe
--rw-r--r--   0 jlheller   (501) staff       (20)      158 2024-01-20 18:11:39.000000 controlSBML-1.1.3/src/controlSBML.egg-info/requires.txt
--rw-r--r--   0 jlheller   (501) staff       (20)       12 2024-01-20 18:11:39.000000 controlSBML-1.1.3/src/controlSBML.egg-info/top_level.txt
-drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-01-20 18:11:39.483539 controlSBML-1.1.3/tests/
--rw-r--r--   0 jlheller   (501) staff       (20)     7319 2023-10-22 22:21:58.000000 controlSBML-1.1.3/tests/test_antimony_builder.py
--rw-r--r--   0 jlheller   (501) staff       (20)    13764 2024-01-20 07:53:42.000000 controlSBML-1.1.3/tests/test_control_sbml.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1836 2023-12-14 15:55:33.000000 controlSBML-1.1.3/tests/test_dict_array.py
--rw-r--r--   0 jlheller   (501) staff       (20)     3664 2023-12-06 21:55:51.000000 controlSBML-1.1.3/tests/test_grid.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1293 2023-10-03 21:36:07.000000 controlSBML-1.1.3/tests/test_iterate_biomodels.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1682 2023-11-17 17:51:12.000000 controlSBML-1.1.3/tests/test_make_roadrunner.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1324 2023-11-25 16:58:23.000000 controlSBML-1.1.3/tests/test_option_set.py
--rw-r--r--   0 jlheller   (501) staff       (20)     3312 2023-12-15 00:43:08.000000 controlSBML-1.1.3/tests/test_parallel_search.py
--rw-r--r--   0 jlheller   (501) staff       (20)     6349 2023-12-15 23:39:39.000000 controlSBML-1.1.3/tests/test_sbml_system.py
--rw-r--r--   0 jlheller   (501) staff       (20)    10483 2024-01-20 03:38:29.000000 controlSBML-1.1.3/tests/test_siso_closed_loop_designer.py
--rw-r--r--   0 jlheller   (501) staff       (20)     1528 2024-01-20 01:16:07.000000 controlSBML-1.1.3/tests/test_siso_maker.py
--rw-r--r--   0 jlheller   (501) staff       (20)     7095 2023-12-16 16:28:22.000000 controlSBML-1.1.3/tests/test_siso_transfer_function_builder.py
--rw-r--r--   0 jlheller   (501) staff       (20)     2576 2023-08-08 19:01:28.000000 controlSBML-1.1.3/tests/test_staircase.py
--rw-r--r--   0 jlheller   (501) staff       (20)     4149 2023-08-12 04:10:23.000000 controlSBML-1.1.3/tests/test_timeseries.py
--rw-r--r--   0 jlheller   (501) staff       (20)     8938 2023-12-27 19:30:01.000000 controlSBML-1.1.3/tests/test_util.py
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.391037 controlsbml-1.2.0/
+-rw-r--r--   0 jlheller   (501) staff       (20)     1075 2022-03-18 16:48:50.000000 controlsbml-1.2.0/LICENSE
+-rw-r--r--   0 jlheller   (501) staff       (20)     8716 2024-05-22 21:42:48.390883 controlsbml-1.2.0/PKG-INFO
+-rw-r--r--   0 jlheller   (501) staff       (20)     6718 2024-05-22 21:41:13.000000 controlsbml-1.2.0/README.md
+-rw-r--r--   0 jlheller   (501) staff       (20)      792 2024-05-22 21:38:38.000000 controlsbml-1.2.0/pyproject.toml
+-rw-r--r--   0 jlheller   (501) staff       (20)      119 2024-05-22 21:42:48.391900 controlsbml-1.2.0/setup.cfg
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.343133 controlsbml-1.2.0/src/
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.358663 controlsbml-1.2.0/src/controlSBML/
+-rw-r--r--   0 jlheller   (501) staff       (20)      490 2024-05-07 23:10:00.000000 controlsbml-1.2.0/src/controlSBML/__init__.py
+-rw-r--r--   0 jlheller   (501) staff       (20)      324 2024-05-22 21:39:39.000000 controlsbml-1.2.0/src/controlSBML/_version.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    24522 2024-05-22 14:41:34.000000 controlsbml-1.2.0/src/controlSBML/antimony_builder.py
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.378294 controlsbml-1.2.0/src/controlSBML/archive/
+-rw-r--r--   0 jlheller   (501) staff       (20)     1872 2023-10-05 00:19:08.000000 controlsbml-1.2.0/src/controlSBML/archive/__init__.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     5347 2023-08-12 23:21:53.000000 controlsbml-1.2.0/src/controlSBML/archive/control_analysis.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    12704 2023-08-29 16:47:26.000000 controlsbml-1.2.0/src/controlSBML/archive/control_base.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     7868 2023-08-13 00:07:22.000000 controlsbml-1.2.0/src/controlSBML/archive/control_plot.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    12826 2024-02-29 02:32:01.000000 controlsbml-1.2.0/src/controlSBML/archive/control_sbml.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     2490 2023-12-15 06:19:54.000000 controlsbml-1.2.0/src/controlSBML/archive/history.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    23900 2023-09-19 21:32:07.000000 controlsbml-1.2.0/src/controlSBML/archive/iosystem_factory.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     4299 2023-08-29 22:42:51.000000 controlsbml-1.2.0/src/controlSBML/archive/logger.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     8709 2024-03-11 17:50:59.000000 controlsbml-1.2.0/src/controlSBML/archive/mimo_transfer_function_builder.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     8879 2023-09-11 19:52:33.000000 controlsbml-1.2.0/src/controlSBML/archive/nonlinear_io_system.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3129 2022-03-18 16:48:50.000000 controlsbml-1.2.0/src/controlSBML/archive/sequential_model.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3474 2023-09-11 18:47:38.000000 controlsbml-1.2.0/src/controlSBML/archive/simulate_system.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    12943 2024-01-19 19:27:40.000000 controlsbml-1.2.0/src/controlSBML/archive/siso_closed_loop_designer.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    21362 2023-09-19 21:50:01.000000 controlsbml-1.2.0/src/controlSBML/archive/siso_closed_loop_system.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    10718 2024-05-07 16:52:58.000000 controlsbml-1.2.0/src/controlSBML/archive/siso_design_evaluator.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    16115 2024-02-29 02:32:01.000000 controlsbml-1.2.0/src/controlSBML/archive/siso_transfer_function_builder.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     4067 2023-09-19 00:18:27.000000 controlsbml-1.2.0/src/controlSBML/archive/temporal_series.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    11400 2024-05-12 18:39:06.000000 controlsbml-1.2.0/src/controlSBML/constants.py
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.379446 controlsbml-1.2.0/src/controlSBML/control_extensions/
+-rw-r--r--   0 jlheller   (501) staff       (20)        0 2022-03-18 16:48:50.000000 controlsbml-1.2.0/src/controlSBML/control_extensions/__init__.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     5298 2022-03-18 16:48:50.000000 controlsbml-1.2.0/src/controlSBML/control_extensions/state_space_tf.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    41211 2024-05-18 01:31:13.000000 controlsbml-1.2.0/src/controlSBML/control_sbml.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     4954 2024-03-20 16:16:40.000000 controlsbml-1.2.0/src/controlSBML/dict_array.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    10525 2024-03-12 17:47:58.000000 controlsbml-1.2.0/src/controlSBML/gpz_fitter.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    11250 2024-03-20 02:40:07.000000 controlsbml-1.2.0/src/controlSBML/grid.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     2364 2023-10-12 02:01:23.000000 controlsbml-1.2.0/src/controlSBML/iterate_biomodels.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1285 2022-03-18 16:48:50.000000 controlsbml-1.2.0/src/controlSBML/make_roadrunner.py
+-rw-r--r--   0 jlheller   (501) staff       (20)      276 2023-10-01 01:32:07.000000 controlsbml-1.2.0/src/controlSBML/msgs.py
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.381040 controlsbml-1.2.0/src/controlSBML/option_management/
+-rw-r--r--   0 jlheller   (501) staff       (20)        0 2022-03-18 16:48:50.000000 controlsbml-1.2.0/src/controlSBML/option_management/__init__.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     6293 2024-05-09 01:22:03.000000 controlsbml-1.2.0/src/controlSBML/option_management/option_manager.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3168 2024-03-11 19:08:49.000000 controlsbml-1.2.0/src/controlSBML/option_management/options.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1513 2023-11-27 20:55:20.000000 controlsbml-1.2.0/src/controlSBML/option_set.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     6746 2024-05-10 18:13:51.000000 controlsbml-1.2.0/src/controlSBML/parallel_search.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     6115 2024-05-22 19:56:04.000000 controlsbml-1.2.0/src/controlSBML/point_evaluator.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     6473 2024-03-12 23:30:03.000000 controlsbml-1.2.0/src/controlSBML/poly_fitter.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    24317 2024-05-21 19:06:26.000000 controlsbml-1.2.0/src/controlSBML/sbml_system.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    19971 2024-05-18 11:40:54.000000 controlsbml-1.2.0/src/controlSBML/siso_closed_loop_designer.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     6193 2024-05-12 20:50:30.000000 controlsbml-1.2.0/src/controlSBML/siso_maker.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    12217 2024-03-31 22:34:48.000000 controlsbml-1.2.0/src/controlSBML/siso_transfer_function_builder.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    10568 2024-05-08 20:43:53.000000 controlsbml-1.2.0/src/controlSBML/siso_transfer_function_fitter.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     4994 2024-03-14 02:38:00.000000 controlsbml-1.2.0/src/controlSBML/staircase.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     7817 2024-03-27 21:08:33.000000 controlsbml-1.2.0/src/controlSBML/timeseries.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    22192 2024-05-21 18:17:38.000000 controlsbml-1.2.0/src/controlSBML/util.py
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.390346 controlsbml-1.2.0/src/controlSBML.egg-info/
+-rw-r--r--   0 jlheller   (501) staff       (20)     8716 2024-05-22 21:42:48.000000 controlsbml-1.2.0/src/controlSBML.egg-info/PKG-INFO
+-rw-r--r--   0 jlheller   (501) staff       (20)     2546 2024-05-22 21:42:48.000000 controlsbml-1.2.0/src/controlSBML.egg-info/SOURCES.txt
+-rw-r--r--   0 jlheller   (501) staff       (20)        1 2024-05-22 21:42:48.000000 controlsbml-1.2.0/src/controlSBML.egg-info/dependency_links.txt
+-rw-r--r--   0 jlheller   (501) staff       (20)        1 2022-12-26 19:09:32.000000 controlsbml-1.2.0/src/controlSBML.egg-info/not-zip-safe
+-rw-r--r--   0 jlheller   (501) staff       (20)      158 2024-05-22 21:42:48.000000 controlsbml-1.2.0/src/controlSBML.egg-info/requires.txt
+-rw-r--r--   0 jlheller   (501) staff       (20)       12 2024-05-22 21:42:48.000000 controlsbml-1.2.0/src/controlSBML.egg-info/top_level.txt
+drwxr-xr-x   0 jlheller   (501) staff       (20)        0 2024-05-22 21:42:48.389837 controlsbml-1.2.0/tests/
+-rw-r--r--   0 jlheller   (501) staff       (20)    12767 2024-05-22 14:42:02.000000 controlsbml-1.2.0/tests/test_antimony_builder.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    21995 2024-05-19 02:36:27.000000 controlsbml-1.2.0/tests/test_control_sbml.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1836 2024-03-09 21:48:24.000000 controlsbml-1.2.0/tests/test_dict_array.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     7531 2024-03-31 22:37:35.000000 controlsbml-1.2.0/tests/test_gpz_fitter.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3898 2024-03-20 02:39:19.000000 controlsbml-1.2.0/tests/test_grid.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1325 2024-03-12 21:15:13.000000 controlsbml-1.2.0/tests/test_iterate_biomodels.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1682 2023-11-17 17:51:12.000000 controlsbml-1.2.0/tests/test_make_roadrunner.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1324 2023-11-25 16:58:23.000000 controlsbml-1.2.0/tests/test_option_set.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3312 2024-03-09 21:46:35.000000 controlsbml-1.2.0/tests/test_parallel_search.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     5121 2024-03-18 21:46:09.000000 controlsbml-1.2.0/tests/test_poly_fitter.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     9687 2024-05-21 18:18:36.000000 controlsbml-1.2.0/tests/test_sbml_system.py
+-rw-r--r--   0 jlheller   (501) staff       (20)    11944 2024-05-07 16:52:58.000000 controlsbml-1.2.0/tests/test_siso_closed_loop_designer.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     1528 2024-01-20 01:16:07.000000 controlsbml-1.2.0/tests/test_siso_maker.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     6212 2024-03-17 01:12:32.000000 controlsbml-1.2.0/tests/test_siso_transfer_function_builder.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3506 2024-05-07 16:52:58.000000 controlsbml-1.2.0/tests/test_siso_transfer_function_fitter.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     3908 2024-03-12 21:51:39.000000 controlsbml-1.2.0/tests/test_staircase.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     4149 2023-08-12 04:10:23.000000 controlsbml-1.2.0/tests/test_timeseries.py
+-rw-r--r--   0 jlheller   (501) staff       (20)     9971 2024-05-08 20:05:18.000000 controlsbml-1.2.0/tests/test_util.py
```

### Comparing `controlSBML-1.1.3/LICENSE` & `controlsbml-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/PKG-INFO` & `controlsbml-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlSBML
-Version: 1.1.3
+Version: 1.2.0
 Summary: Control analysis of SBML models
 Author-email: Joseph Hellerstein <joseph.hellerstein@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Joseph Hellerstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,14 +66,19 @@
 To find the current version:
 ```
 import controlSBML as ctl
 ctl.__version__
 ```
 
 ## Version History
+* 1.2.0
+    * Implemented differential control
+    * Extended noise model to include lognormal distribution, offset, and slope
+    * Implemented several examples, some of which are based on student projects
+    * Two algorithms for fitting. gpz fits the transfer function in order by gain (g), poles (p), zeroes (z). poly fits a polynomial in s to the simulations.
 * 1.1.03 1/20/2024
     * Better error checking
     * API uses parameter names kI, kP, kF
 * 1.1.02 12/27/2023
     * Fix bug in dependencies. Update header documentation.
 * 1.1.01 12/27/2023
     * Complete change in the architecture. Instead of using NonlinearIOSystems in the python control package, controlSBML generates Antimony code to implement staircase functions and closed loops.
```

### Comparing `controlSBML-1.1.3/README.md` & `controlsbml-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 To find the current version:
 ```
 import controlSBML as ctl
 ctl.__version__
 ```
 
 ## Version History
+* 1.2.0
+    * Implemented differential control
+    * Extended noise model to include lognormal distribution, offset, and slope
+    * Implemented several examples, some of which are based on student projects
+    * Two algorithms for fitting. gpz fits the transfer function in order by gain (g), poles (p), zeroes (z). poly fits a polynomial in s to the simulations.
 * 1.1.03 1/20/2024
     * Better error checking
     * API uses parameter names kI, kP, kF
 * 1.1.02 12/27/2023
     * Fix bug in dependencies. Update header documentation.
 * 1.1.01 12/27/2023
     * Complete change in the architecture. Instead of using NonlinearIOSystems in the python control package, controlSBML generates Antimony code to implement staircase functions and closed loops.
```

### Comparing `controlSBML-1.1.3/pyproject.toml` & `controlsbml-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "controlSBML"
-version = "1.1.03"
+version = "1.2.0"
 description = "Control analysis of SBML models"
 authors = [{ name = "Joseph Hellerstein", email = "joseph.hellerstein@gmail.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.6"
 
 dependencies = [
```

### Comparing `controlSBML-1.1.3/src/controlSBML/antimony_builder.py` & `controlsbml-1.2.0/src/controlSBML/antimony_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 import controlSBML.constants as cn
 from controlSBML import util
 
 import numpy as np
 import re
 import tellurium as te  # type: ignore
+from typing import Optional
 
 IN = "_in"
 OT = "_ot"
 
 
 class AntimonyBuilder(object):
 
@@ -59,23 +60,24 @@
         Args:
             antimony: str (Antimony)
             symbol_dct: dict
                 key: str (symbol name)
                 value: str (symbol type)
         """
         self.antimony = antimony
-        self.antimony_strs = antimony.split("\n")
+        self.antimony_strs = self.antimony.split("\n")
         self.insert_pos = self._findMainModelEndPosition()  ## Add
         ##self.control_module_name = self._calculateControlModuleName(control_module_name)
         self._initialized_output = False
         # Find the main module
-        rr = te.loada(antimony)
+        self.roadrunner = te.loada(antimony)
         if symbol_dct is None:
-            symbol_dct = util.makeRoadrunnerSymbolDct(rr)
+            symbol_dct = util.makeRoadrunnerSymbolDct(self.roadrunner)
         self.symbol_dct = dict(symbol_dct)
+        self.closed_loop_symbols = []
 
     def copy(self):
         """
         Returns:
             AntimonyBuilder
         """
         builder = AntimonyBuilder(self.antimony, symbol_dct=self.symbol_dct.copy())
@@ -173,24 +175,29 @@
         return "\n".join([str(o) for o in self.antimony_strs])
 
     def addStatement(self, statement):
         """
         Args:
             statement: str
         """
-        def insert(stg, increment=1):
-            self.antimony_strs.insert(self.insert_pos, stg)
-            self.insert_pos += increment
-        #
         if not self._initialized_output:
-            self._initialized_output = True
-            insert("")
-            insert("//vvvvvvvvvAdded by ControlSBMLvvvvvvvvvv")
-            insert("//^^^^^^^^^Added by ControlSBML^^^^^^^^^^", increment=0)
-        insert(statement)
+            self.initializeOutput()
+        self._insert(statement)
+
+    def _insert(self, stg, increment=1):
+        self.antimony_strs.insert(self.insert_pos, stg)
+        self.insert_pos += increment
+
+    def initializeOutput(self):
+        self.antimony_strs = self.antimony.split("\n")
+        self.insert_pos = self._findMainModelEndPosition()
+        self._initialized_output = True
+        self._insert("")
+        self._insert("//vvvvvvvvvAdded by ControlSBMLvvvvvvvvvv")
+        self._insert("//^^^^^^^^^Added by ControlSBML^^^^^^^^^^", increment=0)
 
     def makeBoundarySpecies(self, species_name):
         """
         Args:
             species_name: str
         """
         self.symbol_dct[species_name] = cn.TYPE_BOUNDARY_SPECIES
@@ -233,21 +240,22 @@
             generic_name (_type_): _description_
             input_name (_type_): _description_
             output_name (_type_): _description_
         """
         suffix = self.makeClosedLoopSuffix(input_name, output_name)
         return "%s%s" % (generic_name, suffix)
     
-    def makeAdditionStatement(self, *pargs, is_assignment=True):
+    def makeAdditionStatement(self, *pargs, is_assignment=True, comment=""):
         """
         Creates an addition statement that looks for a leanding "-".
 
         Args:
             *pargs: str
             is_assignment: bool (True means that the statement is an assignment statement)
+            comment: str
         """
         statement = pargs[0]
         if is_assignment:
             statement += " := "
         else:
             statement += " = "
         for idx, argument in enumerate(pargs[1:]):
@@ -258,70 +266,121 @@
                 else:
                     statement += " - " + argument_str[1:]
             else:
                 if idx > 0:
                     statement += " + " + argument_str
                 else:
                     statement += argument_str
+        if len(comment) > 0:
+            statement = statement + "  # " + comment
         self.addStatement(statement) 
 
-    def makeSinusoidSignal(self, amplitude, frequency, prefix="sinusoid", suffix=""):
+    def oldmakeSinusoidSignal(self, amplitude, frequency, is_offset_amplitude=True, prefix="sinusoid", suffix=""):
         """
         Makes a sinusoid. The created variable is prefix + suffix + "_ot"
         Prefix is used to scope within a control loop. Suffix is used to scope between control loops.
 
         Args:
             amplitude: float
             frequency: float
+            is_offset_amplitude: bool (True means that the signal is offset by its amplitude)
             prefix: str (beginning of the name)
             suffix: str (ending of the name)
         Returns:
             str: name of the sinusoid
         """
         self.addStatement("")
         self.makeComment("Make sinusoid: amplitude=%s, frequency=%s" % (str(amplitude), str(frequency)))
         name = prefix +  suffix +  OT
         statement = "%s := %f*sin(2*pi*%f*time)" % (name, amplitude, frequency)
+        if is_offset_amplitude:
+            statement += " + %f" % (amplitude)
         self.addStatement(statement) 
         return name
-    
-    def _makeInputOutputNames(self, prefix, suffix):
-        base_name = prefix + suffix
+
+    def makeNoiseElement(self, noise:cn.NoiseSpec, prefix:str="sinusoid", suffix:str="")->str:
+        """
+        Makes a sinusoid with random noise and a ramp. The created variable is prefix + suffix + "_ot"
+        Prefix is used to scope within a control loop. Suffix is used to scope between control loops.
+
+        Args:
+            noise: cn.NoiseSpec (noise specification)
+            prefix: str (beginning of the name)
+            suffix: str (ending of the name)
+        Returns:
+            str: name of the sinusoid
+        """
+        self.addStatement("")
+        self.makeComment("Make sinusoid: %s" % str(noise))
+        new_suffix = suffix + OT
+        name = self._makeScopedName(prefix, new_suffix)
+        statement = "%s := 0" % (name)
+        if (not np.isclose(noise.sine_amp, 0)) and (not np.isclose(noise.sine_freq, 0)):
+            statement += " + %f*sin(2*pi*%f*time)" % (noise.sine_amp, noise.sine_freq)
+        if not np.isclose(noise.random_mag, 0):
+            statement += " + %f*lognormal(0, %f)" % (noise.random_mag, noise.random_std)
+        if not np.isclose(noise.offset, 0):
+            statement += " + %f" % noise.offset
+        if not np.isclose(noise.slope, 0):
+            statement += " + %f*time" % noise.slope
+        self.addStatement(statement) 
+        return name
+
+    def _makeScopedName(self, prefix, suffix, is_symbol=True):
+        name = prefix + suffix
+        if is_symbol:
+            self.closed_loop_symbols.append(name)
+        return name
+
+    def _makeInputOutputName(self, prefix, suffix):
+        base_name = self._makeScopedName(prefix, suffix, is_symbol=False)
         name_in = base_name + IN
+        self.closed_loop_symbols.append(name_in)
         name_ot = base_name + OT
+        self.closed_loop_symbols.append(name_ot)
         return name_in, name_ot
-    
-    def makeFilterElement(self, kf, prefix="filter", suffix=""):
+
+    def makeFilterElement(self, kF:float, prefix:str="filter", suffix:str="", kF_nofilter=100):
         """
         Makes a filter. prefix + suffix + IN is the input and prefix + suffix + OT is the output.
         Prefix is used to scope within a control loop. Suffix is used to scope between control loops.
 
         Args:
-            kf: float
+            kF: float
             prefix: str (beginning of the name)
             suffix: str (ending of the name)
+            kF_nofilter: float (value of kF when no filter is used)
         Returns:
             str: name of the filter input
             str: name of the filter output
+            str: filter derivative calculation
         Usage:
             suffix = "_S1_S3"
             name_in, name_ot = self.makeFilter(0.5, suffix=suffix)
             self.makeAddition(name_in, "S3")   # S3 is the output of the system
             self.makeAddition("control_error", setpoint, "-"+name_ot)
         """
+        #
         self.addStatement("")
-        self.makeComment("Filter: kf=%s" % (str(kf)))
-        name_in, name_ot = self._makeInputOutputNames(prefix, suffix)
-        if (kf is not None) and (kf > 0):
-            statement = "%s' =  -%f*%s + %f*%s" % (name_ot, kf, name_ot, kf, name_in)
-            self.addStatement(statement)
-            self.makeAdditionStatement(name_ot, 0, is_assignment=False)   # Initialize the filter output
+        self.makeComment("Make filter: kF=%s" % (str(kF)))
+        kF_name = self._makeScopedName("kF", suffix)
+        name_in, name_ot = self._makeInputOutputName(prefix, suffix)
+        if (kF is None) or np.isclose(kF, 0):
+            new_kF = kF_nofilter
         else:
-            self.makeAdditionStatement(name_ot, name_in)
-        return name_in, name_ot
+            new_kF = kF
+        self.makeAdditionStatement(kF_name, new_kF, is_assignment=False)
+        # Construct the filter calculation
+        filter_derivative_calculation = f"-{kF_name}*{name_ot} + {kF_name}*{name_in}"
+        # Use a dummy reaction to integrate instead of "'" to avoid antimony limitations with
+        # combining rate rules and assignment rules
+        statement = " -> %s; %s " % (name_ot, filter_derivative_calculation) 
+        self.addStatement(statement)
+        self.makeAdditionStatement(name_ot, 0, is_assignment=False)   # Initialize the filter output
+        return name_in, name_ot, filter_derivative_calculation
     
     def makeControlErrorSignal(self, setpoint, forward_output_name, sign, prefix="control_error", suffix=""):
         """
         Constructs the control error variable.
 
         Args:
             setpoint: float/str
@@ -331,96 +390,149 @@
             suffix: str (ending of the name)
         Returns:
             str (name of the control error)
         Usage:
             suffix = "_S1_S3"
             control_error_name = self.makeControlError(setpoint, "S3", suffix=suffix)   # S3 is the output of the system
         """
-        name_ot = prefix + suffix + OT
+        self.addStatement("")
+        self.makeComment("Make the control error")
+        new_suffix = suffix + OT
+        name_ot = self._makeScopedName(prefix, new_suffix)
         if sign == 1:
-            operator = "+"
+            statement = "%s := %s - %s" % (name_ot, forward_output_name, str(setpoint))
+        elif sign == -1:
+            statement = "%s := %s - %s" % (name_ot, str(setpoint), forward_output_name)
         else:
-            operator = "-"
-        statement = "%s := %s %s %s" % (name_ot, str(setpoint), operator, forward_output_name)
+            raise ValueError("Invalid sign: %s" % sign)
         self.addStatement(statement)
         return name_ot
     
-    def makePIControllerElement(self, kp=None, ki=None, prefix="controller", suffix=""):
+    def makePIDControllerElement(self,
+                                 filter_derivative_calculation:str,
+                                 kP:Optional[float]=None,
+                                 kI:Optional[float]=None,
+                                 kD:Optional[float]=None,
+                                 prefix:Optional[str]="controller",
+                                 suffix:Optional[str]="",
+                                 sign:Optional[int]=-1):
         """
-        Makes a PI controller. prefix + suffix + IN is the input and prefix + suffix + OT is the output.
+        Makes a PID controller. prefix + suffix + IN is the input and prefix + suffix + OT is the output.
         Prefix is used to scope within a control loop. Suffix is used to scope between control loops.
+        Assumes there is no filter.
 
         Args:
-            kp: float
-            ki: float
+            filter_derivative_calculation: str (calculation for the derivative of the filter)
+            kP: float
+            kI: float
+            kD: float
             prefix: str (beginning of the name)
             suffix: str (ending of the name)
+            sign: int (1 or -1) (1 means that the setpoint is subtracted from the output)
         Returns:
             str: name of the controller input
             str: name of the controller output
-        Usage:
-            suffix = "_S1_S3"
-            name_in, name_ot = self.makeController(kp=1, suffix=suffix)
-            control_error_name = self.makeControlError(setpoint, "S3", suffix=suffix)   # S3 is the output of the system
-            self.makeAddition(name_in, control_error_name)  # control_error is input to the controller
-            self.makeAddition("S1", name_ot)   # S1 is the input to the system and is set by the controller
         """
+        base_name = prefix + "_" +  "%s" + suffix # type: ignore
+        def makeControllerScopedName(name):
+            scoped_name = base_name % name
+            self.closed_loop_symbols.append(scoped_name)
+            return scoped_name
+        #
         self.addStatement("")
-        self.makeComment("PI Controller: kp=%s, ki=%s" % (str(kp), str(ki)))
-        name_in, name_ot = self._makeInputOutputNames(prefix, suffix)
+        self.makeComment("Make the PID controller")
+        name_in, name_ot = self._makeInputOutputName(prefix, suffix)
+        # Constants for parameters
+        if kP is not None:
+            kP_name = makeControllerScopedName("kP")
+            self.makeAdditionStatement(kP_name, str(kP), is_assignment=False)
+        if kI is not None:
+            kI_name = makeControllerScopedName("kI")
+            self.makeAdditionStatement(kI_name, str(kI), is_assignment=False)
+        if kD is not None:
+            kD_name = makeControllerScopedName("kD")
+            self.makeAdditionStatement(kD_name, str(kD), is_assignment=False)
+        # Make the derivative of the control error
+        if kD is not None:
+            derivative_error_name = base_name % "derivative_error"
+            self.closed_loop_symbols.append(derivative_error_name)
+            sign_filter_calculation = f"{sign}*{filter_derivative_calculation}"
+            statement = "%s := %s" % (derivative_error_name, sign_filter_calculation)  # type: ignore
+            self.addStatement(statement)
         # Make the integral of the control error
-        integral_error_name = prefix + "_integral_error" + suffix
-        statement = "%s' = %s" % (integral_error_name, name_in)
-        self.addStatement(statement)
-        self.makeAdditionStatement(integral_error_name, 0, is_assignment=False)   #  integral_error_name = 0
+        if kI is not None:
+            integral_error_name = base_name % "integral_error"
+            self.closed_loop_symbols.append(integral_error_name)
+            statement = "%s' = %s" % (integral_error_name, name_in)
+            self.addStatement(statement)
+            self.makeAdditionStatement(integral_error_name, 0, is_assignment=False)   #  integral_error_name = 0
         # Construct the control law
-        if kp is not None:
-            statement = "%s := %f*%s" % (name_ot, kp, name_in)
+        if kP is not None:
+            statement = "%s := %s*%s" % (name_ot, kP_name, name_in)
         else:
             statement = "%s = 0" % name_ot
-        if ki is not None:
-            statement = statement + "+ %f*%s" % (ki, integral_error_name)
+        if kI is not None:
+            statement = statement + " + %s*%s" % (kI_name, integral_error_name)
+        if kD is not None:
+            statement = statement + " + %s*%s" % (kD_name, derivative_error_name)
         self.addStatement(statement)
         return name_in, name_ot
 
-    def makeSISOClosedLoopSystem(self, input_name, output_name, kp=None, ki=None, kf=None, setpoint=0,
-                           noise_amplitude=0, noise_frequency=20, disturbance_ampliude=0, disturbance_frequency=20,
+    def makeSISOClosedLoopSystem(self, input_name, output_name, kP=None, kI=None, kD=None, kF=None, setpoint=0,
+                           noise_spec=cn.NoiseSpec(), disturbance_spec=cn.DisturbanceSpec(),
                            initial_output_value=None, sign=-1):
         """
+        Creates a closed loop system with a single input and a single output. Does not create a filter
+        if kF is in [0, None]
+
         Args:
             input_name: str (input to system)
             output_name: str (output from system)
-            kp: float
-            ki: float
-            kd: float
-            kf: float
+            kP: float
+            kI: float
+            kD: float
+            kF: float
             setpoint: float (setpoint)
-            noise_amplitude: float (Amplitude of the additions to the output)
-            noise_frequency: float (Frequency of the additions to the output)
-            disturbance_amplitude: float (Amplitude of the disturbance)
-            disturbance_frequency: float (Frequency of the disturbance)
+            noise_spec: cn.NoiseSpec
+            disturbance_spec: cn.DisturbanceSpec
             initial_input_value: float (initial value of the input)
         """
+        self.addStatement("")
+        self.makeComment("**CREATING CLOSED LOOP SYSTEM**")
         suffix = self.makeClosedLoopSuffix(input_name, output_name)
+        # Symbol for setpoint
+        setpoint_name = self._makeScopedName("setpoint", suffix)
+        self.makeAdditionStatement(setpoint_name, setpoint, is_assignment=False)
         # Handle the initial value of the input
-        if initial_output_value is not None:
-            self.makeAdditionStatement(output_name, initial_output_value, is_assignment=False)
+        if initial_output_value is None:
+            initial_output_value = self.roadrunner[output_name]
+        self.makeAdditionStatement(output_name, initial_output_value, is_assignment=False)
         # Make the elements of the closed loop
-        noise_ot = self.makeSinusoidSignal(noise_amplitude, noise_frequency, prefix="noise", suffix=suffix)
-        disturbance_ot = self.makeSinusoidSignal(disturbance_ampliude, disturbance_frequency, prefix="disturbance", suffix=suffix)
-        filter_in, filter_ot = self.makeFilterElement(kf, prefix="filter", suffix=suffix)
-        controller_in, controller_ot = self.makePIControllerElement(kp, ki, prefix="controller", suffix=suffix)
-        control_error_name = self.makeControlErrorSignal(setpoint, filter_ot, sign, prefix="control_error", 
+        noise_ot = self.makeNoiseElement(noise_spec, prefix="noise", suffix=suffix)
+        disturbance_ot = self.makeNoiseElement(disturbance_spec, prefix="disturbance", suffix=suffix)
+        filter_in, filter_ot, filter_derivative_calculation =   \
+              self.makeFilterElement(kF, prefix="filter", suffix=suffix)
+        controller_in, controller_ot = self.makePIDControllerElement(
+              filter_derivative_calculation,
+              kP=kP, kI=kI, kD=kD, prefix="controller", suffix=suffix, sign=sign)
+        if filter_ot is None:
+            comparison_signal_str = "(" + output_name + " + " + noise_ot + ")"
+        else:
+            comparison_signal_str = filter_ot
+        control_error_name = self.makeControlErrorSignal(setpoint_name,
+                                                         comparison_signal_str,
+                                                         sign, prefix="control_error", 
                                                          suffix=suffix)
         # Connect the pieces by specifying assignment statements
         self.addStatement("")
         self.makeComment("Connect the elements of the closed loop")
         self.makeAdditionStatement(controller_in, control_error_name)
         self.makeAdditionStatement(input_name, controller_ot, disturbance_ot)
-        self.makeAdditionStatement(filter_in, output_name, noise_ot)
+        if filter_in is not None:
+            self.makeAdditionStatement(filter_in, output_name, noise_ot)
     
     def getInputManipulationName(self, input_name):
         """
         Constructs the name of the input that is being manipulated since floating species can be manipulated
         by a boundary reaction rate.
 
         Args:
@@ -429,14 +541,29 @@
         if (input_name in self.floating_species_names):
             # The input is a floating species that is being controlled by a boundary reaction
             name = self.makeParameterNameForBoundaryReaction(input_name)
         else:
             name = input_name
         return name
 
+    def _getClosedLoopSymbols(self, input_name, output_name)->list[str]:
+        """
+        Finds the names of closed loop symbols used for the system defined with the current input and output.
+        This method is used for validation purposes only.
+
+        Returns:
+            input_name: str
+            output_name: str
+            list[str]: list of symbols
+        """
+        search_string = self.makeClosedLoopSuffix(input_name, output_name)
+        rr = te.loada(str(self))
+        symbols = [n for n in rr.keys() if (search_string in n) and (not "(" in n) and (not "[" in n)]
+        return symbols
+
     def makeStaircase(self, input_name, times=cn.TIMES, initial_value=cn.DEFAULT_INITIAL_VALUE,
                  num_step=cn.DEFAULT_NUM_STEP, final_value=cn.DEFAULT_FINAL_VALUE):
         """
         Adds events for the staircase.
         Args:
             species_name: str
             initial_value: float (value for first step)
```

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/__init__.py` & `controlsbml-1.2.0/src/controlSBML/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/control_analysis.py` & `controlsbml-1.2.0/src/controlSBML/archive/control_analysis.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/control_base.py` & `controlsbml-1.2.0/src/controlSBML/archive/control_base.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/control_plot.py` & `controlsbml-1.2.0/src/controlSBML/archive/control_plot.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/control_sbml.py` & `controlsbml-1.2.0/src/controlSBML/archive/control_sbml.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         if "input_names" not in kwargs:
             kwargs["input_names"] = self.input_names
         if "output_names" not in kwargs:
             kwargs["output_names"] = self.output_names
         return NonlinearIOSystem(name, self, **kwargs)
     
     @Expander(cn.KWARGS, cn.SIM_KWARGS)
-    def makeMIMOTransferFunctionDF(self, num_numerator=cn.DEFAULT_NUM_NUMERATOR, num_denominator=cn.DEFAULT_NUM_DENOMINATOR,
+    def makeMIMOTransferFunctionDF(self, num_numerator=cn.DEFAULT_NUM_ZERO, num_denominator=cn.DEFAULT_NUM_POLE,
                  staircase=None, 
                  is_fixed_input_species=False, do_simulate_on_update=False,
                  is_steady_state=True, **kwargs):
         """
         Constructs transfer functions between all inputs and outputs.
 
         Parameters
@@ -149,15 +149,15 @@
         transfer_function_df = fitter_result_df.copy()
         for input_name in transfer_function_df.index:
             for output_name in transfer_function_df.columns:
                 transfer_function_df.loc[input_name, output_name] = fitter_result_df.loc[input_name, output_name].transfer_function
         return transfer_function_df
     
     @Expander(cn.KWARGS, cn.ALL_KWARGS)
-    def plotBode(self, num_numerator=cn.DEFAULT_NUM_NUMERATOR, num_denominator=cn.DEFAULT_NUM_DENOMINATOR,
+    def plotBode(self, num_numerator=cn.DEFAULT_NUM_ZERO, num_denominator=cn.DEFAULT_NUM_POLE,
                  staircase=None, is_magnitude=True, is_phase=True, **kwargs):
         """
         Constructs bode plots for a MIMO system whose tansfer functions are obtained by system identification.
 
         Parameters
         ----------
         staircase:
@@ -212,15 +212,15 @@
             kwargs["is_steady_state"] = True
         response_df = builder.makeStaircaseResponse(staircase=staircase, **kwargs)
         return builder.plotStaircaseResponse(response_df, **mgr.plot_fig_options)
     
     @Expander(cn.KWARGS, cn.SIM_KWARGS)
     def fitMIMOTransferFunction(self,
             input_names=None, output_names=None, staircase=Staircase(),
-            num_numerator=cn.DEFAULT_NUM_NUMERATOR, num_denominator=cn.DEFAULT_NUM_DENOMINATOR,
+            num_numerator=cn.DEFAULT_NUM_ZERO, num_denominator=cn.DEFAULT_NUM_POLE,
             is_fixed_input_species=False,
             do_simulate_on_update=False,
             **kwargs):
         """
         Constructs transfer functions for a MIMO system whose tansfer functions are obtained by system identification.
 
         Parameters
@@ -254,15 +254,15 @@
                                                                num_denominator=num_denominator,
                                                                staircase=staircase, **new_kwargs)
         return fitter_result_df
 
     @Expander(cn.KWARGS, cn.ALL_KWARGS)
     def plotFitMIMOTransferFunction(self,
             input_names=None, output_names=None, staircase=Staircase(),
-            num_numerator=cn.DEFAULT_NUM_NUMERATOR, num_denominator=cn.DEFAULT_NUM_DENOMINATOR,
+            num_numerator=cn.DEFAULT_NUM_ZERO, num_denominator=cn.DEFAULT_NUM_POLE,
             is_fixed_input_species=False,
             do_simulate_on_update=False,
             **kwargs):
         """
         Constructs transfer functions for a MIMO system whose tansfer functions are obtained by system identification.
 
         Parameters
```

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/history.py` & `controlsbml-1.2.0/src/controlSBML/archive/history.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/iosystem_factory.py` & `controlsbml-1.2.0/src/controlSBML/archive/iosystem_factory.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/logger.py` & `controlsbml-1.2.0/src/controlSBML/archive/logger.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/mimo_transfer_function_builder.py` & `controlsbml-1.2.0/src/controlSBML/archive/mimo_transfer_function_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,16 @@
             column names: str (output)
             index: str (input)
             values: PlotResult
         """
         return cls._plotMIMO(response_df, tfb.SISOTransferFunctionBuilder.plotStaircaseResponse, **options)
     
     @Expander(cn.KWARGS, cn.SIM_KWARGS)
-    def fitTransferFunction(self, num_numerator=cn.DEFAULT_NUM_NUMERATOR, 
-                            num_denominator=cn.DEFAULT_NUM_DENOMINATOR, staircase=Staircase(), **sim_kwargs):
+    def fitTransferFunction(self, num_numerator=cn.DEFAULT_NUM_ZERO, 
+                            num_denominator=cn.DEFAULT_NUM_POLE, staircase=Staircase(), **sim_kwargs):
         """
         Constructs transfer functions for the NonlinearIOSystem.
 
         Parameters
         ----------
         num_numerator: int (number of numerator terms)
         num_denominator: int (number of denominator terms)
@@ -199,15 +199,15 @@
         fitter_dct = {n: [] for n in self.sys.output_names}
         staircase_dct = self._makeStaircaseDct(staircase)
         for output_name in self.sys.output_names:
             for input_name in self.sys.input_names:
                 sys = self.sys.getSubsystem(self.sys.name, [input_name], [output_name])
                 siso_tfb = tfb.SISOTransferFunctionBuilder(sys)
                 # FIXME: Always getting the same transfer function
-                fitter_result = siso_tfb.fitTransferFunction(num_numerator, num_denominator,
+                fitter_result = siso_tfb.plotTransferFunctionFit(num_numerator, num_denominator,
                                                              staircase=staircase_dct[input_name], **sim_kwargs)
                 fitter_dct[output_name].append(fitter_result)
         # Construct the output
         fitter_df = self._makeResultDF(fitter_dct, self.sys.input_names)
         return fitter_df
     
     @classmethod
```

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/nonlinear_io_system.py` & `controlsbml-1.2.0/src/controlSBML/archive/nonlinear_io_system.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/sequential_model.py` & `controlsbml-1.2.0/src/controlSBML/archive/sequential_model.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/simulate_system.py` & `controlsbml-1.2.0/src/controlSBML/archive/simulate_system.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/siso_closed_loop_designer.py` & `controlsbml-1.2.0/src/controlSBML/archive/siso_closed_loop_designer.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/siso_closed_loop_system.py` & `controlsbml-1.2.0/src/controlSBML/archive/siso_closed_loop_system.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/siso_design_evaluator.py` & `controlsbml-1.2.0/src/controlSBML/archive/siso_design_evaluator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Evaluates a closed loop design. Saves the best design using MSE criteria. Preserves all designs."""
 
 from controlSBML import util
 from controlSBML.sbml_system import SBMLSystem
 import controlSBML.constants as cn
 
 import numpy as np
-import pandas as pd
+import pandas as pd # type: ignore
 import os
-from typing import List
+from typing import List, Optional
 
 
 class EvaluatorResult(dict):
     # Container of evaluation results
 
-    def __init__(self, kp_spec=False, ki_spec=False, kf_spec=False):
+    def __init__(self, kp_spec=False, ki_spec=False, kf_spec=False, kd_spec=False):
         self[cn.MSE] = []
         self.attrs = [cn.MSE]
         if kp_spec:
             self[cn.CP_KP] = []
             self.attrs.append(cn.CP_KP)
         if ki_spec:
             self[cn.CP_KI] = []
             self.attrs.append(cn.CP_KI)
         if kf_spec:
             self[cn.CP_KF] = []
             self.attrs.append(cn.CP_KF)
+        if kd_spec:
+            self[cn.CP_KD] = []
+            self.attrs.append(cn.CP_KD)
 
     def __len__(self):
         keys = list(self.keys())
         if len(keys) == 0:
             return 0
         return len(self[keys[0]])
 
@@ -46,23 +49,26 @@
 
         Returns:
             EvaluatorResult
         """
         kp_spec = cn.CP_KP in dataframe.columns
         ki_spec = cn.CP_KI in dataframe.columns
         kf_spec = cn.CP_KF in dataframe.columns
-        evaluator_result = EvaluatorResult(kp_spec=kp_spec, ki_spec=ki_spec, kf_spec=kf_spec)
+        kd_spec = cn.CP_KD in dataframe.columns
+        evaluator_result = EvaluatorResult(kp_spec=kp_spec, ki_spec=ki_spec, kf_spec=kf_spec, kd_spec=kd_spec)
         for _, row in dataframe.iterrows():
             kwargs = {cn.MSE: row[cn.MSE]}
             if kp_spec:
                 kwargs[cn.CP_KP] = row[cn.CP_KP]
             if ki_spec:
                 kwargs[cn.CP_KI] = row[cn.CP_KI]
             if kf_spec:
                 kwargs[cn.CP_KF] = row[cn.CP_KF]
+            if kd_spec:
+                kwargs[cn.CP_KD] = row[cn.CP_KD]
             evaluator_result.add(**kwargs)
         return evaluator_result
     
     def writeCsv(self, file_path):
         df = self.getDataframe()
         df.to_csv(file_path, index=False)
 
@@ -74,14 +80,16 @@
         evaluator_result[cn.MSE] = list(self[cn.MSE])
         if cn.CP_KP in self:
             evaluator_result[cn.CP_KP] = list(self[cn.CP_KP])
         if cn.CP_KI in self:
             evaluator_result[cn.CP_KI] = list(self[cn.CP_KI])
         if cn.CP_KF in self:
             evaluator_result[cn.CP_KF] = list(self[cn.CP_KF])
+        if cn.CP_KD in self:
+            evaluator_result[cn.CP_KD] = list(self[cn.CP_KD])
         return evaluator_result
 
     @classmethod
     def merge(cls, evaluator_results):
         """
         Merges multiple evaluator results.
 
@@ -98,26 +106,28 @@
                 merged_result[key].extend(results[key])
         return merged_result
 
 
 class SISODesignEvaluator:
     # Evaluates designs and remembers the best one
 
-    def __init__(self, system:SBMLSystem, input_name, output_name, setpoint:float=1, times:List[float]=cn.TIMES,
+    def __init__(self, system:SBMLSystem, input_name, output_name, setpoint:float=1, 
+                 times:List[float]=cn.TIMES,  # type: ignore
                  save_path=None):
         self.system = system
         self.setpoint = setpoint
         self.times = times
         self.input_name = input_name
         self.output_name = output_name
         self.save_path = save_path
         # Best results
         self.kp = None
         self.ki = None
         self.kf = None
+        self.kd = None
         self.residual_mse = None
         # All results
         self.evaluator_result = None
 
     @classmethod
     def merge(cls, evaluators):
         """
@@ -125,14 +135,15 @@
 
         Args:
             evaluators (_type_): _description_
         """
         def update(evaluator, merged_evaluator):
             merged_evaluator.kp = evaluator.kp
             merged_evaluator.ki = evaluator.ki
+            merged_evaluator.kd = evaluator.kd
             merged_evaluator.kf = evaluator.kf
             merged_evaluator.residual_mse = evaluator.residual_mse
         #
         merged_evaluator = evaluators[0]
         #merged_evaluator = merged_evaluator.copy(is_set_outputs=True)
         merged_evaluator = merged_evaluator.copy()
         results = [e.evaluator_result for e in evaluators]
@@ -141,26 +152,18 @@
         ser = df[cn.MSE].dropna()
         min_mse = np.min(ser)
         idx = ser[ser == min_mse].index[0]
         if cn.CP_KP in df.columns:
             merged_evaluator.kp = df[cn.CP_KP].values[idx]
         if cn.CP_KI in df.columns:
             merged_evaluator.ki = df[cn.CP_KI].values[idx]
+        if cn.CP_KD in df.columns:
+            merged_evaluator.kd = df[cn.CP_KD].values[idx]
         if cn.CP_KF in df.columns:
             merged_evaluator.kf = df[cn.CP_KF].values[idx]
-        if False:
-            for evaluator in evaluators:
-                if evaluator.residual_mse is None:
-                    continue
-                if merged_evaluator.residual_mse is None:
-                    update(evaluator, merged_evaluator)
-                    continue
-                if evaluator.residual_mse < merged_evaluator.residual_mse:
-                    update(evaluator, merged_evaluator)
-                    continue
         return merged_evaluator
         
     def copy(self, is_set_outputs:bool=True):
         """
         Args:
             is_set_outputs (bool, optional): copy the outputs. Defaults to True.
         """
@@ -169,19 +172,21 @@
         if evaluator.evaluator_result is not None:
             evaluator.evaluator_result = self.evaluator_result.copy()
         else:
             evaluator.evaluator_result = None
         if is_set_outputs:
             evaluator.kp = self.kp
             evaluator.ki = self.ki
+            evaluator.kd = self.kd
             evaluator.kf = self.kf
             evaluator.residual_mse = self.residual_mse
         return evaluator
 
-    def evaluate(self, kp:float=None, ki:float=None, kf:float=None):
+    def evaluate(self, kp:Optional[float]=None, ki:Optional[float]=None, kf:Optional[float]=None,
+                 kd:Optional[float]=None) -> bool:
         """
         Evaluates the closed loop system. Updates the control parameters if the design is better.
 
         Args:
             kp: float (proportional gain)
             ki: float (integral gain)
             kf: float (feedforward gain)
@@ -194,25 +199,25 @@
         #
         # Initialization
         if self.evaluator_result is None:
             if (self.save_path is not None) and (os.path.isfile(self.save_path)):
                 df = pd.read_csv(self.save_path)
                 self.evaluator_result = EvaluatorResult.makeFromDataframe(df)
             else:
-                self.evaluator_result = EvaluatorResult(kp_spec=kp, ki_spec=ki, kf_spec=kf)
+                self.evaluator_result = EvaluatorResult(kp_spec=kp, ki_spec=ki, kf_spec=kf, kd_spec=kd)  # type: ignore
         # Evaluate the design
-        value_dct = {cn.CP_KP: kp, cn.CP_KI: ki, cn.CP_KF: kf}
+        value_dct = {cn.CP_KP: kp, cn.CP_KI: ki, cn.CP_KF: kf, cn.CP_KD: kd}
         original_value_dct = dict(value_dct)
         for key, value in original_value_dct.items():
             if value is None:
                 del value_dct[key]
-        is_feasible, residual_mse = self.calculateMse(**value_dct)
+        is_feasible, residual_mse = self.calculateMse(**value_dct)  # type: ignore
         # Save the results
-        self.evaluator_result.add(**value_dct, mse=residual_mse)
-        self.evaluator_result.writeCsv(self.save_path)
+        self.evaluator_result.add(mse=residual_mse, **value_dct)  # type: ignore
+        self.evaluator_result.writeCsv(self.save_path)            # type: ignore
         if not is_feasible:
             return False
         if self.residual_mse is None:
             update(residual_mse=residual_mse, **value_dct)
         elif residual_mse < self.residual_mse:
             update(residual_mse=residual_mse, **value_dct)
         return True
@@ -220,26 +225,26 @@
     def calculateMse(self, max_output:float=1e6, min_output:float=0, **parameter_dct:dict):
         """
         Attempts to calculate the mean squared error of the closed loop system. Reports if system is unstable.
 
         Args:
             max_output: float (maximum output)
             min_output: float (minimum output)
-            parameter_dct: dict: {name: value for eack of kp, ki, kf}
+            parameter_dct: dict: {name: value for eack of kp, ki, kd, kf}
 
         Returns:
             bool (successful simulation)
             float (mean squared error)
         """
         try:
             response_ts, _ = self.system.simulateSISOClosedLoop(setpoint=self.setpoint,
                         input_name=self.input_name, output_name=self.output_name,
                         times=self.times,
                         is_steady_state=self.system.is_steady_state, inplace=False,
-                        **parameter_dct)
+                        **parameter_dct)  # type: ignore
         except Exception:
             return False, None
         # Check for large outputs
         outputs = response_ts[self.output_name].values
         max_value = np.max([np.max(outputs), np.abs(np.min(outputs))])
         min_value = np.min([np.max(outputs), np.abs(np.min(outputs))])
         if (max_value > max_output) or (min_value < min_output):
@@ -251,30 +256,32 @@
         #
         residuals = self.setpoint - response_ts[self.output_name].values
         mse = np.mean(residuals**2)
         return True, mse
     
     @classmethod
     def makeFromDataframe(cls, system:SBMLSystem, input_name:str, output_name:str, dataframe:pd.DataFrame,
-                setpoint:float=1, times:List[float]=cn.TIMES,
+                setpoint:float=1, times:np.ndarray[float]=cn.TIMES,  # type: ignore
                 save_path=None):
         """
         Creates a SISODesignEvaluator object from a dataframe
 
         Args:
             dataframe (dataframe): columns: kp, ki, kf, mse
 
         Returns:
             EvaluatorResult
         """
         evaluator = cls(system, input_name, output_name,
-                setpoint=setpoint, times=times, save_path=save_path)
+                setpoint=setpoint, times=times, save_path=save_path)  # type: ignore
         evaluator_result = EvaluatorResult.makeFromDataframe(dataframe)
         df = dataframe.sort_values(cn.MSE)
         if cn.CP_KP in df.columns:
             evaluator.kp = df[cn.CP_KP].values[0]
         if cn.CP_KI in df.columns:
             evaluator.ki = df[cn.CP_KI].values[0]
+        if cn.CP_KD in df.columns:
+            evaluator.kd = df[cn.CP_KD].values[0]
         if cn.CP_KF in df.columns:
             evaluator.kf = df[cn.CP_KF].values[0]
         evaluator.residual_mse = df[cn.MSE].values[0]
         return evaluator
```

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/siso_transfer_function_builder.py` & `controlsbml-1.2.0/src/controlSBML/archive/siso_transfer_function_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,16 +300,16 @@
     def _getStaircaseColumnName(timeseries):
         all_columns = set(timeseries.columns)
         other_columns = [c for c in timeseries.columns if STAIRCASE not in c]
         staircase_column = list(all_columns.difference(other_columns))[0]
         return staircase_column, other_columns
 
     @Expander(cn.KWARGS, cn.SIM_KWARGS)
-    def fitTransferFunction(self, num_numerator=cn.DEFAULT_NUM_NUMERATOR,
-                            num_denominator=cn.DEFAULT_NUM_DENOMINATOR, staircase=Staircase(), 
+    def fitTransferFunction(self, num_numerator=cn.DEFAULT_NUM_ZERO,
+                            num_denominator=cn.DEFAULT_NUM_POLE, staircase=Staircase(), 
                             fit_start_time=None, fit_end_time=None, **kwargs):
         """
         Constructs a transfer function for the NonlinearIOSystem.
 
         Parameters
         ----------
         num_numerator: int (number of numerator terms)
```

### Comparing `controlSBML-1.1.3/src/controlSBML/archive/temporal_series.py` & `controlsbml-1.2.0/src/controlSBML/archive/temporal_series.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/constants.py` & `controlsbml-1.2.0/src/controlSBML/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,55 @@
 from docstring_expander.kwarg import Kwarg # type: ignore
 import matplotlib.pyplot
 import numpy as np
 import pandas as pd # type: ignore
 import os
 
 
-DEFAULT_NUM_STEP = 5
-
+##########################
 # Classes
+##########################
+class NoiseSpec(object):
+    # Specifications for a noise model
+    def __init__(self, sine_amp=0, sine_freq=0, random_mag=0, random_std=0, offset=None, slope=0):
+        """_summary_
+
+        Args:
+            sine_amp (int, optional): Amplitude of the sine wave. Defaults to 0.
+            sine_freq (int, optional): Frequency of the sine wave. Defaults to 0.
+            random_mag (int, optional): Magnitude scalinging of the log-normal random variable. Defaults to 0.
+            random_std (int, optional): Standard deviation of the normal for the log-normal random variable added to the function. Defaults to 0.
+            offset (int, optional): Constant offset. Defaults to  sine_amp.
+            slope (int, optional): Slope w.r.t. time. Defaults to 0.
+        """
+        self.sine_amp = sine_amp
+        self.sine_freq = sine_freq
+        self.random_mag = random_mag
+        self.random_std = random_std
+        if offset is None:
+            if (np.isclose(sine_amp, 0) and np.isclose(slope, 0)):
+                offset = sine_amp
+            else:
+                offset = 0
+        self.offset = offset
+        self.slope = slope
+
+    def __str__(self):
+        result = f"NoiseSpec(sine_amp={self.sine_amp}, sine_freq={self.sine_freq}, random_mag={self.random_mag}"
+        result += f" random_std={self.random_std}, dc_gain={self.offset}, slope={self.slope})"
+        return result
+    
+    def __eq__(self, other):
+        return self.__dict__ == other.__dict__
+
+class DisturbanceSpec(NoiseSpec):
+    # Specifications for a disturbance model
+    pass
+
+
 class LegendSpec():
 
     def __init__(self, names, crd=(1.15, 1), loc="upper right"):
         """
 
         Parameters
         ----------
@@ -58,123 +96,220 @@
 ################ DIRECTORIES #################
 PROJECT_DIR = os.path.dirname(os.path.abspath(__file__))
 for _ in range(2):
   PROJECT_DIR = os.path.dirname(PROJECT_DIR)
 CODE_DIR = os.path.join(PROJECT_DIR, "controlSBML")
 PLOT_DIR = PROJECT_DIR
 TEST_DIR = os.path.join(PROJECT_DIR, "tests")
+MODEL_DIR = os.path.join(PROJECT_DIR, "models")
 NOTEBOOK_DIR = os.path.join(PROJECT_DIR, "notebooks")
 DATA_DIR = os.path.join(PROJECT_DIR, "data")
 BIOMODELS_ZIP_FILENAME = "biomodels.zip"
+MTOR_PATH = os.path.join(MODEL_DIR, "Varusai2018.xml")
+WOLF_PATH = os.path.join(MODEL_DIR, "BIOMD0000000206.xml")
 
 # Constants
 END_TIME = 5.0  # Default endtime
 EVENT = "event"
+FITTER_METHOD = "fitter_method"
 INPUT = "input"
 IN = "in"
-IS_PLOT = False
+IS_PLOT = "is_plot"
 MAX = "max"
 MIN = "min"
 MSE = "mse"
 OUT = "out"
 OUTPUT = "output"
 OUT_STATE = "out_state"
 PARAMS = "params"
 POINTS_PER_TIME = 10
+REASON = "reason"
 SCORE = "score"
-SETPOINT = "setpoint"
 START_TIME = 0.0  # Default start time
 STATE = "state"
 STEP_VAL = 1  # Multiplier used for simulation input
 TIME = "time"
 
 # Keyword options
 O_AX = "ax"
 O_AX2 = "ax2"
+O_DISTURBANCE_SPEC = "disturbance_spec"
 O_END_TIME = "end_time"
 O_FIGURE = "figure"
 O_FIGSIZE = "figsize"
-O_STEP_VAL = "step_val"
+O_FINAL_VALUE = "final_value"
+O_FITTER_METHOD = "fitter_method"
+O_KP_SPEC = "kP_spec"
+O_KI_SPEC = "kI_spec"
+O_KD_SPEC = "kD_spec"
+O_KF_SPEC = "kF_spec"
+O_INITIAL_VALUE = "initial_value"
+O_INPUT_NAME = "input_name"
+O_INPUT_NAMES = "input_names"
+O_IS_GREEDY = "is_greedy"
+O_IS_FIXED_INPUT_SPECIES = "is_fixed_input_species"
+O_IS_STEADY_STATE = "is_steady_state"
 O_IS_PLOT = "is_plot"
+O_LEGEND = "legend"
 O_LEGEND_CRD = "legend_crd"  # Legend coordinate
 O_LEGEND_SPEC = "legend_spec"
+O_MARKERS = "markers"
+O_MARKERSIZE = "markersize"
+O_NOISE_SPEC = "noise_spec"
+O_NUM_POINT = "num_point"
+O_NUM_PROCESS = "num_process"
+O_NUM_RESTART = "num_restart"
+O_NUM_STEP = "num_step"
+O_OUTPUT_NAME = "output_name"
+O_OUTPUT_NAMES = "output_names"
 O_POINTS_PER_TIME = "points_per_time"
 O_PREDICTED = "predicted"
+O_SELECTIONS = "selections"   # Selections for the plot
+O_SETPOINT = "setpoint"
+O_SIGN = "sign"
 O_STAIRCASE = "staircase"
 O_START_TIME = "start_time"
+O_STEP_VAL = "step_val"
 O_SUPTITLE = "suptitle"
+O_TIMES = "times"
 O_TITLE = "title"
 O_WRITEFIG = "writefig"  # Write the figure
 O_XLABEL = "xlabel"
+O_XLABEL_ANGLE = "xlabel_angle"
 O_XLIM = "xlim"
 O_XTICKLABELS = "xticklabels"
 O_YLABEL = "ylabel"
 O_YLIM = "ylim"
 O_YTICKLABELS = "yticklabels"
 
 # Control parameters
 CP_KP = "kP"
 CP_KI = "kI"
 CP_KF = "kF"
-CONTROL_PARAMETERS = [CP_KP, CP_KI, CP_KF]
+CP_KD = "kD"
+CONTROL_PARAMETERS = [CP_KP, CP_KI, CP_KD, CP_KF]
 KP_SPEC = "kP_spec"
 KI_SPEC = "kI_spec"
+KD_SPEC = "kD_spec"
 KF_SPEC = "kF_spec"
-CONTROL_PARAMETER_SPECS = [KP_SPEC, KI_SPEC, KF_SPEC]
+CONTROL_PARAMETER_SPECS = [KP_SPEC, KI_SPEC, KD_SPEC, KF_SPEC]
+
+# URLs
+WOLF_URL = "https://www.ebi.ac.uk/biomodels/services/download/get-files/MODEL3352181362/2/BIOMD0000000206_url.xml"
+METFORMIN_URL = "https://www.ebi.ac.uk/biomodels/model/download/BIOMD0000001039.5?filename=Zake2021_Metformin%2BMice%2BIV.xml"
+MTOR_URL = "https://www.ebi.ac.uk/biomodels/model/download/BIOMD0000000823.2?filename=Varusai2018.xml"
+
+# Transfer function building
+DEFAULT_NUM_ZERO = 1
+DEFAULT_NUM_POLE = 3
+DEFAULT_DEVIATION = 0.5
+
+# Plot line colors
+PREDICTED_COLOR = "blue"
+SIMULATED_COLOR = "brown"
+INPUT_COLOR = "red"
+
+COMMENT_STR = "//"
+DEFAULT_NUM_STEP = 5
+DEFAULT_INITIAL_VALUE = 0
+DEFAULT_FINAL_VALUE = 10
+DEFAULT_POINT_PER_STEP = 10
+
+# TimeSeries
+MS_IN_SEC = 1000.0
+SEC_IN_MS = 1.0/MS_IN_SEC
+TIMESERIES_INDEX_NAME = "miliseconds"
+TIMES = np.linspace(DEFAULT_INITIAL_VALUE, DEFAULT_FINAL_VALUE, DEFAULT_POINT_PER_STEP*DEFAULT_FINAL_VALUE)
+
+# Types
+TYPE_PARAMETER = "parameter"
+TYPE_BOUNDARY_SPECIES = "boundary_species"
+TYPE_FLOATING_SPECIES = "floating_species"
+TYPE_REACTION = "reaction"
+TYPE_ASSIGNMENT = "assignment"   # assignment rule
+VALID_INPUT_TYPES = [TYPE_BOUNDARY_SPECIES, TYPE_FLOATING_SPECIES, TYPE_PARAMETER, TYPE_ASSIGNMENT]
+VALID_OUTPUT_TYPES = [TYPE_BOUNDARY_SPECIES, TYPE_FLOATING_SPECIES, TYPE_PARAMETER, TYPE_ASSIGNMENT, TYPE_REACTION]
+ANTIMONY_TYPES = list(set(VALID_INPUT_TYPES + VALID_OUTPUT_TYPES))
+
+# Staircase
+DEFAULT_NUM_STEP = 5
+DEFAULT_INITIAL_VALUE = 0
+DEFAULT_FINAL_VALUE = 10
+DEFAULT_NUM_POINT = 100
+
+# Fitter methods
+FITTER_METHOD_GPZ = "gpz"
+FITTER_METHOD_POLY = "poly"
+DEFAULT_FITTER_METHOD = FITTER_METHOD_POLY
+
 
 # Default values of options
 SIM_DCT = dict(
       step_val=STEP_VAL,
       start_time=START_TIME,
       end_time=END_TIME,
       points_per_time=POINTS_PER_TIME,
+      times=TIMES,
+      initial_value=DEFAULT_INITIAL_VALUE,
+      final_value=DEFAULT_FINAL_VALUE,
       )
 # Options for a single plot
-PLOT_DCT = dict(
+PLOT_DCT:dict = dict(
+      legend=None,
       legend_spec=None,
       legend_crd=None,
+      markers=None,
+      markersize=8,
       ylim=None,
       xlim=None,
       xlabel="",
       ylabel="",
       title="",
       ax=None,
       ax2=None,
       xticklabels=None,
       yticklabels=None,
+      xlabel_angle=0,
       )
 # Options for the full figure
 FIG_DCT = dict(
       is_plot=True,
       figure=None,
       figsize=(10, 10),
       suptitle="",
       writefig=False,
       )
 
 DEFAULT_DCTS = [PLOT_DCT, FIG_DCT, SIM_DCT]
 
-
 # Must maintain this in correspondence with SIM_DCT, PLOT_DCT, FIG_DCT
 KWARGS = [
     #SIMULATION OPTIONS
     Kwarg(O_AX, default=None, dtype=matplotlib.pyplot.axes, doc="Plotting axis"),
     Kwarg(O_AX2, default=None, dtype=matplotlib.pyplot.axes, doc="Plotting 2nd axis"),
     Kwarg(O_END_TIME, default=10, dtype=float, doc="end time of simulation"),
+    Kwarg(O_MARKERS, default=None, dtype=list, doc="list of markers for plots"),
+    Kwarg(O_MARKERSIZE, default=8, dtype=float, doc="size of markers"),
     Kwarg(O_POINTS_PER_TIME, default=10, dtype=float,
           doc="number of simulation points per time period"),
+    Kwarg(O_INITIAL_VALUE, default=DEFAULT_INITIAL_VALUE, dtype=float, doc="initial value of step input"),
+    Kwarg(O_FINAL_VALUE, default=DEFAULT_FINAL_VALUE, dtype=float, doc="final value of step input"),
+    Kwarg(O_TIMES, default=np.linspace(0, 10, 100), dtype=np.array, doc="times of simulations"),
     Kwarg(O_START_TIME, default=0, dtype=float, doc="when simulation begins"),
     #PLOT OPTIONS
+    Kwarg(O_LEGEND, default=None, dtype=list,
+          doc="List of names for plots"),
     Kwarg(O_LEGEND_SPEC, default=None, dtype=LegendSpec,
           doc="Position of the legend"),
     Kwarg(O_LEGEND_CRD, default=None, dtype=tuple,
           doc="Coordinate position of the legend"),
     Kwarg(O_STEP_VAL, default=10, dtype=float, doc="value of step input"),
     Kwarg(O_TITLE, default="", dtype=str, doc="Plot title"),
     Kwarg(O_XLABEL, default="", dtype=str, doc="x-axis label"),
+    Kwarg(O_XLABEL_ANGLE, default=0, dtype=int, doc="x-axis label angle"),
     Kwarg(O_XLIM, default=None, dtype=(float, float), doc="Lower and upper values of x axis"),
     Kwarg(O_XTICKLABELS, default=None, dtype=list, doc="x-axis tic marks"),
     Kwarg(O_YLIM, default=None, dtype=(float, float), doc="Lower and upper values of y axis"),
     Kwarg(O_YLABEL, default="", dtype=str, doc="y-axis label"),
     Kwarg(O_YTICKLABELS, default=None, dtype=list, doc="y-axis tic marks"),
     # FIGURE OPTIONS
     Kwarg(O_FIGURE, default=None, dtype=matplotlib, doc="Figure option"),
@@ -186,49 +321,12 @@
 SIM_KWARGS = list(SIM_DCT.keys())
 PLOT_KWARGS = list(PLOT_DCT.keys())
 FIG_KWARGS = list(FIG_DCT.keys())
 ALL_KWARGS = []
 for kwargs in [SIM_KWARGS, PLOT_KWARGS, FIG_KWARGS]:
     ALL_KWARGS.extend(kwargs)
 
-# TimeSeries
-MS_IN_SEC = 1000.0
-SEC_IN_MS = 1.0/MS_IN_SEC
-TIMESERIES_INDEX_NAME = "miliseconds"
-TIMES = np.linspace(0, 5, 50)
-
-# URLs
-WOLF_URL = "https://www.ebi.ac.uk/biomodels/services/download/get-files/MODEL3352181362/2/BIOMD0000000206_url.xml"
-METFORMIN_URL = "https://www.ebi.ac.uk/biomodels/model/download/BIOMD0000001039.5?filename=Zake2021_Metformin%2BMice%2BIV.xml"
-MTOR_URL = "https://www.ebi.ac.uk/biomodels/model/download/BIOMD0000000823.2?filename=Varusai2018.xml"
-
-# Transfer function building
-DEFAULT_NUM_NUMERATOR = 1
-DEFAULT_NUM_DENOMINATOR = 3
-DEFAULT_DEVIATION = 0.5
-
-# Plot line colors
-PREDICTED_COLOR = "blue"
-SIMULATED_COLOR = "brown"
-INPUT_COLOR = "red"
-
-COMMENT_STR = "//"
-DEFAULT_NUM_STEP = 5
-DEFAULT_INITIAL_VALUE = 0
-DEFAULT_FINAL_VALUE = 10
-DEFAULT_POINT_PER_STEP = 10
-
-# Types
-TYPE_PARAMETER = "parameter"
-TYPE_BOUNDARY_SPECIES = "boundary_species"
-TYPE_FLOATING_SPECIES = "floating_species"
-TYPE_REACTION = "reaction"
-TYPE_ASSIGNMENT = "assignment"   # assignment rule
-VALID_INPUT_TYPES = [TYPE_BOUNDARY_SPECIES, TYPE_FLOATING_SPECIES, TYPE_PARAMETER, TYPE_ASSIGNMENT]
-VALID_OUTPUT_TYPES = [TYPE_BOUNDARY_SPECIES, TYPE_FLOATING_SPECIES, TYPE_PARAMETER, TYPE_ASSIGNMENT, TYPE_REACTION]
-ANTIMONY_TYPES = list(set(VALID_INPUT_TYPES + VALID_OUTPUT_TYPES))
-
-# Staircase
-DEFAULT_NUM_STEP = 5
-DEFAULT_INITIAL_VALUE = 0
-DEFAULT_FINAL_VALUE = 10
-DEFAULT_NUM_POINT = 100
+# Design results
+DESIGN_RESULT_SUCCESS = "Design successful."
+DESIGN_RESULT_CANNOT_SIMULATE = "No design. Cannot simulate the closed loop system." 
+DESIGN_RESULT_OUTPUT_TOO_SMALL = "No design. Output is too small."
+DESIGN_RESULT_OUTPUT_TOO_LARGE = "No design. Output is too large."
```

### Comparing `controlSBML-1.1.3/src/controlSBML/control_extensions/state_space_tf.py` & `controlsbml-1.2.0/src/controlSBML/control_extensions/state_space_tf.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/dict_array.py` & `controlsbml-1.2.0/src/controlSBML/dict_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
  Usage:
     dl = DictList(key1, key2, ...)   # Insert None to maintain length if a value is missing
     dl.append(key1=value1, key2=value2, ...)
     dl.addkey(key)  # Adds the key, inserting leading None values to maintain length
     len(dl)        # Returns the length of the lists
 """
 
-import pandas as pd
+import pandas as pd # type: ignore
 import numpy as np
 from typing import List
 
 class DictArray(dict):
 
     def __init__(self, *args:List[str]):
         """
@@ -83,15 +83,15 @@
     def append(self, **kwargs)->None:
         """
         Appends values to list. If a new key is encountered include it (is_addkey=True)
 
         Args:
             kwargs: dict of key, value pairs
         """
-        fill_list = list(np.repeat(None, len(self)))
+        fill_list = list(np.repeat(None, len(self)))   # type: ignore
         for key, value in kwargs.items():
             if not key in self.keys():
                 self[key] = list(fill_list)
             self[key].append(value)
         for key in self.keys():
             if not key in kwargs.keys():
                 self[key].append(None)
@@ -145,16 +145,16 @@
         # Get the list of keys
         keys = []
         for dl in dict_lists:
             keys.extend(dl.keys())
         keys = list(set(keys))
         # Process the lists
         for dl in dict_lists:
-            merged_fills = list(np.repeat(None, len(merged_dl)))
-            dl_fills = list(np.repeat(None, len(dl)))
+            merged_fills = list(np.repeat(None, len(merged_dl)))   # type: ignore
+            dl_fills = list(np.repeat(None, len(dl)))             # type: ignore
             for key in keys:
                 if not key in merged_dl.keys():
                     merged_dl[key] = list(merged_fills)
                 if key in dl.keys():
                     merged_dl[key].extend(dl[key])
                 else:
                     merged_dl[key].extend(dl_fills)
```

### Comparing `controlSBML-1.1.3/src/controlSBML/grid.py` & `controlsbml-1.2.0/src/controlSBML/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 """
 from controlSBML.option_management.option_manager import OptionManager
 import controlSBML.constants as cn
 
 import itertools
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
-import typing
+import pandas as pd  # type: ignore
+from typing import Optional, Callable, List
 
 DEFAULT_MIN = 0
 DEFAULT_MAX = 10
 DEFAULT_NUM_COORDINATE = 3
 NAME = "name"
 
 class Point(dict):
@@ -62,16 +62,17 @@
         self.update(kwargs)
 
     def __repr__(self)->str:
         return "Point({})".format(", ".join(["{}: {}".format(k, v) for k, v in self.items()]))
 
 
 class Axis:
-    def __init__(self, parameter_name:str, min_value:float=None, max_value:float=None, num_coordinate:int=None,
-                 is_random:bool=False, notifier=None):
+    def __init__(self, parameter_name:str, min_value:Optional[float]=DEFAULT_MIN,
+                 max_value:Optional[float]=DEFAULT_MAX, num_coordinate:Optional[int]=DEFAULT_NUM_COORDINATE,
+                 is_random:Optional[bool]=False, notifier:Optional[Callable]=None):
         """
         Specifies the axis for a parameter.
 
         Args:
             parameter_parameter_name: str (parameter_name of parameter)
             min_value: float (minimum value for parameter)
             max_value: float (maximum value for parameter)
@@ -116,15 +117,15 @@
         """
         Sets the number of coordinates for the axis.
 
         Args:
             num_coordinate: int (number of point coordinates for parameter)
         """
         self.num_coordinate = num_coordinate
-        self.notifier() 
+        self.notifier()
 
     @property
     def coordinates(self):
         """
         Finds the boundary coordinates for grids for this Axis
 
         Returns:
@@ -137,15 +138,15 @@
         Finds the coordinate for a point on this axis.
         Args:
             idx: int (index of coordinate)
 
         Returns:
             float
         """
-        if idx < 0 or idx >= self.num_coordinate - 1:
+        if idx < 0 or idx >= self.num_coordinate - 1:  # type: ignore
             raise ValueError("Invalid index: {}".format(idx))
         coordinates = self.coordinates
         if self.is_random:
             return np.random.uniform(coordinates[idx], coordinates[idx + 1])
         else:
             return (coordinates[idx] + coordinates[idx + 1])/2
    
@@ -188,24 +189,24 @@
     def recalculatePoints(self):
         """
         Recalculates the points.
         """
         self._points = None
 
     def __repr__(self)->str:
-        dct = {NAME: [], cn.MIN: [], cn.MAX: [], "num_coordinate": []}
+        dct: dict = {NAME: [], cn.MIN: [], cn.MAX: [], "num_coordinate": []}
         for parameter_name, axis in self.axis_dct.items():
             dct[NAME].append(parameter_name)
             dct[cn.MIN].append(axis.min_value)
             dct[cn.MAX].append(axis.max_value)
             dct["num_coordinate"].append(axis.num_coordinate)
         return str(pd.DataFrame(dct))
 
-    def addAxis(self, parameter_name:str, min_value:float=None,
-                          max_value:float=None, num_coordinate:int=None):
+    def addAxis(self, parameter_name:str, min_value:Optional[float]=None,
+                          max_value:Optional[float]=None, num_coordinate:Optional[int]=None):
         """
         Creates an axis for a parameter.
         Args:
             parameter_name: str (name of parameter)
             min_value: float (minimum value for parameter)
             max_value: float (maximum value for parameter)
             num_coordinate: int (number of point coordinates for parameter)
@@ -214,15 +215,15 @@
             min_value = self.default_min
         if max_value is None:
             max_value = self.default_max
         if num_coordinate is None:
             num_coordinate = self.default_num_coordinate
         if parameter_name in self.axis_dct:
             raise ValueError("Parameter name already exists: {}".format(parameter_name))
-        if min_value >= max_value:
+        if min_value > max_value:
             raise ValueError("min_value must be less than max_value: {} >= {}".format(min_value, max_value))
         self.axis_dct[parameter_name] = Axis(parameter_name, min_value=min_value, max_value=max_value,
                                              num_coordinate=num_coordinate, is_random=self.is_random,
                                              notifier=self.notifyAxisChange)
         self.recalculatePoints()
         
     @property
@@ -232,15 +233,15 @@
 
         Returns:
             int: number of points
         """
         return len(self.points)
     
     @property
-    def points(self)->typing.List[Point]:
+    def points(self)->List[Point]:
         """
         Gets the list of points.
 
         Returns:
             list-dict: list of points
         """
         if self._points is None:
@@ -250,17 +251,18 @@
     def _iteratePoints(self):
         """
         Creates an iterator that returns a point.
 
         Returns:
             Point
         """
-        index_lists = [list(range(self.axis_dct[p].num_coordinate - 1)) for p in self.axis_dct.keys()]
-        for indices in itertools.product(*index_lists):
-            yield Point(**{a.parameter_name: a.getPointCoordinate(i) for a, i in zip(self.axis_dct.values(), indices)})
+        lsts = [a.coordinates for a in self.axis_dct.values()]
+        for point_values in itertools.product(*lsts):
+            dct = {n: v for n, v in zip(self.axis_dct.keys(), point_values)}
+            yield Point(**dct)
 
     def getAxis(self, parameter_name:str)->Axis:
         """
         Gets the Axis for a parameter.
 
         Args:
             parameter_name: str (name of parameter)
```

### Comparing `controlSBML-1.1.3/src/controlSBML/iterate_biomodels.py` & `controlsbml-1.2.0/src/controlSBML/iterate_biomodels.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/make_roadrunner.py` & `controlsbml-1.2.0/src/controlSBML/make_roadrunner.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/option_management/option_manager.py` & `controlsbml-1.2.0/src/controlSBML/option_management/option_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Manages options used in ControlSBML."""
 
 import controlSBML.constants as cn
 from controlSBML.option_management.options import Options
 
-from docstring_expander.expander import Expander
+from docstring_expander.expander import Expander # type: ignore
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 
 
 class OptionManager(object):
     figure_idx = 0  # Index for automated figure generation
@@ -128,18 +128,29 @@
              _, ax  = plt.subplots(1)
              new_kwargs[cn.O_AX]  = ax
         if new_kwargs[cn.O_LEGEND_SPEC] is not None:
             legend_spec = new_kwargs[cn.O_LEGEND_SPEC]
             ax.legend(legend_spec.names,
                   bbox_to_anchor=legend_spec.crd,
                   loc=legend_spec.loc)
+        if new_kwargs[cn.O_LEGEND] is not None:
+            o_legend = new_kwargs[cn.O_LEGEND]
+            if isinstance(o_legend, list):
+                ax.legend(new_kwargs[cn.O_LEGEND])
+            elif not o_legend:
+                ax.legend([])
         if new_kwargs[cn.O_TITLE] != cn.PLOT_DCT[cn.O_TITLE]:
             ax.set_title(new_kwargs[cn.O_TITLE])
         if new_kwargs[cn.O_XLABEL] != cn.PLOT_DCT[cn.O_XLABEL]:
             ax.set_xlabel(new_kwargs[cn.O_XLABEL])
+        if new_kwargs[cn.O_XLABEL_ANGLE] is not None:
+            labels = ax.get_xticklabels()
+            xticks = ax.get_xticks()
+            ax.set_xticks(xticks)
+            ax.set_xticklabels(labels, rotation=new_kwargs[cn.O_XLABEL_ANGLE], ha='right')
         if new_kwargs[cn.O_XLIM] is not None:
             ax.set_xlim(new_kwargs[cn.O_XLIM])
         if new_kwargs[cn.O_XTICKLABELS] is not None:
             ax.set_xticklabels(new_kwargs[cn.O_XTICKLABELS])
         if new_kwargs[cn.O_YLABEL] != cn.PLOT_DCT[cn.O_YLABEL]:
             ax.set_ylabel(new_kwargs[cn.O_YLABEL])
         if new_kwargs[cn.O_YLIM] is not None:
```

### Comparing `controlSBML-1.1.3/src/controlSBML/option_management/options.py` & `controlsbml-1.2.0/src/controlSBML/option_management/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,7 +96,10 @@
         #
         opts_lst = []
         for dct in self.default_dcts:
             opts = Options({k: self[k] if k in self.keys() else v
                   for k, v in dct.items()}, default_dcts=[dct])
             opts_lst.append(opts)
         return opts_lst
+    
+    def asDict(self):
+        return dict(self)
```

### Comparing `controlSBML-1.1.3/src/controlSBML/option_set.py` & `controlsbml-1.2.0/src/controlSBML/option_set.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/src/controlSBML/parallel_search.py` & `controlsbml-1.2.0/src/controlSBML/parallel_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,17 @@
     best_result = search.getBestCandidate()  # Returns the candidate with the lowest score
     df = search.getSearchResuts()  # Returns a dataframe with the scores and other results from the evaluator
 """
 import controlSBML.constants as cn
 from controlSBML.dict_array import DictArray
 
 import multiprocessing as mp
-import numpy as np
-import pandas as pd
-import random
+import random  # type: ignore
+from tqdm import tqdm # type: ignore
 from typing import List
-from tqdm import tqdm
 
 
 class Evaluator(object):
     # The constructed object should be light weight and pickleable.
     
     def initialize(self)->None:
         """
@@ -84,16 +82,16 @@
             raise ValueError("Must run search() first")
         return self._search_results_dict_array.getDataframe()
 
     def search(self):
         num_process = min(len(self.candidates), self.num_process)
         if num_process == 1:
             # Run in a single process
-            procnum = 0
             return_dct = {}
+            procnum = 0
             self._evaluateCandidates(procnum, self.evaluator, self.candidates, num_process, return_dct)
             self._search_results_dict_array = return_dct[procnum]
         else:
             # Initialize for parallel calculations
             jobs = []
             num_process = min(num_process, len(self.candidates))
             random.shuffle(self.candidates)   # Process in random order
```

### Comparing `controlSBML-1.1.3/src/controlSBML/point_evaluator.py` & `controlsbml-1.2.0/src/controlSBML/point_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Evaluates a single design point."""
 
 import controlSBML.constants as cn
 from controlSBML.parallel_search import Evaluator
 from controlSBML.sbml_system import SBMLSystem
 
 import numpy as np
-from typing import Tuple
+from typing import Tuple, Union
+import warnings
 
 
 ##################################################################
 class PointEvaluator(Evaluator):
     # Evaluates a point in the design space
-    def __init__(self, sbml_system:SBMLSystem, input_name:str, output_name:str, setpoint:float, times:np.array,
-                 is_greedy:bool=False):
+    def __init__(self, sbml_system:SBMLSystem, input_name:str, output_name:str, setpoint:float, 
+                 sign:float, times:np.array, is_greedy:bool=False):
         """
         Args:
             sbml_system (SBMLSystem): Should be a copy of the original system so it is light weight
             input_name (str): system input
             output_name (str): system output
             setpoint (float):
             times (np.array):
@@ -24,14 +25,15 @@
         """
         self.sbml_system = sbml_system
         if sbml_system.isInitialized():
             raise ValueError("sbml_system should be a copy of the original system so it is light weight")
         self.input_name = input_name
         self.output_name = output_name
         self.setpoint = setpoint
+        self.sign = sign
         self.times = times
         self.siso_evaluator = None
         self.is_greedy = is_greedy
 
     def initialize(self)->None:
         pass
 
@@ -42,67 +44,75 @@
         Args:
             candidate_dct: dict (key: name of parameter, value: value of parameter)
         Returns:
             dict
                 score: float (MSE)
                 cadidate_dct keys, values
         """
-        #
-        if self.is_greedy:
-            new_dct = self._searchForFeasibleClosedLoopSystem(**candidate_dct)
-            if new_dct is None:
-                result_dct[cn.SCORE] = None
-                return result_dct
-        else:
-            new_dct = dict(candidate_dct)
+        # FIXME
+#        if self.is_greedy:
+#            new_dct = self._searchForFeasibleClosedLoopSystem(**candidate_dct)
+#            if new_dct is None:
+#                result_dct[cn.SCORE] = None
+#                return result_dct
+#        else:
+#            new_dct = dict(candidate_dct)
+        new_dct = dict(candidate_dct)
         result_dct = dict(new_dct)
-        _, residual_mse = self._calculateMse(**new_dct)
-        result_dct[cn.SCORE] = residual_mse
+        reason, residual_mse = self._calculateMse(**new_dct)   # type: ignore
+        result_dct[cn.SCORE] = residual_mse # type: ignore
+        result_dct[cn.REASON] = reason  # type: ignore
         return result_dct
 
-    def _calculateMse(self, max_output:float=1e6, min_output:float=0, **parameter_dct:dict)->Tuple[bool, any]:
+    def _calculateMse(self, **parameter_dct:dict)->Tuple[str, object]:
         """
         Attempts to calculate the mean squared error of the closed loop system. Reports if system is unstable.
 
         Args:
-            max_output: float (maximum output)
-            min_output: float (minimum output)
-            parameter_dct: dict: {name: value for eack of kp, ki, kf}
+            parameter_dct: dict: {name: value for each of kP, kI, kF}
 
         Returns:
-            bool (successful simulation)
+            str (description of design result)
             float (mean squared error)
         """
+        SIZE_MARGIN = 1e6
+        _ = self.sbml_system.roadrunner  # Initialize roadrunner
+        max_output = SIZE_MARGIN*self.sbml_system._max_value_dct[self.output_name]
+        min_output = self.sbml_system._min_value_dct[self.output_name]/SIZE_MARGIN
         try:
-            response_ts, _ = self.sbml_system.simulateSISOClosedLoop(setpoint=self.setpoint,
+            response_ts, builder = self.sbml_system.simulateSISOClosedLoop(setpoint=self.setpoint,
                         input_name=self.input_name, output_name=self.output_name,
-                        times=self.times,
+                        times=self.times, sign=self.sign,
                         is_steady_state=self.sbml_system.is_steady_state, inplace=False,
-                        **parameter_dct)
+                        **parameter_dct)  # type: ignore
         except Exception as error:
             if "CVODE" in str(error):
-                return False, None
+                return cn.DESIGN_RESULT_CANNOT_SIMULATE, None
             else:
                 raise ValueError(str(error))
         # Check for large outputs
+        if response_ts is None:
+            return cn.DESIGN_RESULT_CANNOT_SIMULATE, None
         outputs = response_ts[self.output_name].values
         max_value = np.max([np.max(outputs), np.abs(np.min(outputs))])
-        min_value = np.min([np.max(outputs), np.abs(np.min(outputs))])
-        if (max_value > max_output) or (min_value < min_output):
-            return False, None
-        # Check for negative values
-        for column in response_ts.columns:
-            if np.any(response_ts[column].values < 0):
-                return False, None
+        if False:
+            # Disable these checks
+            if max_value > max_output:
+                return cn.DESIGN_RESULT_OUTPUT_TOO_LARGE, None
+            min_value = np.min([np.max(outputs), np.abs(np.min(outputs))])
+            if min_value < min_output:
+                return cn.DESIGN_RESULT_OUTPUT_TOO_SMALL, None
         #
         residuals = self.setpoint - response_ts[self.output_name].values
-        mse = np.mean(residuals**2)
-        return True, mse
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            mse = np.mean(residuals**2)
+        return cn.DESIGN_RESULT_SUCCESS, mse
     
-    def _searchForFeasibleClosedLoopSystem(self, max_iteration:int=10, **parameter_dct)->dict:
+    def _searchForFeasibleClosedLoopSystem(self, max_iteration:int=10, **parameter_dct)->Union[dict, None]:
         """
         Does a greedy search to find values of the parameters that are minimally stable.
 
         Args:
             max_iteration: int (maximum number of iterations)
             parameter_dct: dict (name: value)
                 key: name of parameter
```

### Comparing `controlSBML-1.1.3/src/controlSBML/sbml_system.py` & `controlsbml-1.2.0/src/controlSBML/sbml_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,36 @@
 from controlSBML import msgs
 from controlSBML.make_roadrunner import makeRoadrunner
 from controlSBML.timeseries import Timeseries
 from controlSBML import util
 from controlSBML.option_management.option_manager import OptionManager
 
 import matplotlib.pyplot as plt
-import pandas as pd
-import numpy as np
-import tellurium as te
+import pandas as pd  # type: ignore
+import numpy as np  # type: ignore
+import tellurium as te  # type: ignore
+from typing import Optional, List, Tuple
 
 
 class SBMLSystem(object):
 
     def __init__(self, model_reference, input_names=None, output_names=None, is_fixed_input_species=False,
+                 noise_spec=cn.NoiseSpec(),
+                 disturbance_spec=cn.DisturbanceSpec(),
                  model_id="model", is_steady_state=False, roadrunner=None):
         """
         model_reference: str
             string, SBML file or Roadrunner object
         input_names: name (id) of reaction whose flux is being controlled
                      or the name of a chemical species
         output_names: list-str
             output species
         is_fixed_input_species: bool (input species are fixed)
+        noise_spec: cn.NoiseSpec
+        disturbance_spec: cn.DisturbanceSpec
         model_id: str (identifier of the model)
         is_steady_state: bool (start the simulation at steady state)
         """
         if input_names is None:
             input_names = []
         if output_names is None:
             output_names = []
@@ -37,21 +42,25 @@
         self._specified_output_names = output_names
         # First initializations
         self.model_reference = model_reference
         self.model_id = model_id
         self.is_fixed_input_species = is_fixed_input_species
         self.is_steady_state = is_steady_state
         self.is_fixed_input_species = is_fixed_input_species
+        self.noise_spec = noise_spec
+        self.disturbance_spec = disturbance_spec
         # The following are calculated on first reference
         self._antimony_builder = None
         self._roadrunner = roadrunner
         self._input_names = None
         self._output_names = None
         self._original_antimony = None
         self._symbol_dct = None
+        self._min_value_dct = None # Minimum values for the speciesj
+        self._max_value_dct = None # Maximum values for the species
         
 
     #################### PROPERTIES ####################
     @property
     def original_antimony(self):
         if self._original_antimony is None:
             self._original_antimony = self._getAntimony()
@@ -63,14 +72,18 @@
             self._symbol_dct = self._makeSymbolDct()
         return self._symbol_dct
 
     @property
     def roadrunner(self):
         if self._roadrunner is None:
             self._roadrunner = makeRoadrunner(self.model_reference)
+            data = self._roadrunner.simulate()
+            keys = [k[1:-1] if k[0] == "[" and k[-1] == "]" else k for k in data.colnames]
+            self._min_value_dct = {keys[n]: data[:, n].min() for n in range(len(keys))}
+            self._max_value_dct = {keys[n]: data[:, n].max() for n in range(len(keys))}
         return self._roadrunner
 
     # FIXME: Does not copy updates to the antimony?
     @property
     def antimony_builder(self):
         if self._antimony_builder is None:
             try:
@@ -105,14 +118,15 @@
 
         Returns:
             _type_: _description_
         """
         system = SBMLSystem(self.model_reference, input_names=self._specified_input_names,
                             output_names=self._specified_output_names,
                             is_fixed_input_species=self.is_fixed_input_species, model_id=self.model_id,
+                            noise_spec=self.noise_spec, disturbance_spec=self.disturbance_spec,
                             is_steady_state=self.is_steady_state)
         return system
     
     def __eq__(self, other):
         is_debug = False
         is_equal = True
         is_equal = is_equal and (self.model_reference == other.model_reference)
@@ -316,102 +330,98 @@
             is_steady_state = self.is_steady_state
         if num_point is None:
             num_point = int(cn.POINTS_PER_TIME*(end_time - start_time))
         if is_steady_state:
             self.setSteadyState()
         return self._simulate(start_time, end_time, num_point, is_steady_state, is_reload=False)
     
-    def _simulate(self, start_time, end_time, num_point, antimony_builder=None, is_steady_state=False, is_reload=False):
+    def _simulate(self, start_time:float, end_time:float, num_point:int, 
+                  antimony_builder:Optional[AntimonyBuilder]=None,
+                  selections:Optional[list]=None,
+                  is_steady_state:Optional[bool]=False, is_reload:Optional[bool]=False):
         """
         Simulates the system the roadrunner object.
 
         Parameters
         ----------
         start_time: float
         end_time: float
         num_point: int
         antimoney_builder: AntimonyBuilder
+        selections: list-str (names of species to be selected)
         is_steady_state: bool (start the simulation at steady state)
 
         Returns
         -------
-        DataFrame
+        Timeseries
         """
-        if antimony_builder is None:
-            antimony_builder = self.antimony_builder
-        antimony = str(antimony_builder)
-        if antimony[-1] == "\n":
-            antimony = antimony[:-1]
+        # Set defaults
+        selections = [] if selections is None else selections
+        antimony_builder = self.antimony_builder if antimony_builder is None else antimony_builder
+        # Initializations
+        antimony_str = str(antimony_builder)
+        if antimony_str[-1] == "\n":
+            antimony_str = antimony_str[:-1]
         if is_reload:
             try:
                 self._roadrunner = te.loada(str(antimony_builder))
             except Exception as exp:
                 raise ValueError("Cannot reload antimony: %s" % exp)
         else:
             self.roadrunner.reset()
         if is_steady_state:
             self.setSteadyState()
-        selections = list(self.input_names)
-        selections.extend(self.output_names)
-        selections.insert(0, cn.TIME)
-        data = self.roadrunner.simulate(float(start_time), float(end_time), num_point, selections=selections)
-        ts = Timeseries(data)
+        new_selections = list(selections)
+        new_selections.extend(self.input_names)
+        new_selections.extend(self.output_names)
+        new_selections = list(set(new_selections))
+        if not cn.TIME in new_selections:
+            new_selections.insert(0, cn.TIME)
+        try:
+            data = self.roadrunner.simulate(float(start_time), float(end_time), num_point, selections=new_selections)
+            ts = Timeseries(data)
+        except Exception as exp:
+            print(exp)
+            ts = None
         return ts
     
     def isInitialized(self)->bool:
         """
         Determines if the system has been initialized.
 
         Returns
         -------
         bool
         """
         return self._antimony_builder is not None
 
-    # FIXME: Delete since duplicated in controlSBML 
-    def plotModel(self, start_time=cn.START_TIME, end_time=cn.END_TIME, num_point=None, **kwargs):
-        """
-        Plots the original model.
-
-        Args:
-            start_time: float
-            end_time: float
-            num_point: int
-            kwargs: dict (kwargs for plotOneTS)
-        Returns:
-            Timeseries
-        """
-        if num_point is None:
-            num_point = int(cn.POINTS_PER_TIME*(end_time - start_time))
-        roadrunner = makeRoadrunner(self.model_reference)
-        data = roadrunner.simulate(start_time, end_time, num_point)
-        ts = Timeseries(data)
-        util.plotOneTS(ts, **kwargs)
-        return ts
-
-    def simulateSISOClosedLoop(self, input_name=None, output_name=None, kp=None, ki=None, kf=None, setpoint=1,
+    def simulateSISOClosedLoop(self, input_name=None, output_name=None, kP=None, kI=None, kD=None, kF=None,
+                               setpoint=1,
                                start_time=cn.START_TIME, end_time=cn.END_TIME, times=None, num_point=None,
                                is_steady_state=False, inplace=False, initial_input_value=None,
-                               sign=-1):
+                               selections:Optional[list[str]]=None,
+                               sign=-1)->Tuple[Timeseries, AntimonyBuilder]:
         """
         Simulates a closed loop system.
 
         Args:
             input_name: str
             output_name: str
-            kp: float
-            ki float
-            kf: float
+            kP: float
+            kI float
+            kD: float
+            kF: float
             setpoint: float (setpoint)
             times: np.ndarray (times for the simulation)
             start_time: float (overridden by times)
             end_time: float (overridden by times)
             num_point: int (overridden by times)
             inplace: bool (update the existing model with the closed loop statements)
             initial_input_value: float (initial value of the input)
+            selections: list-str (names of species to be selected)
             sign: float (sign of the feedback)
         Returns:
             Timeseries
             AntimonyBuilder
         """
         if times is not None:
             start_time = times[0]
@@ -431,47 +441,64 @@
         #
         if input_name in builder.boundary_species_names:
             new_input_name = input_name
         elif input_name in builder.floating_species_names:
             new_input_name = builder.makeParameterNameForBoundaryReaction(input_name)
         else:
             new_input_name = input_name
-        builder.makeSISOClosedLoopSystem(new_input_name, output_name, kp=kp, ki=ki, kf=kf, setpoint=setpoint,
+        builder.makeSISOClosedLoopSystem(new_input_name, output_name, kP=kP, kI=kI, kD=kD, kF=kF, setpoint=setpoint,
+                                         noise_spec=self.noise_spec, disturbance_spec=self.disturbance_spec,
                                          initial_output_value=initial_input_value, sign=sign)
         # Run the simulation
-        result = self._simulate(start_time, end_time, num_point, is_steady_state=is_steady_state,
-                            antimony_builder=builder, is_reload=True), builder
-        return result
+        if selections is None:
+            selections = []
+        new_selections = list(selections)
+        new_selections.extend([cn.TIME, input_name, output_name])
+        new_selections = list(set(new_selections))
+        if new_selections[0] != cn.TIME:
+            new_selections.remove(cn.TIME)
+            new_selections.insert(0, cn.TIME)  # Time should be the first selection
+        new_selections.extend(builder.closed_loop_symbols)
+        ts = self._simulate(start_time, end_time, num_point, is_steady_state=is_steady_state,
+                            antimony_builder=builder, is_reload=True, selections=new_selections)
+        return ts, builder
     
     def simulateStaircase(self, input_name, output_name, times=cn.TIMES, initial_value=cn.DEFAULT_INITIAL_VALUE,
-                 num_step=cn.DEFAULT_NUM_STEP, final_value=cn.DEFAULT_FINAL_VALUE, is_steady_state=True, inplace=True):
+                 num_step=cn.DEFAULT_NUM_STEP, final_value=cn.DEFAULT_FINAL_VALUE,
+                 selections:Optional[List[str]]=None,
+                 is_steady_state=True, inplace=True):
         """
         Adds events for the staircase.
         Args:
             input_name: str
             output_name: str
             initial_value: float (value for first step)
             final_value: float (value for final step)
             num_step: int (number of steps in staircase)
             num_point_in_step: int (number of points in each step)
+            selections: list-str (names of species to be selected)
+            is_steady_state: bool (start the simulation at steady state)
             inplace: bool (update the existing model with the Staircase statements)
         Returns:
             Timeseries
             AntimonyBuilder
         """
         if inplace:
             builder = self.antimony_builder
         else:
             builder = self.antimony_builder.copy()
+        if selections is None:
+            selections = [cn.TIME, input_name, output_name]
         builder.addStatement("")
         builder.makeComment("Staircase: %s->%s" % (input_name, output_name))
         builder.makeStaircase(input_name, times=times, initial_value=initial_value,
                                             num_step=num_step, final_value=final_value)
         ts = self._simulate(start_time=times[0], antimony_builder=builder, end_time=times[-1], num_point=len(times),
-                            is_steady_state=is_steady_state, is_reload=True)
+                            is_steady_state=is_steady_state, is_reload=True,
+                            selections=selections)
         return ts, builder
     
     @staticmethod 
     def setYAxColor(ax, position, color):
         # Set the colors of the labels, axes, and spines
         ax.tick_params(axis='y', labelcolor=color)
         ax.spines[position].set_color(color)
@@ -484,55 +511,69 @@
         else:
             names = self.output_names
             name_type ="output"
         if len(names) < 1:
             raise ValueError("No %s name is specified." % name_type)
         return names[0]
     
-    def plotSISOClosedLoop(self, timeseries, setpoint, mgr=None, markers=None, **kwargs):
+    def plotSISOClosedLoop(self, timeseries:Timeseries, setpoint, selections=None, 
+                           mgr:Optional[OptionManager]=None, **kwargs):
         """
         Plots the results of a closed lop simulation. Input and output are defined in the SBMLSystem constructor.
 
         Args:
             timeseries: Timeseries
+            selections: list-str (names of variables to be selected)
             setpoint: float
             kwargs: dict (kwargs for plotOneTS)
         """
         input_name = self.getName(is_input=True)
         output_name = self.getName(is_input=False)
         is_plot, new_kwargs = util.setNoPlot(kwargs)
         if mgr is None:
             mgr = OptionManager(new_kwargs)
         new_kwargs["is_plot"] = False
-        df = pd.DataFrame(timeseries[output_name], columns=[output_name])
+        if selections is None:
+            columns = [output_name]
+            colors = [cn.SIMULATED_COLOR]
+        else:
+            columns = selections
+            columns.remove(cn.TIME)
+            colors = None
+            new_kwargs["markers"] = None
+        df = pd.DataFrame(timeseries[columns], columns=columns)
+        # Plot the other left axis lines
+        if cn.O_LEGEND in new_kwargs.keys():
+            if isinstance(new_kwargs[cn.O_LEGEND], list):
+                new_kwargs[cn.O_LEGEND].append(cn.O_SETPOINT)
         new_kwargs.setdefault(cn.O_AX2, 0)
-        plot_result = util.plotOneTS(df, colors=[cn.SIMULATED_COLOR], markers=markers, **new_kwargs)
+        plot_result = util.plotOneTS(df, colors=colors, **new_kwargs)
         ax = plot_result.ax
         ax.set_ylabel(output_name)
         # Plot the setpoint
-        setpoint_arr = np.ones(len(timeseries))*setpoint
+        setpoint_arr = np.repeat(setpoint, len(timeseries.index))
         times = np.array(timeseries.index)/cn.MS_IN_SEC
         ax.plot(times, setpoint_arr, color=cn.SIMULATED_COLOR,
             linestyle="--")
-        # Do the plots
+        # Do second axis plots
         mgr.plot_opts.set(cn.O_AX, ax)
         if mgr.plot_opts[cn.O_AX2] is None:
             ax2 = ax.twinx()
             mgr.plot_opts[cn.O_AX2] = ax2
         else:
             ax2 = mgr.plot_opts[cn.O_AX2]
         # Plot the staircase
         ax2.plot(times, timeseries[input_name], color=cn.INPUT_COLOR)
         self.setYAxColor(ax, "left", cn.SIMULATED_COLOR)
         self.setYAxColor(ax2, "right", cn.INPUT_COLOR)
         ax2.set_ylabel(input_name)
-        #mgr.doPlotOpts()
         ax.legend([])
-        #mgr.doFigOpts()
         if is_plot:
+            mgr.doPlotOpts()
+            mgr.doFigOpts()
             plt.show()
 
     def printModel(self, is_updated_model=True):
         """
         Prints the antimony for the model.
 
         Args:
@@ -585,15 +626,14 @@
         """
         Provides the names of valid model inputs.
 
         Returns:
             str
         """
         return self.getValidSymbols(is_input=True, is_str=True)
-        
 
     def getValidOutputs(self):
         """
         Provides the names of valid model inputs.
 
         Returns:
             str
```

### Comparing `controlSBML-1.1.3/src/controlSBML/siso_closed_loop_designer.py` & `controlsbml-1.2.0/src/controlSBML/siso_closed_loop_designer.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,47 +10,53 @@
 from controlSBML.timeseries import Timeseries
 from controlSBML.grid import Grid
 from controlSBML.option_management.option_manager import OptionManager
 from controlSBML.parallel_search import ParallelSearch
 from controlSBML.point_evaluator import PointEvaluator
 
 import collections
-import control
+import control  # type: ignore
 import matplotlib.pyplot as plt
 import numpy as np
 import os
-import pandas as pd
-import seaborn as sns
+import pandas as pd  # type: ignore
+import seaborn as sns  # type: ignore
 
-CP_KP = "kp"
-CP_KI = "ki"
-CP_KF = "kf"
-CONTROL_PARAMETERS = [CP_KP, CP_KI, CP_KF]
+CP_kP = "kP"
+CP_kI = "kI"
+CP_kF = "kF"
+CP_kD = "kD"
+CONTROL_PARAMETERS = [CP_kP, CP_kI, CP_kF, CP_kD]
 MAX_VALUE = 1e3  # Maximum value for a parameter
 MIN_VALUE = 0  # Minimum value for a paramete
 DEFAULT_INITIAL_VALUE = 1   # Default initial value for a parameter
 SETPOINT = 1
 BELOW_MIN_MULTIPLIER = 1e-3
 ABOVE_MAX_MULTIPLIER = 1e-3
 LOWPASS_POLE = 1e4 # Pole for low pass filter
 # Column names
-PARAMETER_DISPLAY_DCT = {CP_KP: r'$k_p$', CP_KI: r'$k_i$', CP_KF: r'$k_f$'}
+PARAMETER_DISPLAY_DCT = {CP_kP: r'$k_p$', CP_kI: r'$k_i$', CP_kF: r'$k_f$', CP_kD: r'$k_d$'}
 
 Workunit = collections.namedtuple("Workunit",
-    "system input_name output_name setpoint times is_greedy num_restart is_report")    
+    "system input_name output_name setpoint times is_greedy num_restart is_report") 
+# DesignResult
+#   dataframe: table of design results
+#   max_count: maximum count of the design parameters that successfully simulate
+DesignResult = collections.namedtuple("DesignResult", "dataframe max_count")
 
 
-def _calculateClosedLoopTransferFunction(open_loop_transfer_function=None, kp=None, ki=None, kd=None, kf=None, sign=-1):
+def _calculateClosedLoopTransferFunction(open_loop_transfer_function=None, kP=None, kI=None, kD=None, kF=None,
+                                         sign=-1):
     # Construct the transfer functions
     if open_loop_transfer_function is None:
         return None
-    controller_tf = util.makePIDTransferFunction(kP=kp, kI=ki, kD=kd)
+    controller_tf = util.makePIDTransferFunction(kP=kP, kI=kI, kD=kD)
     # Filter
-    if kf is not None:
-        filter_tf = control.TransferFunction([kf], [1, kf])
+    if kF is not None:
+        filter_tf = control.TransferFunction([kF], [1, kF])
     else:
         filter_tf = 1
     # Closed loop transfer function
     forward_tf = open_loop_transfer_function*controller_tf
     final_tf = control.feedback(forward_tf, filter_tf, sign=sign)
     # Ensure that the resulting transfer function is proper
     if len(final_tf.num[0][0]) == len(final_tf.den[0][0]):
@@ -96,47 +102,49 @@
         self.save_path = save_path
         # Calculated properties
         self.start_time = self.times[0]
         self.end_time = self.times[-1]
         self.num_point = len(self.times)
         self.sign = sign
         # Outputs
-        self.kp = None
-        self.ki = None
-        self.kf = None
+        self.kP = None
+        self.kI = None
+        self.kD = None
+        self.kF = None
         self.closed_loop_system = None
         self.residual_mse = None
         self.minimizer_result = None
         self._design_result_df = None   # Calculated in property
         #
         self._initializeDesigner()
         self.siso = None # SISOClosedLoopSystem
 
     @property
     def closed_loop_transfer_function(self):
         if self.open_loop_transfer_function is None:
             return None
-        return _calculateClosedLoopTransferFunction(open_loop_transfer_function=self.open_loop_transfer_function, kp=self.kp, ki=self.ki,
-                                      kf=self.kf, sign=self.sign)
+        return _calculateClosedLoopTransferFunction(open_loop_transfer_function=self.open_loop_transfer_function,
+                                                    kP=self.kP, kI=self.kI, kD=self.kD,
+                                                    kF=self.kF, sign=self.sign)
     @property
     def closed_loop_timeseries(self):
         _, closed_loop_ts = self.simulateTransferFunction(transfer_function=self.closed_loop_transfer_function)
         return closed_loop_ts
     
-    def set(self, kp=None, ki=None, kf=None):
+    def set(self, kP=None, kI=None, kD=None, kF=None):
         """
         Sets values of the design parameters
 
         Args:
-            kp (float)
-            ki (float)
-            kd (float)
-            kf (float)
+            kP (float)
+            kI (float)
+            kD (float)
+            kF (float)
         """
-        value_dct = {CP_KP: kp, CP_KI: ki, CP_KF: kf}
+        value_dct = {CP_kP: kP, CP_kI: kI, CP_kD: kD, CP_kF: kF}
         for name, value in value_dct.items():
             if value is None:
                 continue
             self.__setattr__(name, value)
         self.closed_loop_system = None
 
     def get(self):
@@ -152,18 +160,18 @@
                 value = self.__getattribute__(name)
                 dct[name] = value
         return dct 
     
     def _initializeDesigner(self):
         self.minimizer_result = None
         self.residual_mse = None # Root mean square of residuals
-        self.kp = None
-        self.ki = None
-        self.kd = None
-        self.kf = None
+        self.kP = None
+        self.kI = None
+        self.kD = None
+        self.kF = None
 
     def plotDesignResult(self, **kwargs):
         """
         Plots the design results.
 
         Args:
             kwargs: arguments for plotting
@@ -190,15 +198,18 @@
         # Find the parameters in the design result
         parameter_names = []
         idx = list(self.design_result_df.index)[0]
         for name in CONTROL_PARAMETERS:
             if not name in self.design_result_df.columns:
                 continue
             if not np.isnan(self.design_result_df.loc[idx, name]):
-                parameter_names.append(name)
+                # Make sure that the parameter is actually used (not zero)
+                sum_val = self.design_result_df[name].sum()**2   # Consider negative values
+                if not np.isclose(sum_val, 0):
+                    parameter_names.append(name)
         # Determine the type of plot
         mgr = OptionManager(kwargs)
         if len(parameter_names) == 1:
             # Line plot
             ax = mgr.getAx()
             parameter_name = parameter_names[0]
             yv = self.design_result_df[cn.SCORE].values
@@ -227,29 +238,30 @@
                 makePlot(parameter_names[dct[idx][0]], parameter_names[dct[idx][1]], axes[idx], vmin=min_mse, vmax=max_mse)
             fig.subplots_adjust(hspace=0.8)  # Increase horizontal space between plots
         else:
             raise ValueError("Cannot plot %d parameters" % len(parameter_names))
         mgr.doPlotOpts()
         mgr.doFigOpts()
 
-    def design(self, kp_spec=False, ki_spec=False, kf_spec=False, is_greedy=True,
+    def design(self, kP_spec=False, kI_spec=False, kD_spec=False, kF_spec=False, is_greedy=True,
                num_restart=5, min_value=MIN_VALUE, max_value=MAX_VALUE,
-               num_coordinate=3, save_path=None, num_process:int=-1, is_report:bool=False):
+               num_coordinate=3, num_process:int=-1, is_report:bool=False)->DesignResult:
         """
         Design objective: Create a feasible system (stable, no negative inputs/outputs) that minimizes residuals.
         Args:
-            kp_spec, ki_spec, kf_spec (bool, float): if True, the parameter is fitted. If float, then keeps at this value.
+            kP_spec, kI_spec, kD_spec, kF_spec: if True, the parameter is fitted. If float, then keeps at this value.
             num_restart: int (number of times to restart the minimizer)
             is_greedy: bool (if True, then a greedy search is done to find a feasible system)
             min_value: float/dict (parameter name: value)
             max_value: float/dict (parameter name: value)
             num_coordinate: int (number of coordinates for a parameter; minimum is 2)
-            save_path: str (path to save the results)
             is_report: bool (provide progress report)
             num_process: int (number of processes to use)
+        Returns:
+            DesignResult
         """
         def addAxis(grid, parameter_name, parameter_spec):
             """
             Adds the grid access based on the parameter specification.
 
             Args:
                 grid: Grid
@@ -258,100 +270,110 @@
             """
             if parameter_spec is None:
                 return
             if isinstance(parameter_spec, bool):
                 if parameter_spec:
                     grid.addAxis(parameter_name, min_value=min_value, max_value=max_value, num_coordinate=num_coordinate)
                 return
-            if isinstance(parameter_spec, float):
+            if util.isNumber(parameter_spec):
                 grid.addAxis(parameter_name, min_value=parameter_spec, max_value=parameter_spec, num_coordinate=1)
-        #
-        # Initial check
-        if self.open_loop_transfer_function is not None:
-            if (not util.isStablePoles(self.open_loop_transfer_function)) and (not util.isStableZeros(self.open_loop_transfer_function)):
-                msg = "The open loop transfer function has unstable poles and zeros. Design may fail."
-                msgs.warn(msg)
         # Initializations
         grid = Grid(min_value=min_value, max_value=max_value, num_coordinate=num_coordinate)
-        addAxis(grid, CP_KP, kp_spec)
-        addAxis(grid, CP_KI, ki_spec)
-        addAxis(grid, CP_KF, kf_spec)
+        if type(kP_spec) in [bool, float]:
+            addAxis(grid, CP_kP, kP_spec)
+        if type(kI_spec) in [bool, float]:
+            addAxis(grid, CP_kI, kI_spec)
+        if type(kD_spec) in [bool, float]:
+            addAxis(grid, CP_kD, kD_spec)
+        if type(kF_spec) in [bool, float]:
+            addAxis(grid, CP_kF, kF_spec)
         #
         return self.designAlongGrid(grid, is_greedy=is_greedy, num_restart=num_restart, is_report=is_report,
                                     num_process=num_process)
 
-    def oldsimulateTransferFunction(self, transfer_function=None, period=None):
-        """
-        Simulates the closed loop transfer function based on the parameters of the object.
-
-        Args
-            transfer_function (control.TransferFunction): closed loop transfer function
-        Returns
-            (np.array, np.array): times, predictions
-        Raises
-            ValueError: if there are no parameters defined for the closed loop transfer function
-        """
-        if transfer_function is None:
-            if self.closed_loop_transfer_function is None:
-                raise ValueError("No closed loop transfer function defined.")
-            transfer_function = self.closed_loop_transfer_function
-        if period is not None:
-            U = np.sin(2*np.pi*self.times/period)
-        else:
-            U = np.repeat(1, len(self.times))
-        U = U*self.setpoint
-        new_times, predictions = control.forced_response(transfer_function, T=self.times, U=U)
-        return new_times, predictions
-
     def designAlongGrid(self, grid:Grid, is_greedy:bool=False, num_restart:int=1,
-                        is_report:bool=False, num_process:int=-1):
+                        is_report:bool=False, num_process:int=-1)->DesignResult:
         """
         Design objective: Create a feasible system (stable, no negative inputs/outputs) that minimizes residuals.
+        For systems with random noise or disturbance, uses the maximum value of the score.
 
         Args:
             grid: Grid
             is_greedy: bool (if True, then a greedy search is done to find a feasible system)
-            num_restart: int (number of times to start the search) 
+            num_restart: int (number of times to start the search)
             is_report: bool (provide progress report)
             num_proc: int (number of processes to use; -1 means use all available processors)
+        Returns:
+            DesignResult
         """
-        point_evaluator = PointEvaluator(self.system.copy(), self.input_name, self.output_name, 
-                                            self.setpoint, self.times, is_greedy=is_greedy)
-        parallel_search = ParallelSearch(point_evaluator, grid.points, num_process=num_process, is_report=is_report) # type: ignore
-        search_results = []
+        def getValue(val):
+            if isinstance(val, pd.Series):
+                return np.mean(val)
+            else:
+                return float(val)
+        #
+        point_evaluator = PointEvaluator(self.system.copy(), self.input_name, self.output_name,
+                                            self.setpoint, self.sign, self.times, is_greedy=is_greedy)
+        # Expand the number of points
+        points = []
         for _ in range(num_restart):
-            parallel_search.search()
-            search_results.append(parallel_search.getSearchResults())
-        # Merge the results and sort by score
-        search_result_df = pd.concat(search_results)
-        search_result_df = search_result_df.reset_index()
+            points.extend(grid.points)
+        # Do the search
+        parallel_search = ParallelSearch(point_evaluator, points, num_process=num_process, is_report=is_report) # type: ignore
+        parallel_search.search()
+        search_result_df = parallel_search.getSearchResults()
         if len(search_result_df) == 0:
-            self.kp, self.ki, self.kf = None, None, None
-            return
-        # Have search results
-        search_result_df = search_result_df.sort_values(cn.SCORE)
-        search_result_df = search_result_df.reset_index()
+            df = pd.DataFrame([[None, None, None, None, None, cn.DESIGN_RESULT_CANNOT_SIMULATE]],
+                              columns=[CP_kP, CP_kI, CP_kD, CP_kF, cn.SCORE, cn.REASON])
+            return DesignResult(dataframe=df, max_count=0)
+        # Merge the results and sort by score
+        search_result_df = search_result_df.sort_values(cn.SCORE, ascending=True)  # type: ignore
+        search_result_df = search_result_df.reset_index(drop=True)
+        result_df = search_result_df.copy()
+        # Handle replications of the same design parameters and select successful designs
+        search_result_df = search_result_df[search_result_df[cn.SCORE].notna()]
+        del search_result_df[cn.REASON]
+        sort_columns = list(grid.axis_dct.keys())
+        groupby = search_result_df.groupby(sort_columns)
+        count_df = groupby.count()
+        max_count = np.max(count_df[cn.SCORE])
+        sel = count_df == max_count
+        mean_df = groupby.max()
+        threshold_mean_df = mean_df[sel]
+        threshold_mean_df = threshold_mean_df[threshold_mean_df[cn.SCORE].notna()]
+        sorted_mean_df = threshold_mean_df.reset_index()
+        sorted_mean_df = sorted_mean_df.sort_values(cn.SCORE, ascending=True)
+        sorted_mean_df = sorted_mean_df.reset_index()
+        # Check for no result
+        if len(sorted_mean_df) == 0:
+            df = pd.DataFrame([[None, None, None, None, None, cn.DESIGN_RESULT_CANNOT_SIMULATE]],
+                              columns=[CP_kP, CP_kI, CP_kD, CP_kF, cn.SCORE, cn.REASON])
+            return DesignResult(dataframe=df, max_count=0)
         # Record the result
-        self.residual_mse = search_result_df.loc[0, cn.SCORE]
-        if CP_KP in search_result_df.columns:
-            self.kp = search_result_df.loc[0, CP_KP]
-        if CP_KI in search_result_df.columns:
-            self.ki = search_result_df.loc[0, CP_KI]
-        if CP_KF in search_result_df.columns:
-            self.kf = search_result_df.loc[0, CP_KF]
+        self.residual_mse = sorted_mean_df.loc[0, cn.SCORE]
+        if CP_kP in sorted_mean_df.columns:
+            self.kP = getValue(sorted_mean_df.loc[0, CP_kP])
+        if CP_kI in sorted_mean_df.columns:
+            self.kI = getValue(sorted_mean_df.loc[0, CP_kI])
+        if CP_kD in sorted_mean_df.columns:
+            self.kD = getValue(sorted_mean_df.loc[0, CP_kD])
+        if CP_kF in sorted_mean_df.columns:
+            self.kF = getValue(sorted_mean_df.loc[0, CP_kF])
         # Save the results
         if self.save_path is not None:
-            search_result_df.to_csv(self.save_path, index=False)
+            sorted_mean_df.to_csv(self.save_path, index=False)
+        self._design_result_df = sorted_mean_df
+        return DesignResult(dataframe=result_df, max_count=max_count)
 
     @property
     def design_result_df(self):
         """
         Returns:
             pd.DataFrame
-                columns: kp, ki, kf, mse
+                columns: kP, kI, kD, kF, mse
         """
         if self._design_result_df is None:
             if (self.save_path is not None) and (os.path.isfile(self.save_path)):
                 self._design_result_df = pd.read_csv(self.save_path)
             else:
                 return None
         return self._design_result_df
@@ -401,15 +423,15 @@
         text = ["%s=%f " % (name, param_dct[name]) for name in param_dct.keys()]
         ax.set_title(" ".join(text))
         plt.rcParams['axes.titley'] = 0.9    # y is in axes-relative coordinates.
         if is_plot:
             plt.show()
         # Title lists values of the design parameters
 
-    def evaluate(self, is_plot=True, **kwargs):
+    def evaluate(self, **kwargs):
         """
         Creates an SBMLSystem using the design parameters. Records the builder.
 
         Args:
             kwargs: plot options
         Returns:
             Timeseries (from simulation)
@@ -429,12 +451,10 @@
             msgs.warn(msg)
         if success:
             if not "title" in kwargs:
                 param_dct = self.get()
                 text = ["%s=%f " % (name, param_dct[name]) for name in param_dct.keys()]
                 title = " ".join(text)
             self.system.plotSISOClosedLoop(simulated_ts, self.setpoint, markers=["", ""], title=title, **kwargs)
-            if is_plot:
-                plt.show()
             return simulated_ts, antimony_builder
         else:
             return None, None
```

### Comparing `controlSBML-1.1.3/src/controlSBML/siso_maker.py` & `controlsbml-1.2.0/src/controlSBML/siso_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,20 @@
         """
         Creates a close loop system and a companion step response plot.
         <filename>_closedloop.png.
         """
         try:
             ts, _ = self.system.simulateSISOClosedLoop(input_name=self.input_name, output_name=self.output_name,
                                                     setpoint=setpoint,
-                                           kp=1, ki=None, kf=None, is_steady_state=False)
+                                           kP=1, kI=None, kF=None, is_steady_state=False)
         except Exception as error:
             raise ValueError("Error in closed loop for %s: %s" % (self.model_id, error))
         # Make the plot
         is_plot, new_kwargs = util.setNoPlot(kwargs)
-        self.system.plotSISOClosedLoop(ts, setpoint=setpoint, figsize=(5,5), title=self.model_id, **new_kwargs)
+        self.system.plotSISOClosedLoop(ts, setpoint, figsize=(5,5), title=self.model_id, **new_kwargs)
         plot_filename = self.model_id + CLOSED_LOOP_SFX + PNG_EXT
         plt.savefig(plot_filename)
         if is_plot:
             plt.show()
 
     @classmethod
     def runModel(cls, model, is_plot=True, **kwargs):
```

### Comparing `controlSBML-1.1.3/src/controlSBML/siso_transfer_function_builder.py` & `controlsbml-1.2.0/src/controlSBML/siso_transfer_function_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,195 +1,68 @@
 """
-Builds a transfer function for a SISO NonlinearIOSystem
+Builds a transfer function for a SISO System with options for the fitting method.
 
     plotStaircaseResponse: plots response to a staircase input to the transfer function
 
     TO DO
     1. Tests for fitting
 """
 
 import controlSBML.constants as cn
 import controlSBML as ctl
 from controlSBML import msgs
 from controlSBML import util
 from controlSBML.option_management.option_manager import OptionManager
 from controlSBML.staircase import Staircase
+from controlSBML.poly_fitter import PolyFitter
+from controlSBML.gpz_fitter import GPZFitter
 
-import control
-from docstring_expander.expander import Expander
-import lmfit
+from docstring_expander.expander import Expander # type: ignore
 import numpy as np
 
 
 MIN_ELAPSED_TIME = 1e-2
 STAIRCASE = "staircase"
-MIN_PARAMETER_VALUE = -10
-MAX_PARAMETER_VALUE = 10
-INITIAL_PARAMETER_VALUE = 0.1
-NUMERATOR_PREFIX = "n"
-DENOMINATOR_PREFIX = "d"
-MAX_ABS_RESIDUAL = 10
-
-global _mse_history
-
-
-################## FUNCTIONS ####################
-def _makeParameters(num_numerator, num_denominator, min_value=MIN_PARAMETER_VALUE, max_value=MAX_PARAMETER_VALUE,
-                    initial_value=INITIAL_PARAMETER_VALUE):
-    """
-    Makes the parameters used to construct a transfer function.
-
-    Parameters
-    ----------
-    num_numerator: int (number of numerator terms)
-    num_denominator: int (number of denominator terms)
-    min_value: float
-    max_value: float
-    initial_value: float (if None, choose random value)
-
-    Returns
-    -------
-    lmfit.Parameter
-    """
-    pfit = lmfit.Parameters()
-    for idx in range(num_numerator):
-        if initial_value is None:
-            initial_value = np.random.uniform(min_value, max_value)
-        pfit.add(name='%s%d' % (NUMERATOR_PREFIX, idx),
-              min=min_value,
-              value=initial_value,
-              max=max_value)
-    for idx in range(num_denominator):
-        if initial_value is None:
-            initial_value = np.random.uniform(min_value, max_value)
-        pfit.add(name='%s%d' % (DENOMINATOR_PREFIX, idx),
-              min=min_value,
-              value=initial_value,
-              max=max_value)
-    return pfit
-
-def _makeTransferFunction(parameters):
-    """
-    Constructs a transfer function from a dictionary representation.
-
-    Parameters
-    ----------
-    parameters: lmfit.Parameter
-        parameters.valuesdict(): dict
-            key=n<int>: numerator coefficient for int-th element
-            key=d<int>: denominator coefficient for int-th element
-
-    Returns
-    -------
-    control.TransferFunction
-    """
-    tf_dct = parameters.valuesdict()
-    def makeVec(letter):
-        """
-        Creates a vector for the keys are a single letter followed
-        by an index.
+MIN_PARAMETER_VALUE = -1e6
+MAX_PARAMETER_VALUE = 1e6
 
-        Parameters
-        ----------
-        letter: char
-
-        Returns
-        -------
-        np.array
-        """
-        dct = {int(k[1:]): v for k, v in tf_dct.items() if k[0] == letter}
-        size = max([i for i in dct.keys()]) + 1
-        arr = list(np.repeat(0, size))
-        for idx, value in dct.items():
-            arr[idx] = value
-        return np.array(arr)
-    #
-    num_arr = makeVec(NUMERATOR_PREFIX)
-    den_arr = makeVec(DENOMINATOR_PREFIX)
-    tf = control.TransferFunction(num_arr, den_arr)
-    new_tf = util.simplifyTransferFunction(tf)
-    if len(new_tf.num[0][0]) > len(new_tf.den[0][0]):
-        # Avoid improper transfer function
-        new_tf = tf
-    return new_tf
-
-def _calculateTransferFunctionResiduals(parameters, data_in, data_out):
-    """
-    Computes the residuals for a transfer function.
-
-    Parameters
-    ----------
-    parameters: lmfit.Parameters
-        n<int>: numerator coefficient for int-th element
-        d<int>: denominator coefficient
-    data_in: (list-float, list-float) (times, input signal)
-    data_out: array-float (calibration data)
-    Returns
-    -------
-    float
-    """
-    def isDone(last_history:int=10, min_history:int=50, threshold:float=1e-3):
-        """
-        Checks if further progress is unlikely.
 
-        Returns
-        -------
-        bool
-            True if MSEs are not changing significantly
-        """
-        if len(_mse_history) < min_history:
-            return False
-        history_arr = np.array(_mse_history)
-        median_mse = np.median(history_arr)
-        credible_history_arr = history_arr[history_arr < median_mse]
-        last_arr = credible_history_arr[-last_history:]
-        metric = np.std(last_arr)/median_mse
-        return metric < threshold
-    #
-    global _mse_history
-    #
-    times, inputs = data_in
-    tf = _makeTransferFunction(parameters)
-    times, y_arr = control.forced_response(tf, T=times, U=inputs)
-    residuals = data_out - y_arr
-    is_bads = [np.isnan(v) or np.isinf(v) or (v is None) for v in residuals]
-    is_bad = any(is_bads)
-    if is_bad:
-        residuals = np.repeat(1e10, len(times))
-    mse = np.sum(residuals**2)/len(residuals)
-    _mse_history.append(mse)
-    if isDone():
-        # Force the minimizer to stop
-        residuals = np.repeat(0, len(residuals))
-    return residuals
-
-
-################## CLASSES ####################
 class SISOTransferFunctionBuilder(object):
 
-    def __init__(self, sbml_system, input_name=None, output_name=None):
+    def __init__(self, sbml_system, input_name=None, output_name=None, fitter_method=cn.FITTER_METHOD_POLY):
         """
         Parameters
         ----------
         sys: SBMLSystem
         input_name: str
         output_name: str
+        fitter_method: str (method for fitting the transfer function, either 'poly' or 'gpz')
         """
         #
         self.sbml_system = sbml_system
-        self.input_name = input_name
-        self.output_name = output_name
-        if self.input_name is None:
+        #
+        if input_name is None:
+            if (sbml_system.input_names is None) or (len(sbml_system.input_names) == 0):
+                raise ValueError("No input name specified")
             self.input_name = sbml_system.input_names[0]
-        if self.output_name is None:
+        else:
+            self.input_name = input_name
+        #
+        if output_name is None:
+            if (sbml_system.output_names is None) or (len(sbml_system.output_names) == 0):
+                raise ValueError("No output name specified")
             self.output_name = sbml_system.output_names[0]
+        else:
+            self.output_name = output_name
         #
+        self.fitter_method = fitter_method
 
     def copy(self):
-        return SISOTransferFunctionBuilder(self.sbml_system, input_name=self.input_name, output_name=self.output_name)
+        return SISOTransferFunctionBuilder(self.sbml_system, input_name=self.input_name, output_name=self.output_name,
+                                           fitter_method=self.fitter_method)
 
     @Expander(cn.KWARGS, cn.SIM_KWARGS)
     def makeStaircaseResponse(self, staircase=Staircase(), mgr=None, times=None,
            is_steady_state=True, **kwargs):
         """
         Constructs the staircase response of the NonlinearIOSystem.
         Assumes a single output. If there is more than one,
@@ -225,14 +98,16 @@
             mgr.options[cn.END_TIME] = times[-1]
         mgr.options[cn.O_POINTS_PER_TIME] = points_per_time
         # Do the simulations
         result_ts, antimony_builder = self.sbml_system.simulateStaircase(self.input_name, self.output_name, times=times,
                                                 initial_value=staircase.initial_value, num_step=staircase.num_step,
                                                 final_value=staircase.final_value, is_steady_state=is_steady_state,
                                                 inplace=False)
+        if result_ts is None:
+            raise ValueError("Unable to simulate staircase response")
         staircase.setNumPoint(len(result_ts))
         staircase_name = "%s_%s" % (self.input_name, STAIRCASE)
         staircase_arr= staircase.staircase_arr
         result_ts[staircase_name] = staircase_arr
         del result_ts[self.input_name]
         return result_ts, antimony_builder
 
@@ -270,35 +145,39 @@
             is_fig = True
         else:
             is_fig = False
         #
         new_response_ts, staircase_name, output_name = cls._extractStaircaseResponseInformation(response_ts)
         staircase_ts = response_ts[staircase_name]
         response_ts = new_response_ts
-        # Do the plots
-        plot_result = util.plotOneTS(response_ts, mgr=mgr, colors=[cn.SIMULATED_COLOR])
-        ax = plot_result.ax
-        mgr.plot_opts.set(cn.O_AX, ax)
-        mgr.plot_opts.set(cn.O_YLABEL, output_name)
-        if mgr.plot_opts[cn.O_AX2] is None:
-            ax2 = ax.twinx()
-            mgr.plot_opts[cn.O_AX2] = ax2
+        if mgr.plot_opts.asDict().get(cn.IS_PLOT, True):
+            # Do the plots
+            plot_result = util.plotOneTS(response_ts, mgr=mgr, colors=[cn.SIMULATED_COLOR])
+            ax = plot_result.ax
+            mgr.plot_opts.set(cn.O_AX, ax)
+            mgr.plot_opts.set(cn.O_YLABEL, output_name)
+            if mgr.plot_opts[cn.O_AX2] is None:
+                ax2 = ax.twinx()
+                mgr.plot_opts[cn.O_AX2] = ax2
+            else:
+                ax2 = mgr.plot_opts[cn.O_AX2]
+            # Plot the staircase
+            times = np.array(response_ts.index)/cn.MS_IN_SEC
+            ax2.plot(times, staircase_ts, color=cn.INPUT_COLOR,
+                linestyle="--")
+            cls.setYAxColor(ax, "left", cn.SIMULATED_COLOR)
+            cls.setYAxColor(ax2, "right", cn.INPUT_COLOR)
+            ax2.set_ylabel(staircase_name)
+            mgr.doPlotOpts()
+            ax.legend([])
+            if is_fig:
+                mgr.doFigOpts()
         else:
-            ax2 = mgr.plot_opts[cn.O_AX2]
-        # Plot the staircase
-        times = np.array(response_ts.index)/cn.MS_IN_SEC
-        ax2.plot(times, staircase_ts, color=cn.INPUT_COLOR,
-            linestyle="--")
-        cls.setYAxColor(ax, "left", cn.SIMULATED_COLOR)
-        cls.setYAxColor(ax2, "right", cn.INPUT_COLOR)
-        ax2.set_ylabel(staircase_name)
-        mgr.doPlotOpts()
-        ax.legend([])
-        if is_fig:
-            mgr.doFigOpts()
+            ax = None
+            ax2 = None
         #
         return util.PlotResult(time_series=response_ts, ax=ax, ax2=ax2)
     
     @classmethod
     def _extractStaircaseResponseInformation(cls, timeseries):
         """Extracts informatin present in the staircase response.
 
@@ -319,29 +198,30 @@
     @staticmethod
     def _getStaircaseColumnName(timeseries):
         all_columns = set(timeseries.columns)
         other_columns = [c for c in timeseries.columns if STAIRCASE not in c]
         staircase_column = list(all_columns.difference(other_columns))[0]
         return staircase_column, other_columns
 
-    @Expander(cn.KWARGS, cn.SIM_KWARGS)
-    def fitTransferFunction(self, num_numerator=cn.DEFAULT_NUM_NUMERATOR,
-                            num_denominator=cn.DEFAULT_NUM_DENOMINATOR, staircase=Staircase(), 
+    @Expander(cn.KWARGS, cn.ALL_KWARGS)
+    def plotTransferFunctionFit(self, num_zero=cn.DEFAULT_NUM_ZERO,
+                            num_pole=cn.DEFAULT_NUM_POLE, staircase=Staircase(), 
                             fit_start_time=None, fit_end_time=None, **kwargs):
         """
-        Constructs a transfer function for the NonlinearIOSystem.
+        Constructs a transfer function for the System. This is done by first estimating the gain to the
+        staircase input and then estimating the transients, zeroes and poles.
 
         Parameters
         ----------
-        num_numerator: int (number of numerator terms)
-        num_denominator: int (number of denominator terms)
+        num_zero: int (number of zeros)
+        num_pole: int (number of poles)
         staircase: Staircase
         fit_start_time: float (time at which fitting starts)
         fit_end_time: float (time at which fitting ends)
-        kwargs: dict (simulation options as described below)
+        kwargs: dict (options as described below)
         #@expand
 
         Returns
         -------
         FitterResult
             transfer_function: control.TransferFunction
             time_series: ("predicted" <name> <name>_staircase)
@@ -349,121 +229,67 @@
             minimizer_result: lmfit.MinimizerResult
             stderr: dict (key: term, value: stderr)
             nfev: number of function evaluations
             redchi: float (reduced ChiSq)
             parameters: lmfit.Parameters
             antimony_builder: AntimonyBuilder
         """
-        global _mse_history
+        def adjustArray(arr):
+            # Normalizes by mean and shapes
+            new_arr = arr - np.mean(arr)
+            new_arr = np.reshape(new_arr, (len(new_arr),))
+            return new_arr
         #
-        # Get the calibration data
+        fitter_method = kwargs.get(cn.FITTER_METHOD, self.fitter_method)
+        new_kwargs = dict(kwargs)
+        if cn.FITTER_METHOD in new_kwargs:
+            del new_kwargs[cn.FITTER_METHOD]
+        mgr = OptionManager(new_kwargs)
+        # Get the observational data
         new_staircase = staircase.copy()
-        data_ts, antimony_builder = self.makeStaircaseResponse(staircase=new_staircase, **kwargs)
+        data_ts, antimony_builder = self.makeStaircaseResponse(staircase=new_staircase, **mgr.sim_opts)
         ms_times = util.cleanTimes(data_ts.index)
-        output_ts, staircase_column_name, _ = self._extractStaircaseResponseInformation(data_ts)
-        data_ts.index = ms_times
-        output_ts.index = ms_times
-        new_staircase.name = staircase_column_name
+        _, input_name, _ = self._extractStaircaseResponseInformation(data_ts)
+        data_ts.index = ms_times.astype(int)
         #  Construct the fitting data
         start_idx = 0
         end_idx = len(ms_times)
         if fit_start_time is not None:
             start_idx = np.sum(ms_times <= cn.MS_IN_SEC*fit_start_time)
         if fit_end_time is not None:
             end_idx = np.sum(ms_times <= cn.MS_IN_SEC*fit_end_time)
         if np.isclose(start_idx, end_idx):
-            msgs.error("Start time is greater than end time")
+            msgs.error("fit_start_time >= fit_end_time")
         sel_ms_times = ms_times[start_idx:end_idx]
-        sel_ts = data_ts.loc[sel_ms_times]
-        staircase_arr = sel_ts[staircase_column_name].values
-        sel_sec_times = sel_ms_times/cn.MS_IN_SEC
-        data_in = (sel_sec_times, staircase_arr)
-        data_out = sel_ts[self.output_name]
+        new_data_ts = data_ts.loc[sel_ms_times]
         # Do the fit
-        parameters = _makeParameters(num_numerator, num_denominator)
-        _mse_history = []   # History of mean squared errors
-        mini = lmfit.Minimizer(_calculateTransferFunctionResiduals,
-                               parameters, fcn_args=(data_in, data_out))
-        minimizer_result = mini.leastsq()
-        residuals = _calculateTransferFunctionResiduals(minimizer_result.params, data_in, data_out)
-        max_abs_residual = np.max(np.abs(residuals))
-        if max_abs_residual > MAX_ABS_RESIDUAL:
-            msgs.warn("Possible numerical instability: max abs residual is %f" % max_abs_residual)
-        rms_residuals = np.sqrt(np.mean((residuals**2)))
-        stderr_dct = {k: v.stderr for k,v in minimizer_result.params.items()}
-        transfer_function = _makeTransferFunction(minimizer_result.params)
+        if fitter_method == cn.FITTER_METHOD_POLY:
+            fitter = PolyFitter(new_data_ts, input_name=input_name, output_name=self.output_name,
+                                num_zero=num_zero, num_pole=num_pole)
+        elif fitter_method == cn.FITTER_METHOD_GPZ:
+            fitter = GPZFitter(new_data_ts, input_name=input_name, output_name=self.output_name,
+                                num_zero=num_zero, num_pole=num_pole)
+        else:
+            raise ValueError("Unknown method: %s" % fitter_method)
+        fitter.fit()
         #
-        _, y_arr = control.forced_response(transfer_function, T=sel_sec_times, U=staircase_arr, X0=0)
-        output_ts = output_ts.loc[sel_ms_times]
-        output_ts[cn.O_PREDICTED] = y_arr
-        output_ts[staircase_column_name] = staircase_arr
-        output_ts = ctl.Timeseries(output_ts)
-        output_ts.index = sel_ms_times
+        _, y_arr = fitter.simulateTransferFunction(fitter.transfer_function)
+        df = new_data_ts.copy()
+        times = new_data_ts.index/cn.MS_IN_SEC
+        df[cn.O_PREDICTED] = y_arr
+        output_ts = ctl.Timeseries(df, times=times)
+        residuals = output_ts[self.output_name] - output_ts[cn.O_PREDICTED].values
+        rms_residuals = np.sqrt(np.mean(residuals**2))
         fitter_result = cn.FitterResult(
               input_name=self.input_name,
               output_name=self.output_name,
-              transfer_function=transfer_function,
-              stderr=stderr_dct,
-              nfev=minimizer_result.nfev,
-              rms_residuals = rms_residuals,
-              redchi=minimizer_result.redchi,
+              transfer_function=fitter.transfer_function,
               time_series=output_ts,
-              staircase_arr=staircase_arr,
-              staircase_name=staircase_column_name,
-              parameters=minimizer_result.params,
+              staircase_name=input_name,
               antimony_builder=antimony_builder,
-              )
-        return fitter_result
-    
-    @classmethod
-    @Expander(cn.KWARGS, cn.PLOT_KWARGS)
-    def plotFitterResult(cls, fitter_result, mgr=None, **kwargs):
-        """
-        Plots the results of fitting a transfer function for the NonlinearIOSystem.
-        If an option manager is specified, then the caller handles figure generation.
-
-        Parameters
-        ----------
-        fitter_result: FitterResult
-        mgr: OptionManager
-        kwargs: dict
-        #@expand
-        """
-        # Initializations
-        if mgr is None:
-            is_fig = True
-            mgr = OptionManager(kwargs)
-        else:
-            is_fig = False
-        output_name = fitter_result.output_name
-        staircase_arr = fitter_result.staircase_arr
-        staircase_name = fitter_result.staircase_name
-        transfer_function = fitter_result.transfer_function
-        times = fitter_result.time_series.index
-        #
-        ts = fitter_result.time_series.drop(staircase_name, axis=1)
-        util.plotOneTS(ts, mgr=mgr,
-                       colors=[cn.SIMULATED_COLOR, cn.PREDICTED_COLOR],
-                       markers=["o", ""])
-        ax = mgr.plot_opts[cn.O_AX]
-        mgr.plot_opts.set(cn.O_YLABEL, output_name)
-        if mgr.plot_opts[cn.O_AX2] is None:
-            ax2 = ax.twinx()
-            mgr.plot_opts[cn.O_AX2] = ax2
-        else:
-            ax2 = mgr.plot_opts[cn.O_AX2]
-        ax2.set_ylabel(staircase_name, color=cn.INPUT_COLOR)
-        ax2.plot(times/cn.MS_IN_SEC, staircase_arr, color=cn.INPUT_COLOR, linestyle="--")
-        latex = util.latexifyTransferFunction(transfer_function)
-        if len(mgr.plot_opts[cn.O_TITLE]) == 0:
-            #title = "%s->%s;  %s   " % (input_name, output_name, latex)
-            title = latex
-        else:
-            title = mgr.plot_opts[cn.O_TITLE]
-        cls.setYAxColor(ax, "left", cn.SIMULATED_COLOR)
-        cls.setYAxColor(ax2, "right", cn.INPUT_COLOR)
-        ax.set_title(title, y=0.2, pad=-14, fontsize=14, loc="right")
-        mgr.doPlotOpts()
-        ax.legend([output_name, cn.O_PREDICTED], loc="upper left")
-        if is_fig:
-            mgr.doFigOpts()
-        return util.PlotResult(time_series=fitter_result.time_series, ax=ax, ax2=ax2)
+              rms_residuals=rms_residuals)
+        is_plot = kwargs.get(cn.IS_PLOT, True)
+        if is_plot:
+            new_kwargs = dict(mgr.plot_opts.asDict())
+            new_kwargs.update(mgr.fig_opts.asDict())
+            fitter.plot(**new_kwargs) 
+        return fitter_result
```

### Comparing `controlSBML-1.1.3/src/controlSBML/staircase.py` & `controlsbml-1.2.0/src/controlSBML/staircase.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Create a staircase of values. Build multiple staircases."""
 import controlSBML.constants as cn
 
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
+import pandas as pd  # type: ignore
+from typing import Tuple, Optional
 
 
 C_NUM_POINT = "num_point"
 C_NUM_STEP = "num_step"
 
 
 class Staircase(object):
@@ -28,14 +29,15 @@
         self.initial_value = initial_value
         self.num_step = num_step
         self.final_value = final_value
         self.setNumPoint(num_point)  # self.num_point
         self.name = name
         self._updateState()
         #self.staircase_arr is dynamically
+        self.step_start_idxs = None
 
     def __repr__(self):
         dct = {"initial_value": self.initial_value, "num_step": self.num_step,
                "final_value": self.final_value, "num_point": self.num_point}
         return str(dct)
 
     def setNumPoint(self, num_point):
@@ -47,14 +49,15 @@
                          final_value=self.final_value,
                          num_point=self.num_point,
                          name=self.name)
 
     def _updateState(self):
         self.num_level = self.num_step + 1
         self.point_per_level = int(self.num_point/self.num_level)
+        self.step_start_arr = np.array([n*self.point_per_level for n in range(self.num_level)])
 
     @property
     def staircase_arr(self):
         self._updateState()
         #
         steps = []  # Steps in the staircase
         #
@@ -69,15 +72,43 @@
         if num_add_more < 0:
             raise RuntimeError("Negative residual count")
         elif num_add_more > 0:
             final_values = np.repeat(self.final_value, num_add_more)
             staircase_arr = np.append(staircase_arr, final_values)
         #
         return staircase_arr
-        
+    
+    def makeEndStepInfo(self, start_idx:int=0, end_idx:Optional[int]=None, num_point=3)->Tuple[np.ndarray, np.ndarray]:
+        """
+        Returns information about the end of the steps.
+
+        Args:
+            num_point: int (number at the end of the step to report)
+            start_idx: int (starting index)
+            end_idx: int (ending index)
+
+        Returns
+        -------
+        np.array[float]: num_point values at the end of the steps
+        np.array[int]: indices of the points in staircase_arr
+        """
+        if num_point > self.point_per_level:
+            raise ValueError("num_point > point_per_level")
+        if end_idx is None:
+            end_idx = self.num_point - 1
+        arr = self.staircase_arr
+        trail_values = []
+        idxs = []
+        for idx in range(self.num_step+1):
+            end_pos = self.step_start_arr[idx] + self.point_per_level
+            start_pos = end_pos - num_point
+            if (start_pos >= start_idx) and (end_pos-1 <= end_idx):
+                trail_values.extend(arr[start_pos:end_pos])
+                idxs.extend(list(range(start_pos, end_pos)))
+        return np.array(trail_values), np.array(idxs)
 
     @classmethod
     def makeRelativeStaircase(cls, center=5, fractional_deviation=0.1,
                               num_step=cn.DEFAULT_NUM_STEP, num_point=cn.DEFAULT_NUM_POINT):
         """
         Specifies the staircase relative to a center point.
 
@@ -93,15 +124,18 @@
         Staircase
         """
         max_deviation = center*fractional_deviation
         return cls(initial_value=center - max_deviation,
             final_value=center + max_deviation,
             num_step=num_step, num_point=num_point)
         
-    def plot(self):
+    def plot(self, is_plot=True):
         """
         Plots the staircase.
         """
-        staircase_ser = pd.Series(self.staircase_arr)
-        fig, ax = plt.subplots()
-        staircase_ser.plot(ax=ax)
-        return fig
+        if is_plot:
+            staircase_ser = pd.Series(self.staircase_arr)
+            fig, ax = plt.subplots()
+            staircase_ser.plot(ax=ax)
+            return fig
+        else:
+            return None
```

### Comparing `controlSBML-1.1.3/src/controlSBML/timeseries.py` & `controlsbml-1.2.0/src/controlSBML/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 import controlSBML as ctl
 from controlSBML import util
 import controlSBML.constants as cn
 
 import numpy as np
-import pandas as pd
+import pandas as pd # type: ignore
 
 ############# FUNCTIONS ###############
 def findCommonIndices(index1, index2):
     """
     Finds the indices common to both.
 
     Parameters
```

### Comparing `controlSBML-1.1.3/src/controlSBML/util.py` & `controlsbml-1.2.0/src/controlSBML/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import control # type: ignore
 from controlSBML.option_management.option_manager import OptionManager
 from controlSBML import msgs
 
 from docstring_expander.expander import Expander # type: ignore
 import matplotlib.pyplot as plt
 import numpy as np
+import os
 import pandas as pd # type: ignore
 import seaborn as sns # type: ignore
 import urllib.request
 from typing import Optional, List
 
 
 REPO_URL =  "https://github.com/ModelEngineering/controlSBML/raw/main"
@@ -52,14 +53,28 @@
     local_python = "python.py"
     _, _ = urllib.request.urlretrieve(url=url, filename=local_python)
     with open(local_python, "r") as fd:
         code_str = "".join(fd.readlines())
     print(code_str)
     exec(code_str, globals())
 
+def getModelPath(filename:str)->str:
+    """
+    Obtains a local model from the github repository.
+
+    Parameters
+    ----------
+    file_name: str (without extension)
+
+    Returns
+    -------
+    str
+    """
+    return os.path.join(cn.MODEL_DIR, filename + ".ant")
+
 def getModel(file_name=MODEL_823_FILE):
     """
 
     Parameters
     ----------
     file_name: str (filename with extension)
 
@@ -82,15 +97,15 @@
 
     Parameters
     ----------
     time_series: TimeSeries
     mgr: OptionsManager
     colors: list-str
     markers: list-str
-    legend: bool (whether to show legend)
+    legend: True (show legend), False (no legend), List (legend names)
     #@expand
 
     Returns
     -------
     PlotResult
     """
     MARKERS = ["o", "s", "v", "^", "x", "+"]
@@ -113,20 +128,33 @@
         fig = kwargs[cn.O_FIGURE]
     else:
         fig = None
     if ax is None:
         fig, ax = plt.subplots(1)
         mgr.plot_opts.set(cn.O_AX, ax)
     times = np.array(time_series.index)/cn.MS_IN_SEC
+    if mgr.plot_opts[cn.O_XLIM] is None:
+        mgr.plot_opts.set(cn.O_XLIM, [times[0], times[-1]])
     sel_colors = list(colors)
     sel_markers = list(markers)
+    if cn.O_SELECTIONS in kwargs.keys():
+        selections = kwargs[cn.O_SELECTIONS]
+    else:
+        selections = time_series.columns
     for column in time_series.columns:
+        if not column in selections:
+            continue
         ax.plot(times, time_series[column], color=sel_colors.pop(0), marker=sel_markers.pop(0))
-    if legend:
-        legend_spec = cn.LegendSpec(time_series.columns, crd=mgr.plot_opts[cn.O_LEGEND_CRD])
+    ax.set_xlim(mgr.plot_opts[cn.O_XLIM])
+    if isinstance(legend, bool):
+        if legend:
+            legend_spec = cn.LegendSpec(time_series.columns, crd=mgr.plot_opts[cn.O_LEGEND_CRD])
+            mgr.plot_opts.set(cn.O_LEGEND_SPEC, default=legend_spec)
+    elif isinstance(legend, list):
+        legend_spec = cn.LegendSpec(legend, crd=mgr.plot_opts[cn.O_LEGEND_CRD])
         mgr.plot_opts.set(cn.O_LEGEND_SPEC, default=legend_spec)
     mgr.doPlotOpts()
     if is_fig:
         mgr.doFigOpts()
     return PlotResult(ax=ax, ax2=None, fig=fig, time_series=time_series)
 
 @Expander(cn.KWARGS, cn.PLOT_KWARGS)
@@ -206,15 +234,15 @@
 
     Args:
         kP: float
         kI: float
         kD: float
 
     Raises:
-        ValueError: must provide at least one of kp, ki, kd
+        ValueError: must provide at least one of kP, kI, kD
 
     Returns:
         control.TransferFunction
     """
     is_none = True
     controller_tf = control.tf([0], [1], name=name, inputs=input_name, outputs=output_name)
     if kP is not None:
@@ -223,15 +251,15 @@
     if kI is not None:
         is_none = False
         controller_tf += control.tf([kI], [1, 0])
     if kD is not None:
         is_none = False
         controller_tf += control.tf([kD, 0], [1])
     if is_none:
-        raise ValueError("At least one of kp, ki, kd, kf must be defined")
+        raise ValueError("At least one of kP, kI, kD, kF must be defined")
     controller_tf.name = name
     controller_tf.input_labels = [input_name]
     controller_tf.output_labels = [output_name]
     return controller_tf
 
 def mat2DF(mat:np.array, column_names:Optional[List[str]]=None, row_names:Optional[List[str]]=None):
     """
@@ -411,15 +439,63 @@
         if isLastZero(num) and isLastZero(den):
             num = num[:-1]
             den = den[:-1]
         else:
             break
     return control.TransferFunction(num, den)
 
-def latexifyTransferFunction(tf, num_decimal=2):
+def latexifyTransferFunction(tf):
+    """_summary_
+
+    Args:
+        tf (_type_): _description_
+
+    Raises:
+        RuntimeError: _description_
+
+    Returns:
+        _type_: _description_
+    """
+    LEFT_NUMERATOR = "left_numerator"
+    RIGHT_NUMERATOR = "right_numerator"
+    FRACTION_BAR = "fraction_bar"
+    LEFT_DENOMINATOR = "left_denominator"
+    RIGHT_DENOMINATOR = "right_denominator"
+    NEWLINE = "\n"
+    stg = str(tf)
+    latex = ""
+    stage = LEFT_NUMERATOR
+    for pos in range(len(stg)):
+        if stage == FRACTION_BAR:
+            if stg[pos] == "-":
+                continue
+            stage = LEFT_DENOMINATOR
+        if stg[pos:pos+1] == NEWLINE:
+            if stage == LEFT_NUMERATOR:
+                stage = RIGHT_NUMERATOR
+                latex += r'\frac{'
+            elif stage == RIGHT_NUMERATOR:
+                stage = FRACTION_BAR
+                latex += "}"
+            elif stage == FRACTION_BAR:
+                if stg[pos] == "-":
+                    continue
+                stage = LEFT_DENOMINATOR
+            elif stage == LEFT_DENOMINATOR:
+                stage = RIGHT_NUMERATOR
+                latex += "{"
+            elif stage == RIGHT_DENOMINATOR:
+                latex += "}"
+            else:
+                raise RuntimeError("Unknown stage")
+        else:
+            latex += stg[pos]
+    return r'$%s$' % latex
+
+def oldlatexifyTransferFunction(tf, num_decimal=10):
     """
     Generates latex for the transfer function, rounding to the number of decimal digits.
 
     Args:
         tf (control.TransferFunction)
         num_decimal (int, optional): number of decimal digits
     """
@@ -527,15 +603,15 @@
         arg_min: float
         arg_max: float
         num_point: int
         max_mse: float (maximum root mean square error if the same)
     """
     values = np.linspace(arg_min, arg_max, num_point)
     squared_diff_arr = np.array([(func1(v) - func2(v))**2 for v in values])
-    mse = np.sum(squared_diff_arr)/len(values)
+    mse = np.mean(squared_diff_arr)
     if mse < max_rmse**2:
         return True
     else:
         return False
     
 def allEqual(list1, list2):
     if len(list1) != len(list2):
@@ -611,20 +687,57 @@
     """
     Rounds so that there are the specified number of non-zero digits.
 
     Args:
         number (float)
         num_digits (int, optional)
     """
+    if np.isclose(number, 0):
+        return 0
     log_number = np.log10(number)
     if log_number > 0:
         return np.round(number, num_digits)
     required_decimal = -int(log_number) + num_digits
     return np.round(number, required_decimal)
 
+def subsetDct(dct:dict, keys:List[str], default:Optional[dict]=None)->dict:
+    """
+    Returns a subset of a dictionary.
+
+    Args:
+        dct: dict
+        keys: list-str
+        default: dict (default values of subsetted keys)
+    Returns:
+        dict
+    """
+    new_dct = {}
+    for key in keys:
+        if key in dct.keys():
+            new_dct[key] = dct[key]
+        elif (default is not None) and (key in default.keys()):
+            new_dct[key] = default[key]
+    return new_dct
+
+def differenceDct(dct1, dct2):
+    """
+    Returns the difference between two dictionaries.
+
+    Args:
+        dct1: dict
+        dct2: dict
+    Returns:
+        dict
+    """
+    new_dct = {}
+    for key, value in dct1.items():
+        if key not in dct2.keys():
+            new_dct[key] = value
+    return new_dct
+
 
 ############### CLASSES ################
 
 class PlotResult(object):
     """
     Contains data returned from a plot method.
```

### Comparing `controlSBML-1.1.3/src/controlSBML.egg-info/PKG-INFO` & `controlsbml-1.2.0/src/controlSBML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlSBML
-Version: 1.1.3
+Version: 1.2.0
 Summary: Control analysis of SBML models
 Author-email: Joseph Hellerstein <joseph.hellerstein@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Joseph Hellerstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,14 +66,19 @@
 To find the current version:
 ```
 import controlSBML as ctl
 ctl.__version__
 ```
 
 ## Version History
+* 1.2.0
+    * Implemented differential control
+    * Extended noise model to include lognormal distribution, offset, and slope
+    * Implemented several examples, some of which are based on student projects
+    * Two algorithms for fitting. gpz fits the transfer function in order by gain (g), poles (p), zeroes (z). poly fits a polynomial in s to the simulations.
 * 1.1.03 1/20/2024
     * Better error checking
     * API uses parameter names kI, kP, kF
 * 1.1.02 12/27/2023
     * Fix bug in dependencies. Update header documentation.
 * 1.1.01 12/27/2023
     * Complete change in the architecture. Instead of using NonlinearIOSystems in the python control package, controlSBML generates Antimony code to implement staircase functions and closed loops.
```

### Comparing `controlSBML-1.1.3/src/controlSBML.egg-info/SOURCES.txt` & `controlsbml-1.2.0/src/controlSBML.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 setup.cfg
 src/controlSBML/__init__.py
 src/controlSBML/_version.py
 src/controlSBML/antimony_builder.py
 src/controlSBML/constants.py
 src/controlSBML/control_sbml.py
 src/controlSBML/dict_array.py
+src/controlSBML/gpz_fitter.py
 src/controlSBML/grid.py
 src/controlSBML/iterate_biomodels.py
 src/controlSBML/make_roadrunner.py
 src/controlSBML/msgs.py
 src/controlSBML/option_set.py
 src/controlSBML/parallel_search.py
 src/controlSBML/point_evaluator.py
+src/controlSBML/poly_fitter.py
 src/controlSBML/sbml_system.py
 src/controlSBML/siso_closed_loop_designer.py
 src/controlSBML/siso_maker.py
 src/controlSBML/siso_transfer_function_builder.py
+src/controlSBML/siso_transfer_function_fitter.py
 src/controlSBML/staircase.py
 src/controlSBML/timeseries.py
 src/controlSBML/util.py
 src/controlSBML.egg-info/PKG-INFO
 src/controlSBML.egg-info/SOURCES.txt
 src/controlSBML.egg-info/dependency_links.txt
 src/controlSBML.egg-info/not-zip-safe
@@ -49,19 +52,22 @@
 src/controlSBML/control_extensions/state_space_tf.py
 src/controlSBML/option_management/__init__.py
 src/controlSBML/option_management/option_manager.py
 src/controlSBML/option_management/options.py
 tests/test_antimony_builder.py
 tests/test_control_sbml.py
 tests/test_dict_array.py
+tests/test_gpz_fitter.py
 tests/test_grid.py
 tests/test_iterate_biomodels.py
 tests/test_make_roadrunner.py
 tests/test_option_set.py
 tests/test_parallel_search.py
+tests/test_poly_fitter.py
 tests/test_sbml_system.py
 tests/test_siso_closed_loop_designer.py
 tests/test_siso_maker.py
 tests/test_siso_transfer_function_builder.py
+tests/test_siso_transfer_function_fitter.py
 tests/test_staircase.py
 tests/test_timeseries.py
 tests/test_util.py
```

### Comparing `controlSBML-1.1.3/tests/test_dict_array.py` & `controlsbml-1.2.0/tests/test_dict_array.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from controlSBML.dict_array import DictArray
 
 import unittest
 
 
 IGNORE_TEST = False
-DICTS = [{"kp": 1}, {"ki": 2, "kp": 3}, {"kf": 4, "kp": 5}]
+DICTS = [{"kP": 1}, {"kI": 2, "kP": 3}, {"kF": 4, "kP": 5}]
 
 #############################
 # Tests
 #############################
 class TestDictList(unittest.TestCase):
 
     def setUp(self):
@@ -42,15 +42,15 @@
         self.check(dl=dl)
         self.assertTrue(dl == self.dl)
 
     def testAppend(self):
         if IGNORE_TEST:
             return
         dl = self.dl.copy()
-        dl.append(kp=6)
+        dl.append(kP=6)
         self.check(dl=dl)
 
     def testMakeDicts(self):
         if IGNORE_TEST:
             return
         dcts = self.dl.makeDicts()
         dl = self.dl.makeFromDicts(dcts)
@@ -64,14 +64,14 @@
         self.assertEqual(dl, self.dl)
 
     def testEquals(self):
         if IGNORE_TEST:
             return
         dl = self.dl.copy()
         self.assertTrue(dl == self.dl)
-        dl.append(kp=6)
+        dl.append(kP=6)
         self.assertFalse(dl == self.dl)
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `controlSBML-1.1.3/tests/test_grid.py` & `controlsbml-1.2.0/tests/test_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from controlSBML.grid import Grid, Axis
-from controlSBML.timeseries import Timeseries
+from controlSBML.grid import Grid, Axis  # type: ignore
 
 import numpy as np
 import unittest
 
 
 IGNORE_TEST = False
 IS_PLOT = False
@@ -67,15 +66,15 @@
             self.grid.addAxis(parameter_name, min_value=1000, max_value=10, num_coordinate=NUM_COORDINATE)
 
     def test_num_point(self):
         if IGNORE_TEST:
             return
         self.grid.addAxis("test1", min_value=0, max_value=10, num_coordinate=NUM_COORDINATE)
         self.grid.addAxis("test2", min_value=0, max_value=10, num_coordinate=NUM_COORDINATE)
-        self.assertEqual(self.grid.num_point, (NUM_COORDINATE-1)**2)
+        self.assertEqual(self.grid.num_point, NUM_COORDINATE**2)
 
     def testRepr(self):
         if IGNORE_TEST:
             return
         self.grid.addAxis("test1", min_value=0, max_value=10, num_coordinate=NUM_COORDINATE)
         self.grid.addAxis("test2", min_value=0, max_value=10, num_coordinate=NUM_COORDINATE)
         self.assertEqual(str(self.grid).count("test"), 2)
@@ -83,14 +82,20 @@
     def testIteratePoint(self):
         if IGNORE_TEST:
             return
         self.grid.addAxis("test1", min_value=0, max_value=10, num_coordinate=5)
         self.grid.addAxis("test2", min_value=100, max_value=200, num_coordinate=NUM_COORDINATE)
         points = list(self.grid._iteratePoints())
         self.assertEqual(len(points), self.grid.num_point)
+        #
+        grid = Grid()
+        grid.addAxis("test1", min_value=5, max_value=5, num_coordinate=1)
+        grid.addAxis("test2", min_value=15, max_value=15, num_coordinate=1)
+        points = list(grid._iteratePoints())
+        self.assertEqual(len(points), 1)
 
     def testPlot(self):
         if IGNORE_TEST:
             return
         for is_random in [True, False]:
             grid = Grid(is_random=is_random)
             grid.addAxis("parm1", min_value=0, max_value=10, num_coordinate=10)
```

### Comparing `controlSBML-1.1.3/tests/test_iterate_biomodels.py` & `controlsbml-1.2.0/tests/test_iterate_biomodels.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from controlSBML.iterate_biomodels import iterateBiomodels
+from controlSBML.iterate_biomodels import iterateBiomodels  # type: ignore
 
 import os
 import unittest
-import tellurium as te
+import tellurium as te  # type: ignore
 
 
 IGNORE_TEST = False
 IS_PLOT = False
 
 
 #############################
```

### Comparing `controlSBML-1.1.3/tests/test_make_roadrunner.py` & `controlsbml-1.2.0/tests/test_make_roadrunner.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/tests/test_option_set.py` & `controlsbml-1.2.0/tests/test_option_set.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/tests/test_parallel_search.py` & `controlsbml-1.2.0/tests/test_parallel_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import time
 import unittest
 
 
 IGNORE_TEST = False
 IS_PLOT = False
-CANDIDATES = [{"kp": 1}, {"ki": 2, "kp": 3}, {"kf": 4, "kp": 5}]
+CANDIDATES = [{"kP": 1}, {"kI": 2, "kP": 3}, {"kF": 4, "kP": 5}]
 
 
 class MyEvaluator(Evaluator):
 
     def __init__(self, wait_time:float=0):
         self.wait_time = wait_time
 
@@ -64,15 +64,15 @@
         search = ParallelSearch(evaluator, candidates, num_process=num_process)
         search.search()
         best_candidate = search.getBestCandidate()
         self.assertEqual(len(search._search_results_dict_array), len(candidates))
         self.assertTrue(best_candidate is not None)
         if expected_score is not None:
             self.assertEqual(best_candidate[cn.SCORE], expected_score)
-        trues = [c in best_candidate.keys() for c in ["kp", "ki", "kf", "score"]]
+        trues = [c in best_candidate.keys() for c in ["kP", "kI", "kF", "score"]]
         self.assertTrue(all(trues))
 
     def testSearchOneProcess(self):
         if IGNORE_TEST:
             return
         self.doSearch(1)
```

### Comparing `controlSBML-1.1.3/tests/test_sbml_system.py` & `controlsbml-1.2.0/tests/test_sbml_system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from controlSBML.sbml_system import SBMLSystem
-from controlSBML import util
-import controlSBML.constants as cn
-from controlSBML.timeseries import Timeseries
+from controlSBML.sbml_system import SBMLSystem # type: ignore
+from controlSBML import util # type: ignore
+import controlSBML.constants as cn # type: ignore
+from controlSBML.timeseries import Timeseries # type: ignore
 
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
+import pandas as pd # type: ignore
 import unittest
 
 
 IGNORE_TEST = False
 IS_PLOT = False
 IMPROPER_LINEAR_MDL = """
 // Illustrate Antimony File
@@ -64,14 +64,28 @@
             _ = SBMLSystem(LINEAR_MDL, ["S1"], ["S9"])
 
     def testConstructor3(self):
         if IGNORE_TEST:
                 return
         self.system = SBMLSystem(LINEAR_MDL, ["aa"], ["bb"], is_fixed_input_species=True)
 
+    def testRoadrunner(self):
+        if IGNORE_TEST:
+            return
+        def test(dct):
+            self.assertIsNotNone(dct)
+            self.assertGreater(len(dct), 0)
+        #
+        _ = self.system.roadrunner
+        self.assertTrue("RoadRunner" in str(type(self.system._roadrunner)))
+        test(self.system._max_value_dct)
+        test(self.system._min_value_dct)
+        trues = [l < u for l, u in zip(self.system._min_value_dct.values(), self.system._max_value_dct.values())]
+        self.assertTrue(all(trues))
+
     def testGet(self):
         if IGNORE_TEST:
             return
         for name in SPECIES_NAMES:
             self.assertEqual(self.system.get(name), self.system._roadrunner[name])
 
     def testSet(self):
@@ -90,15 +104,15 @@
        
     def testSimulateSISOClosedLoop(self):
         if IGNORE_TEST:
             return
         def test(is_fixed_input_species):
             system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], is_fixed_input_species=is_fixed_input_species)
             setpoint = 5
-            ts, _ = system.simulateSISOClosedLoop("S1", "S3", kp=2, ki=0.8, kf=0.5, setpoint=setpoint, end_time=200, num_point=1000)
+            ts, _ = system.simulateSISOClosedLoop("S1", "S3", kP=2, kI=0.8, kF=0.5, setpoint=setpoint, end_time=200, num_point=1000)
             self.assertGreater(len(ts), 0)
             if is_fixed_input_species:
                 tolerance = 0.1
             else:
                 tolerance = 0.1
             self.assertLess(np.abs(ts["S3"].values[-1] - setpoint), tolerance)
             if IS_PLOT:
@@ -111,20 +125,67 @@
                     title = "Boundary reaction"
                 util.plotOneTS(ts, ax2=0, figsize=(8,8), title=title)
                 plt.show()
         #
         test(True)
         test(False)
 
+    def testSimulateSISOClosedLoopWithNoiseDisturbance(self):
+        if IGNORE_TEST:
+            return
+        def test(sine_amp, random_mag):
+            noise_spec = cn.NoiseSpec(sine_amp=sine_amp, random_mag=random_mag)
+            system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], noise_spec=noise_spec,
+                                is_fixed_input_species=True)
+            setpoint = 5
+            ts, _ = system.simulateSISOClosedLoop("S1", "S3", kP=2, kI=0.8, kF=0.5,
+                                                        setpoint=setpoint, end_time=200, num_point=1000)
+            TOLERANCE = 0.5
+            abs_control_error = np.abs(ts["S3"].values[-1] - setpoint)
+            self.assertGreater(len(ts), 0)
+            self.assertLess(abs_control_error, TOLERANCE)
+            if IS_PLOT:
+                for column in ts.columns:
+                    if column not in ["time", "S1", "S3"]:
+                        del ts[column]
+                util.plotOneTS(ts, ax2=0, figsize=(8,8), title=f"Sine amp: {sine_amp}, Noise mag: {random_mag}")
+                plt.show()
+        #
+        test(sine_amp=0.1, random_mag=0.1)
+
+    def testSimulateSISOClosedLoopWithNoiseDisturbance2(self):
+        if IGNORE_TEST:
+            return
+        def test(sine_amp, random_mag):
+            if np.isclose(sine_amp, 0):
+                sine_freq = 0
+            else:
+                sine_freq = 0.1
+            if np.isclose(random_mag, 0):
+                random_std = 0
+            else:
+                random_std = 0.01
+            noise_spec = cn.NoiseSpec(sine_amp=sine_amp, sine_freq=sine_freq, random_mag=random_mag,
+                                      random_std=random_std)
+            system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], noise_spec=noise_spec, disturbance_spec=noise_spec,
+                                is_fixed_input_species=True)
+            setpoint = 5
+            ts, _ = system.simulateSISOClosedLoop("S1", "S3", kP=2, kI=0.8, kF=0.5,
+                                                        setpoint=setpoint, end_time=200, num_point=1000)
+            self.assertGreater(ts["noise_S1_S3_ot"].std(), 0)
+            self.assertGreater(ts["disturbance_S1_S3_ot"].std(), 0)
+        #
+        test(sine_amp=0.1, random_mag=0.1)
+
     def testSimulateStaircase(self):
         if IGNORE_TEST:
             return
         times = np.linspace(0, 50, 500)
         def test(is_fixed_input_species):
-            system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], is_fixed_input_species=True)
+            system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], is_fixed_input_species=is_fixed_input_species)
             ts, _ = system.simulateStaircase("S1", "S3", times=times, final_value=10, num_step=5, is_steady_state=False)
             self.assertGreater(len(ts), 0)
             variance = np.var(ts["S3"])
             self.assertFalse(np.isclose(variance, 0))
             if IS_PLOT:
                 util.plotOneTS(ts, ax2=0, figsize=(8,8), ylim=[0, 10])
                 plt.show()
@@ -139,28 +200,32 @@
         self.assertTrue(system == self.system)
         #
         times = np.linspace(0, 50, 500)
         _ = system.simulateStaircase("S1", "S3", times=times, final_value=10, num_step=5, is_steady_state=False)
         self.assertFalse(system == self.system)
 
     def testPlotSISOClosedLoop(self):
-        #if IGNORE_TEST:
-        #    return
-        system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], is_fixed_input_species=False)
-        setpoint = 5
-        ts, _ = system.simulateSISOClosedLoop(input_name="S1", output_name="S3", kp=2, ki=0.8, kf=0.5,
-                                           setpoint=setpoint, end_time=100, num_point=1000)
-        self.system.plotSISOClosedLoop(ts, setpoint, figsize=(5,5), title="Closed Loop", is_plot=IS_PLOT)
-
-    def testPlotModel(self):
         if IGNORE_TEST:
             return
-        system = SBMLSystem(LINEAR_MDL)
-        ts = system.plotModel(is_plot=IS_PLOT)
-        self.assertTrue(isinstance(ts, Timeseries))
+        noise_spec = cn.NoiseSpec(sine_amp=1, sine_freq=10, random_mag=0.1, random_std=0.1)
+        disturbance_spec = cn.NoiseSpec(sine_amp=1, sine_freq=10, random_mag=0.1, random_std=0.1, offset=3)
+        system = SBMLSystem(LINEAR_MDL, ["S1"], ["S3"], is_fixed_input_species=True,
+                            noise_spec=noise_spec,
+                            disturbance_spec=disturbance_spec
+                            )
+        setpoint = 5
+        selections = ["time", "S3",
+                      "noise_S1_S3_ot",
+                      "disturbance_S1_S3_ot"
+                      ]
+        ts, _ = system.simulateSISOClosedLoop(input_name="S1", output_name="S3", kP=2, kI=0.8, kF=0.5,
+                                              selections=selections,
+                                              setpoint=setpoint, end_time=100, num_point=1000)
+        self.system.plotSISOClosedLoop(ts, setpoint, figsize=(5,5), markers=["+", "o"], selections=selections,
+                                       title="Closed Loop", is_plot=IS_PLOT, legend=selections)
 
     def testGetValidSymbolsInput(self):
         if IGNORE_TEST:
             return
         input_ser = self.system.getValidSymbols(is_input=True, is_str=False)
         self.assertTrue(isinstance(input_ser, pd.Series))
         self.assertTrue("S1" in input_ser.loc[cn.TYPE_FLOATING_SPECIES])
@@ -180,8 +245,8 @@
         self.assertFalse("J1" in output_ser.index)
         #
         out_str = self.system.getValidOutputs()
         self.assertTrue(isinstance(out_str, str))
 
 
 if __name__ == '__main__':
-  unittest.main()
+    unittest.main()
```

### Comparing `controlSBML-1.1.3/tests/test_siso_closed_loop_designer.py` & `controlsbml-1.2.0/tests/test_siso_closed_loop_designer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 from controlSBML.staircase import Staircase # type: ignore
 import controlSBML.util as util # type: ignore
 
 import copy
 import control # type: ignore
 import numpy as np
 import os
+import pandas as pd  # type: ignore
 import sympy # type: ignore
 import unittest
 
 IGNORE_TEST = False
 IS_PLOT = False
 FIGSIZE = (5, 5)
-helpers.setupPlotting(__file__)
+#helpers.setupPlotting(__file__)
 MODEL = """
 model *main_model()
 S0 -> S1; k0*S0
 S1 -> S2; k1*S1
 
 k0 = 1
 k1 = 1
@@ -60,25 +61,25 @@
 k0 = 0
 k1 = 1
 k2 = 2
 k3 = 3
 end
 """
 # Construct a transfer function for the model. This is a linear model, and so it should be accurate.
-CONTROL_PARAMETERS = ["kp", "ki", "kf"]
+CONTROL_PARAMETERS = ["kP", "kI", "kD", "kF"]
 INPUT_NAME = "S0"
 OUTPUT_NAME = "S2"
 SYSTEM = SBMLSystem(MODEL2, input_names=[INPUT_NAME], output_names=[OUTPUT_NAME], is_fixed_input_species=True)
 TRANSFER_FUNCTION = control.TransferFunction(np.array([1.51083121, 2.01413339]), np.array([1.67214802, 1.24125478, 9.99999997]))
 TIMES = np.linspace(0, 20, 200)
 PARAMETER_DCT = {p: n+1 for n, p in enumerate(CONTROL_PARAMETERS)}
 SETPOINT = 3
 SAVE_PATH = os.path.join(cn.TEST_DIR, "siso_closed_loop_designer.csv")
 REMOVE_FILES = [SAVE_PATH]
-CONTROL_PARAMETER_SPECS = ["kp_spec", "ki_spec", "kf_spec"]
+CONTROL_PARAMETER_SPECS = ["kP_spec", "kI_spec", "kD_spec", "kF_spec"]
 #if False:
 #    # Required to construct the transfer function
 #    builder = SISOTransferFunctionBuilder(SYSTEM, input_name=INPUT_NAME, output_name=OUTPUT_NAME)
 #    staircase = ctl.Staircase(final_value=15, num_step=5)
 #    fitter_result = builder.fitTransferFunction(num_numerator=2, num_denominator=3, staircase=staircase)
 #    if False:
 #        builder.plotFitTransferFunction(fitter_result, figsize=(5,5))
@@ -126,171 +127,203 @@
         for name in CONTROL_PARAMETERS:
             self.assertEqual(dct[name], PARAMETER_DCT[name])
 
     def testCalculateClosedLoopTf(self):
         if IGNORE_TEST:
             return
         sys_tf = control.tf([1], [1, 2])
-        closed_loop_tf_kp = cld._calculateClosedLoopTransferFunction(open_loop_transfer_function=sys_tf, kp=3)
-        closed_loop_tf_ki = cld._calculateClosedLoopTransferFunction(open_loop_transfer_function=sys_tf, ki=3)
-        _, ys_kp = control.step_response(closed_loop_tf_kp, TIMES)
-        _, ys_ki = control.step_response(closed_loop_tf_ki, TIMES)
-        self.assertTrue(ys_kp[-1] < ys_ki[-1])
-        self.assertTrue(np.isclose(ys_ki[-1], 1, atol=0.01))
+        closed_loop_tf_kP = cld._calculateClosedLoopTransferFunction(open_loop_transfer_function=sys_tf, kP=3)
+        closed_loop_tf_kI = cld._calculateClosedLoopTransferFunction(open_loop_transfer_function=sys_tf, kI=3)
+        closed_loop_tf_kP = cld._calculateClosedLoopTransferFunction(open_loop_transfer_function=sys_tf, kP=3, kD=2)
+        _, ys_kP = control.step_response(closed_loop_tf_kP, TIMES)
+        _, ys_kI = control.step_response(closed_loop_tf_kI, TIMES)
+        self.assertTrue(ys_kP[-1] < ys_kI[-1])
+        self.assertTrue(np.isclose(ys_kI[-1], 1, atol=0.01))
 
     def testDesign(self):
         if IGNORE_TEST:
             return
         self.init()
         def checkParams(names):
             for name in names:
                 self.assertIsNotNone(getattr(designer, name))
             other_names = set(CONTROL_PARAMETERS) - set(names)
             for name in other_names:
                 self.assertIsNone(getattr(designer, name))
         designer = cld.SISOClosedLoopDesigner(SYSTEM, self.sys_tf, times=np.linspace(0, 200, 1000))
-        designer.design(kp_spec=True, ki_spec=True, num_restart=1, max_value=10)
+        designer.design(kP_spec=True, kI_spec=True, kD_spec=0.1, num_restart=1, max_value=10)
         param_dct = designer.get()
         designer.evaluate(is_plot=IS_PLOT)
-        checkParams(["kp", "ki"])
+        checkParams(["kP", "kI", "kD"])
         #
         designer = cld.SISOClosedLoopDesigner(SYSTEM, self.sys_tf, times=np.linspace(0, 200, 1000), setpoint=5)
         designer.set(**param_dct)
         designer.evaluate(is_plot=IS_PLOT)
 
     def testSimulate(self):
         if IGNORE_TEST:
             return
         def calcDiff(arr):
             return np.abs(arr[-1] - 1)
         #
         sys_tf = control.tf([1], [1, 1])
         designer = cld.SISOClosedLoopDesigner(SYSTEM, sys_tf)
-        designer.set(kp=20)
+        designer.set(kP=20)
         _, prediction1s = designer.simulateTransferFunction()
-        designer.set(kp=20, ki=50)
+        designer.set(kP=20, kI=50)
+        designer.set(kP=20, kI=50, kD=2)
         _, prediction2s = designer.simulateTransferFunction()
         self.assertLess(calcDiff(prediction2s), calcDiff(prediction1s))
 
     def testPlot(self):
         if IGNORE_TEST:
             return
+        self.init()
         self.designer.set(**PARAMETER_DCT)
         self.designer.plot(is_plot=IS_PLOT, markers=["", ""])
-        self.designer.set(kp=10, ki=5)
+        self.designer.set(kP=10, kI=5, kD=2)
         self.designer.plot(is_plot=IS_PLOT)
 
-    def makeDesigner(self, end_time=200):
+    def makeDesigner(self, end_time=200, is_save_path=True):
         times = np.linspace(0, end_time, 10*end_time)
         system = copy.deepcopy(SYSTEM)
         transfer_function = copy.deepcopy(TRANSFER_FUNCTION)
-        designer = cld.SISOClosedLoopDesigner(system, transfer_function, times=times, save_path=SAVE_PATH)
+        if is_save_path:
+            save_path = SAVE_PATH
+        else:
+            save_path = None
+        designer = cld.SISOClosedLoopDesigner(system, transfer_function, times=times, save_path=save_path)
         return designer
 
     def testPlot2(self):
         if IGNORE_TEST:
             return
         designer = self.makeDesigner()
-        designer.design(kp_spec=True, ki_spec=True, min_value=0.1, max_value=10, num_restart=1)
+        designer.design(kP_spec=True, kI_spec=True, min_value=0.1, max_value=10, num_restart=1)
         designer.plot(is_plot=IS_PLOT, markers=["", ""])
-        self.assertGreater(designer.kp, 0)
-        self.assertGreater(designer.ki, 0)
-        self.assertIsNone(designer.kf)
+        self.assertGreater(designer.kP, 0)
+        self.assertGreater(designer.kI, 0)
+        self.assertIsNone(designer.kF)
 
     def testPlot3(self):
         if IGNORE_TEST:
             return
         designer = self.makeDesigner()
-        designer.design(kp_spec=True, ki_spec=True, kf_spec=True, min_value=0.1, max_value=10, 
+        designer.design(kP_spec=True, kI_spec=True, kF_spec=True, min_value=0.1, max_value=10, 
                         num_coordinate=5, num_restart=1, is_report=IGNORE_TEST)
         designer.plot(is_plot=IS_PLOT, markers=["", ""])
-        self.assertGreater(designer.kp, 0)
-        self.assertGreater(designer.ki, 0)
-        self.assertGreater(designer.kf, 0)
+        self.assertGreater(designer.kP, 0)
+        self.assertGreater(designer.kI, 0)
 
     def testDesignAlongGrid(self):
         if IGNORE_TEST:
             return
         designer = self.makeDesigner()
         grid = Grid(min_value=0.1, max_value=10, num_coordinate=5)
-        grid.addAxis("kp")
-        designer.designAlongGrid(grid)
-        self.assertGreater(designer.kp, 0)
-        self.assertIsNone(designer.ki)
-        self.assertIsNone(designer.kf)
+        grid.addAxis("kP")
+        result = designer.designAlongGrid(grid, num_process=2)
+        self.assertTrue(isinstance(result.dataframe, pd.DataFrame))
+        self.assertGreater(designer.kP, 0)
+        self.assertIsNone(designer.kI)
+        self.assertIsNone(designer.kD)
+        self.assertIsNone(designer.kF)
     
     def testDesignAlongGridParallel(self):
         if IGNORE_TEST:
             return
         designer = self.makeDesigner()
         grid = Grid(min_value=0.1, max_value=10, num_coordinate=11)
         grid = Grid(min_value=0.1, max_value=10, num_coordinate=5, is_random=False)
-        grid.addAxis("kp")
-        grid.addAxis("ki")
+        grid.addAxis("kP")
+        grid.addAxis("kD")
         designer.designAlongGrid(grid, is_report=IGNORE_TEST)
-        self.assertGreater(designer.kp, 0)
-        self.assertGreater(designer.ki, 0)
-        self.assertIsNone(designer.kf)
+        self.assertGreater(designer.kP, 0)
+        self.assertGreater(designer.kD, 0)
+        self.assertIsNone(designer.kI)
+        self.assertIsNone(designer.kF)
 
     def testPlotDesignResult(self):
-        #if IGNORE_TEST:
-        #    return
-        designer = self.makeDesigner()
+        # Plots a previously computed result
+        if IGNORE_TEST:
+            return
+        designer = self.makeDesigner(is_save_path=False)
+        def test(parameter_names):
+            dct = {}
+            for spec in CONTROL_PARAMETER_SPECS:
+                if spec in parameter_names:
+                    dct[spec] = True
+                else:
+                    dct[spec] = False
+            designer.design(min_value=0.1, max_value=10, 
+                 num_coordinate=4, num_restart=1, is_report=IGNORE_TEST, **dct)
+            designer.plotDesignResult(is_plot=IS_PLOT, figsize=(15,15))
+        #
+        test(["kP_spec", "kI_spec", "kD_spec"])
+        test(["kP_spec", "kI_spec"])
+        test(["kP_spec"])
+
+    def testPlotDesignResult2(self):
+        # Check for selection of parameters
+        if IGNORE_TEST:
+            return
         def test(parameter_names):
+            designer = self.makeDesigner(is_save_path=False)
             dct = {}
             for spec in CONTROL_PARAMETER_SPECS:
                 if spec in parameter_names:
                     dct[spec] = True
                 else:
                     dct[spec] = False
             designer.design(min_value=0.1, max_value=10, 
                  num_coordinate=4, num_restart=1, is_report=IGNORE_TEST, **dct)
             designer.plotDesignResult(is_plot=IS_PLOT, figsize=(15,15))
         #
-        test(["kp_spec", "ki_spec", "kf_spec"])
-        test(["kp_spec", "ki_spec"])
-        test(["kp_spec"])
+        test(["kP_spec", "kI_spec", "kD_spec"])
+        with self.assertRaises(ValueError):
+            test(["kP_spec", "kI_spec", "kD_spec", "kF_spec"])
+        test(["kP_spec", "kI_spec"])
+        test(["kP_spec"])
 
     def test_closed_loop_tf(self):
         # Checks that the closed loop transfer function is calculated correctly
         if IGNORE_TEST:
             return
         # Setup
-        s, kp, ki = sympy.symbols("s kp ki")
+        s, kP, kI = sympy.symbols("s kP kI")
         # System transfer function
         sys_tf = control.tf([1], [1, 1])
         systf = 1/(s + 1)
         # Symbolic calculation of transfer function
-        ctltf = kp + ki/s
+        ctltf = kP + kI/s
         looptf = sympy.simplify(systf*ctltf)
         cltf = sympy.simplify(looptf/(1 + looptf))
         #
         designer = cld.SISOClosedLoopDesigner(self.system, sys_tf, setpoint=5)
-        designer.set(kp=2, ki=3)
+        designer.set(kP=2, kI=3)
         closed_loop_tf = designer.closed_loop_transfer_function
         func1 = lambda x: np.real(closed_loop_tf(x))
-        cltf_nums = cltf.subs({kp: 2, ki: 3})
+        cltf_nums = cltf.subs({kP: 2, kI: 3})
         func2 = lambda x: sympy.N(cltf_nums.subs({s: x}))
         result = util.compareSingleArgumentFunctions(func1, func2, 0, 100)
         self.assertTrue(result)
 
     def testBug1(self):
         if IGNORE_TEST:
             return
         # Setup
         system = SBMLSystem(LINEAR_MDL, input_names=["k0"], output_names=["S3"], is_fixed_input_species=True,
                                 is_steady_state=False)
         linear_bldr = SISOTransferFunctionBuilder(system)
         linear_staircase = Staircase(initial_value=0, final_value=10, num_step=5)
-        fitter_result = linear_bldr.fitTransferFunction(num_numerator=2, num_denominator=3, 
-                                                    staircase=linear_staircase, fit_start_time=20,
-                                                start_time=0, end_time=200)
+        fitter_result = linear_bldr.plotTransferFunctionFit(num_zero=1, num_pole=2, 
+                                                    staircase=linear_staircase, fit_start_time=5,
+                                                start_time=0, end_time=200, is_plot=IS_PLOT, figsize=FIGSIZE)
         linear_tf = fitter_result.transfer_function
         #
         times = np.linspace(0, 1000, 10000)
         designer = cld.SISOClosedLoopDesigner(system, linear_tf, times=times, setpoint=5)
-        designer.design(kp_spec=True, ki_spec=True, num_restart=2, max_value=100)
+        designer.design(kP_spec=True, kI_spec=True, num_restart=2, max_value=100)
         designer.evaluate(is_plot=IS_PLOT, figsize=FIGSIZE)
     
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `controlSBML-1.1.3/tests/test_siso_maker.py` & `controlsbml-1.2.0/tests/test_siso_maker.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/tests/test_siso_transfer_function_builder.py` & `controlsbml-1.2.0/tests/test_siso_transfer_function_builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import controlSBML.constants as cn
+import controlSBML.constants as cn  # type: ignore
 import controlSBML as ctl
-import controlSBML.siso_transfer_function_builder as stb
-from controlSBML.sbml_system import SBMLSystem
-from controlSBML.staircase import Staircase
-import controlSBML.util as util
+import controlSBML.siso_transfer_function_builder as stb  # type: ignore
+from controlSBML.sbml_system import SBMLSystem # type: ignore
+from controlSBML.staircase import Staircase # type: ignore
+import controlSBML.util as util # type: ignore
 import helpers
 
 import copy
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 import unittest
 import shutil
-import tellurium as te
+import tellurium as te # type: ignore
 import tempfile
 
 
-IGNORE_TEST = True
-IS_PLOT = True
-PLOT_PATH = helpers.setupPlotting(__file__)
+IGNORE_TEST = False
+IS_PLOT = False
+#PLOT_PATH = helpers.setupPlotting(__file__)
 END_TIME = 5
 DT = 0.01
 POINTS_PER_TIME = int(1.0 / DT)
 NUM_TIME = int(POINTS_PER_TIME*END_TIME) + 1
 TIMES = [n*DT for n in range(0, NUM_TIME)]
 LINEAR_MDL = """
 // Illustrate Antimony File
@@ -32,66 +32,43 @@
 J2: S2 -> ; S2
 
 k1 = 5
 S1 = 10
 S2 = 0
 end
 """
+NEG_MODEL = """
+// Negative relationship between S0 and S3
+model *neg()
+$S1 -> S2; k1*S1
+S2 -> S3; k2*S2
+S3 ->; k3*S3
+S3 -> ; k4*S0
+S1 = 10
+$S0 = 10
+S3 = 10
+k1 = 1
+k2 = 2
+k3 = 2
+k4 = 2
+end
+"""
 INPUT_NAME = "S1"
 OUTPUT_NAME = "S2"
 INITIAL_VALUE = 2
 FINAL_VALUE = 15
 STAIRCASE= Staircase(initial_value=INITIAL_VALUE, final_value=FINAL_VALUE, num_step=5)
 SYSTEM = SBMLSystem(LINEAR_MDL, input_names=[INPUT_NAME], output_names=[OUTPUT_NAME], is_fixed_input_species=True)
 BUILDER = stb.SISOTransferFunctionBuilder(SYSTEM)
 RESPONSE_TS, _ = BUILDER.makeStaircaseResponse(staircase=STAIRCASE, times=np.linspace(0, END_TIME, NUM_TIME))
 
 
 #############################
 # Tests
 #############################
-class TestFunctions(unittest.TestCase):
-
-    def testMakeParameters(self):
-        if IGNORE_TEST:
-            return
-        def test(parameters, prefix, expected_count):
-            names = [n for n in parameters.valuesdict().keys()
-                  if n[0] == prefix]
-            self.assertEqual(len(names), expected_count)
-        #
-        parameters = stb._makeParameters(3, 4)
-        test(parameters, stb.NUMERATOR_PREFIX, 3)
-        test(parameters, stb.DENOMINATOR_PREFIX, 4)
-        self.assertTrue(len(parameters.valuesdict()) == 7)
-
-    def testMakeTransferFunction(self):
-        if IGNORE_TEST:
-            return
-        parameters = stb._makeParameters(2, 2)
-        tf = stb._makeTransferFunction(parameters)
-        self.assertTrue(tf.poles()[0] == -1)
-        self.assertTrue(tf.dcgain() == 1)
-
-    def testCalculateTransferFunctionResiduals(self):
-        if IGNORE_TEST:
-            return
-        times = list(RESPONSE_TS.index)
-        data_in = (times, RESPONSE_TS["S1_staircase"].values)
-        data_out = RESPONSE_TS["S2"].values
-        parameters = stb._makeParameters(3, 3)
-        residuals = stb._calculateTransferFunctionResiduals(parameters, data_in,
-              data_out)
-        self.assertEqual(len(residuals), len(times))
-        self.assertTrue("float" in str(residuals.dtype))
-
-
-#############################
-# Tests
-#############################
 class TestSBMLSystem(unittest.TestCase):
 
     def setUp(self):
         if IGNORE_TEST:
             return
         self.init()
         self.removeFiles()
@@ -119,16 +96,14 @@
                 path = os.path.join(cn.PLOT_DIR, ffile)
                 if os.path.isfile(path) and IGNORE_TEST:
                     os.remove(path)
         # FIXME: This won't work in windows
         if IS_PLOT and ("var" in cn.PLOT_DIR):
             shutil.rmtree(cn.PLOT_DIR)
         #
-        if os.path.isfile(PLOT_PATH):
-            os.remove(PLOT_PATH)
 
     def testConstructor(self):
         if IGNORE_TEST:
             return
         self.init()
         self.assertTrue(isinstance(self.builder, stb.SISOTransferFunctionBuilder ))
 
@@ -151,52 +126,56 @@
 
     def testFitTransferFunction(self):
         if IGNORE_TEST:
             return
         self.init()
         system = SBMLSystem(LINEAR_MDL, input_names=[INPUT_NAME], output_names=[OUTPUT_NAME], is_fixed_input_species=True)
         builder = stb.SISOTransferFunctionBuilder(system)
-        fitter_result = builder.fitTransferFunction(num_numerator=4, num_denominator=4,
-              end_time=100)
-        if IS_PLOT:
-            builder.plotFitterResult(fitter_result, is_plot=IS_PLOT)
+        fitter_result = builder.plotTransferFunctionFit(is_plot=IS_PLOT,
+                                                        figsize=(5,5))
         self.assertTrue(isinstance(fitter_result.time_series, ctl.Timeseries))
-        self.assertLess(fitter_result.rms_residuals, 0.2)
-
-    def testFitTransferFunctionTimes(self):
-        if IGNORE_TEST:
-            return
-        self.init()
-        times = np.linspace(0, 100, 1000)
-        system = SBMLSystem(LINEAR_MDL, input_names=[INPUT_NAME], output_names=[OUTPUT_NAME], is_fixed_input_species=True)
-        builder = stb.SISOTransferFunctionBuilder(system)
-        fitter_result = builder.fitTransferFunction(num_numerator=4, num_denominator=4,
-              end_time=100, fit_start_time=0, fit_end_time=40, times=times, staircase=STAIRCASE)
-        if IS_PLOT:
-            builder.plotFitterResult(fitter_result, is_plot=IS_PLOT)
-        self.assertTrue(isinstance(fitter_result.time_series, ctl.Timeseries))
-        self.assertLess(fitter_result.rms_residuals, 0.1)
+        self.assertLess(fitter_result.rms_residuals, 1)
 
     def testPlotFitTransferFunction(self):
         if IGNORE_TEST:
             return
         system = SBMLSystem(LINEAR_MDL, input_names=[INPUT_NAME], output_names=[OUTPUT_NAME], is_fixed_input_species=True)
         builder = stb.SISOTransferFunctionBuilder(system)
-        fitter_result = builder.fitTransferFunction(num_numerator=4, num_denominator=4,
-              end_time=50)
-        builder.plotFitterResult(fitter_result, is_plot=IS_PLOT, figsize=(5,5))
+        _ = builder.plotTransferFunctionFit(num_zero=3, num_pole=3,
+              end_time=500, is_plot=IS_PLOT, figsize=(5,5))
 
     def testFitTransferFunction2(self):
         if IGNORE_TEST:
             return
-        system = SBMLSystem(cn.WOLF_URL,
+        system = SBMLSystem(cn.WOLF_PATH,
               input_names=["na"], output_names=["s6"])
         builder = stb.SISOTransferFunctionBuilder(system)
         staircase = Staircase(initial_value=50, final_value=100)
-        fitter_result = builder.fitTransferFunction(1, 2, staircase=staircase,
-              end_time=5)
-        builder.plotFitterResult(fitter_result, is_plot=IS_PLOT)
+        fitter_result = builder.plotTransferFunctionFit(1, 2, staircase=staircase,
+              end_time=5, is_plot=IS_PLOT)
         self.assertTrue(isinstance(fitter_result.time_series, ctl.Timeseries))
 
+    def testFitTransferFunctionDecrease(self):
+        if IGNORE_TEST:
+            return
+        system = SBMLSystem(NEG_MODEL,
+              input_names=["S0"], output_names=["S3"])
+        builder = stb.SISOTransferFunctionBuilder(system)
+        staircase = Staircase()
+        fitter_result = builder.plotTransferFunctionFit(num_zero=1, num_pole=2, staircase=staircase,
+                                                    fit_start_time=2, fit_end_time=10, is_plot=IS_PLOT)
+
+    def testFitTransferFunctionBug(self):
+        if IGNORE_TEST:
+            return
+        url = URL = "https://www.ebi.ac.uk/biomodels/services/download/get-files/MODEL1304160000/2/BIOMD0000000449_url.xml"
+        system = SBMLSystem(url,
+              input_names=["IR"], output_names=["GLUT4"], is_fixed_input_species=True)
+        builder = stb.SISOTransferFunctionBuilder(system, fitter_method=cn.FITTER_METHOD_POLY)
+        staircase = Staircase(initial_value=10, final_value=25)
+        _ = builder.plotTransferFunctionFit(num_zero=1, num_pole=3, staircase=staircase,
+                                            times=np.linspace(0, 1000, 10000),
+              fit_start_time=100, fit_end_time=1000, is_plot=IS_PLOT)
+
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `controlSBML-1.1.3/tests/test_staircase.py` & `controlsbml-1.2.0/tests/test_staircase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-from controlSBML.staircase import Staircase
-import helpers
+from controlSBML.staircase import Staircase  # type: ignore
 
 import matplotlib.pyplot as plt
 import numpy as np
-import os
 import unittest
 
 
 IGNORE_TEST = False
 IS_PLOT = False
 INITIAL_VALUE = 5
 FINAL_VALUE = 10
 NUM_STEP = 5
 NUM_POINT = 100
-PLOT_PATH = helpers.setupPlotting(__file__)
+#PLOT_PATH = helpers.setupPlotting(__file__)
     
 
 class TestStaircase(unittest.TestCase):
 
     def setUp(self):
          self.remove()
          if False:
              self.staircase = Staircase.makeRelativeStaircase(
                  center=10, fractional_deviation=0.1, num_step=5, num_point=100)
          
     def tearDown(self):
         self.remove()
          
     def remove(self):
-        if os.path.isfile(PLOT_PATH):
-            if not IS_PLOT: 
-                os.remove(PLOT_PATH)
+        return
 
     def testConstructor(self):
         if IGNORE_TEST:
             return
 
         def test(num_point, num_step, initial_value=0, final_value=5):
             staircase = Staircase(initial_value=initial_value,
@@ -43,15 +39,14 @@
                                     num_point=num_point)
             self.assertTrue(len(staircase.staircase_arr), num_point)
             num_distinct = len(set(staircase.staircase_arr))
             self.assertEqual(num_distinct, num_step + 1)
             self.assertEqual(staircase.staircase_arr[0], initial_value)
             self.assertEqual(staircase.staircase_arr[-1], final_value)
             _ = staircase.plot()
-            plt.savefig(PLOT_PATH)
         #
         test(20, 4)
         test(19, 4)
         test(191, 17)
         test(91, 15)
 
     def testMakeRealtive(self):
@@ -69,13 +64,45 @@
         self.assertTrue(np.isclose(staircase.staircase_arr[0], center - deviation))
         self.assertTrue(isinstance(staircase, Staircase))
 
     def testPlot(self):
         if IGNORE_TEST:
             return
         staircase = Staircase.makeRelativeStaircase(5, 2)
-        staircase.plot()
-        plt.savefig(PLOT_PATH)
+        staircase.plot(is_plot=IS_PLOT)
+
+    def testMakeEndStepInfo(self):
+        if IGNORE_TEST:
+            return
+        def test(num_point_per_end, num_step):
+            num_point = (3 + num_point_per_end)*(num_step+1)
+            staircase = Staircase(initial_value=0, final_value=10, num_step=num_step, num_point=num_point)
+            values, idxs = staircase.makeEndStepInfo(num_point=num_point_per_end)
+            self.assertEqual(len(values), num_point_per_end*(num_step+1))
+            self.assertEqual(len(idxs), num_point_per_end*(num_step+1))
+            for value, idx in zip(values, idxs):
+                self.assertEqual(staircase.staircase_arr[idx], value)
+        #
+        test(2, 5)
+        test(1, 2)
+        test(10, 200)
+
+    def testMakeEndStepInfo2(self):
+        if IGNORE_TEST:
+            return
+        # Check that taking into account start and end
+        def test(num_point_per_end, num_step):
+            num_point = (3 + num_point_per_end)*(num_step+1)
+            staircase = Staircase(initial_value=0, final_value=10, num_step=num_step, num_point=num_point)
+            start_idx = staircase.point_per_level
+            values, idxs = staircase.makeEndStepInfo(num_point=num_point_per_end,
+                                                      start_idx=start_idx)
+            self.assertEqual(len(values), num_point_per_end*(num_step))
+            self.assertEqual(len(idxs), num_point_per_end*(num_step))
+        #
+        test(2, 5)
+        test(1, 2)
+        test(10, 200)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `controlSBML-1.1.3/tests/test_timeseries.py` & `controlsbml-1.2.0/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `controlSBML-1.1.3/tests/test_util.py` & `controlsbml-1.2.0/tests/test_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from controlSBML import util
-from controlSBML.timeseries import Timeseries
-import controlSBML.constants as cn
+from controlSBML import util  # type: ignore
+from controlSBML.timeseries import Timeseries # type: ignore
+import controlSBML.constants as cn  # type: ignore
 import controlSBML as ctl
 
-import control
-import pandas as pd
+import control # type: ignore
+import pandas as pd # type: ignore
 import numpy as np
-import tellurium as te
+import tellurium as te # type: ignore
 import unittest
 
 
 IGNORE_TEST = False
 IS_PLOT = False
 SIZE = 10
 if IS_PLOT:
@@ -59,19 +59,49 @@
         self.assertTrue("roadrunner" in str(type(rr)))
 
     def testPlotOneTS(self):
         if IGNORE_TEST:
           return
         util.plotOneTS(TS, ylabel="values", xlabel="sec",
               is_plot=IS_PLOT)
+        
+    def testSubsetDct(self):
+        if IGNORE_TEST:
+          return
+        dct = {"a": 1, "b": 2, "c": 3}
+        subset = util.subsetDct(dct, ["a", "c"])
+        self.assertTrue(len(subset) == 2)
+        self.assertTrue("b" not in subset)
+
+    def testSubsetDct2(self):
+        if IGNORE_TEST:
+          return
+        dct = {"a": 1, "b": 2}
+        subset = util.subsetDct(dct, ["a", "c"], {"c": 3})
+        self.assertTrue(len(subset) == 2)
+        self.assertTrue("b" not in subset)
+        self.assertTrue(subset["c"] == 3)
+
+    def testDifferenceDct(self):
+        if IGNORE_TEST:
+          return
+        dct1 = {"a": 1, "b": 2, "c": 3}
+        dct2 = {"a": 1, "b": 2, "c": 3}
+        diff = util.differenceDct(dct1, dct2)
+        self.assertTrue(len(diff) == 0)
+        #
+        dct2 = {"a": 1, "b": 2}
+        diff = util.differenceDct(dct1, dct2)
+        self.assertTrue(len(diff) == 1)
+        self.assertTrue("c" in diff)
 
     def testPlotManyTS(self):
         if IGNORE_TEST:
           return
-        df = TS.applymap(lambda v: 100*v)
+        df = TS.map(lambda v: 100*v)
         ts = Timeseries(df, times=df.index)
         util.plotManyTS(TS, ts, ylabel="values", xlabel="sec",
               is_plot=IS_PLOT, names=["first", "second"])
         util.plotManyTS(TS, ts, ylabel="values", xlabel="sec",
               is_plot=IS_PLOT, names=["first", "second"], ncol=2)
 
     def testMakeSimulationTimes(self):
@@ -173,15 +203,15 @@
         tf = control.TransferFunction([1], [1, 0.0002, 1])
         latex = util.latexifyTransferFunction(tf)
         self.assertTrue(latex.count("$"))
         self.assertTrue(latex.count("frac"))
         #
         tf = control.TransferFunction([0], [1, 0.0002, 1])
         latex = util.latexifyTransferFunction(tf)
-        self.assertFalse("frac" in latex)
+        self.assertTrue("frac" in latex)
         #
         tf = control.TransferFunction([1, 0, 0], [1, 0.0002, 1])
         latex = util.latexifyTransferFunction(tf)
 
     def testCleanTimes(self):
         if IGNORE_TEST:
            return
```

