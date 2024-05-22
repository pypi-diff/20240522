# Comparing `tmp/gnssrefl-3.2.2.tar.gz` & `tmp/gnssrefl-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-3.2.2.tar", last modified: Tue May 21 15:47:01 2024, max compression
+gzip compressed data, was "gnssrefl-3.3.0.tar", last modified: Wed May 22 20:14:08 2024, max compression
```

## Comparing `gnssrefl-3.2.2.tar` & `gnssrefl-3.3.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.937650 gnssrefl-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 15:46:54.000000 gnssrefl-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 15:46:54.000000 gnssrefl-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-21 15:47:01.937650 gnssrefl-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-21 15:46:54.000000 gnssrefl-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.913650 gnssrefl-3.2.2/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.913650 gnssrefl-3.2.2/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/filesizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_cl_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44629 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (127)   202799 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/max_resolve_RH_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/mjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57682 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    25343 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinex_coords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/sd_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.913650 gnssrefl-3.2.2/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 15:47:01.000000 gnssrefl-3.2.2/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:47:01.941650 gnssrefl-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:47:01.937650 gnssrefl-3.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-21 15:46:55.000000 gnssrefl-3.2.2/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.337307 gnssrefl-3.3.0/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.337307 gnssrefl-3.3.0/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/filesizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_cl_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44629 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50908 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)    50896 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (127)   202799 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40683 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/max_resolve_RH_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/mjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57874 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25817 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex_coords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/sd_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.337307 gnssrefl-3.3.0/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/test/test_rinex2snr.py
```

### Comparing `gnssrefl-3.2.2/LICENSE` & `gnssrefl-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/PKG-INFO` & `gnssrefl-3.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.2.2
+Version: 3.3.0
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.2.2 
+# gnssrefl v3.3.0 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.2.2/README.md` & `gnssrefl-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gnssrefl v3.2.2 
+# gnssrefl v3.3.0 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.2.2/gnssrefl/EGM96.py` & `gnssrefl-3.3.0/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/check_rinex_file.py` & `gnssrefl-3.3.0/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/computemp1mp2.py` & `gnssrefl-3.3.0/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/daily_avg.py` & `gnssrefl-3.3.0/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/daily_avg_cl.py` & `gnssrefl-3.3.0/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-3.3.0/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/decipher_argt.py` & `gnssrefl-3.3.0/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_ioc.py` & `gnssrefl-3.3.0/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_noaa.py` & `gnssrefl-3.3.0/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_orbits.py` & `gnssrefl-3.3.0/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_psmsl.py` & `gnssrefl-3.3.0/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_rinex.py` & `gnssrefl-3.3.0/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_teqc.py` & `gnssrefl-3.3.0/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_tides.py` & `gnssrefl-3.3.0/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_unr.py` & `gnssrefl-3.3.0/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/download_wsv.py` & `gnssrefl-3.3.0/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/filesizes.py` & `gnssrefl-3.3.0/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gnssir_cl.py` & `gnssrefl-3.3.0/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gnssir_cl_old.py` & `gnssrefl-3.3.0/gnssrefl/gnssir_cl_old.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gnssir_input.py` & `gnssrefl-3.3.0/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gnssir_v2.py` & `gnssrefl-3.3.0/gnssrefl/gnssir_v2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gnsssnr.f` & `gnssrefl-3.3.0/gnssrefl/gnsssnr.f`

 * *Files 0% similar despite different names*

