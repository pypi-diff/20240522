# Comparing `tmp/gradco-0.1.0.tar.gz` & `tmp/gradco-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradco-0.1.0.tar", last modified: Wed May 22 13:08:21 2024, max compression
+gzip compressed data, was "gradco-0.1.1.tar", last modified: Wed May 22 13:55:27 2024, max compression
```

## Comparing `gradco-0.1.0.tar` & `gradco-0.1.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:08:21.028074 gradco-0.1.0/
--rw-r--r--   0 windels    (502) staff       (20)      158 2023-07-04 12:55:34.000000 gradco-0.1.0/AUTHORS.rst
--rw-r--r--   0 windels    (502) staff       (20)     2978 2023-07-04 12:55:34.000000 gradco-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 windels    (502) staff       (20)       97 2023-07-04 12:55:34.000000 gradco-0.1.0/HISTORY.rst
--rw-r--r--   0 windels    (502) staff       (20)     1078 2023-07-04 12:55:34.000000 gradco-0.1.0/LICENSE
--rw-r--r--   0 windels    (502) staff       (20)      100 2023-07-04 12:55:34.000000 gradco-0.1.0/MANIFEST.in
--rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 13:08:21.028004 gradco-0.1.0/PKG-INFO
--rw-r--r--   0 windels    (502) staff       (20)      409 2023-07-04 12:55:34.000000 gradco-0.1.0/README.rst
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:08:21.000537 gradco-0.1.0/c_module/
--rw-r--r--   0 windels    (502) staff       (20)     4362 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/dense_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1084 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/dense_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4086 2023-12-28 11:03:57.000000 gradco-0.1.0/c_module/directed_graph.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1048 2023-12-27 08:52:51.000000 gradco-0.1.0/c_module/directed_graph.hh
--rw-r--r--   0 windels    (502) staff       (20)    21422 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/gradco_module.cpp
--rw-r--r--   0 windels    (502) staff       (20)      969 2024-01-17 12:42:27.000000 gradco-0.1.0/c_module/matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4957 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/sparse_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1406 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/sparse_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4779 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/symmetric_dense_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1118 2024-02-16 11:24:52.000000 gradco-0.1.0/c_module/symmetric_dense_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)    74463 2023-12-27 08:52:51.000000 gradco-0.1.0/c_module/unordered_dense.h
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:08:21.003887 gradco-0.1.0/docs/
--rw-r--r--   0 windels    (502) staff       (20)     6778 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/Makefile
--rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/authors.rst
--rw-r--r--   0 windels    (502) staff       (20)     8155 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/conf.py
--rw-r--r--   0 windels    (502) staff       (20)       33 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/contributing.rst
--rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/history.rst
--rw-r--r--   0 windels    (502) staff       (20)      688 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/index.rst
--rw-r--r--   0 windels    (502) staff       (20)      244 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/installation.rst
--rw-r--r--   0 windels    (502) staff       (20)     6709 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/make.bat
--rw-r--r--   0 windels    (502) staff       (20)       90 2023-07-04 12:55:34.000000 gradco-0.1.0/docs/usage.rst
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:08:21.005139 gradco-0.1.0/generate_tests/
--rw-r--r--   0 windels    (502) staff       (20)       92 2023-07-04 12:55:34.000000 gradco-0.1.0/generate_tests/bit_array_to_graphlet_signatures_3nodes.csv
--rw-r--r--   0 windels    (502) staff       (20)     1422 2023-07-04 12:55:34.000000 gradco-0.1.0/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv
--rw-r--r--   0 windels    (502) staff       (20)     9294 2023-07-04 12:55:34.000000 gradco-0.1.0/generate_tests/generate_unit_test_code.py
--rw-r--r--   0 windels    (502) staff       (20)     4613 2023-07-23 12:45:41.000000 gradco-0.1.0/generate_tests/generate_unit_test_code_orbit_adjacency.py
--rwxr-xr-x   0 windels    (502) staff       (20)   130744 2023-07-04 12:55:34.000000 gradco-0.1.0/generate_tests/orca
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:08:21.027763 gradco-0.1.0/gradco.egg-info/
--rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 13:08:20.000000 gradco-0.1.0/gradco.egg-info/PKG-INFO
--rw-r--r--   0 windels    (502) staff       (20)     1601 2024-05-22 13:08:20.000000 gradco-0.1.0/gradco.egg-info/SOURCES.txt
--rw-r--r--   0 windels    (502) staff       (20)        1 2024-05-22 13:08:20.000000 gradco-0.1.0/gradco.egg-info/dependency_links.txt
--rw-r--r--   0 windels    (502) staff       (20)       25 2024-05-22 13:08:20.000000 gradco-0.1.0/gradco.egg-info/top_level.txt
--rw-r--r--   0 windels    (502) staff       (20)    27184 2024-05-02 07:58:26.000000 gradco-0.1.0/gradco.py
--rwxr-xr-x   0 windels    (502) staff       (20)  2580760 2023-07-04 12:55:34.000000 gradco-0.1.0/ncount2
--rw-r--r--   0 windels    (502) staff       (20)      546 2024-05-22 13:05:59.000000 gradco-0.1.0/pyproject.toml
--rw-r--r--   0 windels    (502) staff       (20)    48654 2024-01-18 15:31:58.000000 gradco-0.1.0/python_count_functions.py
--rw-r--r--   0 windels    (502) staff       (20)       61 2024-05-22 13:08:21.028296 gradco-0.1.0/setup.cfg
--rw-r--r--   0 windels    (502) staff       (20)     1736 2024-05-22 13:07:13.000000 gradco-0.1.0/setup.py
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:08:21.027213 gradco-0.1.0/test/
--rw-r--r--   0 windels    (502) staff       (20)        0 2023-12-20 14:53:52.000000 gradco-0.1.0/test/__init__.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A10_10_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A10_11_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A12_12_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A12_13_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A13_13_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160739 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A14_14_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A1_1_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A1_2_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158721 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A3_3_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A4_4_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A4_5_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A5_5_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A6_6_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A6_7_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A8_8_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A9_10_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.0/test/test_A9_11_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G1_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G2_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G3_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G4_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G5_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G6_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G7_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.0/test/test_G8_windels.py
--rw-r--r--   0 windels    (502) staff       (20)     5202 2024-02-16 11:24:52.000000 gradco-0.1.0/test/test_helper.py
--rw-r--r--   0 windels    (502) staff       (20)      498 2023-07-04 12:55:34.000000 gradco-0.1.0/tox.ini
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.485643 gradco-0.1.1/
+-rw-r--r--   0 windels    (502) staff       (20)      158 2023-07-04 12:55:34.000000 gradco-0.1.1/AUTHORS.rst
+-rw-r--r--   0 windels    (502) staff       (20)     2978 2023-07-04 12:55:34.000000 gradco-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 windels    (502) staff       (20)       97 2023-07-04 12:55:34.000000 gradco-0.1.1/HISTORY.rst
+-rw-r--r--   0 windels    (502) staff       (20)     1078 2023-07-04 12:55:34.000000 gradco-0.1.1/LICENSE
+-rw-r--r--   0 windels    (502) staff       (20)      100 2023-07-04 12:55:34.000000 gradco-0.1.1/MANIFEST.in
+-rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 13:55:27.485556 gradco-0.1.1/PKG-INFO
+-rw-r--r--   0 windels    (502) staff       (20)      409 2023-07-04 12:55:34.000000 gradco-0.1.1/README.rst
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.455896 gradco-0.1.1/c_module/
+-rw-r--r--   0 windels    (502) staff       (20)     4362 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/dense_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1084 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/dense_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4086 2023-12-28 11:03:57.000000 gradco-0.1.1/c_module/directed_graph.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1048 2023-12-27 08:52:51.000000 gradco-0.1.1/c_module/directed_graph.hh
+-rw-r--r--   0 windels    (502) staff       (20)    21422 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/gradco_module.cpp
+-rw-r--r--   0 windels    (502) staff       (20)      969 2024-01-17 12:42:27.000000 gradco-0.1.1/c_module/matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4957 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/sparse_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1406 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/sparse_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4779 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/symmetric_dense_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1118 2024-02-16 11:24:52.000000 gradco-0.1.1/c_module/symmetric_dense_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)    74463 2023-12-27 08:52:51.000000 gradco-0.1.1/c_module/unordered_dense.h
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.460266 gradco-0.1.1/docs/
+-rw-r--r--   0 windels    (502) staff       (20)     6778 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/Makefile
+-rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/authors.rst
+-rw-r--r--   0 windels    (502) staff       (20)     8155 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/conf.py
+-rw-r--r--   0 windels    (502) staff       (20)       33 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/contributing.rst
+-rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/history.rst
+-rw-r--r--   0 windels    (502) staff       (20)      688 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/index.rst
+-rw-r--r--   0 windels    (502) staff       (20)      244 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/installation.rst
+-rw-r--r--   0 windels    (502) staff       (20)     6709 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/make.bat
+-rw-r--r--   0 windels    (502) staff       (20)       90 2023-07-04 12:55:34.000000 gradco-0.1.1/docs/usage.rst
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.461346 gradco-0.1.1/generate_tests/
+-rw-r--r--   0 windels    (502) staff       (20)       92 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/bit_array_to_graphlet_signatures_3nodes.csv
+-rw-r--r--   0 windels    (502) staff       (20)     1422 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv
+-rw-r--r--   0 windels    (502) staff       (20)     9294 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/generate_unit_test_code.py
+-rw-r--r--   0 windels    (502) staff       (20)     4613 2023-07-23 12:45:41.000000 gradco-0.1.1/generate_tests/generate_unit_test_code_orbit_adjacency.py
+-rwxr-xr-x   0 windels    (502) staff       (20)   130744 2023-07-04 12:55:34.000000 gradco-0.1.1/generate_tests/orca
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.483926 gradco-0.1.1/gradco.egg-info/
+-rw-r--r--   0 windels    (502) staff       (20)      235 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/PKG-INFO
+-rw-r--r--   0 windels    (502) staff       (20)     1601 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/SOURCES.txt
+-rw-r--r--   0 windels    (502) staff       (20)        1 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/dependency_links.txt
+-rw-r--r--   0 windels    (502) staff       (20)       25 2024-05-22 13:55:27.000000 gradco-0.1.1/gradco.egg-info/top_level.txt
+-rw-r--r--   0 windels    (502) staff       (20)    28239 2024-05-22 13:50:26.000000 gradco-0.1.1/gradco.py
+-rwxr-xr-x   0 windels    (502) staff       (20)  2580760 2023-07-04 12:55:34.000000 gradco-0.1.1/ncount2
+-rw-r--r--   0 windels    (502) staff       (20)      546 2024-05-22 13:05:59.000000 gradco-0.1.1/pyproject.toml
+-rw-r--r--   0 windels    (502) staff       (20)    48654 2024-01-18 15:31:58.000000 gradco-0.1.1/python_count_functions.py
+-rw-r--r--   0 windels    (502) staff       (20)       61 2024-05-22 13:55:27.485870 gradco-0.1.1/setup.cfg
+-rw-r--r--   0 windels    (502) staff       (20)     1658 2024-05-22 13:55:16.000000 gradco-0.1.1/setup.py
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 13:55:27.483397 gradco-0.1.1/test/
+-rw-r--r--   0 windels    (502) staff       (20)        0 2023-12-20 14:53:52.000000 gradco-0.1.1/test/__init__.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A10_10_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A10_11_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A12_12_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A12_13_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A13_13_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160739 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A14_14_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A1_1_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A1_2_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158721 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A3_3_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A4_4_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A4_5_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A5_5_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A6_6_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A6_7_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A8_8_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A9_10_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.1/test/test_A9_11_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G1_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G2_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G3_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G4_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G5_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G6_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G7_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.1/test/test_G8_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)     5202 2024-02-16 11:24:52.000000 gradco-0.1.1/test/test_helper.py
+-rw-r--r--   0 windels    (502) staff       (20)      498 2023-07-04 12:55:34.000000 gradco-0.1.1/tox.ini
```

### Comparing `gradco-0.1.0/CONTRIBUTING.rst` & `gradco-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/LICENSE` & `gradco-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/dense_matrix.cpp` & `gradco-0.1.1/c_module/dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/dense_matrix.hh` & `gradco-0.1.1/c_module/dense_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/directed_graph.cpp` & `gradco-0.1.1/c_module/directed_graph.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/directed_graph.hh` & `gradco-0.1.1/c_module/directed_graph.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/gradco_module.cpp` & `gradco-0.1.1/c_module/gradco_module.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/matrix.hh` & `gradco-0.1.1/c_module/matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/sparse_matrix.cpp` & `gradco-0.1.1/c_module/sparse_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/sparse_matrix.hh` & `gradco-0.1.1/c_module/sparse_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/symmetric_dense_matrix.cpp` & `gradco-0.1.1/c_module/symmetric_dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/symmetric_dense_matrix.hh` & `gradco-0.1.1/c_module/symmetric_dense_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/c_module/unordered_dense.h` & `gradco-0.1.1/c_module/unordered_dense.h`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/docs/Makefile` & `gradco-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/docs/conf.py` & `gradco-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/docs/index.rst` & `gradco-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/docs/make.bat` & `gradco-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv` & `gradco-0.1.1/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/generate_tests/generate_unit_test_code.py` & `gradco-0.1.1/generate_tests/generate_unit_test_code.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/generate_tests/generate_unit_test_code_orbit_adjacency.py` & `gradco-0.1.1/generate_tests/generate_unit_test_code_orbit_adjacency.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/generate_tests/orca` & `gradco-0.1.1/generate_tests/orca`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/gradco.egg-info/SOURCES.txt` & `gradco-0.1.1/gradco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/gradco.py` & `gradco-0.1.1/gradco.py`

 * *Files 5% similar despite different names*

```diff
@@ -324,14 +324,48 @@
         for _hop, o1, o2, A in self.generate_orbit_adjacencies(hop=1):
             key = (_hop, o1, o2)
             if key in orbit_2_scaling:
                 scaling = orbit_2_scaling[key]
                 GDVs[o1] = A.sum(axis=1).squeeze() / scaling
         return np.stack(GDVs).T
 
