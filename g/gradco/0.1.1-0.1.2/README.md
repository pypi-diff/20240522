# Comparing `tmp/gradco-0.1.1.tar.gz` & `tmp/gradco-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradco-0.1.1.tar", last modified: Wed May 22 13:55:27 2024, max compression
+gzip compressed data, was "gradco-0.1.2.tar", last modified: Wed May 22 14:08:53 2024, max compression
```

## Comparing `gradco-0.1.1.tar` & `gradco-0.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.485643 gradco-0.1.1/
--rw-r--r--   0 windels    (502) staff       (20)      158 2023-07-04 12:55:34.000000 gradco-0.1.1/AUTHORS.rst
--rw-r--r--   0 windels    (502) staff       (20)     2978 2023-07-04 12:55:34.000000 gradco-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 windels    (502) staff       (20)       97 2023-07-04 12:55:34.000000 gradco-0.1.1/HISTORY.rst
--rw-r--r--   0 windels    (502) staff       (20)     1078 2023-07-04 12:55:34.000000 gradco-0.1.1/LICENSE
--rw-r--r--   0 windels    (502) staff       (20)      100 2023-07-04 12:55:34.000000 gradco-0.1.1/MANIFEST.in
--rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 13:55:27.485556 gradco-0.1.1/PKG-INFO
--rw-r--r--   0 windels    (502) staff       (20)      409 2023-07-04 12:55:34.000000 gradco-0.1.1/README.rst
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.455896 gradco-0.1.1/c_module/
--rw-r--r--   0 windels    (502) staff       (20)     4362 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/dense_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1084 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/dense_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4086 2023-12-28 11:03:57.000000 gradco-0.1.1/c_module/directed_graph.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1048 2023-12-27 08:52:51.000000 gradco-0.1.1/c_module/directed_graph.hh
--rw-r--r--   0 windels    (502) staff       (20)    21422 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/gradco_module.cpp
--rw-r--r--   0 windels    (502) staff       (20)      969 2024-01-17 12:42:27.000000 gradco-0.1.1/c_module/matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4957 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/sparse_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1406 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/sparse_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4779 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/symmetric_dense_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1118 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/symmetric_dense_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)    74463 2023-12-27 08:52:51.000000 gradco-0.1.1/c_module/unordered_dense.h
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.460266 gradco-0.1.1/docs/
--rw-r--r--   0 windels    (502) staff       (20)     6778 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/Makefile
--rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/authors.rst
--rw-r--r--   0 windels    (502) staff       (20)     8155 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/conf.py
--rw-r--r--   0 windels    (502) staff       (20)       33 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/contributing.rst
--rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/history.rst
--rw-r--r--   0 windels    (502) staff       (20)      688 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/index.rst
--rw-r--r--   0 windels    (502) staff       (20)      244 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/installation.rst
--rw-r--r--   0 windels    (502) staff       (20)     6709 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/make.bat
--rw-r--r--   0 windels    (502) staff       (20)       90 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/usage.rst
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.461346 gradco-0.1.1/generate_tests/
--rw-r--r--   0 windels    (502) staff       (20)       92 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/bit_array_to_graphlet_signatures_3nodes.csv
--rw-r--r--   0 windels    (502) staff       (20)     1422 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv
--rw-r--r--   0 windels    (502) staff       (20)     9294 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/generate_unit_test_code.py
--rw-r--r--   0 windels    (502) staff       (20)     4613 2023-07-23 12:45:41.000000 gradco-0.1.1/generate_tests/generate_unit_test_code_orbit_adjacency.py
--rwxr-xr-x   0 windels    (502) staff       (20)   130744 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/orca
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.483926 gradco-0.1.1/gradco.egg-info/
--rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/PKG-INFO
--rw-r--r--   0 windels    (502) staff       (20)     1601 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/SOURCES.txt
--rw-r--r--   0 windels    (502) staff       (20)        1 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/dependency_links.txt
--rw-r--r--   0 windels    (502) staff       (20)       25 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/top_level.txt
--rw-r--r--   0 windels    (502) staff       (20)    28239 2024-05-22 13:50:26.000000 gradco-0.1.1/gradco.py
--rwxr-xr-x   0 windels    (502) staff       (20)  2580760 2023-07-04 12:55:34.000000 gradco-0.1.1/ncount2
--rw-r--r--   0 windels    (502) staff       (20)      546 2024-05-22 13:05:59.000000 gradco-0.1.1/pyproject.toml
--rw-r--r--   0 windels    (502) staff       (20)    48654 2024-01-18 15:31:58.000000 gradco-0.1.1/python_count_functions.py
--rw-r--r--   0 windels    (502) staff       (20)       61 2024-05-22 13:55:27.485870 gradco-0.1.1/setup.cfg
--rw-r--r--   0 windels    (502) staff       (20)     1658 2024-05-22 13:55:16.000000 gradco-0.1.1/setup.py
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.483397 gradco-0.1.1/test/
--rw-r--r--   0 windels    (502) staff       (20)        0 2023-12-20 14:53:52.000000 gradco-0.1.1/test/__init__.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A10_10_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A10_11_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A12_12_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A12_13_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A13_13_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160739 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A14_14_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A1_1_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A1_2_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158721 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A3_3_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A4_4_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A4_5_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A5_5_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A6_6_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A6_7_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A8_8_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A9_10_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A9_11_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G1_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G2_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G3_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G4_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G5_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G6_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G7_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G8_windels.py
--rw-r--r--   0 windels    (502) staff       (20)     5202 2024-02-16 11:24:52.000000 gradco-0.1.1/test/test_helper.py
--rw-r--r--   0 windels    (502) staff       (20)      498 2023-07-04 12:55:34.000000 gradco-0.1.1/tox.ini
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 14:08:53.179448 gradco-0.1.2/
+-rw-r--r--   0 windels    (502) staff       (20)      158 2023-07-04 12:55:34.000000 gradco-0.1.2/AUTHORS.rst
+-rw-r--r--   0 windels    (502) staff       (20)     2978 2023-07-04 12:55:34.000000 gradco-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 windels    (502) staff       (20)       97 2023-07-04 12:55:34.000000 gradco-0.1.2/HISTORY.rst
+-rw-r--r--   0 windels    (502) staff       (20)     1078 2023-07-04 12:55:34.000000 gradco-0.1.2/LICENSE
+-rw-r--r--   0 windels    (502) staff       (20)      100 2023-07-04 12:55:34.000000 gradco-0.1.2/MANIFEST.in
+-rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 14:08:53.179378 gradco-0.1.2/PKG-INFO
+-rw-r--r--   0 windels    (502) staff       (20)      409 2023-07-04 12:55:34.000000 gradco-0.1.2/README.rst
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 14:08:53.151027 gradco-0.1.2/c_module/
+-rw-r--r--   0 windels    (502) staff       (20)     4362 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/dense_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1084 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/dense_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4086 2023-12-28 11:03:57.000000 gradco-0.1.2/c_module/directed_graph.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1048 2023-12-27 08:52:51.000000 gradco-0.1.2/c_module/directed_graph.hh
+-rw-r--r--   0 windels    (502) staff       (20)    21422 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/gradco_module.cpp
+-rw-r--r--   0 windels    (502) staff       (20)      969 2024-01-17 12:42:27.000000 gradco-0.1.2/c_module/matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4957 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/sparse_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1406 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/sparse_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4779 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/symmetric_dense_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1118 2024-02-16 11:24:52.000000 gradco-0.1.2/c_module/symmetric_dense_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)    74463 2023-12-27 08:52:51.000000 gradco-0.1.2/c_module/unordered_dense.h
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 14:08:53.154068 gradco-0.1.2/docs/
+-rw-r--r--   0 windels    (502) staff       (20)     6778 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/Makefile
+-rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/authors.rst
+-rw-r--r--   0 windels    (502) staff       (20)     8155 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/conf.py
+-rw-r--r--   0 windels    (502) staff       (20)       33 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/contributing.rst
+-rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/history.rst
+-rw-r--r--   0 windels    (502) staff       (20)      688 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/index.rst
+-rw-r--r--   0 windels    (502) staff       (20)      244 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/installation.rst
+-rw-r--r--   0 windels    (502) staff       (20)     6709 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/make.bat
+-rw-r--r--   0 windels    (502) staff       (20)       90 2023-07-04 12:55:34.000000 gradco-0.1.2/docs/usage.rst
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 14:08:53.155193 gradco-0.1.2/generate_tests/
+-rw-r--r--   0 windels    (502) staff       (20)       92 2023-07-04 12:55:34.000000 gradco-0.1.2/generate_tests/bit_array_to_graphlet_signatures_3nodes.csv
+-rw-r--r--   0 windels    (502) staff       (20)     1422 2023-07-04 12:55:34.000000 gradco-0.1.2/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv
+-rw-r--r--   0 windels    (502) staff       (20)     9294 2023-07-04 12:55:34.000000 gradco-0.1.2/generate_tests/generate_unit_test_code.py
+-rw-r--r--   0 windels    (502) staff       (20)     4613 2023-07-23 12:45:41.000000 gradco-0.1.2/generate_tests/generate_unit_test_code_orbit_adjacency.py
+-rwxr-xr-x   0 windels    (502) staff       (20)   130744 2023-07-04 12:55:34.000000 gradco-0.1.2/generate_tests/orca
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 14:08:53.179122 gradco-0.1.2/gradco.egg-info/
+-rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 14:08:53.000000 gradco-0.1.2/gradco.egg-info/PKG-INFO
+-rw-r--r--   0 windels    (502) staff       (20)     1601 2024-05-22 14:08:53.000000 gradco-0.1.2/gradco.egg-info/SOURCES.txt
+-rw-r--r--   0 windels    (502) staff       (20)        1 2024-05-22 14:08:53.000000 gradco-0.1.2/gradco.egg-info/dependency_links.txt
+-rw-r--r--   0 windels    (502) staff       (20)       25 2024-05-22 14:08:53.000000 gradco-0.1.2/gradco.egg-info/top_level.txt
+-rw-r--r--   0 windels    (502) staff       (20)    29093 2024-05-22 14:03:23.000000 gradco-0.1.2/gradco.py
+-rwxr-xr-x   0 windels    (502) staff       (20)  2580760 2023-07-04 12:55:34.000000 gradco-0.1.2/ncount2
+-rw-r--r--   0 windels    (502) staff       (20)      546 2024-05-22 13:05:59.000000 gradco-0.1.2/pyproject.toml
+-rw-r--r--   0 windels    (502) staff       (20)    48654 2024-01-18 15:31:58.000000 gradco-0.1.2/python_count_functions.py
+-rw-r--r--   0 windels    (502) staff       (20)       61 2024-05-22 14:08:53.179669 gradco-0.1.2/setup.cfg
+-rw-r--r--   0 windels    (502) staff       (20)     1658 2024-05-22 14:07:39.000000 gradco-0.1.2/setup.py
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 14:08:53.178451 gradco-0.1.2/test/
+-rw-r--r--   0 windels    (502) staff       (20)        0 2023-12-20 14:53:52.000000 gradco-0.1.2/test/__init__.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A10_10_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A10_11_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A12_12_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A12_13_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A13_13_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160739 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A14_14_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A1_1_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A1_2_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158721 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A3_3_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A4_4_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A4_5_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A5_5_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A6_6_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A6_7_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A8_8_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A9_10_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.2/test/test_A9_11_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G1_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G2_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G3_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G4_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G5_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G6_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G7_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.2/test/test_G8_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)     5202 2024-02-16 11:24:52.000000 gradco-0.1.2/test/test_helper.py
+-rw-r--r--   0 windels    (502) staff       (20)      498 2023-07-04 12:55:34.000000 gradco-0.1.2/tox.ini
```

### Comparing `gradco-0.1.1/CONTRIBUTING.rst` & `gradco-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/LICENSE` & `gradco-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/dense_matrix.cpp` & `gradco-0.1.2/c_module/dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/dense_matrix.hh` & `gradco-0.1.2/c_module/dense_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/directed_graph.cpp` & `gradco-0.1.2/c_module/directed_graph.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/directed_graph.hh` & `gradco-0.1.2/c_module/directed_graph.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/gradco_module.cpp` & `gradco-0.1.2/c_module/gradco_module.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/matrix.hh` & `gradco-0.1.2/c_module/matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/sparse_matrix.cpp` & `gradco-0.1.2/c_module/sparse_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/sparse_matrix.hh` & `gradco-0.1.2/c_module/sparse_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/symmetric_dense_matrix.cpp` & `gradco-0.1.2/c_module/symmetric_dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/symmetric_dense_matrix.hh` & `gradco-0.1.2/c_module/symmetric_dense_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/c_module/unordered_dense.h` & `gradco-0.1.2/c_module/unordered_dense.h`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/docs/Makefile` & `gradco-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/docs/conf.py` & `gradco-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/docs/index.rst` & `gradco-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/docs/make.bat` & `gradco-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv` & `gradco-0.1.2/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/generate_tests/generate_unit_test_code.py` & `gradco-0.1.2/generate_tests/generate_unit_test_code.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/generate_tests/generate_unit_test_code_orbit_adjacency.py` & `gradco-0.1.2/generate_tests/generate_unit_test_code_orbit_adjacency.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/generate_tests/orca` & `gradco-0.1.2/generate_tests/orca`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/gradco.egg-info/SOURCES.txt` & `gradco-0.1.2/gradco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/gradco.py` & `gradco-0.1.2/gradco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import gradco_c_routines
 import numpy as np
 from scipy.sparse import csr_array, save_npz, load_npz