```diff
@@ -137,17 +137,17 @@
       if (zrec.eq.0.d0) then
         write(errid,*) 'you need real station coords '
         return
       endif
 c     print*,'number of obs main code', nobs
 c     moving sites has been removed
       if (nobs .gt. 25 .or. nobs .eq. 0) then
-        write(errid,*) 'Only obs types <= 25 allowed. You'
-        write(errid,*) 'can try using teqc to remove'
-        write(errid,*) 'unneeded observables'
+        write(errid,*) 'Only <= 25 observable types allowed. '
+        write(errid,*) 'You can try using -strip T when using'
+        write(errid,*) 'rinex2snr or use gfzrnx'
         return
       endif
 
 
       call envTrans(xrec,yrec,zrec,staXYZ,Lat,Long,Ht,North,East,Up)
 c     open output file
       open(fileOUT,file=outfilename, status='unknown')
@@ -555,16 +555,16 @@
 c     KL 18mar05, fixed bug on nobs
         read (fileID,'(a80)') line
         if (line(61:80).eq.'# / TYPES OF OBSERV') then
           read(line, fmt='(I6)') nobs
 c         exit if more than 20 observables
           if (nobs.gt.25) then
              write(fid,*)'this code only supports <=25 observ types'
-             write(fid,*)'If your file has more, reduce using teqc '
-             write(fid,*)'teqc -O.obs S1+S2+S5+S6+S8 should work' 
+             write(fid,*)'try using -strip T when using rinex2snr'
+             write(fid,*)'Or you could try using gfzrnx' 
              return
           endif
 c   KL 19jan09 allowing more lines of OBS types
 c         first line has up to 9 OBS types
           if (nobs .lt. 10) then
             write(dynfmt, fmt='(A, I3.3, A)')
      +                      "(6X,", nobs, "(4X,A2))"
```

### Comparing `gnssrefl-3.2.2/gnssrefl/gnsssnrbigger.f` & `gnssrefl-3.3.0/gnssrefl/gnsssnrbigger.f`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,17 @@
       if (zrec.eq.0.d0) then
         write(errid,*) 'you need real station coords '
         return
       endif
 c     print*,'number of obs main code', nobs
 c     moving sites has been removed
       if (nobs .gt. 25 .or. nobs .eq. 0) then
-        write(errid,*) 'Only obs types <= 25 allowed. You'
-        write(errid,*) 'can try using teqc to remove'
-        write(errid,*) 'unneeded observables'
+        write(errid,*) 'Only works with <= 25 obs types.'
+        write(errid,*) 'You can try -strip T in rinex2snr'
+        write(errid,*) 'or use gfzrnx'
         return
       endif
 
 
       call envTrans(xrec,yrec,zrec,staXYZ,Lat,Long,Ht,North,East,Up)
 c     open output file
       open(fileOUT,file=outfilename, status='unknown')
```

### Comparing `gnssrefl-3.2.2/gnssrefl/gps.py` & `gnssrefl-3.3.0/gnssrefl/gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gpssnr.f` & `gnssrefl-3.3.0/gnssrefl/gpssnr.f`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       integer maxsat, maxeph, maxob
       parameter (maxsat = 150)
       parameter (maxeph = 50)
       parameter (maxob = 20)
       real*8 c
       parameter (c = 0.299792458D+09)     
 
-      integer stderr
+      integer stderr,iuseful,k
       parameter (stderr=6)
       character*80 inline
       character*4 station
       character*2  prn_pickc
       character*1 satID(maxsat)
       integer  nobs, itime(5), prn(maxsat), numsat, flag, sec,
      +   msec, lli(maxob,maxsat), iprn, ios, itrack,  i, 
@@ -133,25 +133,33 @@
 
 c removed subroutine moving_sites bevacuse life is short
       if ((xrec+yrec+zrec) .eq.0) then
         mess='ERROR:No (useful) apriori coordinates - exiting'
         write(errid,*)mess
         return
       endif
-      if (iobs(6) .eq. 0) then
-        mess='ERROR:no L1 SNR data - exiting'
+      iuseful = 0
+      do k = 6, 11
+         if (iobs(k) .gt. 0) then
+            iuseful = iuseful + 1
+         endif
+      enddo
+      if (iuseful .eq. 0) then
+        mess='ERROR:no SNR data found. Fatal error'
         write(errid,*)mess
         return
       endif
+
+c     if (iobs(6) .eq. 0) then
+c       return
+c     endif
       if (nobs .gt. 20) then
         mess = 'ERROR: this code only works for <= 20 obs types'
         write(errid,*)mess
-        mess = '1 solution is to to run teqc on the original RINEX'
-        write(errid,*)mess
-        mess = 'with -O.obs S1+S2+S5 as the option, rerun.'
+        mess = 'try using -strip T when running rinex2snr'
         write(errid,*)mess
         return
       endif
       close(53)
 
 
 c     read the broadcast ephemeris information
@@ -563,16 +571,17 @@
       do while (.not.endofheader)
 c     KL 18mar05, fixed bug on nobs
         read (fileID,'(a80)') line
         if (line(61:80).eq.'# / TYPES OF OBSERV') then
           read(line, fmt='(I6)') nobs
 c         exit if more than 20 observables
           if (nobs.gt.20) then
-             mess ='ERROR:supports <=20 observ types'
+             mess ='ERROR:this code only supports <=20 observ types'
              write(fid,*) mess
+             write(fid,*) nobs 
              return
           endif
 c   KL 19jan09 allowing more lines of OBS types
 c         first line has up to 9 OBS types
           if (nobs .lt. 10) then
             write(dynfmt, fmt='(A, I3.3, A)')
      +                      "(6X,", nobs, "(4X,A2))"
```