+    def get_edge_GDVs(self):
+        # (hop, o1, o2): scaling_constant
+        node_orbits = {(1, 2),
+                       (3, 3),
+                       (4, 5),
+                       (5, 5),
+                       (6, 7),
+                       (8, 8),
+                       (9, 11),
+                       (10, 10),
+                       (10, 11),
+                       (12, 13),
+                       (13, 13),
+                       (14, 14),
+                       }
+
+        gdvs = [None] * 12
+        e = 0
+        for _, o1, o2, A in self.generate_orbit_adjacencies(hop=1):
+            key = (o1, o2)
+            if o1 == 0 and o2 == 0:
+                rows, cols = A.nonzero()
+                triu_indices = rows < cols
+                rows = rows[triu_indices]
+                cols = cols[triu_indices]
+
+            if key in node_orbits:
+                if o1 != o2:
+                    A += A.T
+                # gdvs[e] = A[rows, cols].A1
+                gdvs[e] = A[rows, cols]
+                e += 1
+        return np.stack(gdvs).T
+
     def compute_A12_12_digraph(self, adj):
         import networkx as nx
 
         G = nx.from_numpy_array(adj, create_using=nx.Graph)
         G_digraph = nx.DiGraph(nodes=G.nodes())
         # G_digraph = nx.from_numpy_array(adj, create_using=nx.DiGraph)
         G_digraph.add_edges_from(G.edges())