-
 import time
 from collections.abc import Iterator
 from contextlib import contextmanager
 
 
 @contextmanager
 def time_it() -> Iterator[None]:
@@ -49,23 +48,21 @@
         (3, 4, 4): 3}
 
     def __init__(self, A):
 
         # assert A is a valid adjacency matrix
         self.__assert_has_entries(A)
         self.__assert_equal_dims(A)
-        # self.__assert_unweighted(A)
-        # self.__assert_symmetric(A)
 
         # apply degree ordering
         self.__A, self.__order, self.__reverse_order = self.__apply_degree_ordering(
             A)
 
         # book keeping
-        self.__n = A.shape[0]            # number of nodes
+        self.__n = A.shape[0]  # number of nodes
         self.orbit_adjacencies = None  # where c counts will be stored
 
     # SANITY CHECKS ON ADJACENCY MATRIX
 
     def __assert_unweighted(self, A):
         if not np.all(np.logical_or(A == 0, A == 1)):
             raise ValueError('Adjacency matrix is not unweighted')
@@ -83,22 +80,14 @@
             raise ValueError('Adjacency matrix is not symmetric')
 
     # DEGREE ORDERING
     def __apply_degree_ordering(self, A):
         # scipy returns numpy matrix instead of array
         rowsum = np.asarray(A.sum(axis=1)).squeeze()
         order = np.argsort(rowsum, axis=0)
