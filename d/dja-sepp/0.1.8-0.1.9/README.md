# Comparing `tmp/dja_sepp-0.1.8.tar.gz` & `tmp/dja_sepp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dja_sepp-0.1.8.tar", last modified: Fri May 17 11:49:01 2024, max compression
+gzip compressed data, was "dja_sepp-0.1.9.tar", last modified: Fri May 17 11:58:16 2024, max compression
```

## Comparing `dja_sepp-0.1.8.tar` & `dja_sepp-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.275007 dja_sepp-0.1.8/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.8/LICENSE
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2546 2024-05-17 11:49:01.272786 dja_sepp-0.1.8/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1880 2024-05-17 10:56:47.000000 dja_sepp-0.1.8/README.md
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      809 2024-05-17 11:48:29.000000 dja_sepp-0.1.8/pyproject.toml
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 11:49:01.275667 dja_sepp-0.1.8/setup.cfg
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.114853 dja_sepp-0.1.8/src/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.144599 dja_sepp-0.1.8/src/dja_sepp/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.8/src/dja_sepp/__init__.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.118365 dja_sepp-0.1.8/src/dja_sepp/data/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.267103 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12002 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12704 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14806 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11987 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    49028 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18124 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18921 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8303 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13861 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    10113 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23209 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15354 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8036 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11604 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    34304 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    17928 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    47252 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5323 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    24254 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    31613 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    25376 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5181 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22508 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13854 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    37987 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    19362 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6616 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6628 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15109 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4076 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4856 2024-05-17 11:48:01.000000 dja_sepp-0.1.8/src/dja_sepp/psfex.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.8/src/dja_sepp/s3.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9372 2024-05-17 11:47:30.000000 dja_sepp-0.1.8/src/dja_sepp/sepp.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23244 2024-05-17 11:46:36.000000 dja_sepp-0.1.8/src/dja_sepp/sextractor.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.8/src/dja_sepp/tiles.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.8/src/dja_sepp/utils.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.269774 dja_sepp-0.1.8/src/dja_sepp.egg-info/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2546 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2680 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/SOURCES.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/dependency_links.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/requires.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/top_level.txt
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:58:16.549782 dja_sepp-0.1.9/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.9/LICENSE
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2546 2024-05-17 11:58:16.546841 dja_sepp-0.1.9/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1880 2024-05-17 10:56:47.000000 dja_sepp-0.1.9/README.md
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      809 2024-05-17 11:57:57.000000 dja_sepp-0.1.9/pyproject.toml
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 11:58:16.550297 dja_sepp-0.1.9/setup.cfg
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:58:16.379663 dja_sepp-0.1.9/src/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:58:16.420403 dja_sepp-0.1.9/src/dja_sepp/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.9/src/dja_sepp/__init__.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:58:16.381802 dja_sepp-0.1.9/src/dja_sepp/data/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:58:16.540393 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12002 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12704 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14806 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11987 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    49028 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18124 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18921 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8303 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13861 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    10113 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23209 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15354 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8036 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11604 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    34304 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    17928 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    47252 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5323 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    24254 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    31613 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    25376 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5181 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22508 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13854 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    37987 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    19362 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6616 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6628 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15109 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4076 2024-05-16 12:32:24.000000 dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4856 2024-05-17 11:48:01.000000 dja_sepp-0.1.9/src/dja_sepp/psfex.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.9/src/dja_sepp/s3.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9372 2024-05-17 11:47:30.000000 dja_sepp-0.1.9/src/dja_sepp/sepp.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23613 2024-05-17 11:57:08.000000 dja_sepp-0.1.9/src/dja_sepp/sextractor.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.9/src/dja_sepp/tiles.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.9/src/dja_sepp/utils.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:58:16.543827 dja_sepp-0.1.9/src/dja_sepp.egg-info/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2546 2024-05-17 11:58:16.000000 dja_sepp-0.1.9/src/dja_sepp.egg-info/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2680 2024-05-17 11:58:16.000000 dja_sepp-0.1.9/src/dja_sepp.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 11:58:16.000000 dja_sepp-0.1.9/src/dja_sepp.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 11:58:16.000000 dja_sepp-0.1.9/src/dja_sepp.egg-info/requires.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 11:58:16.000000 dja_sepp-0.1.9/src/dja_sepp.egg-info/top_level.txt
```

### Comparing `dja_sepp-0.1.8/LICENSE` & `dja_sepp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/PKG-INFO` & `dja_sepp-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dja_sepp-0.1.8/README.md` & `dja_sepp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/pyproject.toml` & `dja_sepp-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dja_sepp"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     {name="Aurélien Genin", email="aurelien.genin@polytechnique.org"}
 ]
 description = "Package to run SourceXtractor++ on the DAWN JWST Archive"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dja_sepp-0.1.8/src/dja_sepp/__init__.py` & `dja_sepp-0.1.9/src/dja_sepp/__init__.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt` & `dja_sepp-0.1.9/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/psfex.py` & `dja_sepp-0.1.9/src/dja_sepp/psfex.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/s3.py` & `dja_sepp-0.1.9/src/dja_sepp/s3.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/sepp.py` & `dja_sepp-0.1.9/src/dja_sepp/sepp.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/sextractor.py` & `dja_sepp-0.1.9/src/dja_sepp/sextractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 from sklearn.linear_model import RANSACRegressor
 
 # To work, this file requires you to have SExtractor installed on your machine.
 
 def run_sextractor(detect_img      : str, weight_img   : str, 
                    output_cat      : str, 
                    config_file     : str, params_file  : str,
+                   filter_file     : str,
                    dir_chckimg     : str,
                    detect_thresh   : float = 12.0,
                    analysis_thresh : float = 2.5,
                    verbose         : bool = False) -> None :
     """
     Run SExtractor to create a FITS_LDAC catalog, with vignets to create a PSF.
 
     detect_img : filename of the detection image to use
     weight_img : filename of the weight map
     output_cat : filename of the output catalog
     config_file : filename of the SExtractor configuration file
-    params_file : filename of the SExtarctor parameters file
+    params_file : filename of the SExtractor parameters file
+    filter_file : filename of the convolution filter
     dir_chckimg : path to folder to save checkimages (will be created if non-existing)
     detect_thresh : value of the DETECT_THRESH to use
     analysis_thresh : value of the ANALYSIS_THRESH to use
     verbose : verbose parameter
     """
     # Find SExtractor installed version
     cmd = ""