### Comparing `gnssrefl-3.2.2/gnssrefl/gpsweek.py` & `gnssrefl-3.3.0/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/gpt_1wA.pickle` & `gnssrefl-3.3.0/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/highrate.py` & `gnssrefl-3.3.0/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/installexe_cl.py` & `gnssrefl-3.3.0/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/invsnr_cl.py` & `gnssrefl-3.3.0/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/invsnr_input.py` & `gnssrefl-3.3.0/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/karnak_libraries.py` & `gnssrefl-3.3.0/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/kelly.py` & `gnssrefl-3.3.0/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/llh2xyz.py` & `gnssrefl-3.3.0/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/make_meta.py` & `gnssrefl-3.3.0/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/max_resolve_RH_cl.py` & `gnssrefl-3.3.0/gnssrefl/max_resolve_RH_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/nmea2snr.py` & `gnssrefl-3.3.0/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/nmea2snr_cl.py` & `gnssrefl-3.3.0/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/nyquist_libs.py` & `gnssrefl-3.3.0/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/phase_functions.py` & `gnssrefl-3.3.0/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/prn2gps.py` & `gnssrefl-3.3.0/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/query_unr.py` & `gnssrefl-3.3.0/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/quickLook_cl.py` & `gnssrefl-3.3.0/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/quickLook_function2.py` & `gnssrefl-3.3.0/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/quickPhase.py` & `gnssrefl-3.3.0/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/quicklib.py` & `gnssrefl-3.3.0/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/quickplt.py` & `gnssrefl-3.3.0/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/read_snr_files.py` & `gnssrefl-3.3.0/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/refl_zones.py` & `gnssrefl-3.3.0/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/refl_zones_cl.py` & `gnssrefl-3.3.0/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/refraction.py` & `gnssrefl-3.3.0/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/rh_plot.py` & `gnssrefl-3.3.0/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/rinex2snr.py` & `gnssrefl-3.3.0/gnssrefl/rinex2snr.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,27 +198,32 @@
                         if mk:
                             the_makan_option(station,cyyyy,cyy,cdoy) # looks everywhere in your local directories
                         if not os.path.exists(r):
                             print('Did not find the plain observation file, so now trying other names/directories')
                             # could try this way? - look for file in localpath2. gunzip if necessary
                             allgood = get_local_rinexfile(r,localpath2)
                         if os.path.exists(r):
-                            rinext =float(np.loadtxt(r,usecols=0,dtype='str',max_rows=1))
-                            print('Apparent Rinex version', rinext)
-                            if (rinext != 2.11):
-                                print('Your file is not RINEX v2.11 which is what you told the code it was. Exiting')
-                                sys.exit()
-
                             if screenstats:
                                 print('Found the RINEX 2.11 file', r)