-        # import networkx as nx
-        # G = nx.from_scipy_sparse_array(A)
-        # G = nx.from_numpy_array(A)
-        # core_numbers = nx.core_number(G)
-        # order = np.argsort([ core_numbers[node] for node in G.nodes()], axis=0)
-
-        # order = np.arange(A.shape[0]) # TODO: remove this line
-
         reverse_order = np.argsort(order)
         A = A[order, :]
         A = A[:, order]
         return A, order, reverse_order
 
     def __apply_reverse_ordering(self, A):
         A = A[self.__reverse_order, :]
@@ -173,14 +162,21 @@
     #             if len(rows) > 0:
     #                 print('hiet')
     #                 self.orbit_adjacencies[c_index] = np.vstack((rows, cols, vals))
 
     # GRAPHLET ADJACENCIES
 
     def get_graphlet_adjacency(self, graphlet):
+        """ Return the adjacency matrix for a given graphlet.
+
+        Reference:
+            Windels, Sam FL, Noël Malod-Dognin, and Nataša Pržulj. "Graphlet
+            Laplacians for topology-function and topology-disease
+            relationships." Bioinformatics 35.24 (2019): 5226-5234.
+        """
 
         match graphlet:
             case 0:
                 return self.__get_graphlet_adjacency_0()
             case 1:
                 return self.__get_graphlet_adjacency_1()
             case 2:
@@ -264,23 +260,31 @@
 
     def __get_graphlet_adjacency_8(self):
         A = self.get_orbit_adjacency(1, 14, 14)
         return A
 
     # ORBIT ADJACENCIES
     def generate_orbit_adjacencies(self, hop=None):
+        """ Generate all node orbit adjacencies. """
 
         for (_hop, o1, o2), c_index in self.__ORBIT_ADJ_2_C_INDEX.items():
             if hop is None or _hop == hop:
                 A = self.__get_orbit_adjacency_from_c_index(c_index)
                 yield _hop, o1, o2, A
                 if o1 != o2:
                     yield _hop, o2, o1, A.T
 
     def generate_edge_orbit_adjacencies(self):
+        """ Generate all edge orbit adjacencies.
+
+        Reference:
+            Rossi, Ryan A., Nesreen K. Ahmed, and Eunyee Koh. "Higher-order
+            network representation learning." Companion Proceedings of the The
+            Web Conference 2018. 2018.
+        """
         e = 0
         for (_hop, o1, o2), c_index in self.__ORBIT_ADJ_2_C_INDEX.items():
             if _hop == 1:
                 A = self.__get_orbit_adjacency_from_c_index(c_index)
                 if o1 == o2:
                     yield e, A
                     e += 1
@@ -297,14 +301,23 @@
             A_sparse = self.orbit_adjacencies[i]
             A = csr_array(
                 (A_sparse[2, :], (A_sparse[0, :], A_sparse[1, :])), shape=(self.__n, self.__n))
             A = self.__apply_reverse_ordering(A)
             return A
 
     def get_GDVs(self):