```

### Comparing `gradco-0.1.0/ncount2` & `gradco-0.1.1/ncount2`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/pyproject.toml` & `gradco-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/python_count_functions.py` & `gradco-0.1.1/python_count_functions.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/setup.py` & `gradco-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 import os
 import sysconfig
 import numpy as np
 
 
 def main():
 
-    
     c_module = Extension("gradco_c_routines",
-                              sources=["c_module/directed_graph.cpp", 
-                                       "c_module/gradco_module.cpp",
-                                       "c_module/sparse_matrix.cpp",
-                                       "c_module/dense_matrix.cpp",
-                                       "c_module/symmetric_dense_matrix.cpp",
-                                       ],
-                              depends=["c_module/unordered_dense.h", 
-                                       "c_module/sparse_matrix.hh",
-                                       "c_module/dense_matrix.hh",
-                                       "c_module/symmetric_dense_matrix.hh",
-                                       "c_module/directed_graph.hh"],
-                              include_dirs=[ np.get_include(), "."],
-                              language='c++',
-                              extra_compile_args=['-std=c++17', '-O3'],
-                              )
-    # c++20 
-    # gnu++20 
-    # c++2b => 23 working draft 
-    # gnu++2b => working draft with GNU extensions 
+                         sources=["c_module/directed_graph.cpp",
+                                  "c_module/gradco_module.cpp",
+                                  "c_module/sparse_matrix.cpp",
+                                  "c_module/dense_matrix.cpp",
+                                  "c_module/symmetric_dense_matrix.cpp",
+                                  ],
+                         depends=["c_module/unordered_dense.h",
+                                  "c_module/sparse_matrix.hh",
+                                  "c_module/dense_matrix.hh",
+                                  "c_module/symmetric_dense_matrix.hh",
+                                  "c_module/directed_graph.hh"],
+                         include_dirs=[np.get_include(), "."],
+                         language='c++',
+                         extra_compile_args=['-std=c++17', '-O3'],
+                         )
+    # c++20
+    # gnu++20
+    # c++2b => 23 working draft
+    # gnu++2b => working draft with GNU extensions
 
     setup(name="gradco",  # Name of the package. Used at install: pip install gradco
-          version="0.1.0",
+          version="0.1.1",
           description="GRaphlet and Orbit Adjacency Counter (GROADCO).",
           author="Sam Windels",
           author_email="sam.windels@gmail.com",
           ext_modules=[c_module],
-          py_modules=["gradco"],  # Refers to gradco.py. Name of the module. Used as: import gradco
+          # Refers to gradco.py. Name of the module. Used as: import gradco
+          py_modules=["gradco"],
           python_requires='>=3.10',
           )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gradco-0.1.0/test/test_A10_10_orca.py` & `gradco-0.1.1/test/test_A10_10_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A10_11_orca.py` & `gradco-0.1.1/test/test_A10_11_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A12_12_orca.py` & `gradco-0.1.1/test/test_A12_12_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A12_13_orca.py` & `gradco-0.1.1/test/test_A12_13_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A13_13_orca.py` & `gradco-0.1.1/test/test_A13_13_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A14_14_orca.py` & `gradco-0.1.1/test/test_A14_14_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A1_1_orca.py` & `gradco-0.1.1/test/test_A1_1_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A1_2_orca.py` & `gradco-0.1.1/test/test_A1_2_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A3_3_orca.py` & `gradco-0.1.1/test/test_A3_3_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A4_4_orca.py` & `gradco-0.1.1/test/test_A4_4_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A4_5_orca.py` & `gradco-0.1.1/test/test_A4_5_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A5_5_orca.py` & `gradco-0.1.1/test/test_A5_5_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A6_6_orca.py` & `gradco-0.1.1/test/test_A6_6_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A6_7_orca.py` & `gradco-0.1.1/test/test_A6_7_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A8_8_orca.py` & `gradco-0.1.1/test/test_A8_8_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A9_10_orca.py` & `gradco-0.1.1/test/test_A9_10_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_A9_11_orca.py` & `gradco-0.1.1/test/test_A9_11_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G1_windels.py` & `gradco-0.1.1/test/test_G1_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G2_windels.py` & `gradco-0.1.1/test/test_G2_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G3_windels.py` & `gradco-0.1.1/test/test_G3_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G4_windels.py` & `gradco-0.1.1/test/test_G4_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G5_windels.py` & `gradco-0.1.1/test/test_G5_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G6_windels.py` & `gradco-0.1.1/test/test_G6_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G7_windels.py` & `gradco-0.1.1/test/test_G7_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_G8_windels.py` & `gradco-0.1.1/test/test_G8_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.0/test/test_helper.py` & `gradco-0.1.1/test/test_helper.py`

 * *Files identical despite different names*