@@ -49,14 +51,15 @@
     seg_img = f'{dir_chckimg}/{study_name}_seg.fits'
     verbose_type = 'NORMAL' if verbose else 'QUIET'
     os.environ['LD_LIBRARY_PATH'] = '/usr/lib' # Link 'libcfitsio.so.10'
     subprocess.run(f'{cmd} {detect_img} -c {config_file} \
                    -CATALOG_NAME {output_cat} \
                    -WEIGHT_IMAGE {weight_img} -WEIGHT_TYPE MAP_WEIGHT \
                    -PARAMETERS_NAME {params_file} \
+                   -FILTER-NAME {filter_file} \
                    -CHECKIMAGE_NAME {seg_img} \
                    -DETECT_THRESH {detect_thresh} \
                    -ANALYSIS_THRESH {analysis_thresh} \
                    -VERBOSE_TYPE {verbose_type}',
                    shell=True)
     return output_cat
     
@@ -296,14 +299,15 @@
 
 def extract_stars(detect_img        : str, 
                   weight_img        : str, 
                   output_cat        : str,
                   output_cat_star   : str, 
                   config_file       : str, 
                   params_file       : str,
+                  filter_file       : str,
                   dir_chckimg       : str,
                   detect_thresh     : float = 8.0,
                   analysis_thresh   : float = 2.5,
                   eps_DBSCAN        : float = 0.1, 
                   y_max             : float = -4.5, 
                   mag_fit           : float = 25,
                   y_offsets         : tuple = (-0.5,0.3),
@@ -323,15 +327,16 @@
     in PSFEx to create the PSF of a telescope.
     
     detect_img : filename of the detection image to use
     weight_img : filename of the weight map
     output_cat : filename of the output full catalog
     output_cat_star : filename of the output point-like sources catalog
     config_file : filename of the SExtractor configuration file
-    params_file : filename of the SExtarctor parameters file
+    params_file : filename of the SExtractor parameters file
+    filter_file : filename of the convolution filter
     dir_chckimg : path to folder to save checkimages (will be created if non-existing)
     detect_thresh : value of the DETECT_THRESH to use
     analysis_thresh : value of the ANALYSIS_THRESH to use
     eps_DBSCAN : epsilon parameter for DBSCAN (the higher, the bigger the selected cluster is)
     y_max : MU_MAX-MAG_AUTO threshold for linear regression
     mag_fit : value of MAG_AUTO to calculate the star line position after linear regression
     y_offsets : negative and positive offsets from star_line for the selection box
@@ -344,15 +349,15 @@
     save_chckimg : parameter to save plots to check if everything worked well
     plot : parameter to display plots to check if everything worked well
     clean : delete the full catalog created by SExtractor at the end
     run_sex : run SExtractor. Can be set to False if you already have a FITS_LDAC catalog
     verbose : verbose parameter
     """
     study_name = '.'.join(detect_img.split('/')[-1].split('.')[:-1])
-    if run_sex: run_sextractor(detect_img, weight_img, output_cat, config_file, params_file, dir_chckimg, detect_thresh, analysis_thresh, verbose)
+    if run_sex: run_sextractor(detect_img, weight_img, output_cat, config_file, params_file, filter_file, dir_chckimg, detect_thresh, analysis_thresh, verbose)
     hdul = fits.open(output_cat)
     data = hdul[2].data
     star_line = find_star_line(data, eps_DBSCAN, y_max, mag_fit, verbose, plot, plot_mag_bounds, plot_y_bounds, save_chckimg, f"{dir_chckimg}/starDetect_{study_name}.png")
     star_MUvMAG = MUvMAG_star_selection(data, star_line, y_offsets, mag_bounds, snr_min, plot, plot_mag_bounds, plot_y_bounds, save_chckimg, f"{dir_chckimg}/starLine_{study_name}.png")
     if plot | save_chckimg:
         star_selections = {'MUvMAG' : {'label': 'Stars (MU v. MAG)', 'color': 'r', 'flag': star_MUvMAG}}
         fig, ax = plt.subplots(1,2,figsize=(12,6))
@@ -368,14 +373,15 @@
 def extract_stars_catalog(detect_img        : str, 
                           weight_img        : str,
                           output_cat        : str, 
                           output_cat_star   : str,
                           input_cat_star    : str, 
                           config_file       : str, 
                           params_file       : str,
+                          filter_file       : str,
                           dir_chckimg       : str,
                           detect_thresh     : float = 2.5,
                           analysis_thresh   : float = 2.5,
                           max_sep           : u.Quantity = 1.0*u.arcsec,
                           plot_mag_bounds   : tuple = (18,30),
                           plot_mu_bounds    : tuple = (13,25),
                           plot_rad_bound   : tuple = 20, 
@@ -392,29 +398,30 @@
     detect_img : filename of the detection image to use
     weight_img : filename of the weight map
     output_cat : filename of the output full catalog
     output_cat_star : filename of the output point-like sources catalog
     input_cat_star : filename of the input point-like sources catalog
     config_file : filename of the SExtractor configuration file
     params_file : filename of the SExtarctor parameters file
+    filter_file : filename of the convolution filter
     dir_chckimg : path to folder to save checkimages (will be created if non-existing)
     detect_thresh : value of the DETECT_THRESH to use
     analysis_thresh : value of the ANALYSIS_THRESH to use
     max_sep : maximum angular separation for sources cross-match
     plot_mag_bounds : bounds for MAG_AUTO for the plots
     plot_mu_bounds : bounds for MU_MAX for the plots
     plot_rad_bound : maximum value for FLUX_RADIUS for the plots
     save_chckimg : parameter to save plots to check if everything worked well
     plot : parameter to display plots to check if everything worked well
     clean : delete the full catalog created by SExtractor at the end
     run_sex : run SExtractor. Can be set to False if you already have a FITS_LDAC catalog
     verbose : verbose parameter
     """
     study_name = '.'.join(detect_img.split('/')[-1].split('.')[:-1])
-    if run_sex: run_sextractor(detect_img, weight_img, output_cat, config_file, params_file, dir_chckimg, detect_thresh, analysis_thresh, verbose)
+    if run_sex: run_sextractor(detect_img, weight_img, output_cat, config_file, params_file, filter_file, dir_chckimg, detect_thresh, analysis_thresh, verbose)
     if verbose: print ("Opening star catalogs")
     hdul = fits.open(output_cat, memmap=True, mode='denywrite') 
     data = hdul[2].data
     with fits.open(input_cat_star, memmap=True, mode='denywrite') as hdul_star: 
         data_star = hdul_star[2].data
     coord = SkyCoord(data['ALPHA_J2000'][:], data['DELTA_J2000'][:], unit='deg', frame='icrs')
     coord_star = SkyCoord(data_star['ALPHA_J2000'], data_star['DELTA_J2000'], unit='deg', frame='icrs')
```

### Comparing `dja_sepp-0.1.8/src/dja_sepp/tiles.py` & `dja_sepp-0.1.9/src/dja_sepp/tiles.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp/utils.py` & `dja_sepp-0.1.9/src/dja_sepp/utils.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.8/src/dja_sepp.egg-info/PKG-INFO` & `dja_sepp-0.1.9/src/dja_sepp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dja_sepp-0.1.8/src/dja_sepp.egg-info/SOURCES.txt` & `dja_sepp-0.1.9/src/dja_sepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