+        """ Return the graphlet degree vectors (GDVs) for the graph.
+
+        Reference:
+            Milenković, Tijana, and Nataša Pržulj. "Uncovering biological
+            network function via graphlet degree signatures." Cancer
+            informatics 6 (2008): CIN-S680.
+
+        """
+
         # (hop, o1, o2): scaling_constant
         orbit_2_scaling = {(1, 0, 0): 1,
                            (1, 1, 2): 1,
                            (1, 2, 1): 2,
                            (1, 3, 3): 2,
                            (1, 4, 5): 1,
                            (1, 5, 5): 1,
@@ -325,14 +338,22 @@
             key = (_hop, o1, o2)
             if key in orbit_2_scaling:
                 scaling = orbit_2_scaling[key]
                 GDVs[o1] = A.sum(axis=1).squeeze() / scaling
         return np.stack(GDVs).T
 
     def get_edge_GDVs(self):
+        """ Return the edge graphlet degree vectors (GDVs) for the graph.
+
+        Reference:
+            Solava, Ryan W., Ryan P. Michaels, and Tijana Milenković.
+            "Graphlet-based edge clustering reveals pathogen-interacting
+            proteins." Bioinformatics 28.18 (2012): i480-i486.  
+        """
+
         # (hop, o1, o2): scaling_constant
         node_orbits = {(1, 2),
                        (3, 3),
                        (4, 5),
                        (5, 5),
                        (6, 7),
                        (8, 8),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gradco-0.1.1/ncount2` & `gradco-0.1.2/ncount2`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/pyproject.toml` & `gradco-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/python_count_functions.py` & `gradco-0.1.2/python_count_functions.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/setup.py` & `gradco-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                          )
     # c++20
     # gnu++20
     # c++2b => 23 working draft
     # gnu++2b => working draft with GNU extensions
 
     setup(name="gradco",  # Name of the package. Used at install: pip install gradco
-          version="0.1.1",
+          version="0.1.2",
           description="GRaphlet and Orbit Adjacency Counter (GROADCO).",
           author="Sam Windels",
           author_email="sam.windels@gmail.com",
           ext_modules=[c_module],
           # Refers to gradco.py. Name of the module. Used as: import gradco
           py_modules=["gradco"],
           python_requires='>=3.10',
```

### Comparing `gradco-0.1.1/test/test_A10_10_orca.py` & `gradco-0.1.2/test/test_A10_10_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A10_11_orca.py` & `gradco-0.1.2/test/test_A10_11_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A12_12_orca.py` & `gradco-0.1.2/test/test_A12_12_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A12_13_orca.py` & `gradco-0.1.2/test/test_A12_13_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A13_13_orca.py` & `gradco-0.1.2/test/test_A13_13_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A14_14_orca.py` & `gradco-0.1.2/test/test_A14_14_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A1_1_orca.py` & `gradco-0.1.2/test/test_A1_1_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A1_2_orca.py` & `gradco-0.1.2/test/test_A1_2_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A3_3_orca.py` & `gradco-0.1.2/test/test_A3_3_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A4_4_orca.py` & `gradco-0.1.2/test/test_A4_4_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A4_5_orca.py` & `gradco-0.1.2/test/test_A4_5_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A5_5_orca.py` & `gradco-0.1.2/test/test_A5_5_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A6_6_orca.py` & `gradco-0.1.2/test/test_A6_6_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A6_7_orca.py` & `gradco-0.1.2/test/test_A6_7_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A8_8_orca.py` & `gradco-0.1.2/test/test_A8_8_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A9_10_orca.py` & `gradco-0.1.2/test/test_A9_10_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_A9_11_orca.py` & `gradco-0.1.2/test/test_A9_11_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G1_windels.py` & `gradco-0.1.2/test/test_G1_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G2_windels.py` & `gradco-0.1.2/test/test_G2_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G3_windels.py` & `gradco-0.1.2/test/test_G3_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G4_windels.py` & `gradco-0.1.2/test/test_G4_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G5_windels.py` & `gradco-0.1.2/test/test_G5_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G6_windels.py` & `gradco-0.1.2/test/test_G6_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G7_windels.py` & `gradco-0.1.2/test/test_G7_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_G8_windels.py` & `gradco-0.1.2/test/test_G8_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.1/test/test_helper.py` & `gradco-0.1.2/test/test_helper.py`

 * *Files identical despite different names*