+                            try:
+                                rinext =float(np.loadtxt(r,usecols=0,dtype='str',max_rows=1))
+                                print('Apparent Rinex version', rinext)
+                                if (rinext != 2.11):
+                                    print('Your file is not RINEX v2.11 which is what you told the code it was.')
+                                    #sys.exit()
+
+                            except:
+                                print('I had problems confirming RINEX version. Will ignore that for now.')
+
                             if strip:
                                 if screenstats:
                                     print('Testing out stripping the RINEX 2 file here')
                                 k.strip_rinexfile(r)
                             conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,translator)
+
                         else:
                             print('You Chose the No Look Option, but did not provide the needed RINEX file.')
                     if version == 3:
                         if rate == 'high':
                             csrate = '01' # high rate assumes 1-sec
                         else:
                             csrate = '{:02d}'.format(srate)
```

### Comparing `gnssrefl-3.2.2/gnssrefl/rinex2snr_cl.py` & `gnssrefl-3.3.0/gnssrefl/rinex2snr_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,20 @@
     RINEX obs files are provided by the user or fetched from a long list of archives. Although RINEX 3 is supported, 
     the default is RINEX 2.11 files
 
     beta version of parallel processing available in this release.  Set -par to a number < 11 
     Some archives have been set to non-compliant with this feature. Please look in the first few lines
     of code to see the names of these archives.
 
+    In general, you should not make RINEX 2.11 files with a huge number of observables. Especially do not put
+    Doppler data in your file.  If you have more than 25 observables (multi-GNSS) or 20 (GPS only), the code
+    should send an error message to a log. The location of that log is printed to the screen. If you don't want
+    to remake your RINEX files, you can try the -strip T option, which I believe uses gfzrnx to strip out everything
+    except for SNR data.
+
     Real-time users should use ultra, wum, or wum2
 
     Default orbits are GPS only until day of year 137, 2021 when rapid GFZ orbits became available.  If you still want to use
     the nav message, i.e. GPS only, you can request it.
 
     bkg no longer a boolean input - must be specified with archive name, i.e. bkg-igs or bkg-euref
```

### Comparing `gnssrefl-3.2.2/gnssrefl/rinex3_rinex2.py` & `gnssrefl-3.3.0/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/rinex3_snr.py` & `gnssrefl-3.3.0/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/rinex_coords.py` & `gnssrefl-3.3.0/gnssrefl/rinex_coords.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/rinpy.py` & `gnssrefl-3.3.0/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-3.3.0/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/sd_libs.py` & `gnssrefl-3.3.0/gnssrefl/sd_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/smoosh.py` & `gnssrefl-3.3.0/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/smoosh_snr.py` & `gnssrefl-3.3.0/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/snow_functions.py` & `gnssrefl-3.3.0/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/snowdepth_cl.py` & `gnssrefl-3.3.0/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/spline_functions.py` & `gnssrefl-3.3.0/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/subdaily.py` & `gnssrefl-3.3.0/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/subdaily_cl.py` & `gnssrefl-3.3.0/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/utils.py` & `gnssrefl-3.3.0/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/veg_multiyr.py` & `gnssrefl-3.3.0/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/vwc_cl.py` & `gnssrefl-3.3.0/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/vwc_input.py` & `gnssrefl-3.3.0/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/xnmeasnr.f` & `gnssrefl-3.3.0/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/xyz2llh.py` & `gnssrefl-3.3.0/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/ydoy.py` & `gnssrefl-3.3.0/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl/ymd.py` & `gnssrefl-3.3.0/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-3.3.0/gnssrefl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.2.2
+Version: 3.3.0
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.2.2 
+# gnssrefl v3.3.0 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.2.2/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-3.3.0/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-3.3.0/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/pyproject.toml` & `gnssrefl-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.2.2/setup.py` & `gnssrefl-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "simplekml",
     "earthscope-sdk",
     "jupyterlab",
     "ipywidgets"
 ]
 setup(
     name="gnssrefl",
-    version="3.2.2",
+    version="3.3.0",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-3.2.2/test/test_gps.py` & `gnssrefl-3.3.0/test/test_gps.py`

 * *Files identical despite different names*

