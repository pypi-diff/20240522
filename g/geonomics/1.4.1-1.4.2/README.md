# Comparing `tmp/geonomics-1.4.1.tar.gz` & `tmp/geonomics-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geonomics-1.4.1.tar", last modified: Tue Apr 30 00:22:20 2024, max compression
+gzip compressed data, was "geonomics-1.4.2.tar", last modified: Wed May 22 02:03:54 2024, max compression
```

## Comparing `geonomics-1.4.1.tar` & `geonomics-1.4.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.556071 geonomics-1.4.1/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2024-01-03 01:50:01.000000 geonomics-1.4.1/LICENSE.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.4.1/MANIFEST.in
--rw-rw-r--   0 deth      (1000) deth      (1000)     9440 2024-04-30 00:22:20.556071 geonomics-1.4.1/PKG-INFO
--rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.4.1/README.rst
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.204071 geonomics-1.4.1/geonomics/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.4.1/geonomics/__init__.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.200070 geonomics-1.4.1/geonomics/data/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.R
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2807 2023-06-14 19:20:14.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/env.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/gen.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/geo.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/run_mantel.R
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/default_models/
--rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.4.1/geonomics/data/default_models/selection_params.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/yosemite_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.220071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.224071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.232071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.240071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.328071 geonomics-1.4.1/geonomics/demos/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.4.1/geonomics/demos/_IBD_IBE.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/demos/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.4.1/geonomics/demos/_simult_select.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.4.1/geonomics/demos/_yosemite.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.328071 geonomics-1.4.1/geonomics/help/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/help/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/help/_memory_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/help/_param_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    42853 2024-04-01 12:51:51.000000 geonomics-1.4.1/geonomics/main.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.376071 geonomics-1.4.1/geonomics/ops/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/ops/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/ops/change.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    11576 2024-03-26 13:35:21.000000 geonomics-1.4.1/geonomics/ops/demography.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.4.1/geonomics/ops/mating.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/ops/movement.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     8345 2024-03-29 11:47:20.000000 geonomics-1.4.1/geonomics/ops/mutation.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.4.1/geonomics/ops/selection.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.464071 geonomics-1.4.1/geonomics/sim/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/sim/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/sim/burnin.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.4.1/geonomics/sim/data.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   142795 2024-04-30 00:17:16.000000 geonomics-1.4.1/geonomics/sim/model.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    49119 2024-04-01 12:20:05.000000 geonomics-1.4.1/geonomics/sim/params.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2023-04-13 16:46:44.000000 geonomics-1.4.1/geonomics/sim/stats.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.512071 geonomics-1.4.1/geonomics/structs/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/structs/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5851 2024-04-30 00:00:02.000000 geonomics-1.4.1/geonomics/structs/community.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    88196 2024-04-29 23:24:41.000000 geonomics-1.4.1/geonomics/structs/genome.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     8672 2021-07-09 03:11:40.000000 geonomics-1.4.1/geonomics/structs/individual.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    32817 2021-07-09 03:11:40.000000 geonomics-1.4.1/geonomics/structs/landscape.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   153475 2024-04-01 03:44:04.000000 geonomics-1.4.1/geonomics/structs/species.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.556071 geonomics-1.4.1/geonomics/utils/
--rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/utils/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/utils/_str_repr_.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10991 2023-04-13 17:58:34.000000 geonomics-1.4.1/geonomics/utils/io.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.4.1/geonomics/utils/spatial.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.4.1/geonomics/utils/viz.py
--rw-rw-r--   0 deth      (1000) deth      (1000)       22 2024-04-29 23:26:19.000000 geonomics-1.4.1/geonomics/version.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.204071 geonomics-1.4.1/geonomics.egg-info/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     9440 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/PKG-INFO
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2024-04-30 00:22:20.000000 geonomics-1.4.1/geonomics.egg-info/SOURCES.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/dependency_links.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/requires.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/top_level.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2024-04-30 00:22:20.556071 geonomics-1.4.1/setup.cfg
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2680 2022-01-01 17:57:19.000000 geonomics-1.4.1/setup.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.467279 geonomics-1.4.2/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2024-01-03 01:50:01.000000 geonomics-1.4.2/LICENSE.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.4.2/MANIFEST.in
+-rw-rw-r--   0 deth      (1000) deth      (1000)     9507 2024-05-22 02:03:54.467279 geonomics-1.4.2/PKG-INFO
+-rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.4.2/README.rst
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.067278 geonomics-1.4.2/geonomics/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.4.2/geonomics/__init__.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.059278 geonomics-1.4.2/geonomics/data/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.R
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2807 2023-06-14 19:20:14.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/env.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/gen.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/geo.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/run_mantel.R
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/default_models/
+-rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.4.2/geonomics/data/default_models/selection_params.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/yosemite_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.083278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.087278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.095278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.155278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.287279 geonomics-1.4.2/geonomics/demos/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.4.2/geonomics/demos/_IBD_IBE.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/demos/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.4.2/geonomics/demos/_simult_select.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.4.2/geonomics/demos/_yosemite.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.287279 geonomics-1.4.2/geonomics/help/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/help/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/help/_memory_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/help/_param_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    42853 2024-04-01 12:51:51.000000 geonomics-1.4.2/geonomics/main.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.335279 geonomics-1.4.2/geonomics/ops/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/ops/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/ops/change.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    11819 2024-05-21 23:43:48.000000 geonomics-1.4.2/geonomics/ops/demography.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.4.2/geonomics/ops/mating.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/ops/movement.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     9065 2024-05-22 01:10:47.000000 geonomics-1.4.2/geonomics/ops/mutation.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.4.2/geonomics/ops/selection.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.379279 geonomics-1.4.2/geonomics/sim/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/sim/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/sim/burnin.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.4.2/geonomics/sim/data.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   144014 2024-05-22 01:42:33.000000 geonomics-1.4.2/geonomics/sim/model.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    49072 2024-05-03 04:17:20.000000 geonomics-1.4.2/geonomics/sim/params.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2024-05-03 05:10:11.000000 geonomics-1.4.2/geonomics/sim/stats.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.467279 geonomics-1.4.2/geonomics/structs/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/structs/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5851 2024-04-30 00:00:02.000000 geonomics-1.4.2/geonomics/structs/community.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    88196 2024-04-29 23:24:41.000000 geonomics-1.4.2/geonomics/structs/genome.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     8671 2024-05-21 23:17:26.000000 geonomics-1.4.2/geonomics/structs/individual.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    32867 2024-05-21 22:48:18.000000 geonomics-1.4.2/geonomics/structs/landscape.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   153536 2024-05-22 00:59:51.000000 geonomics-1.4.2/geonomics/structs/species.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.467279 geonomics-1.4.2/geonomics/utils/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/utils/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/utils/_str_repr_.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10991 2023-04-13 17:58:34.000000 geonomics-1.4.2/geonomics/utils/io.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.4.2/geonomics/utils/spatial.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.4.2/geonomics/utils/viz.py
+-rw-rw-r--   0 deth      (1000) deth      (1000)       22 2024-05-22 01:46:45.000000 geonomics-1.4.2/geonomics/version.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.067278 geonomics-1.4.2/geonomics.egg-info/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     9507 2024-05-22 02:03:52.000000 geonomics-1.4.2/geonomics.egg-info/PKG-INFO
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/SOURCES.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/dependency_links.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/requires.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/top_level.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2024-05-22 02:03:54.471279 geonomics-1.4.2/setup.cfg
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2659 2024-05-08 01:39:40.000000 geonomics-1.4.2/setup.py
```

### Comparing `geonomics-1.4.1/LICENSE.txt` & `geonomics-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/PKG-INFO` & `geonomics-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.4.1.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.4.2.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
+Project-URL: Methods Paper, https://doi.org/10.1093/molbev/msab175
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

### Comparing `geonomics-1.4.1/README.rst` & `geonomics-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.R` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.py` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/env.csv` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/env.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/gen.csv` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/gen.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/geo.csv` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/geo.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/run_mantel.R` & `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/run_mantel.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/default_models/selection_params.py` & `geonomics-1.4.2/geonomics/data/default_models/selection_params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif` & `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/demos/_IBD_IBE.py` & `geonomics-1.4.2/geonomics/demos/_IBD_IBE.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/demos/_simult_select.py` & `geonomics-1.4.2/geonomics/demos/_simult_select.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/demos/_yosemite.py` & `geonomics-1.4.2/geonomics/demos/_yosemite.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/help/__init__.py` & `geonomics-1.4.2/geonomics/help/__init__.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/help/_memory_help.py` & `geonomics-1.4.2/geonomics/help/_memory_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/help/_param_help.py` & `geonomics-1.4.2/geonomics/help/_param_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/main.py` & `geonomics-1.4.2/geonomics/main.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/ops/change.py` & `geonomics-1.4.2/geonomics/ops/change.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/ops/demography.py` & `geonomics-1.4.2/geonomics/ops/demography.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
     #run checks on n_pairs
     if asserts:
         assert n_pairs.min() >= 0, 'n_pairs.min() == %0.2f' %(n_pairs.min())
         assert not np.any(np.isnan(n_pairs))
         assert not np.any(np.isinf(n_pairs))
     #add debug plot
     if debug:
+        print(f"n_pairs: {n_pairs.shape}")
         dp._next_plot('n_pairs', n_pairs)
 
     #Feed the land and mating pairs to spp.do_mating, to produce and
     #disperse zygotes
     spp._do_mating(land, pairs, burn)
 
     #calc N raster, set it as spp.N, then get it  
@@ -229,74 +230,80 @@
     #run checks on N
     if asserts:
         assert N.min() >= 0
         assert not np.any(np.isnan(N))
         assert not np.any(np.isinf(N))
     #add debug plot
     if debug:
+        print(f"N: {N.shape}")
         dp._next_plot('N', N)
 
     #get K raster
     K = spp.K
     #run checks on K
     if asserts:
         assert K.min() >= 0
         assert not np.any(np.isnan(K))
         assert not np.any(np.isinf(K))
     #add debug plot
     if debug:
+        print(f"K: {K.shape}")
         dp._next_plot('K', K)
 
     #calc dNdt
     dNdt = _calc_dNdt(R = spp.R, N = N, K = K,
                                     pop_growth_eq = 'logistic')
     #run checks on dNdt
     if asserts:
         assert not np.any(np.isnan(dNdt))
         assert not np.any(np.isinf(dNdt)), ('The following cells are '
             'infinite: \n\t%s') % str([i for i, n in enumerate(
                                         dNdt.ravel()) if np.isinf(n)])
     #add debug plot
     if debug:
+        print(f"dNdt: {dNdt.shape}")
         dp._next_plot('dNdt', dNdt)
 
     #calculate N_b (raster of estimated births)
     N_b = _calc_N_b(b = spp.b,
         n_births_distr_lambda = spp.n_births_distr_lambda, n_pairs = n_pairs)
     #run checks on N_b
     if asserts:
         assert N_b.min() >= 0
         assert not np.any(np.isnan(N_b))
         assert not np.any(np.isinf(N_b))
     #add debug plot
     if debug:
+        print(f"N_b: {N_b.shape}")
         dp._next_plot('N_b', N_b)
 
     #calc N_d (raster of deaths)
     N_d = _calc_Nd(N_b = N_b, dNdt = dNdt)
     #run checks on N_d
     if asserts:
         assert not np.any(np.isnan(N_d))
         assert not np.any(np.isinf(N_d))
     #add debug plot
     if debug:
+        print(f"N_d: {N_d.shape}")
         dp._next_plot('N_d', N_d)
 
     #calc d (raster of probabilities of density-dependent death)
     d = _calc_d(N_d = N_d, N = N, d_min = spp.d_min, d_max = spp.d_max)
 
     #run checks on d
     if asserts:
         assert d.min() >= 0, 'd.min() is %0.2f, at %s' % (d.min(),
                                                         str(d.argmin()))
         assert d.max() <= 1, 'd.max() is %0.2f' % d.max()
         assert not np.any(np.isnan(d))
         assert not np.any(np.isinf(d))
     #add debug plot
     if debug:
+        print(f"d: {d.shape}")
         dp._next_plot('d', d)
 
     #Get death probabilities
     death_probs = d[spp._cells[:,1], spp._cells[:,0]]
     #If with_selection (i.e. if death probs should account for fitness),
     #then use the d raster and individuals' fitnesses to calculate
     #per-individual probabilities of death
```

### Comparing `geonomics-1.4.1/geonomics/ops/mating.py` & `geonomics-1.4.2/geonomics/ops/mating.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/ops/movement.py` & `geonomics-1.4.2/geonomics/ops/movement.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/ops/mutation.py` & `geonomics-1.4.2/geonomics/ops/mutation.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,29 @@
 
 
 #--------------------------------------
 # FUNCTIONS ---------------------------
 #--------------------------------------
 
 def _calc_estimated_total_mutations(spp, burn_T, T):
-    #NOTE: this would actually be a pretty poor estimate, because mutations
-    #will occur in new individuals, not some static population
-    mean_births = np.mean(spp.n_births[-burn_T:])
+    # NOTE: DETH 22-05-24: redoing this calculation, both because:
+    #       a.) previous approach would provide a pretty poor estimate
+    #       (as the previous comment recognized) but was based on gnx prior
+    #       to fixing the bug that prevented the sum of spp.K from providing a
+    #       good estimate of total population size), 
+    #       and b.) it relied on the n_births vector that filled up during the
+    #       burn-in, but that doesn't always exist now that msprime can be used
+    #       to circumvent the demographic burn-in and seed the population with
+    #       Individuals
+    mean_births = np.sum(spp.K) * spp.b * spp.n_births_distr_lambda
     est = mean_births * spp.gen_arch.L * T * spp.gen_arch._mu_tot
-    #give a decent overestimate
+    # that won't always give a great estimate if, for example, demographic
+    # changes will occur and/or mod.walk will be used to run the models for a
+    # an actual runtime that differs from mod.T;
+    # thus, give a decent overestimate and hope for the best!
     est = int(2.5 * est)
     return est
 
 # add a row to the tskit.TableCollection.mutations table for a new mutation
 def _do_add_row_muts_table(spp, individ, homol, locus):
     # update the tskit.TableCollection.mutations table
     node_id = spp[individ]._nodes_tab_ids[homol]
```

### Comparing `geonomics-1.4.1/geonomics/ops/selection.py` & `geonomics-1.4.2/geonomics/ops/selection.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/sim/burnin.py` & `geonomics-1.4.2/geonomics/sim/burnin.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/sim/data.py` & `geonomics-1.4.2/geonomics/sim/data.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/sim/model.py` & `geonomics-1.4.2/geonomics/sim/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,19 @@
             return spp_num
         else:
             raise ValueError(("The Species identifier must be either a str "
                 "(indicating the Species' name) or an int (indicating "
                 "its key in the Community dict). Instead, a %s was "
                 "provided.") % str(type(spp_id)))
 
+    def _get_spp_msprime_init_status(self, spp_id):
+        msprime_init_status = ('msprime' in
+                        self.params['comm']['species'][spp_id]['init'])
+        return msprime_init_status
+
     #method for getting a Trait's number, give a name (str) or number
     def _get_trt_num(self, spp, trt_id):
         if isinstance(trt_id, int) or trt_id is None:
             return(trt_id)
         elif isinstance(trt, str):
             #get nums for all traits with matching names
             trt_nums = [k for k, trt in spp.gen_arch.traits.items(
@@ -592,44 +597,48 @@
     #self.run_burn_timestep or self.run_main_timestep,
     #depending on burn argument)
     #NOTE: because the queue is a list of functions,
     #the user could add, remove, change the order, or repeat
     #functions within the list as desired
     def _make_fn_queue(self, burn=False):
         queue = []
-
         #append the methods to increment the timestep
         #attributes (i.e. the timestep counters)
         if burn:
             queue.append(self._set_burn_t)
         if not burn:
             queue.append(self._set_t)
             queue.append(self._set_comm_t)
             for spp in self.comm.values():
                 queue.append(lambda: self._set_spp_t(spp.idx))
-
         #append the set_age_stage methods to the queue
         for spp in self.comm.values():
-            queue.append(lambda: self._set_age_stage(spp.idx))
+            # NOTE: skip burn-in functions for msprime-init Species
+            if not burn or not self._get_spp_msprime_init_status(spp.name):
+                queue.append(lambda: self._set_age_stage(spp.idx))
         #append the do_movement_methods, if spp._move
         for spp in self.comm.values():
-            if spp._move:
-                queue.append(lambda: self._do_movement(spp.idx))
+            # NOTE: skip burn-in functions for msprime-init Species
+            if not burn or not self._get_spp_msprime_init_status(spp.name):
+                if spp._move:
+                    queue.append(lambda: self._do_movement(spp.idx))
         #append the do_pop_dynamics methods
         #FIXME: Consider whether the order of these needs to be specified, or
         #randomized, should people want to eventually simulate
         #multiple, interacting species
         for spp in self.comm.values():
-            queue.append(lambda: self._do_pop_dynamics(spp.idx))
-
+            # NOTE: skip burn-in functions for msprime-init Species
+            if not burn or not self._get_spp_msprime_init_status(spp.name):
+                queue.append(lambda: self._do_pop_dynamics(spp.idx))
         #append the set_Nt methods
         # (now that this time step's population sizes are set)
         for spp in self.comm.values():
-            queue.append(lambda: self._set_Nt(spp.idx))
-
+            # NOTE: skip burn-in functions for msprime-init Species
+            if not burn or not self._get_spp_msprime_init_status(spp.name):
+                queue.append(lambda: self._set_Nt(spp.idx))
         #add the Changer.make_change, data._DataCollector._write_data, and 
         #stats._StatsCollector._write_stats methods, if this is not the burn-in
         #and if spp and/or land have Changer objects, or if the model has 
         #_DataCollector or _StatsCollector objects (in the self._data_collector 
         #and self._stats_collector attributes)
         if not burn:
             #add land._make_change method
@@ -657,20 +666,32 @@
         return(queue)
 
 
     #method to generate timestep_verbose_output
     def _print_timestep_info(self, mode):
         verbose_msg = '%s:\tit=%i:\tt=%i\n' % (mode, self.it,
                                 [self.burn_t if mode == 'burn' else self.t][0])
-        spps_submsgs = ''.join(['\tspecies: %s%sN=%i\t(births=%i\tdeaths=%i)\n' %
-                        (spp.name,
-                        ' ' * (30 - len(spp.name)),
-                        spp.Nt[:].pop(),
-                        spp.n_births[:].pop(),
-                        spp.n_deaths[:].pop()) for spp in self.comm.values()])
+        spps_submsgs = ''
+        for spp in self.comm.values():
+            if len(spp.Nt) > 0:
+                Nt_val = spp.Nt[:].pop()
+            else:
+                Nt_val = np.nan
+            if len(spp.n_births) > 0:
+                n_births_val = spp.n_births[:].pop()
+            else:
+                n_births_val = np.nan
+            if len(spp.n_deaths) > 0:
+                n_deaths_val = spp.n_deaths[:].pop()
+            else:
+                n_deaths_val = np.nan
+            spacer = ' ' * (30 - len(spp.name))
+            spp_submsg = (f"\tspecies: {spp.name}{spacer}N={Nt_val}"
+                          f"\t(births={n_births_val}\tdeaths={n_deaths_val})\n")
+            spps_submsgs += spp_submsg
         verbose_msg = verbose_msg + spps_submsgs
         print(verbose_msg)
         print('\t' + '.' * (self.__term_width__ - self.__tab_len__), flush=True)
 
 
     #method to run the burn-in or main function
     #queue (as indicated by mode argument)
@@ -695,16 +716,15 @@
                             if self._verbose:
                                 print(('\nAssigning genomes for '
                                        'species "%s"...\n\n') % spp.name,
                                       flush=True)
                             spp._set_genomes_and_tables(self.burn_T, self.T)
                             # replace gnx-simulated Individuals with
                             # msprime-simulated Individuals, if required
-                            if ('msprime' in self.params['comm']['species'][
-                                                            spp.name]['init']):
+                            if self._get_spp_msprime_init_status(spp.name):
                                 msp = self.params['comm']['species'][
                                                 spp.name]['init']['msprime']
                                 spp._init_msprime_pop(land=self.land,
                                                       msprime_init_params=msp,
                                                      )
                     #and then set the reassign_genomes attribute to False, so
                     #that they won't get reassigned again during this iteration
@@ -2009,14 +2029,16 @@
 
         # get array of resulting genomic data (i.e. 'speciome'),
         # genotypes meaned by individual
         if spp.gen_arch.use_tskit:
             speciome = spp._get_genotypes(biallelic=False)
         else:
             speciome = np.mean(np.stack([i.g for i in spp.values()]), axis=2)
+        assert (0 < n_pcs <= 3 and
+                isinstance(n_pcs, int)), "'n_pcs' must be an integer between 0 and 3"
         # run PCA on speciome
         pca = PCA(n_components=n_pcs)
         PCs = pca.fit_transform(speciome)
         # normalize the PC results
         norm_PCs = (PCs - np.min(PCs,
                                  axis=0)) / (np.max(PCs,
                                                     axis=0) - np.min(PCs,
```

### Comparing `geonomics-1.4.1/geonomics/sim/params.py` & `geonomics-1.4.2/geonomics/sim/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,15 +934,14 @@
                             'msprime_source_pops': 'msprime source populations',
                                            }
                     assert spp_dict[arg] >= 0, ("The number of %s to "
                                     "be created must be 0 or a positive "
                                     "integer.") % (int_arg_str_fmt_dict[arg])
             # get the msprime source pops params, if required
             if 'msprime_source_pops' in [*spp_dict]:
-                print('making msprime params')
                 n_pops = spp_dict['msprime_source_pops']
                 msprime_params = params_str_dict['msprime'][n_pops>0]
                 if n_pops > 0:
                     msprime_params = msprime_params % ('\n'.join([
                         MSPRIME_POP_PARAMS % i for i in range(n_pops)]))
             else:
                 msprime_params = ''
```

### Comparing `geonomics-1.4.1/geonomics/sim/stats.py` & `geonomics-1.4.2/geonomics/sim/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 #get the filepath
                 filepath = stat_dict['filepath']
                 #if the filepath does not contain "OTHER_STATS" then it is a
                 #stat that produces more than a single value per species per
                 #timestep it is collected, so write the data to disk
                 #intermittently and then delete the data from memory (if it was
                 #collected this timestep)
-                if "OTHER_STATS" not in filepath and stat in write_list:
+                if stat in write_list and "OTHER_STATS" not in filepath:
                     #get the correct write_fn for this stat
                     write_fn = self.write_fn_dict[stat]
                     #call the write_fn to write the data to disk
                     write_fn(filepath, stat_dict['vals'][t], t)
                     #then replace the last data collected prior to this
                     #timestep's data with None, to free up memory but still
                     #maintain the latest data in case of plotting
```

### Comparing `geonomics-1.4.1/geonomics/structs/community.py` & `geonomics-1.4.2/geonomics/structs/community.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/structs/genome.py` & `geonomics-1.4.2/geonomics/structs/genome.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/structs/individual.py` & `geonomics-1.4.2/geonomics/structs/individual.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,14 @@
         x,y = r.rand(2)*dim
         #clip to 0.01 under the dimensions, so that for landscapes even up to
         #~10000 on a side (this is bigger than I expect most users would
         #want to run) np.float32 can't return a number rounded up to
         #the dimension itself if an extremely high value is drawn
         x = np.clip(x, 0, dim[0]-0.001)
         y = np.clip(y, 0, dim[1]-0.001)
-
     #set the sex, if necessary
     if sex is None:
         #NOTE: For now sex randomly chosen at 50/50. Change if
         #decide to implement sex chroms, or spp.sex_ratio
         sex = r.binomial(1,0.5)
 
     individual = Individual(idx=idx, x=x, y=y, age=age,
```

### Comparing `geonomics-1.4.1/geonomics/structs/landscape.py` & `geonomics-1.4.2/geonomics/structs/landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,16 +459,17 @@
         # transform to constrain all values to 0 <= val <= 1
         I = I + abs(I.min()) + (
         # NOTE: adding a small jitter to keep values from reaching == 0
         #or == 1, as would likely be the case with linear interpolation
                 0.01 * r.rand())
         I = I / (I.max() + (0.01 * r.rand()))
     #use the dim tuple to subset an approriate size if dim not equal
+    # NOTE: dim is ordered as [x,y], i.e., [j, i]
     if dim[0] != dim[1]:
-        I = I[:dim[0], :dim[1]]
+        I = I[:dim[1], :dim[0]]
     return I
 
 
 def _make_defined_lyr(dim, rast, pts, vals, interp_method="cubic",
                                                     num_hab_types=2):
     #pts should be provided as n-by-2 Numpy array, vals as a 1-by-n Numpy array
```

### Comparing `geonomics-1.4.1/geonomics/structs/species.py` & `geonomics-1.4.2/geonomics/structs/species.py`

 * *Files 1% similar despite different names*

```diff
@@ -4740,4854 +4740,4857 @@
 00012830: 2020 2020 2020 2020 2020 2320 2020 2020            #     
 00012840: 2020 666f 7220 7374 6172 7469 6e67 2063    for starting c
 00012850: 6f6f 7264 696e 6174 6520 6173 7369 676e  oordinate assign
 00012860: 6d65 6e74 2069 6e0a 2020 2020 2020 2020  ment in.        
 00012870: 2020 2020 2320 2020 2020 2020 696e 6469      #       indi
 00012880: 7669 6475 616c 732e 5f6d 616b 655f 696e  viduals._make_in
 00012890: 6469 7669 6475 616c 0a20 2020 2020 2020  dividual.       
-000128a0: 2020 2020 2061 7373 6572 7420 2830 203c       assert (0 <
-000128b0: 3d20 636f 6f72 645b 305d 203c 3d20 7365  = coord[0] <= se
-000128c0: 6c66 2e5f 6c61 6e64 5f64 696d 5b30 5d20  lf._land_dim[0] 
-000128d0: 2d20 302e 3030 3120 616e 640a 2020 2020  - 0.001 and.    
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128f0: 3020 3c3d 2063 6f6f 7264 5b31 5d20 3c3d  0 <= coord[1] <=
-00012900: 2073 656c 662e 5f6c 616e 645f 6469 6d5b   self._land_dim[
-00012910: 315d 202d 2030 2e30 3031 292c 2028 0a20  1] - 0.001), (. 
+000128a0: 2020 2020 2023 204e 4f54 453a 206c 616e       # NOTE: lan
+000128b0: 6420 6469 6d73 2061 7265 206f 7264 6572  d dims are order
+000128c0: 6564 2061 7320 5b78 2c79 5d2c 2069 2e65  ed as [x,y], i.e
+000128d0: 2e2c 205b 6a2c 695d 0a20 2020 2020 2020  ., [j,i].       
+000128e0: 2020 2020 2061 7373 6572 7420 2830 203c       assert (0 <
+000128f0: 3d20 636f 6f72 645b 305d 203c 3d20 7365  = coord[0] <= se
+00012900: 6c66 2e5f 6c61 6e64 5f64 696d 5b30 5d20  lf._land_dim[0] 
+00012910: 2d20 302e 3030 3120 616e 640a 2020 2020  - 0.001 and.    
 00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 2020 2020 2243 6f6f 7264 7320 6d75 7374      "Coords must
-00012960: 2062 6520 220a 2020 2020 2020 2020 2020   be ".          
+00012930: 3020 3c3d 2063 6f6f 7264 5b31 5d20 3c3d  0 <= coord[1] <=
+00012940: 2073 656c 662e 5f6c 616e 645f 6469 6d5b   self._land_dim[
+00012950: 315d 202d 2030 2e30 3031 292c 2028 0a20  1] - 0.001), (. 
+00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012990: 2020 2020 2020 2020 2020 2022 7661 6c69             "vali
-000129a0: 6420 666f 7220 7468 6520 7265 6369 7069  d for the recipi
-000129b0: 656e 7420 220a 2020 2020 2020 2020 2020  ent ".          
+00012990: 2020 2020 2243 6f6f 7264 7320 6d75 7374      "Coords must
+000129a0: 2062 6520 220a 2020 2020 2020 2020 2020   be ".          
+000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129e0: 2020 2020 2020 2020 2020 2022 5370 6563             "Spec
-000129f0: 6965 7327 204c 616e 6473 6361 7065 2022  ies' Landscape "
-00012a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000129d0: 2020 2020 2020 2020 2020 2022 7661 6c69             "vali
+000129e0: 6420 666f 7220 7468 6520 7265 6369 7069  d for the recipi
+000129f0: 656e 7420 220a 2020 2020 2020 2020 2020  ent ".          
+00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2020 2020 2228 692e 652e 2c20 7820        "(i.e., x 
-00012a40: 616e 6420 7920 6d75 7374 2062 6520 220a  and y must be ".
+00012a20: 2020 2020 2020 2020 2020 2022 5370 6563             "Spec
+00012a30: 6965 7327 204c 616e 6473 6361 7065 2022  ies' Landscape "
+00012a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 2020 2020 2022 696e 2074 6865 2069 6e63       "in the inc
-00012a90: 6c75 7369 7665 2022 0a20 2020 2020 2020  lusive ".       
+00012a70: 2020 2020 2020 2228 692e 652e 2c20 7820        "(i.e., x 
+00012a80: 616e 6420 7920 6d75 7374 2062 6520 220a  and y must be ".
+00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2220                " 
-00012ad0: 696e 7465 7276 616c 7320 220a 2020 2020  intervals ".    
+00012ac0: 2020 2020 2022 696e 2074 6865 2069 6e63       "in the inc
+00012ad0: 6c75 7369 7665 2022 0a20 2020 2020 2020  lusive ".       
 00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2022 5b30 2c20 6c61 6e64 5f64 696d 5f78   "[0, land_dim_x
-00012b20: 5d20 616e 6422 0a20 2020 2020 2020 2020  ] and".         
+00012b00: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+00012b10: 696e 7465 7276 616c 7320 220a 2020 2020  intervals ".    
+00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b50: 2020 2020 2020 2020 2020 2020 225b 302c              "[0,
-00012b60: 206c 616e 645f 6469 6d5f 795d 2c20 220a   land_dim_y], ".
+00012b50: 2022 5b30 2c20 6c61 6e64 5f64 696d 5f78   "[0, land_dim_x
+00012b60: 5d20 616e 6422 0a20 2020 2020 2020 2020  ] and".         
 00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ba0: 2020 2020 2022 7265 7370 6563 7469 7665       "respective
-00012bb0: 6c79 2e22 290a 0a20 2020 2020 2020 2023  ly.")..        #
-00012bc0: 2065 6974 6865 7220 6765 7420 496e 6469   either get Indi
-00012bd0: 7669 6475 616c 7320 616e 6420 7468 6569  viduals and thei
-00012be0: 7220 7473 6b69 742e 5461 626c 6543 6f6c  r tskit.TableCol
-00012bf0: 6c65 6374 696f 6e0a 2020 2020 2020 2020  lection.        
-00012c00: 2320 6672 6f6d 2074 6865 2067 6976 656e  # from the given
-00012c10: 2067 6e78 2053 7065 6369 6573 206f 626a   gnx Species obj
-00012c20: 6563 742e 2e2e 0a20 2020 2020 2020 2069  ect....        i
-00012c30: 6620 736f 7572 6365 5f73 7070 2069 7320  f source_spp is 
-00012c40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012c50: 2020 2020 2020 2320 7261 6973 6520 7761        # raise wa
-00012c60: 726e 696e 6720 6162 6f75 7420 706f 7465  rning about pote
-00012c70: 6e74 6961 6c20 756e 666f 7265 7365 656e  ntial unforeseen
-00012c80: 2065 6666 6563 7473 206f 6620 696e 7472   effects of intr
-00012c90: 6f64 7563 696e 670a 2020 2020 2020 2020  oducing.        
-00012ca0: 2020 2020 2320 496e 6469 7669 6475 616c      # Individual
-00012cb0: 7320 6672 6f6d 2061 6e20 696e 636f 7272  s from an incorr
-00012cc0: 6563 746c 7920 7061 7261 6d65 7465 7269  ectly parameteri
-00012cd0: 7a65 6420 736f 7572 6365 2053 7065 6369  zed source Speci
-00012ce0: 6573 0a20 2020 2020 2020 2020 2020 2077  es.            w
-00012cf0: 6172 6e69 6e67 732e 7761 726e 2828 2249  arnings.warn(("I
-00012d00: 6e74 726f 6475 6369 6e67 2049 6e64 6976  ntroducing Indiv
-00012d10: 6964 7561 6c73 2066 726f 6d20 6f6e 6520  iduals from one 
-00012d20: 5370 6563 6965 7320 6f62 6a65 6374 2022  Species object "
-00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d40: 2020 2020 2022 696e 746f 2061 6e6f 7468       "into anoth
-00012d50: 6572 2063 6f75 6c64 2063 6175 7365 2075  er could cause u
-00012d60: 6e6e 6f74 6963 6564 2069 7373 7565 732e  nnoticed issues.
-00012d70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00012d80: 2020 2020 2020 2022 4765 6f6e 6f6d 6963         "Geonomic
-00012d90: 7320 7769 6c6c 2063 6865 636b 2061 6e64  s will check and
-00012da0: 2070 7265 7665 6e74 2063 6f6e 666c 6963   prevent conflic
-00012db0: 7420 6265 7477 6565 6e20 220a 2020 2020  t between ".    
-00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dd0: 2273 7472 6963 746c 7920 696e 636f 6d70  "strictly incomp
-00012de0: 6174 6962 6c65 2061 7474 7269 6275 7465  atible attribute
-00012df0: 7320 6f66 2074 6865 2053 7065 6369 6573  s of the Species
-00012e00: 2c20 220a 2020 2020 2020 2020 2020 2020  , ".            
-00012e10: 2020 2020 2020 2020 2247 656e 6f6d 6963          "Genomic
-00012e20: 4172 6368 6974 6563 7475 7265 732c 2061  Architectures, a
-00012e30: 6e64 2054 7261 6974 732e 2048 6f77 6576  nd Traits. Howev
-00012e40: 6572 2c20 6174 7472 6962 7574 6573 2022  er, attributes "
-00012e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e60: 2020 2020 2022 7768 6f73 6520 636f 6d70       "whose comp
-00012e70: 6174 6962 696c 6974 7920 6465 7065 6e64  atibility depend
-00012e80: 7320 6f6e 2074 6865 2073 6369 656e 7469  s on the scienti
-00012e90: 6669 6320 220a 2020 2020 2020 2020 2020  fic ".          
-00012ea0: 2020 2020 2020 2020 2020 2272 6561 736f            "reaso
-00012eb0: 6e69 6e67 2062 6568 696e 6420 7468 6520  ning behind the 
-00012ec0: 7363 656e 6172 696f 2062 6569 6e67 2073  scenario being s
-00012ed0: 696d 756c 6174 6564 2022 0a20 2020 2020  imulated ".     
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012ef0: 2865 2e67 2e2c 206d 7574 6174 696f 6e61  (e.g., mutationa
-00012f00: 6c20 7061 7261 6d65 7465 7273 2c20 220a  l parameters, ".
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2020 2263 6172 7279 696e 6720 6361      "carrying ca
-00012f30: 7061 6369 7479 2070 6172 616d 6574 6572  pacity parameter
-00012f40: 732c 2065 7463 2e29 2022 0a20 2020 2020  s, etc.) ".     
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012f60: 7769 6c6c 2062 6520 616c 6c6f 7765 6420  will be allowed 
-00012f70: 746f 2064 6966 6665 7220 6265 7477 6565  to differ betwee
-00012f80: 6e20 7468 6520 736f 7572 6365 2061 6e64  n the source and
-00012f90: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00012fa0: 2020 2020 2020 2022 7265 6369 7069 656e         "recipien
-00012fb0: 7420 5370 6563 6965 7320 6f62 6a65 6374  t Species object
-00012fc0: 7320 616e 642c 2022 0a20 2020 2020 2020  s and, ".       
-00012fd0: 2020 2020 2020 2020 2020 2020 2022 6966               "if
-00012fe0: 2074 6865 7365 2064 6966 6665 7265 6e63   these differenc
-00012ff0: 6573 2077 6572 6520 756e 696e 7465 6e64  es were unintend
-00013000: 6564 2062 7574 2067 6f20 220a 2020 2020  ed but go ".    
-00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013020: 2275 6e64 6574 6563 7465 642c 2063 6f75  "undetected, cou
-00013030: 6c64 206c 6561 6420 746f 2069 6e63 6f72  ld lead to incor
-00013040: 7265 6374 206f 7220 6d69 736c 6561 6469  rect or misleadi
-00013050: 6e67 2064 6174 6120 220a 2020 2020 2020  ng data ".      
-00013060: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00013070: 6e64 2072 6573 756c 7473 2e20 506c 6561  nd results. Plea
-00013080: 7365 2075 7365 2063 6172 6520 7768 656e  se use care when
-00013090: 2070 6c61 6e6e 696e 672c 2022 0a20 2020   planning, ".   
-000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 2022 696d 706c 656d 656e 7469 6e67 2c20   "implementing, 
-000130c0: 616e 6420 6368 6563 6b69 6e67 2079 6f75  and checking you
-000130d0: 7220 636f 6465 2e22 2929 0a0a 2020 2020  r code."))..    
-000130e0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-000130f0: 6520 736f 7572 6365 2053 7065 6369 6573  e source Species
-00013100: 2066 726f 6d20 7769 7468 696e 2074 6869   from within thi
-00013110: 7320 6d6f 6465 6c2c 2069 6620 6e65 6365  s model, if nece
-00013120: 7373 6172 790a 2020 2020 2020 2020 2020  ssary.          
-00013130: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013140: 736f 7572 6365 5f73 7070 2c20 696e 7429  source_spp, int)
-00013150: 206f 7220 6973 696e 7374 616e 6365 2873   or isinstance(s
-00013160: 6f75 7263 655f 7370 702c 2073 7472 293a  ource_spp, str):
-00013170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013180: 2073 6f75 7263 655f 7370 7020 3d20 7365   source_spp = se
-00013190: 6c66 2e63 6f6d 6d5b 7365 6c66 2e5f 6765  lf.comm[self._ge
-000131a0: 745f 7370 705f 6e75 6d28 736f 7572 6365  t_spp_num(source
-000131b0: 5f73 7070 295d 0a0a 2020 2020 2020 2020  _spp)]..        
-000131c0: 2020 2020 2320 6173 7365 7274 2074 6861      # assert tha
-000131d0: 7420 6578 6163 746c 7920 6f6e 6520 6f66  t exactly one of
-000131e0: 2074 6865 2027 6e27 2061 6e64 2027 696e   the 'n' and 'in
-000131f0: 6469 7669 6473 270a 2020 2020 2020 2020  divids'.        
-00013200: 2020 2020 2320 7061 7261 6d73 2069 7320      # params is 
-00013210: 7072 6f76 6964 6564 2c20 616e 6420 7468  provided, and th
-00013220: 6174 2074 6865 2073 697a 6520 6f66 2027  at the size of '
-00013230: 6e27 0a20 2020 2020 2020 2020 2020 2023  n'.            #
-00013240: 206f 7220 7369 7a65 2061 6e64 2063 6f6e   or size and con
-00013250: 7465 6e74 7320 6f66 2027 696e 6469 7669  tents of 'indivi
-00013260: 6473 2720 6172 6520 7661 6c69 640a 2020  ds' are valid.  
-00013270: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00013280: 2028 286e 2069 7320 6e6f 7420 4e6f 6e65   ((n is not None
-00013290: 2061 6e64 2069 6e64 6976 6964 7320 6973   and individs is
-000132a0: 204e 6f6e 6529 206f 720a 2020 2020 2020   None) or.      
-000132b0: 2020 2020 2020 2020 2020 2020 2020 286e                (n
-000132c0: 2069 7320 4e6f 6e65 2061 6e64 2069 6e64   is None and ind
-000132d0: 6976 6964 7320 6973 206e 6f74 204e 6f6e  ivids is not Non
-000132e0: 6529 292c 2028 2249 6620 7573 696e 6720  e)), ("If using 
-000132f0: 616e 6f74 6865 7220 220a 2020 2020 2020  another ".      
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 2020 2247 656f 6e6f 6d69 6373 2053 7065    "Geonomics Spe
-00013340: 6369 6573 2022 0a20 2020 2020 2020 2020  cies ".         
+00012b90: 2020 2020 2020 2020 2020 2020 225b 302c              "[0,
+00012ba0: 206c 616e 645f 6469 6d5f 795d 2c20 220a   land_dim_y], ".
+00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012be0: 2020 2020 2022 7265 7370 6563 7469 7665       "respective
+00012bf0: 6c79 2e22 290a 0a20 2020 2020 2020 2023  ly.")..        #
+00012c00: 2065 6974 6865 7220 6765 7420 496e 6469   either get Indi
+00012c10: 7669 6475 616c 7320 616e 6420 7468 6569  viduals and thei
+00012c20: 7220 7473 6b69 742e 5461 626c 6543 6f6c  r tskit.TableCol
+00012c30: 6c65 6374 696f 6e0a 2020 2020 2020 2020  lection.        
+00012c40: 2320 6672 6f6d 2074 6865 2067 6976 656e  # from the given
+00012c50: 2067 6e78 2053 7065 6369 6573 206f 626a   gnx Species obj
+00012c60: 6563 742e 2e2e 0a20 2020 2020 2020 2069  ect....        i
+00012c70: 6620 736f 7572 6365 5f73 7070 2069 7320  f source_spp is 
+00012c80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00012c90: 2020 2020 2020 2320 7261 6973 6520 7761        # raise wa
+00012ca0: 726e 696e 6720 6162 6f75 7420 706f 7465  rning about pote
+00012cb0: 6e74 6961 6c20 756e 666f 7265 7365 656e  ntial unforeseen
+00012cc0: 2065 6666 6563 7473 206f 6620 696e 7472   effects of intr
+00012cd0: 6f64 7563 696e 670a 2020 2020 2020 2020  oducing.        
+00012ce0: 2020 2020 2320 496e 6469 7669 6475 616c      # Individual
+00012cf0: 7320 6672 6f6d 2061 6e20 696e 636f 7272  s from an incorr
+00012d00: 6563 746c 7920 7061 7261 6d65 7465 7269  ectly parameteri
+00012d10: 7a65 6420 736f 7572 6365 2053 7065 6369  zed source Speci
+00012d20: 6573 0a20 2020 2020 2020 2020 2020 2077  es.            w
+00012d30: 6172 6e69 6e67 732e 7761 726e 2828 2249  arnings.warn(("I
+00012d40: 6e74 726f 6475 6369 6e67 2049 6e64 6976  ntroducing Indiv
+00012d50: 6964 7561 6c73 2066 726f 6d20 6f6e 6520  iduals from one 
+00012d60: 5370 6563 6965 7320 6f62 6a65 6374 2022  Species object "
+00012d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d80: 2020 2020 2022 696e 746f 2061 6e6f 7468       "into anoth
+00012d90: 6572 2063 6f75 6c64 2063 6175 7365 2075  er could cause u
+00012da0: 6e6e 6f74 6963 6564 2069 7373 7565 732e  nnoticed issues.
+00012db0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00012dc0: 2020 2020 2020 2022 4765 6f6e 6f6d 6963         "Geonomic
+00012dd0: 7320 7769 6c6c 2063 6865 636b 2061 6e64  s will check and
+00012de0: 2070 7265 7665 6e74 2063 6f6e 666c 6963   prevent conflic
+00012df0: 7420 6265 7477 6565 6e20 220a 2020 2020  t between ".    
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2273 7472 6963 746c 7920 696e 636f 6d70  "strictly incomp
+00012e20: 6174 6962 6c65 2061 7474 7269 6275 7465  atible attribute
+00012e30: 7320 6f66 2074 6865 2053 7065 6369 6573  s of the Species
+00012e40: 2c20 220a 2020 2020 2020 2020 2020 2020  , ".            
+00012e50: 2020 2020 2020 2020 2247 656e 6f6d 6963          "Genomic
+00012e60: 4172 6368 6974 6563 7475 7265 732c 2061  Architectures, a
+00012e70: 6e64 2054 7261 6974 732e 2048 6f77 6576  nd Traits. Howev
+00012e80: 6572 2c20 6174 7472 6962 7574 6573 2022  er, attributes "
+00012e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ea0: 2020 2020 2022 7768 6f73 6520 636f 6d70       "whose comp
+00012eb0: 6174 6962 696c 6974 7920 6465 7065 6e64  atibility depend
+00012ec0: 7320 6f6e 2074 6865 2073 6369 656e 7469  s on the scienti
+00012ed0: 6669 6320 220a 2020 2020 2020 2020 2020  fic ".          
+00012ee0: 2020 2020 2020 2020 2020 2272 6561 736f            "reaso
+00012ef0: 6e69 6e67 2062 6568 696e 6420 7468 6520  ning behind the 
+00012f00: 7363 656e 6172 696f 2062 6569 6e67 2073  scenario being s
+00012f10: 696d 756c 6174 6564 2022 0a20 2020 2020  imulated ".     
+00012f20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012f30: 2865 2e67 2e2c 206d 7574 6174 696f 6e61  (e.g., mutationa
+00012f40: 6c20 7061 7261 6d65 7465 7273 2c20 220a  l parameters, ".
+00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f60: 2020 2020 2263 6172 7279 696e 6720 6361      "carrying ca
+00012f70: 7061 6369 7479 2070 6172 616d 6574 6572  pacity parameter
+00012f80: 732c 2065 7463 2e29 2022 0a20 2020 2020  s, etc.) ".     
+00012f90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012fa0: 7769 6c6c 2062 6520 616c 6c6f 7765 6420  will be allowed 
+00012fb0: 746f 2064 6966 6665 7220 6265 7477 6565  to differ betwee
+00012fc0: 6e20 7468 6520 736f 7572 6365 2061 6e64  n the source and
+00012fd0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00012fe0: 2020 2020 2020 2022 7265 6369 7069 656e         "recipien
+00012ff0: 7420 5370 6563 6965 7320 6f62 6a65 6374  t Species object
+00013000: 7320 616e 642c 2022 0a20 2020 2020 2020  s and, ".       
+00013010: 2020 2020 2020 2020 2020 2020 2022 6966               "if
+00013020: 2074 6865 7365 2064 6966 6665 7265 6e63   these differenc
+00013030: 6573 2077 6572 6520 756e 696e 7465 6e64  es were unintend
+00013040: 6564 2062 7574 2067 6f20 220a 2020 2020  ed but go ".    
+00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013060: 2275 6e64 6574 6563 7465 642c 2063 6f75  "undetected, cou
+00013070: 6c64 206c 6561 6420 746f 2069 6e63 6f72  ld lead to incor
+00013080: 7265 6374 206f 7220 6d69 736c 6561 6469  rect or misleadi
+00013090: 6e67 2064 6174 6120 220a 2020 2020 2020  ng data ".      
+000130a0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+000130b0: 6e64 2072 6573 756c 7473 2e20 506c 6561  nd results. Plea
+000130c0: 7365 2075 7365 2063 6172 6520 7768 656e  se use care when
+000130d0: 2070 6c61 6e6e 696e 672c 2022 0a20 2020   planning, ".   
+000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130f0: 2022 696d 706c 656d 656e 7469 6e67 2c20   "implementing, 
+00013100: 616e 6420 6368 6563 6b69 6e67 2079 6f75  and checking you
+00013110: 7220 636f 6465 2e22 2929 0a0a 2020 2020  r code."))..    
+00013120: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+00013130: 6520 736f 7572 6365 2053 7065 6369 6573  e source Species
+00013140: 2066 726f 6d20 7769 7468 696e 2074 6869   from within thi
+00013150: 7320 6d6f 6465 6c2c 2069 6620 6e65 6365  s model, if nece
+00013160: 7373 6172 790a 2020 2020 2020 2020 2020  ssary.          
+00013170: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00013180: 736f 7572 6365 5f73 7070 2c20 696e 7429  source_spp, int)
+00013190: 206f 7220 6973 696e 7374 616e 6365 2873   or isinstance(s
+000131a0: 6f75 7263 655f 7370 702c 2073 7472 293a  ource_spp, str):
+000131b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131c0: 2073 6f75 7263 655f 7370 7020 3d20 7365   source_spp = se
+000131d0: 6c66 2e63 6f6d 6d5b 7365 6c66 2e5f 6765  lf.comm[self._ge
+000131e0: 745f 7370 705f 6e75 6d28 736f 7572 6365  t_spp_num(source
+000131f0: 5f73 7070 295d 0a0a 2020 2020 2020 2020  _spp)]..        
+00013200: 2020 2020 2320 6173 7365 7274 2074 6861      # assert tha
+00013210: 7420 6578 6163 746c 7920 6f6e 6520 6f66  t exactly one of
+00013220: 2074 6865 2027 6e27 2061 6e64 2027 696e   the 'n' and 'in
+00013230: 6469 7669 6473 270a 2020 2020 2020 2020  divids'.        
+00013240: 2020 2020 2320 7061 7261 6d73 2069 7320      # params is 
+00013250: 7072 6f76 6964 6564 2c20 616e 6420 7468  provided, and th
+00013260: 6174 2074 6865 2073 697a 6520 6f66 2027  at the size of '
+00013270: 6e27 0a20 2020 2020 2020 2020 2020 2023  n'.            #
+00013280: 206f 7220 7369 7a65 2061 6e64 2063 6f6e   or size and con
+00013290: 7465 6e74 7320 6f66 2027 696e 6469 7669  tents of 'indivi
+000132a0: 6473 2720 6172 6520 7661 6c69 640a 2020  ds' are valid.  
+000132b0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+000132c0: 2028 286e 2069 7320 6e6f 7420 4e6f 6e65   ((n is not None
+000132d0: 2061 6e64 2069 6e64 6976 6964 7320 6973   and individs is
+000132e0: 204e 6f6e 6529 206f 720a 2020 2020 2020   None) or.      
+000132f0: 2020 2020 2020 2020 2020 2020 2020 286e                (n
+00013300: 2069 7320 4e6f 6e65 2061 6e64 2069 6e64   is None and ind
+00013310: 6976 6964 7320 6973 206e 6f74 204e 6f6e  ivids is not Non
+00013320: 6529 292c 2028 2249 6620 7573 696e 6720  e)), ("If using 
+00013330: 616e 6f74 6865 7220 220a 2020 2020 2020  another ".      
+00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013370: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013380: 6f62 6a65 6374 2061 7320 7468 6520 736f  object as the so
-00013390: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+00013370: 2020 2247 656f 6e6f 6d69 6373 2053 7065    "Geonomics Spe
+00013380: 6369 6573 2022 0a20 2020 2020 2020 2020  cies ".         
+00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000133a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000133d0: 706f 7075 6c61 7469 6f6e 2074 6865 6e20  population then 
-000133e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000133b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000133c0: 6f62 6a65 6374 2061 7320 7468 6520 736f  object as the so
+000133d0: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013410: 2020 2020 2020 2020 2020 2265 6974 6865            "eithe
-00013420: 7220 606e 6020 6f72 2022 0a20 2020 2020  r `n` or ".     
+00013400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013410: 706f 7075 6c61 7469 6f6e 2074 6865 6e20  population then 
+00013420: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
 00013430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013460: 2020 2022 6069 6e64 6976 6964 7360 206d     "`individs` m
-00013470: 7573 7420 6265 2022 0a20 2020 2020 2020  ust be ".       
+00013450: 2020 2020 2020 2020 2020 2265 6974 6865            "eithe
+00013460: 7220 606e 6020 6f72 2022 0a20 2020 2020  r `n` or ".     
+00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134b0: 2022 7072 6f76 6964 6564 2c20 220a 2020   "provided, ".  
+000134a0: 2020 2022 6069 6e64 6976 6964 7360 206d     "`individs` m
+000134b0: 7573 7420 6265 2022 0a20 2020 2020 2020  ust be ".       
 000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134f0: 2020 2020 2020 2262 7574 206e 6f74 2062        "but not b
-00013500: 6f74 682e 2229 0a20 2020 2020 2020 2020  oth.").         
-00013510: 2020 2069 6620 696e 6469 7669 6473 2069     if individs i
-00013520: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00013530: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-00013540: 203c 3d20 6c65 6e28 736f 7572 6365 5f73   <= len(source_s
-00013550: 7070 292c 2028 2260 6e60 206d 7573 7420  pp), ("`n` must 
-00013560: 6e6f 7420 6265 2067 7265 6174 6572 2074  not be greater t
-00013570: 6861 6e20 220a 2020 2020 2020 2020 2020  han ".          
-00013580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 2020 2020 2274 6865 2070 6f70 756c 6174      "the populat
-000135b0: 696f 6e20 7369 7a65 206f 6620 220a 2020  ion size of ".  
+000134f0: 2022 7072 6f76 6964 6564 2c20 220a 2020   "provided, ".  
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013530: 2020 2020 2020 2262 7574 206e 6f74 2062        "but not b
+00013540: 6f74 682e 2229 0a20 2020 2020 2020 2020  oth.").         
+00013550: 2020 2069 6620 696e 6469 7669 6473 2069     if individs i
+00013560: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00013570: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+00013580: 203c 3d20 6c65 6e28 736f 7572 6365 5f73   <= len(source_s
+00013590: 7070 292c 2028 2260 6e60 206d 7573 7420  pp), ("`n` must 
+000135a0: 6e6f 7420 6265 2067 7265 6174 6572 2074  not be greater t
+000135b0: 6861 6e20 220a 2020 2020 2020 2020 2020  han ".          
 000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135e0: 2020 2020 2020 2020 2020 2020 2260 736f              "`so
-000135f0: 7572 6365 5f73 7070 602e 2229 0a20 2020  urce_spp`.").   
-00013600: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00013610: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00013620: 7373 6572 7420 286c 656e 286e 702e 756e  ssert (len(np.un
-00013630: 6971 7565 2869 6e64 6976 6964 7329 2920  ique(individs)) 
-00013640: 3c3d 206c 656e 2873 6f75 7263 655f 7370  <= len(source_sp
-00013650: 7029 2061 6e64 0a20 2020 2020 2020 2020  p) and.         
-00013660: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00013670: 702e 616c 6c28 5b69 6e64 2069 6e20 736f  p.all([ind in so
-00013680: 7572 6365 5f73 7070 2066 6f72 2069 6e64  urce_spp for ind
-00013690: 2069 6e20 696e 6469 7669 6473 5d29 292c   in individs])),
-000136a0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-000136b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000136c0: 6069 6e64 6976 6964 7360 2063 6f6e 7461  `individs` conta
-000136d0: 696e 7320 496e 6469 7669 6475 616c 2069  ins Individual i
-000136e0: 6e64 6963 6573 2074 6861 7420 646f 2022  ndices that do "
-000136f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013700: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00013710: 7420 6578 6973 7420 696e 2060 736f 7572  t exist in `sour
-00013720: 6365 5f73 7070 602e 2229 0a0a 2020 2020  ce_spp`.")..    
-00013730: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-00013740: 7468 6174 2061 6c6c 2053 7065 6369 6573  that all Species
-00013750: 2070 6172 616d 7320 7468 6174 206e 6565   params that nee
-00013760: 6420 746f 206d 6174 6368 2061 7265 2074  d to match are t
-00013770: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
-00013780: 2020 2020 2320 696e 2074 6865 2073 6f75      # in the sou
-00013790: 7263 6520 706f 7075 6c61 7469 6f6e 2773  rce population's
-000137a0: 2053 7065 6369 6573 2061 6e64 2069 6e20   Species and in 
-000137b0: 7468 6973 2053 7065 6369 6573 2720 706f  this Species' po
-000137c0: 700a 2020 2020 2020 2020 2020 2020 7370  p.            sp
-000137d0: 705f 6174 7472 735f 746f 5f63 6865 636b  p_attrs_to_check
-000137e0: 203d 205b 274b 5f6c 6179 6572 272c 0a20   = ['K_layer',. 
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013810: 2027 7365 6c65 6374 696f 6e27 2c0a 2020   'selection',.  
-00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135e0: 2020 2020 2274 6865 2070 6f70 756c 6174      "the populat
+000135f0: 696f 6e20 7369 7a65 206f 6620 220a 2020  ion size of ".  
+00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013620: 2020 2020 2020 2020 2020 2020 2260 736f              "`so
+00013630: 7572 6365 5f73 7070 602e 2229 0a20 2020  urce_spp`.").   
+00013640: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00013650: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00013660: 7373 6572 7420 286c 656e 286e 702e 756e  ssert (len(np.un
+00013670: 6971 7565 2869 6e64 6976 6964 7329 2920  ique(individs)) 
+00013680: 3c3d 206c 656e 2873 6f75 7263 655f 7370  <= len(source_sp
+00013690: 7029 2061 6e64 0a20 2020 2020 2020 2020  p) and.         
+000136a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000136b0: 702e 616c 6c28 5b69 6e64 2069 6e20 736f  p.all([ind in so
+000136c0: 7572 6365 5f73 7070 2066 6f72 2069 6e64  urce_spp for ind
+000136d0: 2069 6e20 696e 6469 7669 6473 5d29 292c   in individs])),
+000136e0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+000136f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013700: 6069 6e64 6976 6964 7360 2063 6f6e 7461  `individs` conta
+00013710: 696e 7320 496e 6469 7669 6475 616c 2069  ins Individual i
+00013720: 6e64 6963 6573 2074 6861 7420 646f 2022  ndices that do "
+00013730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013740: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
+00013750: 7420 6578 6973 7420 696e 2060 736f 7572  t exist in `sour
+00013760: 6365 5f73 7070 602e 2229 0a0a 2020 2020  ce_spp`.")..    
+00013770: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+00013780: 7468 6174 2061 6c6c 2053 7065 6369 6573  that all Species
+00013790: 2070 6172 616d 7320 7468 6174 206e 6565   params that nee
+000137a0: 6420 746f 206d 6174 6368 2061 7265 2074  d to match are t
+000137b0: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
+000137c0: 2020 2020 2320 696e 2074 6865 2073 6f75      # in the sou
+000137d0: 7263 6520 706f 7075 6c61 7469 6f6e 2773  rce population's
+000137e0: 2053 7065 6369 6573 2061 6e64 2069 6e20   Species and in 
+000137f0: 7468 6973 2053 7065 6369 6573 2720 706f  this Species' po
+00013800: 700a 2020 2020 2020 2020 2020 2020 7370  p.            sp
+00013810: 705f 6174 7472 735f 746f 5f63 6865 636b  p_attrs_to_check
+00013820: 203d 205b 274b 5f6c 6179 6572 272c 0a20   = ['K_layer',. 
 00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2773 6578 5f72 6174 696f 272c 0a20 2020  'sex_ratio',.   
-00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013860: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013870: 6d6f 7665 272c 0a20 2020 2020 2020 2020  move',.         
-00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013890: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000138a0: 2020 2020 2020 666f 7220 6174 7472 2069        for attr i
-000138b0: 6e20 7370 705f 6174 7472 735f 746f 5f63  n spp_attrs_to_c
-000138c0: 6865 636b 3a0a 2020 2020 2020 2020 2020  heck:.          
-000138d0: 2020 2020 2020 6173 7365 7274 206e 702e        assert np.
-000138e0: 616c 6c28 6765 7461 7474 7228 736f 7572  all(getattr(sour
-000138f0: 6365 5f73 7070 2c20 6174 7472 2920 3d3d  ce_spp, attr) ==
-00013900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013910: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00013920: 6574 6174 7472 2873 656c 662c 2061 7474  etattr(self, att
-00013930: 7229 292c 2028 0a20 2020 2020 2020 2020  r)), (.         
-00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013950: 2020 2020 2020 2020 2022 626f 7468 2074           "both t
-00013960: 6865 2073 6f75 7263 6520 616e 6420 7265  he source and re
-00013970: 6369 7069 656e 7420 5370 6563 6965 7320  cipient Species 
-00013980: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 2020 2020 226d 7573 7420 6861 7665 2069      "must have i
-000139b0: 6465 6e74 6963 616c 2076 616c 7565 7320  dentical values 
-000139c0: 666f 7220 220a 2020 2020 2020 2020 2020  for ".          
+00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013850: 2027 7365 6c65 6374 696f 6e27 2c0a 2020   'selection',.  
+00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013880: 2773 6578 5f72 6174 696f 272c 0a20 2020  'sex_ratio',.   
+00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000138b0: 6d6f 7665 272c 0a20 2020 2020 2020 2020  move',.         
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138d0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000138e0: 2020 2020 2020 666f 7220 6174 7472 2069        for attr i
+000138f0: 6e20 7370 705f 6174 7472 735f 746f 5f63  n spp_attrs_to_c
+00013900: 6865 636b 3a0a 2020 2020 2020 2020 2020  heck:.          
+00013910: 2020 2020 2020 6173 7365 7274 206e 702e        assert np.
+00013920: 616c 6c28 6765 7461 7474 7228 736f 7572  all(getattr(sour
+00013930: 6365 5f73 7070 2c20 6174 7472 2920 3d3d  ce_spp, attr) ==
+00013940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013950: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00013960: 6574 6174 7472 2873 656c 662c 2061 7474  etattr(self, att
+00013970: 7229 292c 2028 0a20 2020 2020 2020 2020  r)), (.         
+00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013990: 2020 2020 2020 2020 2022 626f 7468 2074           "both t
+000139a0: 6865 2073 6f75 7263 6520 616e 6420 7265  he source and re
+000139b0: 6369 7069 656e 7420 5370 6563 6965 7320  cipient Species 
+000139c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
 000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 2020 2020 2020 2020 6622 7468 6520 6174          f"the at
-000139f0: 7472 6962 7574 6520 277b 6174 7472 7d27  tribute '{attr}'
-00013a00: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-00013a10: 2320 6368 6563 6b20 7468 6174 2061 6c6c  # check that all
-00013a20: 2067 656e 5f61 7263 6820 7061 7261 6d73   gen_arch params
-00013a30: 2074 6861 7420 6e65 6564 2074 6f20 6d61   that need to ma
-00013a40: 7463 6820 6172 6520 7468 6520 7361 6d65  tch are the same
-00013a50: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00013a60: 6e20 7468 6520 736f 7572 6365 2070 6f70  n the source pop
-00013a70: 756c 6174 696f 6e27 7320 5370 6563 6965  ulation's Specie
-00013a80: 7320 616e 6420 7468 6973 2053 7065 6369  s and this Speci
-00013a90: 6573 0a20 2020 2020 2020 2020 2020 2073  es.            s
-00013aa0: 6f75 7263 655f 6765 6e5f 6172 6368 203d  ource_gen_arch =
-00013ab0: 2073 6f75 7263 655f 7370 702e 6765 6e5f   source_spp.gen_
-00013ac0: 6172 6368 0a20 2020 2020 2020 2020 2020  arch.           
-00013ad0: 2073 656c 662e 6765 6e5f 6172 6368 203d   self.gen_arch =
-00013ae0: 2073 656c 662e 6765 6e5f 6172 6368 0a20   self.gen_arch. 
-00013af0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00013b00: 7420 736f 7572 6365 5f67 656e 5f61 7263  t source_gen_arc
-00013b10: 682e 4c20 3d3d 2073 656c 662e 6765 6e5f  h.L == self.gen_
-00013b20: 6172 6368 2e4c 2c20 2822 736f 7572 6365  arch.L, ("source
-00013b30: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b60: 2253 7065 6369 6573 206d 7573 7420 6861  "Species must ha
-00013b70: 7665 2061 2022 0a20 2020 2020 2020 2020  ve a ".         
+000139e0: 2020 2020 226d 7573 7420 6861 7665 2069      "must have i
+000139f0: 6465 6e74 6963 616c 2076 616c 7565 7320  dentical values 
+00013a00: 666f 7220 220a 2020 2020 2020 2020 2020  for ".          
+00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a20: 2020 2020 2020 2020 6622 7468 6520 6174          f"the at
+00013a30: 7472 6962 7574 6520 277b 6174 7472 7d27  tribute '{attr}'
+00013a40: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00013a50: 2320 6368 6563 6b20 7468 6174 2061 6c6c  # check that all
+00013a60: 2067 656e 5f61 7263 6820 7061 7261 6d73   gen_arch params
+00013a70: 2074 6861 7420 6e65 6564 2074 6f20 6d61   that need to ma
+00013a80: 7463 6820 6172 6520 7468 6520 7361 6d65  tch are the same
+00013a90: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+00013aa0: 6e20 7468 6520 736f 7572 6365 2070 6f70  n the source pop
+00013ab0: 756c 6174 696f 6e27 7320 5370 6563 6965  ulation's Specie
+00013ac0: 7320 616e 6420 7468 6973 2053 7065 6369  s and this Speci
+00013ad0: 6573 0a20 2020 2020 2020 2020 2020 2073  es.            s
+00013ae0: 6f75 7263 655f 6765 6e5f 6172 6368 203d  ource_gen_arch =
+00013af0: 2073 6f75 7263 655f 7370 702e 6765 6e5f   source_spp.gen_
+00013b00: 6172 6368 0a20 2020 2020 2020 2020 2020  arch.           
+00013b10: 2073 656c 662e 6765 6e5f 6172 6368 203d   self.gen_arch =
+00013b20: 2073 656c 662e 6765 6e5f 6172 6368 0a20   self.gen_arch. 
+00013b30: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00013b40: 7420 736f 7572 6365 5f67 656e 5f61 7263  t source_gen_arc
+00013b50: 682e 4c20 3d3d 2073 656c 662e 6765 6e5f  h.L == self.gen_
+00013b60: 6172 6368 2e4c 2c20 2822 736f 7572 6365  arch.L, ("source
+00013b70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
 00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ba0: 2020 2020 2273 696d 756c 6174 6564 2067      "simulated g
-00013bb0: 656e 6f6d 6520 6f66 2074 6865 2073 616d  enome of the sam
-00013bc0: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+00013ba0: 2253 7065 6369 6573 206d 7573 7420 6861  "Species must ha
+00013bb0: 7665 2061 2022 0a20 2020 2020 2020 2020  ve a ".         
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 2022 6c65 6e67 7468 2061 7320 7468 6520   "length as the 
-00013c00: 7265 6370 6965 6e74 2053 7065 6369 6573  recpient Species
-00013c10: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00013c20: 6765 6e5f 6172 6368 5f61 7474 7273 5f74  gen_arch_attrs_t
-00013c30: 6f5f 6368 6563 6b20 3d20 5b27 7365 7827  o_check = ['sex'
-00013c40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c60: 2020 2020 2020 2020 2027 7573 655f 7473           'use_ts
-00013c70: 6b69 7427 2c0a 2020 2020 2020 2020 2020  kit',.          
-00013c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c90: 2020 2020 2020 2020 2020 2020 2027 7827               'x'
-00013ca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00013cd0: 2020 2020 2020 2320 4e4f 5445 3a20 6e6f        # NOTE: no
-00013ce0: 7420 7265 7175 6972 696e 6720 7020 746f  t requiring p to
-00013cf0: 2062 6520 7361 6d65 2069 6e20 626f 7468   be same in both
-00013d00: 2070 6f70 756c 6174 696f 6e73 2066 6163   populations fac
-00013d10: 696c 6974 6174 6573 0a20 2020 2020 2020  ilitates.       
-00013d20: 2020 2020 2023 2020 2020 2020 2063 7265       #       cre
-00013d30: 6174 696e 6720 6c6f 6369 2074 6861 7420  ating loci that 
-00013d40: 6469 6666 6572 2069 6e20 7374 616e 6469  differ in standi
-00013d50: 6e67 2067 656e 6574 6963 2076 6172 6961  ng genetic varia
-00013d60: 7469 6f6e 2069 6e0a 2020 2020 2020 2020  tion in.        
-00013d70: 2020 2020 2320 2020 2020 2020 7468 6520      #       the 
-00013d80: 7477 6f20 706f 7075 6c61 7469 6f6e 732c  two populations,
-00013d90: 206f 7220 6576 656e 206c 6f63 6920 7468   or even loci th
-00013da0: 6174 2061 7265 2066 6978 6564 2064 6966  at are fixed dif
-00013db0: 6665 7265 6e74 6c79 0a20 2020 2020 2020  ferently.       
-00013dc0: 2020 2020 2023 2020 2020 2020 2069 6e20       #       in 
-00013dd0: 6f6e 6520 6f72 206d 6f72 6520 706f 7075  one or more popu
-00013de0: 6c61 7469 6f6e 730a 2020 2020 2020 2020  lations.        
-00013df0: 2020 2020 2320 4e4f 5445 3a20 6d61 6b69      # NOTE: maki
-00013e00: 6e67 2069 7420 736f 2074 6861 7420 6174  ng it so that at
-00013e10: 7472 7320 6c69 6b65 206d 7574 2072 6174  trs like mut rat
-00013e20: 652c 2064 6f6d 696e 616e 6365 2070 6172  e, dominance par
-00013e30: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
-00013e40: 2023 2020 2020 2020 2061 6e64 2074 6865   #       and the
-00013e50: 2061 7272 6179 7320 6f66 206e 6575 7472   arrays of neutr
-00013e60: 616c 2061 6e64 2064 656c 6574 206c 6f63  al and delet loc
-00013e70: 6920 6e65 6564 6e27 7420 6265 2074 6865  i needn't be the
-00013e80: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-00013e90: 2020 2020 2073 616d 6520 286d 7574 6174       same (mutat
-00013ea0: 6564 206c 6f63 6920 616c 6d6f 7374 2063  ed loci almost c
-00013eb0: 6572 7461 696e 6c79 2077 6f75 6c64 6e27  ertainly wouldn'
-00013ec0: 7420 6265 0a20 2020 2020 2020 2020 2020  t be.           
-00013ed0: 2023 2020 2020 2020 2069 6620 6e6f 6e2d   #       if non-
-00013ee0: 6e65 7574 7261 6c20 6d75 7461 7469 6f6e  neutral mutation
-00013ef0: 2068 6173 2062 6565 6e20 6861 7070 656e   has been happen
-00013f00: 696e 6720 696e 6465 7065 6e64 656e 746c  ing independentl
-00013f10: 7920 696e 0a20 2020 2020 2020 2020 2020  y in.           
-00013f20: 2023 2020 2020 2020 2062 6f74 6820 706f   #       both po
-00013f30: 7075 6c61 7469 6f6e 7329 2e20 6974 2069  pulations). it i
-00013f40: 736e 2774 2065 6e74 6972 656c 7920 7265  sn't entirely re
-00013f50: 616c 6973 7469 6320 746f 206d 6f64 656c  alistic to model
-00013f60: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
-00013f70: 2020 2320 2020 2020 2020 7468 6973 2077    #       this w
-00013f80: 6179 2c20 6275 7420 616c 736f 206e 6f74  ay, but also not
-00013f90: 2065 6e74 6972 656c 7920 756e 7265 616c   entirely unreal
-00013fa0: 6973 7469 6320 666f 7220 7468 6520 6d6f  istic for the mo
-00013fb0: 6465 6c20 746f 0a20 2020 2020 2020 2020  del to.         
-00013fc0: 2020 2023 2020 2020 2020 2062 6568 6176     #       behav
-00013fd0: 6520 7375 6368 2074 6861 7420 6c6f 6369  e such that loci
-00013fe0: 2074 6861 7420 7765 7265 206e 6575 7420   that were neut 
-00013ff0: 696e 2061 2070 6f70 756c 6174 696f 6e27  in a population'
-00014000: 7320 7072 696f 720a 2020 2020 2020 2020  s prior.        
-00014010: 2020 2020 2320 2020 2020 2020 656e 7669      #       envi
-00014020: 726f 6e6d 656e 7420 6172 6520 7375 6464  ronment are sudd
-00014030: 656e 6c79 206e 6f74 206e 6575 7472 616c  enly not neutral
-00014040: 2069 6e20 7468 6520 6e65 7720 656e 7669   in the new envi
-00014050: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
-00014060: 2020 2020 666f 7220 6174 7472 2069 6e20      for attr in 
-00014070: 6765 6e5f 6172 6368 5f61 7474 7273 5f74  gen_arch_attrs_t
-00014080: 6f5f 6368 6563 6b3a 0a20 2020 2020 2020  o_check:.       
-00014090: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000140a0: 6e70 2e61 6c6c 2867 6574 6174 7472 2873  np.all(getattr(s
-000140b0: 6f75 7263 655f 6765 6e5f 6172 6368 2c20  ource_gen_arch, 
-000140c0: 6174 7472 2920 3d3d 0a20 2020 2020 2020  attr) ==.       
-000140d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140e0: 2020 2020 2020 2067 6574 6174 7472 2873         getattr(s
-000140f0: 656c 662e 6765 6e5f 6172 6368 2c20 6174  elf.gen_arch, at
-00014100: 7472 2929 2c20 2822 626f 7468 2074 6865  tr)), ("both the
-00014110: 2073 6f75 7263 6522 0a20 2020 2020 2020   source".       
-00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 2020 2020 2020 2020 2020 2020 2022 2061               " a
-00014150: 6e64 2072 6563 6970 6965 6e74 2053 7065  nd recipient Spe
-00014160: 6369 6573 2720 220a 2020 2020 2020 2020  cies' ".        
+00013be0: 2020 2020 2273 696d 756c 6174 6564 2067      "simulated g
+00013bf0: 656e 6f6d 6520 6f66 2074 6865 2073 616d  enome of the sam
+00013c00: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 2022 6c65 6e67 7468 2061 7320 7468 6520   "length as the 
+00013c40: 7265 6370 6965 6e74 2053 7065 6369 6573  recpient Species
+00013c50: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00013c60: 6765 6e5f 6172 6368 5f61 7474 7273 5f74  gen_arch_attrs_t
+00013c70: 6f5f 6368 6563 6b20 3d20 5b27 7365 7827  o_check = ['sex'
+00013c80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ca0: 2020 2020 2020 2020 2027 7573 655f 7473           'use_ts
+00013cb0: 6b69 7427 2c0a 2020 2020 2020 2020 2020  kit',.          
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 2020 2020 2020 2020 2020 2020 2027 7827               'x'
+00013ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d00: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00013d10: 2020 2020 2020 2320 4e4f 5445 3a20 6e6f        # NOTE: no
+00013d20: 7420 7265 7175 6972 696e 6720 7020 746f  t requiring p to
+00013d30: 2062 6520 7361 6d65 2069 6e20 626f 7468   be same in both
+00013d40: 2070 6f70 756c 6174 696f 6e73 2066 6163   populations fac
+00013d50: 696c 6974 6174 6573 0a20 2020 2020 2020  ilitates.       
+00013d60: 2020 2020 2023 2020 2020 2020 2063 7265       #       cre
+00013d70: 6174 696e 6720 6c6f 6369 2074 6861 7420  ating loci that 
+00013d80: 6469 6666 6572 2069 6e20 7374 616e 6469  differ in standi
+00013d90: 6e67 2067 656e 6574 6963 2076 6172 6961  ng genetic varia
+00013da0: 7469 6f6e 2069 6e0a 2020 2020 2020 2020  tion in.        
+00013db0: 2020 2020 2320 2020 2020 2020 7468 6520      #       the 
+00013dc0: 7477 6f20 706f 7075 6c61 7469 6f6e 732c  two populations,
+00013dd0: 206f 7220 6576 656e 206c 6f63 6920 7468   or even loci th
+00013de0: 6174 2061 7265 2066 6978 6564 2064 6966  at are fixed dif
+00013df0: 6665 7265 6e74 6c79 0a20 2020 2020 2020  ferently.       
+00013e00: 2020 2020 2023 2020 2020 2020 2069 6e20       #       in 
+00013e10: 6f6e 6520 6f72 206d 6f72 6520 706f 7075  one or more popu
+00013e20: 6c61 7469 6f6e 730a 2020 2020 2020 2020  lations.        
+00013e30: 2020 2020 2320 4e4f 5445 3a20 6d61 6b69      # NOTE: maki
+00013e40: 6e67 2069 7420 736f 2074 6861 7420 6174  ng it so that at
+00013e50: 7472 7320 6c69 6b65 206d 7574 2072 6174  trs like mut rat
+00013e60: 652c 2064 6f6d 696e 616e 6365 2070 6172  e, dominance par
+00013e70: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
+00013e80: 2023 2020 2020 2020 2061 6e64 2074 6865   #       and the
+00013e90: 2061 7272 6179 7320 6f66 206e 6575 7472   arrays of neutr
+00013ea0: 616c 2061 6e64 2064 656c 6574 206c 6f63  al and delet loc
+00013eb0: 6920 6e65 6564 6e27 7420 6265 2074 6865  i needn't be the
+00013ec0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00013ed0: 2020 2020 2073 616d 6520 286d 7574 6174       same (mutat
+00013ee0: 6564 206c 6f63 6920 616c 6d6f 7374 2063  ed loci almost c
+00013ef0: 6572 7461 696e 6c79 2077 6f75 6c64 6e27  ertainly wouldn'
+00013f00: 7420 6265 0a20 2020 2020 2020 2020 2020  t be.           
+00013f10: 2023 2020 2020 2020 2069 6620 6e6f 6e2d   #       if non-
+00013f20: 6e65 7574 7261 6c20 6d75 7461 7469 6f6e  neutral mutation
+00013f30: 2068 6173 2062 6565 6e20 6861 7070 656e   has been happen
+00013f40: 696e 6720 696e 6465 7065 6e64 656e 746c  ing independentl
+00013f50: 7920 696e 0a20 2020 2020 2020 2020 2020  y in.           
+00013f60: 2023 2020 2020 2020 2062 6f74 6820 706f   #       both po
+00013f70: 7075 6c61 7469 6f6e 7329 2e20 6974 2069  pulations). it i
+00013f80: 736e 2774 2065 6e74 6972 656c 7920 7265  sn't entirely re
+00013f90: 616c 6973 7469 6320 746f 206d 6f64 656c  alistic to model
+00013fa0: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
+00013fb0: 2020 2320 2020 2020 2020 7468 6973 2077    #       this w
+00013fc0: 6179 2c20 6275 7420 616c 736f 206e 6f74  ay, but also not
+00013fd0: 2065 6e74 6972 656c 7920 756e 7265 616c   entirely unreal
+00013fe0: 6973 7469 6320 666f 7220 7468 6520 6d6f  istic for the mo
+00013ff0: 6465 6c20 746f 0a20 2020 2020 2020 2020  del to.         
+00014000: 2020 2023 2020 2020 2020 2062 6568 6176     #       behav
+00014010: 6520 7375 6368 2074 6861 7420 6c6f 6369  e such that loci
+00014020: 2074 6861 7420 7765 7265 206e 6575 7420   that were neut 
+00014030: 696e 2061 2070 6f70 756c 6174 696f 6e27  in a population'
+00014040: 7320 7072 696f 720a 2020 2020 2020 2020  s prior.        
+00014050: 2020 2020 2320 2020 2020 2020 656e 7669      #       envi
+00014060: 726f 6e6d 656e 7420 6172 6520 7375 6464  ronment are sudd
+00014070: 656e 6c79 206e 6f74 206e 6575 7472 616c  enly not neutral
+00014080: 2069 6e20 7468 6520 6e65 7720 656e 7669   in the new envi
+00014090: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
+000140a0: 2020 2020 666f 7220 6174 7472 2069 6e20      for attr in 
+000140b0: 6765 6e5f 6172 6368 5f61 7474 7273 5f74  gen_arch_attrs_t
+000140c0: 6f5f 6368 6563 6b3a 0a20 2020 2020 2020  o_check:.       
+000140d0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000140e0: 6e70 2e61 6c6c 2867 6574 6174 7472 2873  np.all(getattr(s
+000140f0: 6f75 7263 655f 6765 6e5f 6172 6368 2c20  ource_gen_arch, 
+00014100: 6174 7472 2920 3d3d 0a20 2020 2020 2020  attr) ==.       
+00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014120: 2020 2020 2020 2067 6574 6174 7472 2873         getattr(s
+00014130: 656c 662e 6765 6e5f 6172 6368 2c20 6174  elf.gen_arch, at
+00014140: 7472 2929 2c20 2822 626f 7468 2074 6865  tr)), ("both the
+00014150: 2073 6f75 7263 6522 0a20 2020 2020 2020   source".       
+00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014190: 2020 2020 2020 2020 2020 2020 2247 656e              "Gen
-000141a0: 6f6d 6963 4172 6368 6974 6563 7475 7265  omicArchitecture
-000141b0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+00014180: 2020 2020 2020 2020 2020 2020 2022 2061               " a
+00014190: 6e64 2072 6563 6970 6965 6e74 2053 7065  nd recipient Spe
+000141a0: 6369 6573 2720 220a 2020 2020 2020 2020  cies' ".        
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 2020 2020 2020 2020 226f 626a 6563 7473          "objects
-000141f0: 206d 7573 7420 6861 7665 2022 0a20 2020   must have ".   
+000141d0: 2020 2020 2020 2020 2020 2020 2247 656e              "Gen
+000141e0: 6f6d 6963 4172 6368 6974 6563 7475 7265  omicArchitecture
+000141f0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
 00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014230: 2022 6964 656e 7469 6361 6c20 7661 6c75   "identical valu
-00014240: 6573 2066 6f72 2074 6865 2022 0a20 2020  es for the ".   
+00014220: 2020 2020 2020 2020 226f 626a 6563 7473          "objects
+00014230: 206d 7573 7420 6861 7665 2022 0a20 2020   must have ".   
+00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 2066 2261 7474 7269 6275 7465 2027 7b61   f"attribute '{a
-00014290: 7474 727d 2722 290a 2020 2020 2020 2020  ttr}'").        
-000142a0: 2020 2020 2320 6368 6563 6b20 7265 636f      # check reco
-000142b0: 6d62 696e 6174 696f 6e20 6174 7472 6962  mbination attrib
-000142c0: 7574 6573 0a20 2020 2020 2020 2020 2020  utes.           
-000142d0: 2072 6563 6f6d 625f 6174 7472 735f 746f   recomb_attrs_to
-000142e0: 5f63 6865 636b 203d 205b 275f 7261 7465  _check = ['_rate
-000142f0: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014310: 2020 2020 2020 2020 2027 5f72 5f64 6973           '_r_dis
-00014320: 7472 5f61 6c70 6861 272c 0a20 2020 2020  tr_alpha',.     
-00014330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014270: 2022 6964 656e 7469 6361 6c20 7661 6c75   "identical valu
+00014280: 6573 2066 6f72 2074 6865 2022 0a20 2020  es for the ".   
+00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142c0: 2066 2261 7474 7269 6275 7465 2027 7b61   f"attribute '{a
+000142d0: 7474 727d 2722 290a 2020 2020 2020 2020  ttr}'").        
+000142e0: 2020 2020 2320 6368 6563 6b20 7265 636f      # check reco
+000142f0: 6d62 696e 6174 696f 6e20 6174 7472 6962  mbination attrib
+00014300: 7574 6573 0a20 2020 2020 2020 2020 2020  utes.           
+00014310: 2072 6563 6f6d 625f 6174 7472 735f 746f   recomb_attrs_to
+00014320: 5f63 6865 636b 203d 205b 275f 7261 7465  _check = ['_rate
+00014330: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
 00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 275f 725f 6469 7374 725f 6265 7461 272c  '_r_distr_beta',
-00014360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014350: 2020 2020 2020 2020 2027 5f72 5f64 6973           '_r_dis
+00014360: 7472 5f61 6c70 6861 272c 0a20 2020 2020  tr_alpha',.     
 00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014380: 2020 2020 2020 275f 6a69 7474 6572 5f62        '_jitter_b
-00014390: 7265 616b 706f 696e 7473 272c 0a20 2020  reakpoints',.   
-000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014390: 275f 725f 6469 7374 725f 6265 7461 272c  '_r_distr_beta',
+000143a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000143b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143c0: 205d 0a20 2020 2020 2020 2020 2020 2066   ].            f
-000143d0: 6f72 2061 7474 7220 696e 2072 6563 6f6d  or attr in recom
-000143e0: 625f 6174 7472 735f 746f 5f63 6865 636b  b_attrs_to_check
-000143f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014400: 2020 6173 7365 7274 206e 702e 616c 6c28    assert np.all(
-00014410: 6765 7461 7474 7228 736f 7572 6365 5f67  getattr(source_g
-00014420: 656e 5f61 7263 682e 7265 636f 6d62 696e  en_arch.recombin
-00014430: 6174 696f 6e73 2c20 6174 7472 2920 3d3d  ations, attr) ==
-00014440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014450: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00014460: 6574 6174 7472 2873 656c 662e 6765 6e5f  etattr(self.gen_
-00014470: 6172 6368 2e72 6563 6f6d 6269 6e61 7469  arch.recombinati
-00014480: 6f6e 732c 2061 7474 7229 292c 2028 0a20  ons, attr)), (. 
-00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144c0: 2020 2020 2262 6f74 6820 7468 6520 736f      "both the so
-000144d0: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+000143c0: 2020 2020 2020 275f 6a69 7474 6572 5f62        '_jitter_b
+000143d0: 7265 616b 706f 696e 7473 272c 0a20 2020  reakpoints',.   
+000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014400: 205d 0a20 2020 2020 2020 2020 2020 2066   ].            f
+00014410: 6f72 2061 7474 7220 696e 2072 6563 6f6d  or attr in recom
+00014420: 625f 6174 7472 735f 746f 5f63 6865 636b  b_attrs_to_check
+00014430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014440: 2020 6173 7365 7274 206e 702e 616c 6c28    assert np.all(
+00014450: 6765 7461 7474 7228 736f 7572 6365 5f67  getattr(source_g
+00014460: 656e 5f61 7263 682e 7265 636f 6d62 696e  en_arch.recombin
+00014470: 6174 696f 6e73 2c20 6174 7472 2920 3d3d  ations, attr) ==
+00014480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014490: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+000144a0: 6574 6174 7472 2873 656c 662e 6765 6e5f  etattr(self.gen_
+000144b0: 6172 6368 2e72 6563 6f6d 6269 6e61 7469  arch.recombinati
+000144c0: 6f6e 732c 2061 7474 7229 292c 2028 0a20  ons, attr)), (. 
+000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014500: 2020 2020 2020 2020 2020 2020 2261 6e64              "and
-00014510: 2072 6563 6970 6965 6e74 2053 7065 6369   recipient Speci
-00014520: 6573 2720 220a 2020 2020 2020 2020 2020  es' ".          
+00014500: 2020 2020 2262 6f74 6820 7468 6520 736f      "both the so
+00014510: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014550: 2020 2020 2020 2020 2020 2022 5265 636f             "Reco
-00014560: 6d62 696e 6174 696f 6e73 206f 626a 6563  mbinations objec
-00014570: 7473 2022 0a20 2020 2020 2020 2020 2020  ts ".           
+00014540: 2020 2020 2020 2020 2020 2020 2261 6e64              "and
+00014550: 2072 6563 6970 6965 6e74 2053 7065 6369   recipient Speci
+00014560: 6573 2720 220a 2020 2020 2020 2020 2020  es' ".          
+00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145a0: 2020 2020 2020 2020 2020 226d 7573 7420            "must 
-000145b0: 6861 7665 2069 6465 6e74 6963 616c 2022  have identical "
-000145c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014590: 2020 2020 2020 2020 2020 2022 5265 636f             "Reco
+000145a0: 6d62 696e 6174 696f 6e73 206f 626a 6563  mbinations objec
+000145b0: 7473 2022 0a20 2020 2020 2020 2020 2020  ts ".           
+000145c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145f0: 2020 2020 2020 2276 616c 7565 7320 666f        "values fo
-00014600: 7220 7468 6520 220a 2020 2020 2020 2020  r the ".        
+000145e0: 2020 2020 2020 2020 2020 226d 7573 7420            "must 
+000145f0: 6861 7665 2069 6465 6e74 6963 616c 2022  have identical "
+00014600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00014610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014630: 2020 2020 2020 2020 2020 2020 2066 2261               f"a
-00014640: 7474 7269 6275 7465 2027 7b61 7474 727d  ttribute '{attr}
-00014650: 2722 290a 0a20 2020 2020 2020 2020 2020  '")..           
-00014660: 2023 2063 6865 636b 2074 7261 6974 7320   # check traits 
-00014670: 616e 6420 7468 6569 7220 7061 7261 6d73  and their params
-00014680: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014690: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
-000146a0: 6169 7473 2069 7320 4e6f 6e65 3a0a 2020  aits is None:.  
-000146b0: 2020 2020 2020 2020 2020 2020 2020 6173                as
-000146c0: 7365 7274 2073 6f75 7263 655f 6765 6e5f  sert source_gen_
-000146d0: 6172 6368 2e74 7261 6974 7320 6973 204e  arch.traits is N
-000146e0: 6f6e 652c 2028 2249 6e64 6976 6964 7561  one, ("Individua
-000146f0: 6c73 2022 0a20 2020 2020 2020 2020 2020  ls ".           
-00014700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 2020 2020 2022 6672 6f6d 2061 2053         "from a S
-00014730: 7065 6369 6573 2077 6974 6820 220a 2020  pecies with ".  
+00014630: 2020 2020 2020 2276 616c 7565 7320 666f        "values fo
+00014640: 7220 7468 6520 220a 2020 2020 2020 2020  r the ".        
+00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014670: 2020 2020 2020 2020 2020 2020 2066 2261               f"a
+00014680: 7474 7269 6275 7465 2027 7b61 7474 727d  ttribute '{attr}
+00014690: 2722 290a 0a20 2020 2020 2020 2020 2020  '")..           
+000146a0: 2023 2063 6865 636b 2074 7261 6974 7320   # check traits 
+000146b0: 616e 6420 7468 6569 7220 7061 7261 6d73  and their params
+000146c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000146d0: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
+000146e0: 6169 7473 2069 7320 4e6f 6e65 3a0a 2020  aits is None:.  
+000146f0: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00014700: 7365 7274 2073 6f75 7263 655f 6765 6e5f  sert source_gen_
+00014710: 6172 6368 2e74 7261 6974 7320 6973 204e  arch.traits is N
+00014720: 6f6e 652c 2028 2249 6e64 6976 6964 7561  one, ("Individua
+00014730: 6c73 2022 0a20 2020 2020 2020 2020 2020  ls ".           
 00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014770: 2254 7261 6974 7320 6361 6e6e 6f74 2062  "Traits cannot b
-00014780: 6520 6164 6465 6420 746f 2061 2022 0a20  e added to a ". 
+00014760: 2020 2020 2020 2022 6672 6f6d 2061 2053         "from a S
+00014770: 7065 6369 6573 2077 6974 6820 220a 2020  pecies with ".  
+00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147c0: 2022 5370 6563 6965 7320 7769 7468 6f75   "Species withou
-000147d0: 7420 7468 656d 2e22 290a 2020 2020 2020  t them.").      
-000147e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000147f0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00014800: 7274 2028 6c65 6e28 736f 7572 6365 5f67  rt (len(source_g
-00014810: 656e 5f61 7263 682e 7472 6169 7473 2920  en_arch.traits) 
-00014820: 3d3d 0a20 2020 2020 2020 2020 2020 2020  ==.             
-00014830: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-00014840: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
-00014850: 6974 7329 292c 2028 2254 6865 2073 6f75  its)), ("The sou
-00014860: 7263 6520 706f 7075 6c61 7469 6f6e 2773  rce population's
-00014870: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00014880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014890: 2020 2020 2020 2020 2020 2022 5370 6563             "Spec
-000148a0: 6965 7320 6f62 6a65 6374 206d 7573 7420  ies object must 
-000148b0: 6861 7665 2074 6865 2022 0a20 2020 2020  have the ".     
+000147b0: 2254 7261 6974 7320 6361 6e6e 6f74 2062  "Traits cannot b
+000147c0: 6520 6164 6465 6420 746f 2061 2022 0a20  e added to a ". 
+000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014800: 2022 5370 6563 6965 7320 7769 7468 6f75   "Species withou
+00014810: 7420 7468 656d 2e22 290a 2020 2020 2020  t them.").      
+00014820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00014830: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00014840: 7274 2028 6c65 6e28 736f 7572 6365 5f67  rt (len(source_g
+00014850: 656e 5f61 7263 682e 7472 6169 7473 2920  en_arch.traits) 
+00014860: 3d3d 0a20 2020 2020 2020 2020 2020 2020  ==.             
+00014870: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
+00014880: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
+00014890: 6974 7329 292c 2028 2254 6865 2073 6f75  its)), ("The sou
+000148a0: 7263 6520 706f 7075 6c61 7469 6f6e 2773  rce population's
+000148b0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
 000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 2020 2022 7361 6d65 206e 756d 6265 7220     "same number 
-000148f0: 6f66 2054 7261 6974 7320 220a 2020 2020  of Traits ".    
+000148d0: 2020 2020 2020 2020 2020 2022 5370 6563             "Spec
+000148e0: 6965 7320 6f62 6a65 6374 206d 7573 7420  ies object must 
+000148f0: 6861 7665 2074 6865 2022 0a20 2020 2020  have the ".     
 00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014920: 2020 2020 2261 7320 7468 6520 7265 6369      "as the reci
-00014930: 7069 656e 7420 5370 6563 6965 732e 2229  pient Species.")
-00014940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014950: 2074 7274 5f61 7474 7273 5f74 6f5f 6368   trt_attrs_to_ch
-00014960: 6563 6b20 3d20 5b27 6e61 6d65 272c 0a20  eck = ['name',. 
-00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014990: 2020 2020 2027 7068 6927 2c0a 2020 2020       'phi',.    
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014920: 2020 2022 7361 6d65 206e 756d 6265 7220     "same number 
+00014930: 6f66 2054 7261 6974 7320 220a 2020 2020  of Traits ".    
+00014940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 2261 7320 7468 6520 7265 6369      "as the reci
+00014970: 7069 656e 7420 5370 6563 6965 732e 2229  pient Species.")
+00014980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014990: 2074 7274 5f61 7474 7273 5f74 6f5f 6368   trt_attrs_to_ch
+000149a0: 6563 6b20 3d20 5b27 6e61 6d65 272c 0a20  eck = ['name',. 
 000149b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149c0: 2020 276c 7972 5f6e 756d 272c 0a20 2020    'lyr_num',.   
-000149d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149d0: 2020 2020 2027 7068 6927 2c0a 2020 2020       'phi',.    
 000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149f0: 2020 2027 6d61 785f 616c 7068 615f 6d61     'max_alpha_ma
-00014a00: 6727 2c0a 2020 2020 2020 2020 2020 2020  g',.            
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a00: 2020 276c 7972 5f6e 756d 272c 0a20 2020    'lyr_num',.   
 00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a20: 2020 2020 2020 2020 2020 2767 616d 6d61            'gamma
-00014a30: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a50: 2020 2020 2020 2020 2027 756e 6976 5f61           'univ_a
-00014a60: 6476 272c 0a20 2020 2020 2020 2020 2020  dv',.           
-00014a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a80: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00014a90: 2020 2020 2020 2020 2020 2020 2320 4e4f              # NO
-00014aa0: 5445 3a20 6e6f 7420 7265 7175 6972 696e  TE: not requirin
-00014ab0: 6720 276e 5f6c 6f63 6927 2074 6f20 6265  g 'n_loci' to be
-00014ac0: 2074 6865 2073 616d 6520 6265 6361 7573   the same becaus
-00014ad0: 6520 7468 6579 2772 650a 2020 2020 2020  e they're.      
-00014ae0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00014af0: 2020 756e 6c69 6b65 6c79 2074 6f20 6265    unlikely to be
-00014b00: 2074 6865 2073 616d 6520 6966 206e 6f6e   the same if non
-00014b10: 2d6e 6575 7472 616c 206d 7574 6174 696f  -neutral mutatio
-00014b20: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
-00014b30: 2020 2023 2020 2020 2020 2068 6173 2062     #       has b
-00014b40: 6565 6e20 6861 7070 656e 696e 6720 696e  een happening in
-00014b50: 6465 7065 6e64 656e 746c 7920 696e 2062  dependently in b
-00014b60: 6f74 6820 706f 7075 6c61 7469 6f6e 730a  oth populations.
-00014b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b80: 666f 7220 6e2c 2074 7274 2069 6e20 7365  for n, trt in se
-00014b90: 6c66 2e67 656e 5f61 7263 682e 7472 6169  lf.gen_arch.trai
-00014ba0: 7473 2e69 7465 6d73 2829 3a0a 2020 2020  ts.items():.    
+00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a30: 2020 2027 6d61 785f 616c 7068 615f 6d61     'max_alpha_ma
+00014a40: 6727 2c0a 2020 2020 2020 2020 2020 2020  g',.            
+00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a60: 2020 2020 2020 2020 2020 2767 616d 6d61            'gamma
+00014a70: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a90: 2020 2020 2020 2020 2027 756e 6976 5f61           'univ_a
+00014aa0: 6476 272c 0a20 2020 2020 2020 2020 2020  dv',.           
+00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ac0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00014ad0: 2020 2020 2020 2020 2020 2020 2320 4e4f              # NO
+00014ae0: 5445 3a20 6e6f 7420 7265 7175 6972 696e  TE: not requirin
+00014af0: 6720 276e 5f6c 6f63 6927 2074 6f20 6265  g 'n_loci' to be
+00014b00: 2074 6865 2073 616d 6520 6265 6361 7573   the same becaus
+00014b10: 6520 7468 6579 2772 650a 2020 2020 2020  e they're.      
+00014b20: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00014b30: 2020 756e 6c69 6b65 6c79 2074 6f20 6265    unlikely to be
+00014b40: 2074 6865 2073 616d 6520 6966 206e 6f6e   the same if non
+00014b50: 2d6e 6575 7472 616c 206d 7574 6174 696f  -neutral mutatio
+00014b60: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
+00014b70: 2020 2023 2020 2020 2020 2068 6173 2062     #       has b
+00014b80: 6565 6e20 6861 7070 656e 696e 6720 696e  een happening in
+00014b90: 6465 7065 6e64 656e 746c 7920 696e 2062  dependently in b
+00014ba0: 6f74 6820 706f 7075 6c61 7469 6f6e 730a  oth populations.
 00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bc0: 666f 7220 6174 7472 2069 6e20 7472 745f  for attr in trt_
-00014bd0: 6174 7473 5f74 6f5f 6368 6563 6b3a 0a20  atts_to_check:. 
-00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bf0: 2020 2020 2020 2061 7373 6572 7420 6e70         assert np
-00014c00: 2e61 6c6c 2867 6574 6174 7472 2874 7274  .all(getattr(trt
-00014c10: 2c20 6174 7472 2920 3d3d 0a20 2020 2020  , attr) ==.     
+00014bc0: 666f 7220 6e2c 2074 7274 2069 6e20 7365  for n, trt in se
+00014bd0: 6c66 2e67 656e 5f61 7263 682e 7472 6169  lf.gen_arch.trai
+00014be0: 7473 2e69 7465 6d73 2829 3a0a 2020 2020  ts.items():.    
+00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c00: 666f 7220 6174 7472 2069 6e20 7472 745f  for attr in trt_
+00014c10: 6174 7473 5f74 6f5f 6368 6563 6b3a 0a20  atts_to_check:. 
 00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c30: 2020 2020 2020 2020 2020 2067 6574 6174             getat
-00014c40: 7472 2873 6f75 7263 655f 6765 6e5f 6172  tr(source_gen_ar
-00014c50: 6368 2e74 7261 6974 735b 6e5d 2c20 6174  ch.traits[n], at
-00014c60: 7472 2929 2c20 280a 2020 2020 2020 2020  tr)), (.        
-00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c90: 2066 2241 7474 7269 6275 7465 2027 7b61   f"Attribute '{a
-00014ca0: 7474 727d 2720 6f66 2074 7261 6974 207b  ttr}' of trait {
-00014cb0: 6e7d 2022 0a20 2020 2020 2020 2020 2020  n} ".           
+00014c30: 2020 2020 2020 2061 7373 6572 7420 6e70         assert np
+00014c40: 2e61 6c6c 2867 6574 6174 7472 2874 7274  .all(getattr(trt
+00014c50: 2c20 6174 7472 2920 3d3d 0a20 2020 2020  , attr) ==.     
+00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c70: 2020 2020 2020 2020 2020 2067 6574 6174             getat
+00014c80: 7472 2873 6f75 7263 655f 6765 6e5f 6172  tr(source_gen_ar
+00014c90: 6368 2e74 7261 6974 735b 6e5d 2c20 6174  ch.traits[n], at
+00014ca0: 7472 2929 2c20 280a 2020 2020 2020 2020  tr)), (.        
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014ce0: 696e 2074 6865 2073 6f75 7263 6520 706f  in the source po
-00014cf0: 7075 6c61 7469 6f6e 2773 2053 7065 6369  pulation's Speci
-00014d00: 6573 2022 0a20 2020 2020 2020 2020 2020  es ".           
-00014d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014d30: 6f62 6a65 6374 206d 7573 7420 6265 2074  object must be t
-00014d40: 6865 2073 616d 6520 6173 2022 0a20 2020  he same as ".   
+00014cd0: 2066 2241 7474 7269 6275 7465 2027 7b61   f"Attribute '{a
+00014ce0: 7474 727d 2720 6f66 2074 7261 6974 207b  ttr}' of trait {
+00014cf0: 6e7d 2022 0a20 2020 2020 2020 2020 2020  n} ".           
+00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014d20: 696e 2074 6865 2073 6f75 7263 6520 706f  in the source po
+00014d30: 7075 6c61 7469 6f6e 2773 2053 7065 6369  pulation's Speci
+00014d40: 6573 2022 0a20 2020 2020 2020 2020 2020  es ".           
 00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d70: 2020 2020 2020 2022 7468 6174 2061 7474         "that att
-00014d80: 7269 6275 7465 2069 6e20 7468 6520 7265  ribute in the re
-00014d90: 6369 7069 656e 7420 220a 2020 2020 2020  cipient ".      
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014d70: 6f62 6a65 6374 206d 7573 7420 6265 2074  object must be t
+00014d80: 6865 2073 616d 6520 6173 2022 0a20 2020  he same as ".   
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014dc0: 2020 2020 2270 6f70 756c 6174 696f 6e27      "population'
-00014dd0: 7320 5370 6563 6965 732e 2229 0a0a 2020  s Species.")..  
-00014de0: 2020 2020 2020 2020 2020 2320 6465 6570            # deep
-00014df0: 636f 7079 2074 6865 2073 6f75 7263 655f  copy the source_
-00014e00: 7370 7020 6f62 6a65 6374 2c20 7468 656e  spp object, then
-00014e10: 2073 7562 7365 7420 746f 206f 6e6c 7920   subset to only 
-00014e20: 7468 6520 736f 7572 6365 0a20 2020 2020  the source.     
-00014e30: 2020 2020 2020 2023 2069 6e64 6976 6964         # individ
-00014e40: 7561 6c73 206e 6565 6465 642c 2077 6869  uals needed, whi
-00014e50: 6368 2077 696c 6c20 616c 736f 2073 6f72  ch will also sor
-00014e60: 7420 616e 6420 7369 6d70 6c69 6679 2074  t and simplify t
-00014e70: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
-00014e80: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00014e90: 2073 6f20 7468 6174 2061 6c6c 2065 7874   so that all ext
-00014ea0: 616e 7420 6e6f 6465 7320 6172 6520 6e6f  ant nodes are no
-00014eb0: 6465 7320 746f 2062 6520 756e 696f 6e65  des to be unione
-00014ec0: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
-00014ed0: 696e 746f 2074 6869 7320 5370 6563 6965  into this Specie
-00014ee0: 7327 2054 6162 6c65 436f 6c6c 6563 7469  s' TableCollecti
-00014ef0: 6f6e 200a 2020 2020 2020 2020 2020 2020  on .            
-00014f00: 736f 7572 6365 5f73 7070 5f63 6f70 7920  source_spp_copy 
-00014f10: 3d20 6465 6570 636f 7079 2873 6f75 7263  = deepcopy(sourc
-00014f20: 655f 7370 7029 0a20 2020 2020 2020 2020  e_spp).         
-00014f30: 2020 2023 2067 6574 2069 6e64 6976 6964     # get individ
-00014f40: 7561 6c73 2066 726f 6d20 7468 6520 6769  uals from the gi
-00014f50: 7665 6e20 5370 6563 6965 7320 6f62 6a65  ven Species obje
-00014f60: 6374 0a20 2020 2020 2020 2020 2020 2069  ct.            i
-00014f70: 6620 696e 6469 7669 6473 2069 7320 6e6f  f individs is no
-00014f80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014f90: 2020 2020 2020 2020 696e 6469 7669 6473          individs
-00014fa0: 5f74 6f5f 7265 6d6f 7665 203d 205b 696e  _to_remove = [in
-00014fb0: 6420 666f 7220 696e 6420 696e 0a20 2020  d for ind in.   
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fe0: 2020 2073 6f75 7263 655f 7370 705f 636f     source_spp_co
-00014ff0: 7079 2069 6620 696e 6420 6e6f 7420 696e  py if ind not in
-00015000: 2069 6e64 6976 6964 735d 0a20 2020 2020   individs].     
-00015010: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00015020: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-00015030: 6976 6964 735f 746f 5f72 656d 6f76 6520  ivids_to_remove 
-00015040: 3d20 5b2a 736f 7572 6365 5f73 7070 5f63  = [*source_spp_c
-00015050: 6f70 795d 5b6e 3a5d 0a20 2020 2020 2020  opy][n:].       
-00015060: 2020 2020 2073 6f75 7263 655f 7370 705f       source_spp_
-00015070: 636f 7079 2e5f 7265 6d6f 7665 5f69 6e64  copy._remove_ind
-00015080: 6976 6964 7561 6c73 2869 6e64 6976 6964  ividuals(individ
-00015090: 733d 696e 6469 7669 6473 5f74 6f5f 7265  s=individs_to_re
-000150a0: 6d6f 7665 290a 2020 2020 2020 2020 2020  move).          
-000150b0: 2020 6966 2069 6e64 6976 6964 7320 6973    if individs is
-000150c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000150d0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-000150e0: 7420 6c65 6e28 736f 7572 6365 5f73 7070  t len(source_spp
-000150f0: 5f63 6f70 7929 203d 3d20 6c65 6e28 696e  _copy) == len(in
-00015100: 6469 7669 6473 290a 2020 2020 2020 2020  divids).        
-00015110: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015120: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00015130: 206c 656e 2873 6f75 7263 655f 7370 705f   len(source_spp_
-00015140: 636f 7079 2920 3d3d 206e 0a0a 2020 2020  copy) == n..    
-00015150: 2020 2020 2020 2020 2320 6761 7468 6572          # gather
-00015160: 2061 6c6c 2072 656d 6169 6e69 6e67 2049   all remaining I
-00015170: 6e64 6976 6964 7561 6c73 2069 6e74 6f20  ndividuals into 
-00015180: 6120 6c69 7374 0a20 2020 2020 2020 2020  a list.         
-00015190: 2020 2069 6e64 6976 6964 7320 3d20 5b2a     individs = [*
-000151a0: 736f 7572 6365 5f73 7070 5f63 6f70 792e  source_spp_copy.
-000151b0: 7661 6c75 6573 2829 5d0a 0a20 2020 2020  values()]..     
-000151c0: 2020 2020 2020 2023 2064 6f75 626c 652d         # double-
-000151d0: 6368 6563 6b20 7468 6174 2074 6865 2073  check that the s
-000151e0: 6f75 7263 655f 7370 705f 636f 7079 2773  ource_spp_copy's
-000151f0: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00015200: 2068 6173 2062 6565 6e0a 2020 2020 2020   has been.      
-00015210: 2020 2020 2020 2320 736f 7274 6564 2061        # sorted a
-00015220: 6e64 2073 696d 706c 6966 6965 640a 2020  nd simplified.  
-00015230: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00015240: 5f73 7070 5f63 6f70 792e 5f73 6f72 745f  _spp_copy._sort_
-00015250: 616e 645f 7369 6d70 6c69 6679 5f74 6162  and_simplify_tab
-00015260: 6c65 5f63 6f6c 6c65 6374 696f 6e28 290a  le_collection().
-00015270: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
-00015280: 6f72 6d61 7420 5461 626c 6543 6f6c 6c65  ormat TableColle
-00015290: 6374 696f 6e20 616e 6420 7265 7475 726e  ction and return
-000152a0: 2074 6865 206c 6973 7420 6f66 206e 6577   the list of new
-000152b0: 2067 6e78 2049 6e64 6976 6964 2069 6478   gnx Individ idx
-000152c0: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-000152d0: 7468 6174 2054 6162 6c65 2773 2069 6e64  that Table's ind
-000152e0: 6976 6964 7561 6c73 2077 696c 6c20 6265  ividuals will be
-000152f0: 2061 7373 6967 6e65 6420 772f 696e 2074   assigned w/in t
-00015300: 6869 7320 5370 6563 6965 730a 2020 2020  his Species.    
-00015310: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
-00015320: 6320 3d20 736f 7572 6365 5f73 7070 5f63  c = source_spp_c
-00015330: 6f70 792e 5f74 630a 2020 2020 2020 2020  opy._tc.        
-00015340: 2020 2020 6e65 7874 5f67 6e78 5f69 6478      next_gnx_idx
-00015350: 7320 3d20 5f70 7265 705f 7473 6b69 745f  s = _prep_tskit_
-00015360: 7461 6263 6f6c 6c5f 666f 725f 676e 785f  tabcoll_for_gnx_
-00015370: 7370 705f 756e 696f 6e28 7463 3d73 6f75  spp_union(tc=sou
-00015380: 7263 655f 7463 2c0a 2020 2020 2020 2020  rce_tc,.        
-00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153c0: 7265 6369 705f 7370 703d 7365 6c66 2c0a  recip_spp=self,.
+00014db0: 2020 2020 2020 2022 7468 6174 2061 7474         "that att
+00014dc0: 7269 6275 7465 2069 6e20 7468 6520 7265  ribute in the re
+00014dd0: 6369 7069 656e 7420 220a 2020 2020 2020  cipient ".      
+00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e00: 2020 2020 2270 6f70 756c 6174 696f 6e27      "population'
+00014e10: 7320 5370 6563 6965 732e 2229 0a0a 2020  s Species.")..  
+00014e20: 2020 2020 2020 2020 2020 2320 6465 6570            # deep
+00014e30: 636f 7079 2074 6865 2073 6f75 7263 655f  copy the source_
+00014e40: 7370 7020 6f62 6a65 6374 2c20 7468 656e  spp object, then
+00014e50: 2073 7562 7365 7420 746f 206f 6e6c 7920   subset to only 
+00014e60: 7468 6520 736f 7572 6365 0a20 2020 2020  the source.     
+00014e70: 2020 2020 2020 2023 2069 6e64 6976 6964         # individ
+00014e80: 7561 6c73 206e 6565 6465 642c 2077 6869  uals needed, whi
+00014e90: 6368 2077 696c 6c20 616c 736f 2073 6f72  ch will also sor
+00014ea0: 7420 616e 6420 7369 6d70 6c69 6679 2074  t and simplify t
+00014eb0: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
+00014ec0: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
+00014ed0: 2073 6f20 7468 6174 2061 6c6c 2065 7874   so that all ext
+00014ee0: 616e 7420 6e6f 6465 7320 6172 6520 6e6f  ant nodes are no
+00014ef0: 6465 7320 746f 2062 6520 756e 696f 6e65  des to be unione
+00014f00: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
+00014f10: 696e 746f 2074 6869 7320 5370 6563 6965  into this Specie
+00014f20: 7327 2054 6162 6c65 436f 6c6c 6563 7469  s' TableCollecti
+00014f30: 6f6e 200a 2020 2020 2020 2020 2020 2020  on .            
+00014f40: 736f 7572 6365 5f73 7070 5f63 6f70 7920  source_spp_copy 
+00014f50: 3d20 6465 6570 636f 7079 2873 6f75 7263  = deepcopy(sourc
+00014f60: 655f 7370 7029 0a20 2020 2020 2020 2020  e_spp).         
+00014f70: 2020 2023 2067 6574 2069 6e64 6976 6964     # get individ
+00014f80: 7561 6c73 2066 726f 6d20 7468 6520 6769  uals from the gi
+00014f90: 7665 6e20 5370 6563 6965 7320 6f62 6a65  ven Species obje
+00014fa0: 6374 0a20 2020 2020 2020 2020 2020 2069  ct.            i
+00014fb0: 6620 696e 6469 7669 6473 2069 7320 6e6f  f individs is no
+00014fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00014fd0: 2020 2020 2020 2020 696e 6469 7669 6473          individs
+00014fe0: 5f74 6f5f 7265 6d6f 7665 203d 205b 696e  _to_remove = [in
+00014ff0: 6420 666f 7220 696e 6420 696e 0a20 2020  d for ind in.   
+00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015020: 2020 2073 6f75 7263 655f 7370 705f 636f     source_spp_co
+00015030: 7079 2069 6620 696e 6420 6e6f 7420 696e  py if ind not in
+00015040: 2069 6e64 6976 6964 735d 0a20 2020 2020   individs].     
+00015050: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00015060: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00015070: 6976 6964 735f 746f 5f72 656d 6f76 6520  ivids_to_remove 
+00015080: 3d20 5b2a 736f 7572 6365 5f73 7070 5f63  = [*source_spp_c
+00015090: 6f70 795d 5b6e 3a5d 0a20 2020 2020 2020  opy][n:].       
+000150a0: 2020 2020 2073 6f75 7263 655f 7370 705f       source_spp_
+000150b0: 636f 7079 2e5f 7265 6d6f 7665 5f69 6e64  copy._remove_ind
+000150c0: 6976 6964 7561 6c73 2869 6e64 6976 6964  ividuals(individ
+000150d0: 733d 696e 6469 7669 6473 5f74 6f5f 7265  s=individs_to_re
+000150e0: 6d6f 7665 290a 2020 2020 2020 2020 2020  move).          
+000150f0: 2020 6966 2069 6e64 6976 6964 7320 6973    if individs is
+00015100: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00015110: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00015120: 7420 6c65 6e28 736f 7572 6365 5f73 7070  t len(source_spp
+00015130: 5f63 6f70 7929 203d 3d20 6c65 6e28 696e  _copy) == len(in
+00015140: 6469 7669 6473 290a 2020 2020 2020 2020  divids).        
+00015150: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00015160: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00015170: 206c 656e 2873 6f75 7263 655f 7370 705f   len(source_spp_
+00015180: 636f 7079 2920 3d3d 206e 0a0a 2020 2020  copy) == n..    
+00015190: 2020 2020 2020 2020 2320 6761 7468 6572          # gather
+000151a0: 2061 6c6c 2072 656d 6169 6e69 6e67 2049   all remaining I
+000151b0: 6e64 6976 6964 7561 6c73 2069 6e74 6f20  ndividuals into 
+000151c0: 6120 6c69 7374 0a20 2020 2020 2020 2020  a list.         
+000151d0: 2020 2069 6e64 6976 6964 7320 3d20 5b2a     individs = [*
+000151e0: 736f 7572 6365 5f73 7070 5f63 6f70 792e  source_spp_copy.
+000151f0: 7661 6c75 6573 2829 5d0a 0a20 2020 2020  values()]..     
+00015200: 2020 2020 2020 2023 2064 6f75 626c 652d         # double-
+00015210: 6368 6563 6b20 7468 6174 2074 6865 2073  check that the s
+00015220: 6f75 7263 655f 7370 705f 636f 7079 2773  ource_spp_copy's
+00015230: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
+00015240: 2068 6173 2062 6565 6e0a 2020 2020 2020   has been.      
+00015250: 2020 2020 2020 2320 736f 7274 6564 2061        # sorted a
+00015260: 6e64 2073 696d 706c 6966 6965 640a 2020  nd simplified.  
+00015270: 2020 2020 2020 2020 2020 736f 7572 6365            source
+00015280: 5f73 7070 5f63 6f70 792e 5f73 6f72 745f  _spp_copy._sort_
+00015290: 616e 645f 7369 6d70 6c69 6679 5f74 6162  and_simplify_tab
+000152a0: 6c65 5f63 6f6c 6c65 6374 696f 6e28 290a  le_collection().
+000152b0: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
+000152c0: 6f72 6d61 7420 5461 626c 6543 6f6c 6c65  ormat TableColle
+000152d0: 6374 696f 6e20 616e 6420 7265 7475 726e  ction and return
+000152e0: 2074 6865 206c 6973 7420 6f66 206e 6577   the list of new
+000152f0: 2067 6e78 2049 6e64 6976 6964 2069 6478   gnx Individ idx
+00015300: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
+00015310: 7468 6174 2054 6162 6c65 2773 2069 6e64  that Table's ind
+00015320: 6976 6964 7561 6c73 2077 696c 6c20 6265  ividuals will be
+00015330: 2061 7373 6967 6e65 6420 772f 696e 2074   assigned w/in t
+00015340: 6869 7320 5370 6563 6965 730a 2020 2020  his Species.    
+00015350: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
+00015360: 6320 3d20 736f 7572 6365 5f73 7070 5f63  c = source_spp_c
+00015370: 6f70 792e 5f74 630a 2020 2020 2020 2020  opy._tc.        
+00015380: 2020 2020 6e65 7874 5f67 6e78 5f69 6478      next_gnx_idx
+00015390: 7320 3d20 5f70 7265 705f 7473 6b69 745f  s = _prep_tskit_
+000153a0: 7461 6263 6f6c 6c5f 666f 725f 676e 785f  tabcoll_for_gnx_
+000153b0: 7370 705f 756e 696f 6e28 7463 3d73 6f75  spp_union(tc=sou
+000153c0: 7263 655f 7463 2c0a 2020 2020 2020 2020  rce_tc,.        
 000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000153e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 2020 2020 2020 2020 636f 6f72 6473 3d63          coords=c
-00015410: 6f6f 7264 732c 0a20 2020 2020 2020 2020  oords,.         
+00015400: 7265 6369 705f 7370 703d 7365 6c66 2c0a  recip_spp=self,.
+00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015450: 6f75 7263 655f 736f 6674 7761 7265 3d27  ource_software='
-00015460: 676e 7827 2c0a 2020 2020 2020 2020 2020  gnx',.          
+00015440: 2020 2020 2020 2020 636f 6f72 6473 3d63          coords=c
+00015450: 6f6f 7264 732c 0a20 2020 2020 2020 2020  oords,.         
+00015460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154a0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000154b0: 2020 2320 2e2e 2e20 6f72 2073 696d 756c    # ... or simul
-000154c0: 6174 6520 7468 656d 2077 2f20 7468 6520  ate them w/ the 
-000154d0: 6769 7665 6e20 6d73 7072 696d 6520 6172  given msprime ar
-000154e0: 6773 0a20 2020 2020 2020 2023 2061 6e64  gs.        # and
-000154f0: 2074 6865 2074 6869 7320 5370 6563 6965   the this Specie
-00015500: 7327 2067 656e 6f6d 6963 2061 7263 6869  s' genomic archi
-00015510: 7465 6374 7572 650a 2020 2020 2020 2020  tecture.        
-00015520: 656c 6966 2073 6f75 7263 655f 7370 7020  elif source_spp 
-00015530: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00015540: 2020 2020 2061 7373 6572 7420 696e 6469       assert indi
-00015550: 7669 6473 2069 7320 4e6f 6e65 2c20 2822  vids is None, ("
-00015560: 5468 6520 2769 6e64 6976 6964 7327 2061  The 'individs' a
-00015570: 7267 756d 656e 7420 696e 6469 6361 7465  rgument indicate
-00015580: 7320 7468 6520 220a 2020 2020 2020 2020  s the ".        
-00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155a0: 2020 2020 2020 2020 2020 2020 2269 6e64              "ind
-000155b0: 6963 6573 206f 6620 496e 6469 7669 6475  ices of Individu
-000155c0: 616c 7320 746f 2062 6520 6164 6465 6420  als to be added 
-000155d0: 6672 6f6d 2022 0a20 2020 2020 2020 2020  from ".         
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155f0: 2020 2020 2020 2020 2020 2022 6120 676e             "a gn
-00015600: 7820 5370 6563 6965 7320 6f62 6a65 6374  x Species object
-00015610: 2073 6572 7669 6e67 2061 7320 6120 736f   serving as a so
-00015620: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
-00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015640: 2020 2020 2020 2020 2020 2022 706f 7075             "popu
-00015650: 6c61 7469 6f6e 2c20 736f 2063 616e 206f  lation, so can o
-00015660: 6e6c 7920 6265 2075 7365 6420 6966 2022  nly be used if "
-00015670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015690: 2020 2020 2022 2773 6f75 7263 655f 6d73       "'source_ms
-000156a0: 7072 696d 655f 7061 7261 6d73 2720 6973  prime_params' is
-000156b0: 204e 6f6e 6520 616e 6420 220a 2020 2020   None and ".    
+00015480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015490: 6f75 7263 655f 736f 6674 7761 7265 3d27  ource_software='
+000154a0: 676e 7827 2c0a 2020 2020 2020 2020 2020  gnx',.          
+000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000154f0: 2020 2320 2e2e 2e20 6f72 2073 696d 756c    # ... or simul
+00015500: 6174 6520 7468 656d 2077 2f20 7468 6520  ate them w/ the 
+00015510: 6769 7665 6e20 6d73 7072 696d 6520 6172  given msprime ar
+00015520: 6773 0a20 2020 2020 2020 2023 2061 6e64  gs.        # and
+00015530: 2074 6865 2074 6869 7320 5370 6563 6965   the this Specie
+00015540: 7327 2067 656e 6f6d 6963 2061 7263 6869  s' genomic archi
+00015550: 7465 6374 7572 650a 2020 2020 2020 2020  tecture.        
+00015560: 656c 6966 2073 6f75 7263 655f 7370 7020  elif source_spp 
+00015570: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00015580: 2020 2020 2061 7373 6572 7420 696e 6469       assert indi
+00015590: 7669 6473 2069 7320 4e6f 6e65 2c20 2822  vids is None, ("
+000155a0: 5468 6520 2769 6e64 6976 6964 7327 2061  The 'individs' a
+000155b0: 7267 756d 656e 7420 696e 6469 6361 7465  rgument indicate
+000155c0: 7320 7468 6520 220a 2020 2020 2020 2020  s the ".        
+000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155e0: 2020 2020 2020 2020 2020 2020 2269 6e64              "ind
+000155f0: 6963 6573 206f 6620 496e 6469 7669 6475  ices of Individu
+00015600: 616c 7320 746f 2062 6520 6164 6465 6420  als to be added 
+00015610: 6672 6f6d 2022 0a20 2020 2020 2020 2020  from ".         
+00015620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015630: 2020 2020 2020 2020 2020 2022 6120 676e             "a gn
+00015640: 7820 5370 6563 6965 7320 6f62 6a65 6374  x Species object
+00015650: 2073 6572 7669 6e67 2061 7320 6120 736f   serving as a so
+00015660: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+00015670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015680: 2020 2020 2020 2020 2020 2022 706f 7075             "popu
+00015690: 6c61 7469 6f6e 2c20 736f 2063 616e 206f  lation, so can o
+000156a0: 6e6c 7920 6265 2075 7365 6420 6966 2022  nly be used if "
+000156b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156e0: 2227 736f 7572 6365 5f73 7070 2720 6973  "'source_spp' is
-000156f0: 2070 726f 7669 6465 642e 2229 0a0a 2020   provided.")..  
-00015700: 2020 2020 2020 2020 2020 2320 6d61 6b65            # make
-00015710: 2073 7572 6520 5370 6563 6965 7320 6861   sure Species ha
-00015720: 7320 6e6f 2073 656c 6563 7469 6f6e 2062  s no selection b
-00015730: 6566 6f72 6520 616c 6c6f 7769 6e67 2075  efore allowing u
-00015740: 7365 206f 6620 6d73 7072 696d 650a 2020  se of msprime.  
-00015750: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00015760: 206e 6f74 2073 656c 662e 7365 6c65 6374   not self.select
-00015770: 696f 6e2c 2028 226d 7370 7269 6d65 2069  ion, ("msprime i
-00015780: 7320 6120 636f 616c 6573 6365 6e74 2022  s a coalescent "
-00015790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000157a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157b0: 2020 2020 2020 2020 2020 2273 696d 756c            "simul
-000157c0: 6174 6f72 2c20 736f 2063 616e 6e6f 7420  ator, so cannot 
-000157d0: 6265 2073 696d 756c 6174 6520 220a 2020  be simulate ".  
+000156d0: 2020 2020 2022 2773 6f75 7263 655f 6d73       "'source_ms
+000156e0: 7072 696d 655f 7061 7261 6d73 2720 6973  prime_params' is
+000156f0: 204e 6f6e 6520 616e 6420 220a 2020 2020   None and ".    
+00015700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015720: 2227 736f 7572 6365 5f73 7070 2720 6973  "'source_spp' is
+00015730: 2070 726f 7669 6465 642e 2229 0a0a 2020   provided.")..  
+00015740: 2020 2020 2020 2020 2020 2320 6d61 6b65            # make
+00015750: 2073 7572 6520 5370 6563 6965 7320 6861   sure Species ha
+00015760: 7320 6e6f 2073 656c 6563 7469 6f6e 2062  s no selection b
+00015770: 6566 6f72 6520 616c 6c6f 7769 6e67 2075  efore allowing u
+00015780: 7365 206f 6620 6d73 7072 696d 650a 2020  se of msprime.  
+00015790: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+000157a0: 206e 6f74 2073 656c 662e 7365 6c65 6374   not self.select
+000157b0: 696f 6e2c 2028 226d 7370 7269 6d65 2069  ion, ("msprime i
+000157c0: 7320 6120 636f 616c 6573 6365 6e74 2022  s a coalescent "
+000157d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015800: 2020 2020 2020 2022 7365 6c65 6374 696f         "selectio
-00015810: 6e2e 2043 6f6e 7369 6465 7220 7573 696e  n. Consider usin
-00015820: 6720 6120 7365 636f 6e64 2022 0a20 2020  g a second ".   
+000157f0: 2020 2020 2020 2020 2020 2273 696d 756c            "simul
+00015800: 6174 6f72 2c20 736f 2063 616e 6e6f 7420  ator, so cannot 
+00015810: 7369 6d75 6c61 7465 2022 0a20 2020 2020  simulate ".     
+00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015850: 2020 2020 2020 2247 656f 6e6f 6d69 6373        "Geonomics
-00015860: 206d 6f64 656c 2074 6f20 7369 6d75 6c61   model to simula
-00015870: 7465 2061 2073 6f75 7263 6520 220a 2020  te a source ".  
+00015840: 2020 2020 2273 656c 6563 7469 6f6e 2e20      "selection. 
+00015850: 436f 6e73 6964 6572 2075 7369 6e67 2061  Consider using a
+00015860: 2073 6563 6f6e 6420 220a 2020 2020 2020   second ".      
+00015870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158a0: 2020 2020 2020 2022 706f 7075 6c61 7469         "populati
-000158b0: 6f6e 2077 6974 6820 7365 6c65 6374 696f  on with selectio
-000158c0: 6e2e 2229 0a0a 2020 2020 2020 2020 2020  n.")..          
-000158d0: 2020 2320 6368 6563 6b20 7468 6174 2072    # check that r
-000158e0: 6571 7569 7265 6420 6d73 7072 696d 6520  equired msprime 
-000158f0: 7061 7261 6d73 2061 7265 2070 726f 7669  params are provi
-00015900: 6465 6420 616e 6420 616e 7920 6f74 6865  ded and any othe
-00015910: 7273 0a20 2020 2020 2020 2020 2020 2023  rs.            #
-00015920: 2070 726f 7669 6465 6420 6172 6520 616d   provided are am
-00015930: 6f6e 6720 7468 6f73 6520 616c 6c6f 7765  ong those allowe
-00015940: 640a 2020 2020 2020 2020 2020 2020 7265  d.            re
-00015950: 7175 6972 6564 5f6d 7370 7269 6d65 5f70  quired_msprime_p
-00015960: 6172 616d 7320 3d20 5b27 7265 636f 6d62  arams = ['recomb
-00015970: 5f72 6174 6527 2c20 276d 7574 5f72 6174  _rate', 'mut_rat
-00015980: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
-00015990: 616c 6c6f 7765 645f 6d73 7072 696d 655f  allowed_msprime_
-000159a0: 7061 7261 6d73 203d 205b 2764 656d 6f67  params = ['demog
-000159b0: 7261 7068 7927 2c20 2770 6f70 756c 6174  raphy', 'populat
-000159c0: 696f 6e5f 7369 7a65 272c 0a20 2020 2020  ion_size',.     
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159f0: 2027 616e 6365 7374 7279 5f6d 6f64 656c   'ancestry_model
-00015a00: 272c 2027 7261 6e64 6f6d 5f73 6565 6427  ', 'random_seed'
-00015a10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a30: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00015a40: 2020 2020 2061 6c6c 5f6d 7370 7269 6d65       all_msprime
-00015a50: 5f70 6172 616d 7320 3d20 2872 6571 7569  _params = (requi
-00015a60: 7265 645f 6d73 7072 696d 655f 7061 7261  red_msprime_para
-00015a70: 6d73 202b 0a20 2020 2020 2020 2020 2020  ms +.           
-00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a90: 2020 2020 2020 2061 6c6c 6f77 6564 5f6d         allowed_m
-00015aa0: 7370 7269 6d65 5f70 6172 616d 7329 0a20  sprime_params). 
-00015ab0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00015ac0: 7420 6e70 2e61 6c6c 285b 6b20 696e 2061  t np.all([k in a
-00015ad0: 6c6c 5f6d 7370 7269 6d65 5f70 6172 616d  ll_msprime_param
-00015ae0: 7320 666f 720a 2020 2020 2020 2020 2020  s for.          
-00015af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b00: 2020 6b20 696e 2073 6f75 7263 655f 6d73    k in source_ms
-00015b10: 7072 696d 655f 7061 7261 6d73 5d29 2c20  prime_params]), 
-00015b20: 2822 5468 6520 6f6e 6c79 2070 6172 616d  ("The only param
-00015b30: 6574 6572 7322 0a20 2020 2020 2020 2020  eters".         
-00015b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b50: 2020 2020 2020 2020 2020 2022 2061 6363             " acc
-00015b60: 6570 7465 6420 696e 2027 736f 7572 6365  epted in 'source
-00015b70: 5f6d 7370 7269 6d65 5f70 6172 616d 7327  _msprime_params'
-00015b80: 2061 7265 3a20 220a 2020 2020 2020 2020   are: ".        
-00015b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ba0: 2020 2020 2020 2020 2020 2066 227b 272c             f"{',
-00015bb0: 2027 2e6a 6f69 6e28 616c 6c5f 6d73 7072   '.join(all_mspr
-00015bc0: 696d 655f 7061 7261 6d73 297d 2e22 290a  ime_params)}.").
-00015bd0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00015be0: 7274 206e 702e 616c 6c28 5b6b 2069 6e20  rt np.all([k in 
-00015bf0: 736f 7572 6365 5f6d 7370 7269 6d65 5f70  source_msprime_p
-00015c00: 6172 616d 7320 666f 720a 2020 2020 2020  arams for.      
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c20: 2020 2020 2020 6b20 696e 2072 6571 7569        k in requi
-00015c30: 7265 645f 6d73 7072 696d 655f 7061 7261  red_msprime_para
-00015c40: 6d73 5d29 2c20 2822 426f 7468 2022 0a20  ms]), ("Both ". 
+00015890: 2020 2022 4765 6f6e 6f6d 6963 7320 6d6f     "Geonomics mo
+000158a0: 6465 6c20 746f 2073 696d 756c 6174 6520  del to simulate 
+000158b0: 6120 736f 7572 6365 2022 0a20 2020 2020  a source ".     
+000158c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158e0: 2020 2020 2270 6f70 756c 6174 696f 6e20      "population 
+000158f0: 7769 7468 2073 656c 6563 7469 6f6e 2e22  with selection."
+00015900: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00015910: 2063 6865 636b 2074 6861 7420 7265 7175   check that requ
+00015920: 6972 6564 206d 7370 7269 6d65 2070 6172  ired msprime par
+00015930: 616d 7320 6172 6520 7072 6f76 6964 6564  ams are provided
+00015940: 2061 6e64 2061 6e79 206f 7468 6572 730a   and any others.
+00015950: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00015960: 6f76 6964 6564 2061 7265 2061 6d6f 6e67  ovided are among
+00015970: 2074 686f 7365 2061 6c6c 6f77 6564 0a20   those allowed. 
+00015980: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+00015990: 7265 645f 6d73 7072 696d 655f 7061 7261  red_msprime_para
+000159a0: 6d73 203d 205b 2772 6563 6f6d 625f 7261  ms = ['recomb_ra
+000159b0: 7465 272c 2027 6d75 745f 7261 7465 275d  te', 'mut_rate']
+000159c0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+000159d0: 6f77 6564 5f6d 7370 7269 6d65 5f70 6172  owed_msprime_par
+000159e0: 616d 7320 3d20 5b27 6465 6d6f 6772 6170  ams = ['demograp
+000159f0: 6879 272c 2027 706f 7075 6c61 7469 6f6e  hy', 'population
+00015a00: 5f73 697a 6527 2c0a 2020 2020 2020 2020  _size',.        
+00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a20: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+00015a30: 6e63 6573 7472 795f 6d6f 6465 6c27 2c20  ncestry_model', 
+00015a40: 2772 616e 646f 6d5f 7365 6564 272c 0a20  'random_seed',. 
+00015a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a70: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00015a80: 2020 616c 6c5f 6d73 7072 696d 655f 7061    all_msprime_pa
+00015a90: 7261 6d73 203d 2028 7265 7175 6972 6564  rams = (required
+00015aa0: 5f6d 7370 7269 6d65 5f70 6172 616d 7320  _msprime_params 
+00015ab0: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ad0: 2020 2020 616c 6c6f 7765 645f 6d73 7072      allowed_mspr
+00015ae0: 696d 655f 7061 7261 6d73 290a 2020 2020  ime_params).    
+00015af0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+00015b00: 702e 616c 6c28 5b6b 2069 6e20 616c 6c5f  p.all([k in all_
+00015b10: 6d73 7072 696d 655f 7061 7261 6d73 2066  msprime_params f
+00015b20: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+00015b30: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00015b40: 2069 6e20 736f 7572 6365 5f6d 7370 7269   in source_mspri
+00015b50: 6d65 5f70 6172 616d 735d 292c 2028 2254  me_params]), ("T
+00015b60: 6865 206f 6e6c 7920 7061 7261 6d65 7465  he only paramete
+00015b70: 7273 220a 2020 2020 2020 2020 2020 2020  rs".            
+00015b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b90: 2020 2020 2020 2020 2220 6163 6365 7074          " accept
+00015ba0: 6564 2069 6e20 2773 6f75 7263 655f 6d73  ed in 'source_ms
+00015bb0: 7072 696d 655f 7061 7261 6d73 2720 6172  prime_params' ar
+00015bc0: 653a 2022 0a20 2020 2020 2020 2020 2020  e: ".           
+00015bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015be0: 2020 2020 2020 2020 6622 7b27 2c20 272e          f"{', '.
+00015bf0: 6a6f 696e 2861 6c6c 5f6d 7370 7269 6d65  join(all_msprime
+00015c00: 5f70 6172 616d 7329 7d2e 2229 0a20 2020  _params)}.").   
+00015c10: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00015c20: 6e70 2e61 6c6c 285b 6b20 696e 2073 6f75  np.all([k in sou
+00015c30: 7263 655f 6d73 7072 696d 655f 7061 7261  rce_msprime_para
+00015c40: 6d73 2066 6f72 0a20 2020 2020 2020 2020  ms for.         
 00015c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c70: 2020 6622 7b27 2061 6e64 2027 2e6a 6f69    f"{' and '.joi
-00015c80: 6e28 7265 7175 6972 6564 5f6d 7370 7269  n(required_mspri
-00015c90: 6d65 5f70 6172 616d 7329 7d20 220a 2020  me_params)} ".  
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cc0: 2020 226d 7573 7420 6265 2070 726f 7669    "must be provi
-00015cd0: 6465 6420 7769 7468 696e 2022 0a20 2020  ded within ".   
+00015c60: 2020 206b 2069 6e20 7265 7175 6972 6564     k in required
+00015c70: 5f6d 7370 7269 6d65 5f70 6172 616d 735d  _msprime_params]
+00015c80: 292c 2028 2242 6f74 6820 220a 2020 2020  ), ("Both ".    
+00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ca0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015cb0: 227b 2720 616e 6420 272e 6a6f 696e 2872  "{' and '.join(r
+00015cc0: 6571 7569 7265 645f 6d73 7072 696d 655f  equired_msprime_
+00015cd0: 7061 7261 6d73 297d 2022 0a20 2020 2020  params)} ".     
 00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d00: 2022 2773 6f75 7263 655f 6d73 7072 696d   "'source_msprim
-00015d10: 655f 7061 7261 6d73 272e 2229 0a0a 2020  e_params'.")..  
-00015d20: 2020 2020 2020 2020 2020 2320 7275 6e20            # run 
-00015d30: 7468 6520 7369 6d75 6c61 7469 6f6e 2061  the simulation a
-00015d40: 6e64 2072 6574 7572 6e20 7465 6d70 6c61  nd return templa
-00015d50: 7465 2049 6e64 6976 6964 7561 6c73 0a20  te Individuals. 
-00015d60: 2020 2020 2020 2020 2020 2075 7365 5f74             use_t
-00015d70: 736b 6974 203d 2073 656c 662e 6765 6e5f  skit = self.gen_
-00015d80: 6172 6368 2e75 7365 5f74 736b 6974 0a20  arch.use_tskit. 
-00015d90: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
-00015da0: 6964 732c 2073 6f75 7263 655f 7463 203d  ids, source_tc =
-00015db0: 205f 7369 6d5f 6d73 7072 696d 655f 696e   _sim_msprime_in
-00015dc0: 6469 7669 6475 616c 7328 6e3d 6e2c 0a20  dividuals(n=n,. 
-00015dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e00: 2020 204c 3d73 656c 662e 6765 6e5f 6172     L=self.gen_ar
-00015e10: 6368 2e4c 2c0a 2020 2020 2020 2020 2020  ch.L,.          
+00015cf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015d00: 6d75 7374 2062 6520 7072 6f76 6964 6564  must be provided
+00015d10: 2077 6974 6869 6e20 220a 2020 2020 2020   within ".      
+00015d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d30: 2020 2020 2020 2020 2020 2020 2020 2227                "'
+00015d40: 736f 7572 6365 5f6d 7370 7269 6d65 5f70  source_msprime_p
+00015d50: 6172 616d 7327 2e22 290a 0a20 2020 2020  arams'.")..     
+00015d60: 2020 2020 2020 2023 2072 756e 2074 6865         # run the
+00015d70: 2073 696d 756c 6174 696f 6e20 616e 6420   simulation and 
+00015d80: 7265 7475 726e 2074 656d 706c 6174 6520  return template 
+00015d90: 496e 6469 7669 6475 616c 730a 2020 2020  Individuals.    
+00015da0: 2020 2020 2020 2020 7573 655f 7473 6b69          use_tski
+00015db0: 7420 3d20 7365 6c66 2e67 656e 5f61 7263  t = self.gen_arc
+00015dc0: 682e 7573 655f 7473 6b69 740a 2020 2020  h.use_tskit.    
+00015dd0: 2020 2020 2020 2020 696e 6469 7669 6473          individs
+00015de0: 2c20 736f 7572 6365 5f74 6320 3d20 5f73  , source_tc = _s
+00015df0: 696d 5f6d 7370 7269 6d65 5f69 6e64 6976  im_msprime_indiv
+00015e00: 6964 7561 6c73 286e 3d6e 2c0a 2020 2020  iduals(n=n,.    
+00015e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e40: 2020 2020 2020 2020 2020 7573 655f 7473            use_ts
-00015e50: 6b69 743d 7573 655f 7473 6b69 742c 0a20  kit=use_tskit,. 
+00015e40: 4c3d 7365 6c66 2e67 656e 5f61 7263 682e  L=self.gen_arch.
+00015e50: 4c2c 0a20 2020 2020 2020 2020 2020 2020  L,.             
 00015e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e90: 2020 202a 2a73 6f75 7263 655f 6d73 7072     **source_mspr
-00015ea0: 696d 655f 7061 7261 6d73 2c0a 2020 2020  ime_params,.    
+00015e80: 2020 2020 2020 2075 7365 5f74 736b 6974         use_tskit
+00015e90: 3d75 7365 5f74 736b 6974 2c0a 2020 2020  =use_tskit,.    
+00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ee0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00015ef0: 2072 756e 2061 6c6c 2054 6162 6c65 436f   run all TableCo
-00015f00: 6c6c 6563 7469 6f6e 2065 6469 7473 2074  llection edits t
-00015f10: 6861 7420 6172 6520 6e65 6365 7373 6172  hat are necessar
-00015f20: 7920 746f 2061 6c69 676e 206d 7370 7269  y to align mspri
-00015f30: 6d65 0a20 2020 2020 2020 2020 2020 2023  me.            #
-00015f40: 206f 7574 7075 7420 7769 7468 2074 6865   output with the
-00015f50: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00015f60: 2063 6f6e 7665 6e74 696f 6e73 2075 7365   conventions use
-00015f70: 6420 696e 2067 6e78 0a20 2020 2020 2020  d in gnx.       
-00015f80: 2020 2020 2023 204e 4f54 453a 2065 6469       # NOTE: edi
-00015f90: 7473 2074 6865 2054 6162 6c65 436f 6c6c  ts the TableColl
-00015fa0: 6563 7469 6f6e 2069 6e20 706c 6163 653b  ection in place;
-00015fb0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-00015fc0: 2020 2020 2072 6574 7572 6e73 2074 6865       returns the
-00015fd0: 206e 6578 7420 6e20 676e 7820 496e 6469   next n gnx Indi
-00015fe0: 7669 6475 616c 2069 6478 7320 6173 7369  vidual idxs assi
-00015ff0: 676e 6564 2074 6f20 7468 6f73 650a 2020  gned to those.  
-00016000: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00016010: 2020 496e 6469 7669 6475 616c 7320 666f    Individuals fo
-00016020: 7220 696e 636f 7270 6f72 6174 696f 6e20  r incorporation 
-00016030: 696e 746f 2074 6865 2067 6976 656e 2053  into the given S
-00016040: 7065 6369 6573 0a20 2020 2020 2020 2020  pecies.         
-00016050: 2020 206e 6578 745f 676e 785f 6964 7873     next_gnx_idxs
-00016060: 203d 205f 7072 6570 5f74 736b 6974 5f74   = _prep_tskit_t
-00016070: 6162 636f 6c6c 5f66 6f72 5f67 6e78 5f73  abcoll_for_gnx_s
-00016080: 7070 5f75 6e69 6f6e 2874 633d 736f 7572  pp_union(tc=sour
-00016090: 6365 5f74 632c 0a20 2020 2020 2020 2020  ce_tc,.         
-000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160c0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
-000160d0: 6970 5f73 7070 3d73 656c 662c 0a20 2020  ip_spp=self,.   
+00015ed0: 2a2a 736f 7572 6365 5f6d 7370 7269 6d65  **source_msprime
+00015ee0: 5f70 6172 616d 732c 0a20 2020 2020 2020  _params,.       
+00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f10: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00015f20: 2020 2020 2020 2020 2020 2020 2320 7275              # ru
+00015f30: 6e20 616c 6c20 5461 626c 6543 6f6c 6c65  n all TableColle
+00015f40: 6374 696f 6e20 6564 6974 7320 7468 6174  ction edits that
+00015f50: 2061 7265 206e 6563 6573 7361 7279 2074   are necessary t
+00015f60: 6f20 616c 6967 6e20 6d73 7072 696d 650a  o align msprime.
+00015f70: 2020 2020 2020 2020 2020 2020 2320 6f75              # ou
+00015f80: 7470 7574 2077 6974 6820 7468 6520 5461  tput with the Ta
+00015f90: 626c 6543 6f6c 6c65 6374 696f 6e20 636f  bleCollection co
+00015fa0: 6e76 656e 7469 6f6e 7320 7573 6564 2069  nventions used i
+00015fb0: 6e20 676e 780a 2020 2020 2020 2020 2020  n gnx.          
+00015fc0: 2020 2320 4e4f 5445 3a20 6564 6974 7320    # NOTE: edits 
+00015fd0: 7468 6520 5461 626c 6543 6f6c 6c65 6374  the TableCollect
+00015fe0: 696f 6e20 696e 2070 6c61 6365 3b0a 2020  ion in place;.  
+00015ff0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00016000: 2020 7265 7475 726e 7320 7468 6520 6e65    returns the ne
+00016010: 7874 206e 2067 6e78 2049 6e64 6976 6964  xt n gnx Individ
+00016020: 7561 6c20 6964 7873 2061 7373 6967 6e65  ual idxs assigne
+00016030: 6420 746f 2074 686f 7365 0a20 2020 2020  d to those.     
+00016040: 2020 2020 2020 2023 2020 2020 2020 2049         #       I
+00016050: 6e64 6976 6964 7561 6c73 2066 6f72 2069  ndividuals for i
+00016060: 6e63 6f72 706f 7261 7469 6f6e 2069 6e74  ncorporation int
+00016070: 6f20 7468 6520 6769 7665 6e20 5370 6563  o the given Spec
+00016080: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
+00016090: 6e65 7874 5f67 6e78 5f69 6478 7320 3d20  next_gnx_idxs = 
+000160a0: 5f70 7265 705f 7473 6b69 745f 7461 6263  _prep_tskit_tabc
+000160b0: 6f6c 6c5f 666f 725f 676e 785f 7370 705f  oll_for_gnx_spp_
+000160c0: 756e 696f 6e28 7463 3d73 6f75 7263 655f  union(tc=source_
+000160d0: 7463 2c0a 2020 2020 2020 2020 2020 2020  tc,.            
 000160e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000160f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016110: 2020 2063 6f6f 7264 733d 636f 6f72 6473     coords=coords
-00016120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016100: 2020 2020 2020 2020 2020 7265 6369 705f            recip_
+00016110: 7370 703d 7365 6c66 2c0a 2020 2020 2020  spp=self,.      
+00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 2020 2020 2020 2020 736f 7572 6365 5f73          source_s
-00016160: 6f66 7477 6172 653d 276d 7370 7269 6d65  oftware='msprime
-00016170: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00016150: 636f 6f72 6473 3d63 6f6f 7264 732c 0a20  coords=coords,. 
+00016160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161b0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-000161c0: 2073 6574 2074 6865 2073 6f75 7263 6520   set the source 
-000161d0: 496e 6469 7669 6475 616c 7327 2063 6f6f  Individuals' coo
-000161e0: 7264 696e 6174 6573 0a20 2020 2020 2020  rdinates.       
-000161f0: 205b 696e 642e 5f73 6574 5f70 6f73 282a   [ind._set_pos(*
-00016200: 636f 6f72 6473 5b69 2c3a 5d29 2066 6f72  coords[i,:]) for
-00016210: 2069 2c20 696e 6420 696e 2065 6e75 6d65   i, ind in enume
-00016220: 7261 7465 2869 6e64 6976 6964 7329 5d0a  rate(individs)].
-00016230: 0a20 2020 2020 2020 2023 2075 7064 6174  .        # updat
-00016240: 6520 7468 6520 696e 6465 7820 7661 6c75  e the index valu
-00016250: 6573 2069 6465 6e74 6966 7969 6e67 2049  es identifying I
-00016260: 6e64 6976 6964 7561 6c73 2069 6e20 676e  ndividuals in gn
-00016270: 7820 616e 6420 7473 6b69 7420 6461 7461  x and tskit data
-00016280: 0a20 2020 2020 2020 206d 6178 5f69 6478  .        max_idx
-00016290: 5f62 3420 3d20 7365 6c66 2e6d 6178 5f69  _b4 = self.max_i
-000162a0: 6e64 5f69 6478 0a20 2020 2020 2020 206e  nd_idx.        n
-000162b0: 6577 5f69 6478 7320 3d20 5b5d 0a20 2020  ew_idxs = [].   
-000162c0: 2020 2020 2066 6f72 2069 2c20 696e 6420       for i, ind 
-000162d0: 696e 2065 6e75 6d65 7261 7465 2869 6e64  in enumerate(ind
-000162e0: 6976 6964 7329 3a0a 2020 2020 2020 2020  ivids):.        
-000162f0: 2020 2020 2320 696e 6372 656d 656e 7420      # increment 
-00016300: 7468 6520 6d61 785f 696e 645f 6964 780a  the max_ind_idx.
-00016310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016320: 2e6d 6178 5f69 6e64 5f69 6478 202b 3d20  .max_ind_idx += 
-00016330: 310a 2020 2020 2020 2020 2020 2020 2320  1.            # 
-00016340: 7365 7420 7468 6520 496e 6469 7669 6475  set the Individu
-00016350: 616c 2773 2067 6e78 2069 6e64 6578 0a20  al's gnx index. 
-00016360: 2020 2020 2020 2020 2020 2069 6e64 2e69             ind.i
-00016370: 6478 203d 2073 656c 662e 6d61 785f 696e  dx = self.max_in
-00016380: 645f 6964 780a 2020 2020 2020 2020 2020  d_idx.          
-00016390: 2020 6e65 775f 6964 7873 2e61 7070 656e    new_idxs.appen
-000163a0: 6428 7365 6c66 2e6d 6178 5f69 6e64 5f69  d(self.max_ind_i
-000163b0: 6478 290a 2020 2020 2020 2020 2020 2020  dx).            
-000163c0: 2320 7365 7420 7468 6520 496e 6469 7669  # set the Indivi
-000163d0: 6475 616c 7327 2069 6473 2066 6f72 2074  duals' ids for t
-000163e0: 6865 2074 736b 6974 206e 6f64 6573 2074  he tskit nodes t
-000163f0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
-00016400: 2069 6e64 2e5f 6e6f 6465 735f 7461 625f   ind._nodes_tab_
-00016410: 6964 7320 3d20 7b6b 3a20 7620 2b20 7365  ids = {k: v + se
-00016420: 6c66 2e5f 7463 2e6e 6f64 6573 2e6e 756d  lf._tc.nodes.num
-00016430: 5f72 6f77 7320 666f 720a 2020 2020 2020  _rows for.      
-00016440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016460: 2020 2020 2020 6b2c 2076 2069 6e20 696e        k, v in in
-00016470: 642e 5f6e 6f64 6573 5f74 6162 5f69 6473  d._nodes_tab_ids
-00016480: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
-00016490: 2020 2020 2020 2320 7365 7420 7468 6520        # set the 
-000164a0: 496e 6469 7669 6475 616c 7327 2069 6473  Individuals' ids
-000164b0: 2066 6f72 2074 6865 2074 736b 6974 2069   for the tskit i
-000164c0: 6e64 6976 6964 7561 6c73 2074 6162 6c65  ndividuals table
-000164d0: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
-000164e0: 4f54 453a 2074 6865 2069 6e76 6572 7365  OTE: the inverse
-000164f0: 2028 7468 6520 496e 6469 7669 6475 616c   (the Individual
-00016500: 7327 2067 6e78 2069 6478 2076 616c 7565  s' gnx idx value
-00016510: 732c 0a20 2020 2020 2020 2020 2020 2023  s,.            #
-00016520: 2020 2020 2020 2061 7320 7265 636f 7265         as recore
-00016530: 6420 696e 2074 6865 2074 736b 6974 2069  d in the tskit i
-00016540: 6e64 6976 6964 7561 6c73 2074 6162 6c65  ndividuals table
-00016550: 2773 0a20 2020 2020 2020 2020 2020 2023  's.            #
-00016560: 2020 2020 2020 206d 6574 6164 6174 6129         metadata)
-00016570: 2073 686f 756c 6420 616c 7265 6164 7920   should already 
-00016580: 6265 2063 6f72 7265 6374 0a20 2020 2020  be correct.     
-00016590: 2020 2020 2020 2023 2020 2020 2020 2062         #       b
-000165a0: 6563 6175 7365 205f 7072 6570 5f74 736b  ecause _prep_tsk
-000165b0: 6974 5f74 6162 636f 6c6c 5f66 6f72 5f67  it_tabcoll_for_g
-000165c0: 6e78 5f73 7070 5f75 6e69 6f6e 0a20 2020  nx_spp_union.   
-000165d0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-000165e0: 2067 656e 6572 6174 6564 2074 6865 2069   generated the i
-000165f0: 6e64 6578 2076 616c 7565 730a 2020 2020  ndex values.    
-00016600: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00016610: 616e 6420 7365 7420 7468 656d 2069 6e20  and set them in 
-00016620: 7468 6520 5461 626c 6543 6f6c 6c65 6374  the TableCollect
-00016630: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00016640: 696e 642e 5f69 6e64 6976 6964 7561 6c73  ind._individuals
-00016650: 5f74 6162 5f69 6420 2b3d 2073 656c 662e  _tab_id += self.
-00016660: 5f74 632e 696e 6469 7669 6475 616c 732e  _tc.individuals.
-00016670: 6e75 6d5f 726f 7773 0a20 2020 2020 2020  num_rows.       
-00016680: 206d 6178 5f69 6478 5f61 6620 3d20 7365   max_idx_af = se
-00016690: 6c66 2e6d 6178 5f69 6e64 5f69 6478 0a20  lf.max_ind_idx. 
-000166a0: 2020 2020 2020 2061 7373 6572 7420 6d61         assert ma
-000166b0: 785f 6964 785f 6166 202d 206d 6178 5f69  x_idx_af - max_i
-000166c0: 6478 5f62 3420 3d3d 206c 656e 2869 6e64  dx_b4 == len(ind
-000166d0: 6976 6964 7329 0a20 2020 2020 2020 2023  ivids).        #
-000166e0: 2063 6f6d 7061 7265 2074 6865 2069 6478   compare the idx
-000166f0: 2076 616c 7565 7320 7468 6174 2077 6572   values that wer
-00016700: 6520 7365 7420 6f6e 2074 6865 2049 6e64  e set on the Ind
-00016710: 6976 6964 7561 6c73 2074 6f20 7468 6f73  ividuals to thos
-00016720: 6520 7468 6174 0a20 2020 2020 2020 2023  e that.        #
-00016730: 2077 6572 6520 7365 7420 696e 2074 6865   were set in the
-00016740: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00016750: 2e69 6e64 6976 6964 7561 6c73 2074 6162  .individuals tab
-00016760: 6c65 0a20 2020 2020 2020 2061 7373 6572  le.        asser
-00016770: 7420 6e70 2e61 6c6c 286e 702e 6172 7261  t np.all(np.arra
-00016780: 7928 6e65 7874 5f67 6e78 5f69 6478 7329  y(next_gnx_idxs)
-00016790: 203d 3d20 6e70 2e61 7272 6179 286e 6577   == np.array(new
-000167a0: 5f69 6478 7329 292c 2028 0a20 2020 2020  _idxs)), (.     
-000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167c0: 2020 2020 2020 2020 2020 2020 2249 6e64              "Ind
-000167d0: 6976 6964 6175 6c20 6964 7820 7661 6c75  ividaul idx valu
-000167e0: 6573 2073 6574 2069 6e20 7468 6520 220a  es set in the ".
+00016190: 2020 2020 2073 6f75 7263 655f 736f 6674       source_soft
+000161a0: 7761 7265 3d27 6d73 7072 696d 6527 2c0a  ware='msprime',.
+000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161f0: 2029 0a0a 2020 2020 2020 2020 2320 7365   )..        # se
+00016200: 7420 7468 6520 736f 7572 6365 2049 6e64  t the source Ind
+00016210: 6976 6964 7561 6c73 2720 636f 6f72 6469  ividuals' coordi
+00016220: 6e61 7465 730a 2020 2020 2020 2020 5b69  nates.        [i
+00016230: 6e64 2e5f 7365 745f 706f 7328 2a63 6f6f  nd._set_pos(*coo
+00016240: 7264 735b 692c 3a5d 2920 666f 7220 692c  rds[i,:]) for i,
+00016250: 2069 6e64 2069 6e20 656e 756d 6572 6174   ind in enumerat
+00016260: 6528 696e 6469 7669 6473 295d 0a0a 2020  e(individs)]..  
+00016270: 2020 2020 2020 2320 7570 6461 7465 2074        # update t
+00016280: 6865 2069 6e64 6578 2076 616c 7565 7320  he index values 
+00016290: 6964 656e 7469 6679 696e 6720 496e 6469  identifying Indi
+000162a0: 7669 6475 616c 7320 696e 2067 6e78 2061  viduals in gnx a
+000162b0: 6e64 2074 736b 6974 2064 6174 610a 2020  nd tskit data.  
+000162c0: 2020 2020 2020 6d61 785f 6964 785f 6234        max_idx_b4
+000162d0: 203d 2073 656c 662e 6d61 785f 696e 645f   = self.max_ind_
+000162e0: 6964 780a 2020 2020 2020 2020 6e65 775f  idx.        new_
+000162f0: 6964 7873 203d 205b 5d0a 2020 2020 2020  idxs = [].      
+00016300: 2020 666f 7220 692c 2069 6e64 2069 6e20    for i, ind in 
+00016310: 656e 756d 6572 6174 6528 696e 6469 7669  enumerate(indivi
+00016320: 6473 293a 0a20 2020 2020 2020 2020 2020  ds):.           
+00016330: 2023 2069 6e63 7265 6d65 6e74 2074 6865   # increment the
+00016340: 206d 6178 5f69 6e64 5f69 6478 0a20 2020   max_ind_idx.   
+00016350: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00016360: 785f 696e 645f 6964 7820 2b3d 2031 0a20  x_ind_idx += 1. 
+00016370: 2020 2020 2020 2020 2020 2023 2073 6574             # set
+00016380: 2074 6865 2049 6e64 6976 6964 7561 6c27   the Individual'
+00016390: 7320 676e 7820 696e 6465 780a 2020 2020  s gnx index.    
+000163a0: 2020 2020 2020 2020 696e 642e 6964 7820          ind.idx 
+000163b0: 3d20 7365 6c66 2e6d 6178 5f69 6e64 5f69  = self.max_ind_i
+000163c0: 6478 0a20 2020 2020 2020 2020 2020 206e  dx.            n
+000163d0: 6577 5f69 6478 732e 6170 7065 6e64 2873  ew_idxs.append(s
+000163e0: 656c 662e 6d61 785f 696e 645f 6964 7829  elf.max_ind_idx)
+000163f0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00016400: 6574 2074 6865 2049 6e64 6976 6964 7561  et the Individua
+00016410: 6c73 2720 6964 7320 666f 7220 7468 6520  ls' ids for the 
+00016420: 7473 6b69 7420 6e6f 6465 7320 7461 626c  tskit nodes tabl
+00016430: 650a 2020 2020 2020 2020 2020 2020 696e  e.            in
+00016440: 642e 5f6e 6f64 6573 5f74 6162 5f69 6473  d._nodes_tab_ids
+00016450: 203d 207b 6b3a 2076 202b 2073 656c 662e   = {k: v + self.
+00016460: 5f74 632e 6e6f 6465 732e 6e75 6d5f 726f  _tc.nodes.num_ro
+00016470: 7773 2066 6f72 0a20 2020 2020 2020 2020  ws for.         
+00016480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164a0: 2020 206b 2c20 7620 696e 2069 6e64 2e5f     k, v in ind._
+000164b0: 6e6f 6465 735f 7461 625f 6964 732e 6974  nodes_tab_ids.it
+000164c0: 656d 7328 297d 0a20 2020 2020 2020 2020  ems()}.         
+000164d0: 2020 2023 2073 6574 2074 6865 2049 6e64     # set the Ind
+000164e0: 6976 6964 7561 6c73 2720 6964 7320 666f  ividuals' ids fo
+000164f0: 7220 7468 6520 7473 6b69 7420 696e 6469  r the tskit indi
+00016500: 7669 6475 616c 7320 7461 626c 650a 2020  viduals table.  
+00016510: 2020 2020 2020 2020 2020 2320 4e4f 5445            # NOTE
+00016520: 3a20 7468 6520 696e 7665 7273 6520 2874  : the inverse (t
+00016530: 6865 2049 6e64 6976 6964 7561 6c73 2720  he Individuals' 
+00016540: 676e 7820 6964 7820 7661 6c75 6573 2c0a  gnx idx values,.
+00016550: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00016560: 2020 2020 6173 2072 6563 6f72 6564 2069      as recored i
+00016570: 6e20 7468 6520 7473 6b69 7420 696e 6469  n the tskit indi
+00016580: 7669 6475 616c 7320 7461 626c 6527 730a  viduals table's.
+00016590: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+000165a0: 2020 2020 6d65 7461 6461 7461 2920 7368      metadata) sh
+000165b0: 6f75 6c64 2061 6c72 6561 6479 2062 6520  ould already be 
+000165c0: 636f 7272 6563 740a 2020 2020 2020 2020  correct.        
+000165d0: 2020 2020 2320 2020 2020 2020 6265 6361      #       beca
+000165e0: 7573 6520 5f70 7265 705f 7473 6b69 745f  use _prep_tskit_
+000165f0: 7461 6263 6f6c 6c5f 666f 725f 676e 785f  tabcoll_for_gnx_
+00016600: 7370 705f 756e 696f 6e0a 2020 2020 2020  spp_union.      
+00016610: 2020 2020 2020 2320 2020 2020 2020 6765        #       ge
+00016620: 6e65 7261 7465 6420 7468 6520 696e 6465  nerated the inde
+00016630: 7820 7661 6c75 6573 0a20 2020 2020 2020  x values.       
+00016640: 2020 2020 2023 2020 2020 2020 2061 6e64       #       and
+00016650: 2073 6574 2074 6865 6d20 696e 2074 6865   set them in the
+00016660: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
+00016670: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+00016680: 2e5f 696e 6469 7669 6475 616c 735f 7461  ._individuals_ta
+00016690: 625f 6964 202b 3d20 7365 6c66 2e5f 7463  b_id += self._tc
+000166a0: 2e69 6e64 6976 6964 7561 6c73 2e6e 756d  .individuals.num
+000166b0: 5f72 6f77 730a 2020 2020 2020 2020 6d61  _rows.        ma
+000166c0: 785f 6964 785f 6166 203d 2073 656c 662e  x_idx_af = self.
+000166d0: 6d61 785f 696e 645f 6964 780a 2020 2020  max_ind_idx.    
+000166e0: 2020 2020 6173 7365 7274 206d 6178 5f69      assert max_i
+000166f0: 6478 5f61 6620 2d20 6d61 785f 6964 785f  dx_af - max_idx_
+00016700: 6234 203d 3d20 6c65 6e28 696e 6469 7669  b4 == len(indivi
+00016710: 6473 290a 2020 2020 2020 2020 2320 636f  ds).        # co
+00016720: 6d70 6172 6520 7468 6520 6964 7820 7661  mpare the idx va
+00016730: 6c75 6573 2074 6861 7420 7765 7265 2073  lues that were s
+00016740: 6574 206f 6e20 7468 6520 496e 6469 7669  et on the Indivi
+00016750: 6475 616c 7320 746f 2074 686f 7365 2074  duals to those t
+00016760: 6861 740a 2020 2020 2020 2020 2320 7765  hat.        # we
+00016770: 7265 2073 6574 2069 6e20 7468 6520 5461  re set in the Ta
+00016780: 626c 6543 6f6c 6c65 6374 696f 6e2e 696e  bleCollection.in
+00016790: 6469 7669 6475 616c 7320 7461 626c 650a  dividuals table.
+000167a0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+000167b0: 702e 616c 6c28 6e70 2e61 7272 6179 286e  p.all(np.array(n
+000167c0: 6578 745f 676e 785f 6964 7873 2920 3d3d  ext_gnx_idxs) ==
+000167d0: 206e 702e 6172 7261 7928 6e65 775f 6964   np.array(new_id
+000167e0: 7873 2929 2c20 280a 2020 2020 2020 2020  xs)), (.        
 000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016810: 2020 2020 2254 6162 6c65 436f 6c6c 6563      "TableCollec
-00016820: 7469 6f6e 2e69 6e64 6976 6964 7561 6c73  tion.individuals
-00016830: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00016800: 2020 2020 2020 2020 2022 496e 6469 7669           "Indivi
+00016810: 6461 756c 2069 6478 2076 616c 7565 7320  daul idx values 
+00016820: 7365 7420 696e 2074 6865 2022 0a20 2020  set in the ".   
+00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2020 2020 2020 2022 7461 626c 6520 646f         "table do
-00016860: 206e 6f74 2061 6772 6565 2077 6974 6820   not agree with 
-00016870: 7468 6f73 6520 7365 7420 6f6e 2074 6865  those set on the
-00016880: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168a0: 2020 2020 2020 2022 496e 6469 7669 6475         "Individu
-000168b0: 616c 7320 7468 656d 7365 6c76 6573 2e22  als themselves."
-000168c0: 290a 0a20 2020 2020 2020 2023 2073 6f72  )..        # sor
-000168d0: 7420 616e 6420 7369 6d70 6c69 6679 2074  t and simplify t
-000168e0: 6865 2074 736b 6974 2e54 6162 6c65 436f  he tskit.TableCo
-000168f0: 6c6c 6563 7469 6f6e 0a20 2020 2020 2020  llection.       
-00016900: 2073 656c 662e 5f73 6f72 745f 616e 645f   self._sort_and_
-00016910: 7369 6d70 6c69 6679 5f74 6162 6c65 5f63  simplify_table_c
-00016920: 6f6c 6c65 6374 696f 6e28 290a 0a20 2020  ollection()..   
-00016930: 2020 2020 2023 2075 6e69 6f6e 2073 6f75       # union sou
-00016940: 7263 6520 696e 6469 7669 6475 616c 7327  rce individuals'
-00016950: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00016960: 2069 6e74 6f20 7468 6973 2053 7065 6369   into this Speci
-00016970: 6573 2720 5461 626c 6543 6f6c 6c0a 2020  es' TableColl.  
-00016980: 2020 2020 2020 6e6f 6465 735f 7461 625f        nodes_tab_
-00016990: 6c65 6e5f 6234 203d 2073 656c 662e 5f74  len_b4 = self._t
-000169a0: 632e 6e6f 6465 732e 6e75 6d5f 726f 7773  c.nodes.num_rows
-000169b0: 0a20 2020 2020 2020 2069 6e64 6976 6964  .        individ
-000169c0: 735f 7461 625f 6c65 6e5f 6234 203d 2073  s_tab_len_b4 = s
-000169d0: 656c 662e 5f74 632e 696e 6469 7669 6475  elf._tc.individu
-000169e0: 616c 732e 6e75 6d5f 726f 7773 0a20 2020  als.num_rows.   
-000169f0: 2020 2020 2073 656c 662e 5f74 632e 756e       self._tc.un
-00016a00: 696f 6e28 736f 7572 6365 5f74 632c 0a20  ion(source_tc,. 
-00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a20: 2020 2020 2020 2020 2020 2023 204e 4f54             # NOT
-00016a30: 453a 2028 666f 7220 6e6f 7720 6174 206c  E: (for now at l
-00016a40: 6561 7374 2920 6173 7375 6d69 6e67 2020  east) assuming  
-00016a50: 7468 6520 696e 7472 6f64 7563 6564 0a20  the introduced. 
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a70: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00016a80: 2020 2069 6e64 6976 6964 7561 6c73 2063     individuals c
-00016a90: 6f6d 6520 6672 6f6d 2074 6f74 616c 6c79  ome from totally
-00016aa0: 2069 6e64 6570 2070 6f70 2c0a 2020 2020   indep pop,.    
-00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ac0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00016ad0: 646f 206e 6f74 2073 6861 7265 2061 204d  do not share a M
-00016ae0: 5243 4120 7769 7468 696e 206f 7572 2064  RCA within our d
-00016af0: 6174 612c 2061 6e64 20e2 88b4 2020 200a  ata, and ...   .
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b10: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00016b20: 2020 2020 6861 7665 206e 6f20 636f 6d6d      have no comm
-00016b30: 6f6e 206e 6f64 6573 2074 6861 7420 6e65  on nodes that ne
-00016b40: 6564 2074 6f20 6265 206d 6170 7065 642c  ed to be mapped,
-00016b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b60: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00016b70: 2020 2020 2068 656e 6365 2077 6520 7072       hence we pr
-00016b80: 6f76 6964 6520 6120 6c69 7374 206f 6620  ovide a list of 
-00016b90: 7473 6b69 742e 4e55 4c4c 730a 2020 2020  tskit.NULLs.    
-00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bb0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00016bc0: 746f 2075 6e69 6f6e 2829 2773 206e 6f64  to union()'s nod
-00016bd0: 655f 6d61 7070 696e 6720 6172 6775 6d65  e_mapping argume
-00016be0: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016c00: 6f64 655f 6d61 7070 696e 673d 5b74 736b  ode_mapping=[tsk
-00016c10: 6974 2e4e 554c 4c5d 202a 736f 7572 6365  it.NULL] *source
-00016c20: 5f74 632e 6e6f 6465 732e 6e75 6d5f 726f  _tc.nodes.num_ro
-00016c30: 7773 2c0a 2020 2020 2020 2020 2020 2020  ws,.            
-00016c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c50: 2320 4e4f 5445 3a20 706f 7075 6c61 7469  # NOTE: populati
-00016c60: 6f6e 7320 6f66 2074 6865 206e 6577 6c79  ons of the newly
-00016c70: 2061 6464 6564 206e 6f64 6573 0a20 2020   added nodes.   
-00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c90: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-00016ca0: 2077 696c 6c20 6265 2066 6c61 6767 6564   will be flagged
-00016cb0: 2062 7920 616e 2069 6e74 6567 6572 0a20   by an integer. 
+00016850: 2022 5461 626c 6543 6f6c 6c65 6374 696f   "TableCollectio
+00016860: 6e2e 696e 6469 7669 6475 616c 7320 220a  n.individuals ".
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016890: 2020 2020 2274 6162 6c65 2064 6f20 6e6f      "table do no
+000168a0: 7420 6167 7265 6520 7769 7468 2074 686f  t agree with tho
+000168b0: 7365 2073 6574 206f 6e20 7468 6520 220a  se set on the ".
+000168c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168e0: 2020 2020 2249 6e64 6976 6964 7561 6c73      "Individuals
+000168f0: 2074 6865 6d73 656c 7665 732e 2229 0a0a   themselves.")..
+00016900: 2020 2020 2020 2020 2320 736f 7274 2061          # sort a
+00016910: 6e64 2073 696d 706c 6966 7920 7468 6520  nd simplify the 
+00016920: 7473 6b69 742e 5461 626c 6543 6f6c 6c65  tskit.TableColle
+00016930: 6374 696f 6e0a 2020 2020 2020 2020 7365  ction.        se
+00016940: 6c66 2e5f 736f 7274 5f61 6e64 5f73 696d  lf._sort_and_sim
+00016950: 706c 6966 795f 7461 626c 655f 636f 6c6c  plify_table_coll
+00016960: 6563 7469 6f6e 2829 0a0a 2020 2020 2020  ection()..      
+00016970: 2020 2320 756e 696f 6e20 736f 7572 6365    # union source
+00016980: 2069 6e64 6976 6964 7561 6c73 2720 5461   individuals' Ta
+00016990: 626c 6543 6f6c 6c65 6374 696f 6e20 696e  bleCollection in
+000169a0: 746f 2074 6869 7320 5370 6563 6965 7327  to this Species'
+000169b0: 2054 6162 6c65 436f 6c6c 0a20 2020 2020   TableColl.     
+000169c0: 2020 206e 6f64 6573 5f74 6162 5f6c 656e     nodes_tab_len
+000169d0: 5f62 3420 3d20 7365 6c66 2e5f 7463 2e6e  _b4 = self._tc.n
+000169e0: 6f64 6573 2e6e 756d 5f72 6f77 730a 2020  odes.num_rows.  
+000169f0: 2020 2020 2020 696e 6469 7669 6473 5f74        individs_t
+00016a00: 6162 5f6c 656e 5f62 3420 3d20 7365 6c66  ab_len_b4 = self
+00016a10: 2e5f 7463 2e69 6e64 6976 6964 7561 6c73  ._tc.individuals
+00016a20: 2e6e 756d 5f72 6f77 730a 2020 2020 2020  .num_rows.      
+00016a30: 2020 7365 6c66 2e5f 7463 2e75 6e69 6f6e    self._tc.union
+00016a40: 2873 6f75 7263 655f 7463 2c0a 2020 2020  (source_tc,.    
+00016a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a60: 2020 2020 2020 2020 2320 4e4f 5445 3a20          # NOTE: 
+00016a70: 2866 6f72 206e 6f77 2061 7420 6c65 6173  (for now at leas
+00016a80: 7429 2061 7373 756d 696e 6720 2074 6865  t) assuming  the
+00016a90: 2069 6e74 726f 6475 6365 640a 2020 2020   introduced.    
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ab0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00016ac0: 696e 6469 7669 6475 616c 7320 636f 6d65  individuals come
+00016ad0: 2066 726f 6d20 746f 7461 6c6c 7920 696e   from totally in
+00016ae0: 6465 7020 706f 702c 0a20 2020 2020 2020  dep pop,.       
+00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b00: 2020 2020 2023 2020 2020 2020 2064 6f20       #       do 
+00016b10: 6e6f 7420 7368 6172 6520 6120 4d52 4341  not share a MRCA
+00016b20: 2077 6974 6869 6e20 6f75 7220 6461 7461   within our data
+00016b30: 2c20 616e 6420 e288 b420 2020 0a20 2020  , and ...   .   
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+00016b60: 2068 6176 6520 6e6f 2063 6f6d 6d6f 6e20   have no common 
+00016b70: 6e6f 6465 7320 7468 6174 206e 6565 6420  nodes that need 
+00016b80: 746f 2062 6520 6d61 7070 6564 2c0a 2020  to be mapped,.  
+00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ba0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00016bb0: 2020 6865 6e63 6520 7765 2070 726f 7669    hence we provi
+00016bc0: 6465 2061 206c 6973 7420 6f66 2074 736b  de a list of tsk
+00016bd0: 6974 2e4e 554c 4c73 0a20 2020 2020 2020  it.NULLs.       
+00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bf0: 2020 2020 2023 2020 2020 2020 2074 6f20       #       to 
+00016c00: 756e 696f 6e28 2927 7320 6e6f 6465 5f6d  union()'s node_m
+00016c10: 6170 7069 6e67 2061 7267 756d 656e 740a  apping argument.
+00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c30: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00016c40: 5f6d 6170 7069 6e67 3d5b 7473 6b69 742e  _mapping=[tskit.
+00016c50: 4e55 4c4c 5d20 2a73 6f75 7263 655f 7463  NULL] *source_tc
+00016c60: 2e6e 6f64 6573 2e6e 756d 5f72 6f77 732c  .nodes.num_rows,
+00016c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c80: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+00016c90: 4f54 453a 2070 6f70 756c 6174 696f 6e73  OTE: populations
+00016ca0: 206f 6620 7468 6520 6e65 776c 7920 6164   of the newly ad
+00016cb0: 6465 6420 6e6f 6465 730a 2020 2020 2020  ded nodes.      
 00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00016ce0: 2020 2074 6861 7420 6973 2031 2067 7265     that is 1 gre
-00016cf0: 6174 6572 2074 6861 6e20 7468 6520 6c61  ater than the la
-00016d00: 7267 6573 740a 2020 2020 2020 2020 2020  rgest.          
-00016d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d20: 2020 2320 2020 2020 2020 706f 7075 6c61    #       popula
-00016d30: 7469 6f6e 2d66 6c61 6720 696e 7465 6765  tion-flag intege
-00016d40: 7220 696e 0a20 2020 2020 2020 2020 2020  r in.           
-00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d60: 2023 2020 2020 2020 2074 6865 2070 7265   #       the pre
-00016d70: 2d69 6e74 726f 6475 6374 696f 6e20 5461  -introduction Ta
-00016d80: 626c 6543 6f6c 6c65 6374 696f 6e0a 2020  bleCollection.  
-00016d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016da0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00016db0: 2020 6f66 2074 6869 7320 5370 6563 6965    of this Specie
-00016dc0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00016de0: 645f 706f 7075 6c61 7469 6f6e 733d 5472  d_populations=Tr
-00016df0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00016cd0: 2020 2020 2020 2320 2020 2020 2020 7769        #       wi
+00016ce0: 6c6c 2062 6520 666c 6167 6765 6420 6279  ll be flagged by
+00016cf0: 2061 6e20 696e 7465 6765 720a 2020 2020   an integer.    
+00016d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d10: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00016d20: 7468 6174 2069 7320 3120 6772 6561 7465  that is 1 greate
+00016d30: 7220 7468 616e 2074 6865 206c 6172 6765  r than the large
+00016d40: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
+00016d50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00016d60: 2020 2020 2020 2070 6f70 756c 6174 696f         populatio
+00016d70: 6e2d 666c 6167 2069 6e74 6567 6572 2069  n-flag integer i
+00016d80: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00016d90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00016da0: 2020 2020 2020 7468 6520 7072 652d 696e        the pre-in
+00016db0: 7472 6f64 7563 7469 6f6e 2054 6162 6c65  troduction Table
+00016dc0: 436f 6c6c 6563 7469 6f6e 0a20 2020 2020  Collection.     
+00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016de0: 2020 2020 2020 2023 2020 2020 2020 206f         #       o
+00016df0: 6620 7468 6973 2053 7065 6369 6573 0a20  f this Species. 
 00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e10: 2320 4e4f 5445 3a20 6265 7374 2074 6f20  # NOTE: best to 
-00016e20: 6a75 7374 2061 6c6c 6f77 2069 7420 746f  just allow it to
-00016e30: 2064 6f20 7468 6973 2c0a 2020 2020 2020   do this,.      
-00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e50: 2020 2020 2020 2320 2020 2020 2020 696e        #       in
-00016e60: 2063 6173 6520 7765 2067 656e 6572 616c   case we general
-00016e70: 697a 6520 7468 696e 6773 206c 6174 6572  ize things later
-00016e80: 206f 6e2c 0a20 2020 2020 2020 2020 2020   on,.           
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2023 2020 2020 2020 2062 7574 2066 6f72   #       but for
-00016eb0: 206e 6f77 2074 6865 7265 2077 696c 6c20   now there will 
-00016ec0: 6163 7475 616c 6c79 2062 650a 2020 2020  actually be.    
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ee0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00016ef0: 6e6f 7468 696e 6720 746f 2063 6865 636b  nothing to check
-00016f00: 2062 6563 6175 7365 2077 6520 6173 7375   because we assu
-00016f10: 6d65 200a 2020 2020 2020 2020 2020 2020  me .            
-00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f30: 2320 2020 2020 2020 6e6f 2073 6861 7265  #       no share
-00016f40: 6420 6e6f 6465 7320 6265 7477 6565 6e0a  d nodes between.
-00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f60: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00016f70: 2020 2020 736f 7572 6365 2061 6e64 2072      source and r
-00016f80: 6563 6970 6965 6e74 2054 6162 6c65 436f  ecipient TableCo
-00016f90: 6c6c 6563 7469 6f6e 730a 2020 2020 2020  llections.      
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 2320 544f 444f 3a20 484f        # TODO: HO
-00016fc0: 5745 5645 522c 2045 5155 414c 4954 5920  WEVER, EQUALITY 
-00016fd0: 4348 4543 4b20 5354 494c 4c20 4641 494c  CHECK STILL FAIL
-00016fe0: 5321 2057 4859 3f0a 2020 2020 2020 2020  S! WHY?.        
-00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017000: 2020 2020 6368 6563 6b5f 7368 6172 6564      check_shared
-00017010: 5f65 7175 616c 6974 793d 4661 6c73 652c  _equality=False,
-00017020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017030: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-00017040: 4f54 453a 2073 686f 756c 6420 636f 7079  OTE: should copy
-00017050: 2070 726f 7665 6e61 6e63 6520 696e 666f   provenance info
-00017060: 206f 7665 720a 2020 2020 2020 2020 2020   over.          
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 2020 2320 2020 2020 2020 6672 6f6d 2074    #       from t
-00017090: 6865 2073 6f75 7263 6520 496e 6469 7669  he source Indivi
-000170a0: 6475 616c 7327 2054 6162 6c65 436f 6c6c  duals' TableColl
-000170b0: 6563 7469 6f6e 0a20 2020 2020 2020 2020  ection.         
-000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170d0: 2020 2023 2020 2020 2020 2074 6f20 7468     #       to th
-000170e0: 6174 206f 6620 7468 6520 7265 6365 6970  at of the receip
-000170f0: 6965 6e74 2053 7065 6369 6573 0a20 2020  ient Species.   
+00016e10: 2020 2020 2020 2020 2020 2061 6464 5f70             add_p
+00016e20: 6f70 756c 6174 696f 6e73 3d54 7275 652c  opulations=True,
+00016e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016e40: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+00016e50: 4f54 453a 2062 6573 7420 746f 206a 7573  OTE: best to jus
+00016e60: 7420 616c 6c6f 7720 6974 2074 6f20 646f  t allow it to do
+00016e70: 2074 6869 732c 0a20 2020 2020 2020 2020   this,.         
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 2020 2023 2020 2020 2020 2069 6e20 6361     #       in ca
+00016ea0: 7365 2077 6520 6765 6e65 7261 6c69 7a65  se we generalize
+00016eb0: 2074 6869 6e67 7320 6c61 7465 7220 6f6e   things later on
+00016ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00016ee0: 2020 2020 2020 6275 7420 666f 7220 6e6f        but for no
+00016ef0: 7720 7468 6572 6520 7769 6c6c 2061 6374  w there will act
+00016f00: 7561 6c6c 7920 6265 0a20 2020 2020 2020  ually be.       
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 2020 2020 2023 2020 2020 2020 206e 6f74       #       not
+00016f30: 6869 6e67 2074 6f20 6368 6563 6b20 6265  hing to check be
+00016f40: 6361 7573 6520 7765 2061 7373 756d 6520  cause we assume 
+00016f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016f60: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+00016f70: 2020 2020 206e 6f20 7368 6172 6564 206e       no shared n
+00016f80: 6f64 6573 2062 6574 7765 656e 0a20 2020  odes between.   
+00016f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fa0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+00016fb0: 2073 6f75 7263 6520 616e 6420 7265 6369   source and reci
+00016fc0: 7069 656e 7420 5461 626c 6543 6f6c 6c65  pient TableColle
+00016fd0: 6374 696f 6e73 0a20 2020 2020 2020 2020  ctions.         
+00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ff0: 2020 2023 2054 4f44 4f3a 2048 4f57 4556     # TODO: HOWEV
+00017000: 4552 2c20 4551 5541 4c49 5459 2043 4845  ER, EQUALITY CHE
+00017010: 434b 2053 5449 4c4c 2046 4149 4c53 2120  CK STILL FAILS! 
+00017020: 5748 593f 0a20 2020 2020 2020 2020 2020  WHY?.           
+00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017040: 2063 6865 636b 5f73 6861 7265 645f 6571   check_shared_eq
+00017050: 7561 6c69 7479 3d46 616c 7365 2c0a 2020  uality=False,.  
+00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017070: 2020 2020 2020 2020 2020 2320 4e4f 5445            # NOTE
+00017080: 3a20 7368 6f75 6c64 2063 6f70 7920 7072  : should copy pr
+00017090: 6f76 656e 616e 6365 2069 6e66 6f20 6f76  ovenance info ov
+000170a0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+000170b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000170c0: 2020 2020 2020 2066 726f 6d20 7468 6520         from the 
+000170d0: 736f 7572 6365 2049 6e64 6976 6964 7561  source Individua
+000170e0: 6c73 2720 5461 626c 6543 6f6c 6c65 6374  ls' TableCollect
+000170f0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
 00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017110: 2020 2020 2020 2020 2072 6563 6f72 645f           record_
-00017120: 7072 6f76 656e 616e 6365 3d54 7275 652c  provenance=True,
-00017130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017110: 2320 2020 2020 2020 746f 2074 6861 7420  #       to that 
+00017120: 6f66 2074 6865 2072 6563 6569 7069 656e  of the receipien
+00017130: 7420 5370 6563 6965 730a 2020 2020 2020  t Species.      
 00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 290a 2020 2020 2020 2020 6e6f 6465    ).        node
-00017160: 735f 7461 625f 6c65 6e5f 6166 203d 2073  s_tab_len_af = s
-00017170: 656c 662e 5f74 632e 6e6f 6465 732e 6e75  elf._tc.nodes.nu
-00017180: 6d5f 726f 7773 0a20 2020 2020 2020 2069  m_rows.        i
-00017190: 6e64 6976 6964 735f 7461 625f 6c65 6e5f  ndivids_tab_len_
-000171a0: 6166 203d 2073 656c 662e 5f74 632e 696e  af = self._tc.in
-000171b0: 6469 7669 6475 616c 732e 6e75 6d5f 726f  dividuals.num_ro
-000171c0: 7773 0a0a 2020 2020 2020 2020 2320 6368  ws..        # ch
-000171d0: 6563 6b20 756e 696f 6e65 6420 7461 626c  eck unioned tabl
-000171e0: 6573 2068 6176 6520 636f 7272 6563 7420  es have correct 
-000171f0: 6c65 6e67 7468 730a 2020 2020 2020 2020  lengths.        
-00017200: 6173 7365 7274 2028 6e6f 6465 735f 7461  assert (nodes_ta
-00017210: 625f 6c65 6e5f 6166 202d 206e 6f64 6573  b_len_af - nodes
-00017220: 5f74 6162 5f6c 656e 5f62 3429 203d 3d20  _tab_len_b4) == 
-00017230: 736f 7572 6365 5f74 632e 6e6f 6465 732e  source_tc.nodes.
-00017240: 6e75 6d5f 726f 7773 0a20 2020 2020 2020  num_rows.       
-00017250: 2061 7373 6572 7420 2828 696e 6469 7669   assert ((indivi
-00017260: 6473 5f74 6162 5f6c 656e 5f61 6620 2d20  ds_tab_len_af - 
-00017270: 696e 6469 7669 6473 5f74 6162 5f6c 656e  individs_tab_len
-00017280: 5f62 3429 203d 3d0a 2020 2020 2020 2020  _b4) ==.        
-00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172b0: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
-000172c0: 632e 696e 6469 7669 6475 616c 732e 6e75  c.individuals.nu
-000172d0: 6d5f 726f 7773 290a 0a20 2020 2020 2020  m_rows)..       
-000172e0: 2023 2063 6865 636b 2074 6861 7420 616c   # check that al
-000172f0: 6c20 676e 7820 6964 7873 2073 746f 7265  l gnx idxs store
-00017300: 6420 696e 2074 6865 2069 6e64 6976 6964  d in the individ
-00017310: 7561 6c73 2074 6162 6c65 2773 0a20 2020  uals table's.   
-00017320: 2020 2020 2023 206d 6574 6164 6174 6120       # metadata 
-00017330: 636f 6c75 6d6e 206f 6363 7572 206f 6e6c  column occur onl
-00017340: 7920 6f6e 6365 2028 6173 6964 6520 6672  y once (aside fr
-00017350: 6f6d 2030 2c0a 2020 2020 2020 2020 2320  om 0,.        # 
-00017360: 7768 6963 6820 6973 2061 206e 756c 6c20  which is a null 
-00017370: 7661 6c75 6520 666f 7220 696e 6469 7669  value for indivi
-00017380: 6475 616c 7320 7468 6174 0a20 2020 2020  duals that.     
-00017390: 2020 2023 206e 6576 6572 2065 7869 7374     # never exist
-000173a0: 6564 2061 7320 2772 6561 6c27 2067 6e78  ed as 'real' gnx
-000173b0: 2049 6e64 6976 6964 7561 6c20 6f62 6a65   Individual obje
-000173c0: 6374 7320 6265 6361 7573 650a 2020 2020  cts because.    
-000173d0: 2020 2020 2320 7468 6579 2077 6572 6520      # they were 
-000173e0: 696e 2074 6865 2070 6173 7420 6f66 2061  in the past of a
-000173f0: 2063 6f61 6c65 7363 656e 7420 7369 6d75   coalescent simu
-00017400: 6c61 7469 6f6e 290a 2020 2020 2020 2020  lation).        
-00017410: 7265 6369 705f 7463 5f69 6e64 6976 6964  recip_tc_individ
-00017420: 7561 6c73 5f69 6473 203d 205b 696e 742e  uals_ids = [int.
-00017430: 6672 6f6d 5f62 7974 6573 280a 2020 2020  from_bytes(.    
-00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2020 2020 2020 7365 6c66 2e5f 7463          self._tc
-00017460: 2e69 6e64 6976 6964 7561 6c73 5b69 5d2e  .individuals[i].
-00017470: 6d65 7461 6461 7461 2c20 276c 6974 746c  metadata, 'littl
-00017480: 6527 2920 666f 720a 2020 2020 2020 2020  e') for.        
-00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174a0: 2020 2020 2020 2020 6920 696e 2072 616e          i in ran
-000174b0: 6765 2873 656c 662e 5f74 632e 696e 6469  ge(self._tc.indi
-000174c0: 7669 6475 616c 732e 6e75 6d5f 726f 7773  viduals.num_rows
-000174d0: 295d 0a20 2020 2020 2020 2061 7373 6572  )].        asser
-000174e0: 7420 286c 656e 2872 6563 6970 5f74 635f  t (len(recip_tc_
-000174f0: 696e 6469 7669 6475 616c 735f 6964 7329  individuals_ids)
-00017500: 203d 3d0a 2020 2020 2020 2020 2020 2020   ==.            
-00017510: 2020 2020 7365 6c66 2e5f 7463 2e69 6e64      self._tc.ind
-00017520: 6976 6964 7561 6c73 2e6e 756d 5f72 6f77  ividuals.num_row
-00017530: 7329 0a20 2020 2020 2020 2063 6f75 6e74  s).        count
-00017540: 7320 3d20 4328 7265 6369 705f 7463 5f69  s = C(recip_tc_i
-00017550: 6e64 6976 6964 7561 6c73 5f69 6473 290a  ndividuals_ids).
-00017560: 2020 2020 2020 2020 666f 7220 6b2c 2076          for k, v
-00017570: 2069 6e20 636f 756e 7473 2e69 7465 6d73   in counts.items
-00017580: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00017590: 6966 206b 2021 3d20 303a 0a20 2020 2020  if k != 0:.     
-000175a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-000175b0: 7420 7620 3d3d 2031 2c20 2866 2267 6e78  t v == 1, (f"gnx
-000175c0: 2049 6e64 6976 6964 7561 6c20 6964 7820   Individual idx 
-000175d0: 7b69 7d20 6f63 6375 7273 206d 6f72 6520  {i} occurs more 
-000175e0: 7468 616e 206f 6e63 6520 220a 2020 2020  than once ".    
-000175f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017600: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-00017610: 2074 6865 206d 6574 6164 6174 6120 636f   the metadata co
-00017620: 6c75 6d6e 206f 6620 7468 6520 756e 696f  lumn of the unio
-00017630: 6e20 6f66 2022 0a20 2020 2020 2020 2020  n of ".         
-00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017650: 2020 2020 2020 2020 2274 6865 2072 6563          "the rec
-00017660: 6970 6965 6e74 2061 6e64 2073 6f75 7263  ipient and sourc
-00017670: 6520 5370 6563 6965 7327 2022 0a20 2020  e Species' ".   
+00017150: 2020 2020 2020 7265 636f 7264 5f70 726f        record_pro
+00017160: 7665 6e61 6e63 653d 5472 7565 2c0a 2020  venance=True,.  
+00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017180: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00017190: 0a20 2020 2020 2020 206e 6f64 6573 5f74  .        nodes_t
+000171a0: 6162 5f6c 656e 5f61 6620 3d20 7365 6c66  ab_len_af = self
+000171b0: 2e5f 7463 2e6e 6f64 6573 2e6e 756d 5f72  ._tc.nodes.num_r
+000171c0: 6f77 730a 2020 2020 2020 2020 696e 6469  ows.        indi
+000171d0: 7669 6473 5f74 6162 5f6c 656e 5f61 6620  vids_tab_len_af 
+000171e0: 3d20 7365 6c66 2e5f 7463 2e69 6e64 6976  = self._tc.indiv
+000171f0: 6964 7561 6c73 2e6e 756d 5f72 6f77 730a  iduals.num_rows.
+00017200: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
+00017210: 2075 6e69 6f6e 6564 2074 6162 6c65 7320   unioned tables 
+00017220: 6861 7665 2063 6f72 7265 6374 206c 656e  have correct len
+00017230: 6774 6873 0a20 2020 2020 2020 2061 7373  gths.        ass
+00017240: 6572 7420 286e 6f64 6573 5f74 6162 5f6c  ert (nodes_tab_l
+00017250: 656e 5f61 6620 2d20 6e6f 6465 735f 7461  en_af - nodes_ta
+00017260: 625f 6c65 6e5f 6234 2920 3d3d 2073 6f75  b_len_b4) == sou
+00017270: 7263 655f 7463 2e6e 6f64 6573 2e6e 756d  rce_tc.nodes.num
+00017280: 5f72 6f77 730a 2020 2020 2020 2020 6173  _rows.        as
+00017290: 7365 7274 2028 2869 6e64 6976 6964 735f  sert ((individs_
+000172a0: 7461 625f 6c65 6e5f 6166 202d 2069 6e64  tab_len_af - ind
+000172b0: 6976 6964 735f 7461 625f 6c65 6e5f 6234  ivids_tab_len_b4
+000172c0: 2920 3d3d 0a20 2020 2020 2020 2020 2020  ) ==.           
+000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172f0: 2020 2020 2073 6f75 7263 655f 7463 2e69       source_tc.i
+00017300: 6e64 6976 6964 7561 6c73 2e6e 756d 5f72  ndividuals.num_r
+00017310: 6f77 7329 0a0a 2020 2020 2020 2020 2320  ows)..        # 
+00017320: 6368 6563 6b20 7468 6174 2061 6c6c 2067  check that all g
+00017330: 6e78 2069 6478 7320 7374 6f72 6564 2069  nx idxs stored i
+00017340: 6e20 7468 6520 696e 6469 7669 6475 616c  n the individual
+00017350: 7320 7461 626c 6527 730a 2020 2020 2020  s table's.      
+00017360: 2020 2320 6d65 7461 6461 7461 2063 6f6c    # metadata col
+00017370: 756d 6e20 6f63 6375 7220 6f6e 6c79 206f  umn occur only o
+00017380: 6e63 6520 2861 7369 6465 2066 726f 6d20  nce (aside from 
+00017390: 302c 0a20 2020 2020 2020 2023 2077 6869  0,.        # whi
+000173a0: 6368 2069 7320 6120 6e75 6c6c 2076 616c  ch is a null val
+000173b0: 7565 2066 6f72 2069 6e64 6976 6964 7561  ue for individua
+000173c0: 6c73 2074 6861 740a 2020 2020 2020 2020  ls that.        
+000173d0: 2320 6e65 7665 7220 6578 6973 7465 6420  # never existed 
+000173e0: 6173 2027 7265 616c 2720 676e 7820 496e  as 'real' gnx In
+000173f0: 6469 7669 6475 616c 206f 626a 6563 7473  dividual objects
+00017400: 2062 6563 6175 7365 0a20 2020 2020 2020   because.       
+00017410: 2023 2074 6865 7920 7765 7265 2069 6e20   # they were in 
+00017420: 7468 6520 7061 7374 206f 6620 6120 636f  the past of a co
+00017430: 616c 6573 6365 6e74 2073 696d 756c 6174  alescent simulat
+00017440: 696f 6e29 0a20 2020 2020 2020 2072 6563  ion).        rec
+00017450: 6970 5f74 635f 696e 6469 7669 6475 616c  ip_tc_individual
+00017460: 735f 6964 7320 3d20 5b69 6e74 2e66 726f  s_ids = [int.fro
+00017470: 6d5f 6279 7465 7328 0a20 2020 2020 2020  m_bytes(.       
+00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017490: 2020 2020 2073 656c 662e 5f74 632e 696e       self._tc.in
+000174a0: 6469 7669 6475 616c 735b 695d 2e6d 6574  dividuals[i].met
+000174b0: 6164 6174 612c 2027 6c69 7474 6c65 2729  adata, 'little')
+000174c0: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
+000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174e0: 2020 2020 2069 2069 6e20 7261 6e67 6528       i in range(
+000174f0: 7365 6c66 2e5f 7463 2e69 6e64 6976 6964  self._tc.individ
+00017500: 7561 6c73 2e6e 756d 5f72 6f77 7329 5d0a  uals.num_rows)].
+00017510: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+00017520: 6c65 6e28 7265 6369 705f 7463 5f69 6e64  len(recip_tc_ind
+00017530: 6976 6964 7561 6c73 5f69 6473 2920 3d3d  ividuals_ids) ==
+00017540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017550: 2073 656c 662e 5f74 632e 696e 6469 7669   self._tc.indivi
+00017560: 6475 616c 732e 6e75 6d5f 726f 7773 290a  duals.num_rows).
+00017570: 2020 2020 2020 2020 636f 756e 7473 203d          counts =
+00017580: 2043 2872 6563 6970 5f74 635f 696e 6469   C(recip_tc_indi
+00017590: 7669 6475 616c 735f 6964 7329 0a20 2020  viduals_ids).   
+000175a0: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
+000175b0: 2063 6f75 6e74 732e 6974 656d 7328 293a   counts.items():
+000175c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000175d0: 6b20 213d 2030 3a0a 2020 2020 2020 2020  k != 0:.        
+000175e0: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
+000175f0: 203d 3d20 312c 2028 6622 676e 7820 496e   == 1, (f"gnx In
+00017600: 6469 7669 6475 616c 2069 6478 207b 697d  dividual idx {i}
+00017610: 206f 6363 7572 7320 6d6f 7265 2074 6861   occurs more tha
+00017620: 6e20 6f6e 6365 2022 0a20 2020 2020 2020  n once ".       
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2020 2020 2020 2020 2269 6e20 7468            "in th
+00017650: 6520 6d65 7461 6461 7461 2063 6f6c 756d  e metadata colum
+00017660: 6e20 6f66 2074 6865 2075 6e69 6f6e 206f  n of the union o
+00017670: 6620 220a 2020 2020 2020 2020 2020 2020  f ".            
 00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 2020 2020 2020 2020 2020 2020 2020 2254                "T
-000176a0: 6162 6c65 436f 6c6c 6563 7469 6f6e 7320  ableCollections 
-000176b0: 696e 6469 7669 6475 616c 7320 7461 626c  individuals tabl
-000176c0: 6573 2e22 290a 0a20 2020 2020 2020 2023  es.")..        #
-000176d0: 2061 6464 2069 6e20 7468 6520 496e 6469   add in the Indi
-000176e0: 7669 6475 616c 732c 206b 6579 6564 2062  viduals, keyed b
-000176f0: 7920 6964 780a 2020 2020 2020 2020 706f  y idx.        po
-00017700: 705f 7369 7a65 5f62 3420 3d20 6c65 6e28  p_size_b4 = len(
-00017710: 7365 6c66 290a 2020 2020 2020 2020 666f  self).        fo
-00017720: 7220 696e 6420 696e 2069 6e64 6976 6964  r ind in individ
-00017730: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00017740: 656c 665b 696e 642e 6964 785d 203d 2069  elf[ind.idx] = i
-00017750: 6e64 0a20 2020 2020 2020 2070 6f70 5f73  nd.        pop_s
-00017760: 697a 655f 6166 203d 206c 656e 2873 656c  ize_af = len(sel
-00017770: 6629 0a20 2020 2020 2020 2061 7373 6572  f).        asser
-00017780: 7420 2870 6f70 5f73 697a 655f 6166 202d  t (pop_size_af -
-00017790: 2070 6f70 5f73 697a 655f 6234 2920 3d3d   pop_size_b4) ==
-000177a0: 206c 656e 2869 6e64 6976 6964 7329 2c20   len(individs), 
-000177b0: 2822 496e 636f 7272 6563 7420 6e75 6d62  ("Incorrect numb
-000177c0: 6572 220a 2020 2020 2020 2020 2020 2020  er".            
-000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177e0: 2020 2020 2220 6f66 2049 6e64 6976 6964      " of Individ
-000177f0: 7561 6c73 2061 6464 6564 2074 6f20 7265  uals added to re
-00017800: 6369 7069 656e 7420 5370 6563 6965 732e  cipient Species.
-00017810: 2229 0a0a 2020 2020 2020 2020 2320 7570  ")..        # up
-00017820: 6461 7465 2065 6163 6820 496e 6469 7669  date each Indivi
-00017830: 6475 616c 2773 205f 696e 6469 7669 6475  dual's _individu
-00017840: 616c 735f 7461 625f 6964 2061 6e64 205f  als_tab_id and _
-00017850: 6e6f 6465 735f 7461 625f 6964 730a 2020  nodes_tab_ids.  
-00017860: 2020 2020 2020 2320 746f 206d 6174 6368        # to match
-00017870: 2074 6865 206e 6577 2c20 756e 696f 6e65   the new, unione
-00017880: 6420 5461 626c 6543 6f6c 6c65 6374 696f  d TableCollectio
-00017890: 6e0a 2020 2020 2020 2020 6e6f 6465 735f  n.        nodes_
-000178a0: 7461 625f 696e 6469 7669 6475 616c 7320  tab_individuals 
-000178b0: 3d20 7365 6c66 2e5f 7463 2e6e 6f64 6573  = self._tc.nodes
-000178c0: 2e69 6e64 6976 6964 7561 6c0a 2020 2020  .individual.    
-000178d0: 2020 2020 666f 7220 6964 782c 2069 6e64      for idx, ind
-000178e0: 2069 6e20 7365 6c66 2e69 7465 6d73 2829   in self.items()
-000178f0: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-00017900: 6469 7669 6475 616c 735f 7461 625f 6964  dividuals_tab_id
-00017910: 203d 206e 702e 6172 6777 6865 7265 280a   = np.argwhere(.
-00017920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017930: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-00017940: 7272 6179 2872 6563 6970 5f74 635f 696e  rray(recip_tc_in
-00017950: 6469 7669 6475 616c 735f 6964 7329 203d  dividuals_ids) =
-00017960: 3d20 6964 7829 2e72 6176 656c 2829 0a20  = idx).ravel(). 
-00017970: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00017980: 7420 6c65 6e28 696e 6469 7669 6475 616c  t len(individual
-00017990: 735f 7461 625f 6964 2920 3d3d 2031 0a20  s_tab_id) == 1. 
-000179a0: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
-000179b0: 6964 7561 6c73 5f74 6162 5f69 6420 3d20  iduals_tab_id = 
-000179c0: 696e 6469 7669 6475 616c 735f 7461 625f  individuals_tab_
-000179d0: 6964 5b30 5d0a 2020 2020 2020 2020 2020  id[0].          
-000179e0: 2020 696e 642e 5f69 6e64 6976 6964 7561    ind._individua
-000179f0: 6c73 5f74 6162 5f69 6420 3d20 696e 6469  ls_tab_id = indi
-00017a00: 7669 6475 616c 735f 7461 625f 6964 0a20  viduals_tab_id. 
-00017a10: 2020 2020 2020 2020 2020 206e 6f64 6573             nodes
-00017a20: 5f74 6162 5f69 6473 203d 206e 702e 6172  _tab_ids = np.ar
-00017a30: 6777 6865 7265 286e 6f64 6573 5f74 6162  gwhere(nodes_tab
-00017a40: 5f69 6e64 6976 6964 7561 6c73 203d 3d0a  _individuals ==.
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a70: 2020 2020 2020 2020 696e 6469 7669 6475          individu
-00017a80: 616c 735f 7461 625f 6964 292e 7261 7665  als_tab_id).rave
-00017a90: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
-00017aa0: 6173 7365 7274 206c 656e 286e 6f64 6573  assert len(nodes
-00017ab0: 5f74 6162 5f69 6473 2920 3d3d 2032 0a20  _tab_ids) == 2. 
-00017ac0: 2020 2020 2020 2020 2020 2069 6e64 2e5f             ind._
-00017ad0: 6e6f 6465 735f 7461 625f 6964 7320 3d20  nodes_tab_ids = 
-00017ae0: 7b69 3a20 6964 2066 6f72 2069 2c20 6964  {i: id for i, id
-00017af0: 2069 6e20 656e 756d 6572 6174 6528 6e6f   in enumerate(no
-00017b00: 6465 735f 7461 625f 6964 7329 7d0a 0a20  des_tab_ids)}.. 
-00017b10: 2020 2020 2020 2023 2066 696e 616c 2063         # final c
-00017b20: 6865 636b 2074 6861 7420 696e 6469 6365  heck that indice
-00017b30: 7320 6368 6563 6b20 6f75 7420 696e 2074  s check out in t
-00017b40: 6865 206f 7468 6572 2064 6972 6563 7469  he other directi
-00017b50: 6f6e 0a20 2020 2020 2020 2023 2028 692e  on.        # (i.
-00017b60: 652e 2c20 6672 6f6d 206e 6f64 6573 2074  e., from nodes t
-00017b70: 6162 2074 6f20 696e 6469 7669 6475 616c  ab to individual
-00017b80: 7320 7461 6220 746f 2067 6e78 2049 6e64  s tab to gnx Ind
-00017b90: 6976 6964 7561 6c73 0a20 2020 2020 2020  ividuals.       
-00017ba0: 2023 2061 6e64 2074 6861 7420 6e6f 6465   # and that node
-00017bb0: 7320 6964 7320 6368 6563 6b20 6f75 7420  s ids check out 
-00017bc0: 746f 6f0a 2020 2020 2020 2020 6375 7272  too.        curr
-00017bd0: 5f6e 6f64 655f 6374 203d 2030 0a20 2020  _node_ct = 0.   
-00017be0: 2020 2020 2066 6f72 206e 6f64 655f 6964       for node_id
-00017bf0: 2c20 6e6f 6465 2069 6e20 656e 756d 6572  , node in enumer
-00017c00: 6174 6528 7365 6c66 2e5f 7463 2e6e 6f64  ate(self._tc.nod
-00017c10: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00017c20: 2023 204e 4f54 453a 2069 676e 6f72 6520   # NOTE: ignore 
-00017c30: 2d31 733b 2074 6865 7920 6172 6520 6d73  -1s; they are ms
-00017c40: 7072 696d 6520 666c 6167 7320 666f 7220  prime flags for 
-00017c50: 6e6f 6e2d 7361 6d70 6c65 206e 6f64 6573  non-sample nodes
-00017c60: 2062 7574 0a20 2020 2020 2020 2020 2020   but.           
-00017c70: 2023 2020 2020 2020 2062 6561 6876 6520   #       beahve 
-00017c80: 6173 2061 2050 7974 686f 6e20 696e 6465  as a Python inde
-00017c90: 7865 7220 6f66 2074 6865 206c 6173 7420  xer of the last 
-00017ca0: 496e 6469 7669 6475 616c 2069 6e20 7468  Individual in th
-00017cb0: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-00017cc0: 2020 2020 2020 5370 6563 6965 7320 616e        Species an
-00017cd0: 6420 7468 7573 2074 6872 6f77 2061 6e20  d thus throw an 
-00017ce0: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
-00017cf0: 2020 6966 206e 6f64 652e 696e 6469 7669    if node.indivi
-00017d00: 6475 616c 2021 3d20 2d31 3a0a 2020 2020  dual != -1:.    
-00017d10: 2020 2020 2020 2020 2020 2020 676e 785f              gnx_
-00017d20: 696e 6469 7669 6475 616c 5f69 6420 3d20  individual_id = 
-00017d30: 696e 742e 6672 6f6d 5f62 7974 6573 2873  int.from_bytes(s
-00017d40: 656c 662e 5f74 632e 696e 6469 7669 6475  elf._tc.individu
-00017d50: 616c 735b 0a20 2020 2020 2020 2020 2020  als[.           
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d80: 206e 6f64 652e 696e 6469 7669 6475 616c   node.individual
-00017d90: 5d2e 6d65 7461 6461 7461 2c20 276c 6974  ].metadata, 'lit
-00017da0: 746c 6527 290a 2020 2020 2020 2020 2020  tle').          
-00017db0: 2020 2020 2020 6966 2067 6e78 5f69 6e64        if gnx_ind
-00017dc0: 6976 6964 7561 6c5f 6964 2069 6e20 5b2a  ividual_id in [*
-00017dd0: 7365 6c66 5d3a 0a20 2020 2020 2020 2020  self]:.         
-00017de0: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
-00017df0: 6e6f 6465 5f63 7420 2b3d 2031 0a20 2020  node_ct += 1.   
-00017e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e10: 2061 7373 6572 7420 2873 656c 665b 676e   assert (self[gn
-00017e20: 785f 696e 6469 7669 6475 616c 5f69 645d  x_individual_id]
-00017e30: 2e5f 696e 6469 7669 6475 616c 735f 7461  ._individuals_ta
-00017e40: 625f 6964 203d 3d0a 2020 2020 2020 2020  b_id ==.        
-00017e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e60: 2020 2020 6e6f 6465 2e69 6e64 6976 6964      node.individ
-00017e70: 7561 6c20 616e 6420 6e6f 6465 5f69 6420  ual and node_id 
-00017e80: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
-00017e90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017ea0: 656c 665b 676e 785f 696e 6469 7669 6475  elf[gnx_individu
-00017eb0: 616c 5f69 645d 2e5f 6e6f 6465 735f 7461  al_id]._nodes_ta
-00017ec0: 625f 6964 732e 7661 6c75 6573 2829 290a  b_ids.values()).
-00017ed0: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
-00017ee0: 7572 725f 6e6f 6465 5f63 7420 3d3d 2032  urr_node_ct == 2
-00017ef0: 2a6c 656e 2873 656c 6629 2c20 2822 4e75  *len(self), ("Nu
-00017f00: 6d62 6572 206f 6620 6375 7272 656e 7420  mber of current 
-00017f10: 496e 6469 7669 6475 616c 7320 220a 2020  Individuals ".  
-00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-00017f50: 2074 6865 2072 6563 6970 6965 6e74 2053   the recipient S
-00017f60: 7065 6369 6573 2064 6f65 7320 6e6f 7420  pecies does not 
-00017f70: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fa0: 2022 6d61 7463 6820 7468 6520 6e75 6d62   "match the numb
-00017fb0: 6572 2065 7870 6563 7465 6420 6261 7365  er expected base
-00017fc0: 6420 6f6e 2022 0a20 2020 2020 2020 2020  d on ".         
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ff0: 2020 2020 2020 2254 6162 6c65 436f 6c6c        "TableColl
-00018000: 6563 7469 6f6e 2063 6f6e 7465 6e74 732e  ection contents.
-00018010: 2229 0a0a 2020 2020 2020 2020 2320 736f  ")..        # so
-00018020: 7274 2061 6e64 2073 696d 706c 6966 7920  rt and simplify 
-00018030: 7468 6520 7473 6b69 742e 5461 626c 6543  the tskit.TableC
-00018040: 6f6c 6c65 6374 696f 6e20 6167 6169 6e0a  ollection again.
-00018050: 2020 2020 2020 2020 7365 6c66 2e5f 736f          self._so
-00018060: 7274 5f61 6e64 5f73 696d 706c 6966 795f  rt_and_simplify_
-00018070: 7461 626c 655f 636f 6c6c 6563 7469 6f6e  table_collection
-00018080: 2829 0a0a 2020 2020 2020 2020 2320 7265  ()..        # re
-00018090: 7365 7420 7468 6520 636f 6f72 6473 2061  set the coords a
-000180a0: 6e64 2063 656c 6c73 2061 7474 7273 0a20  nd cells attrs. 
-000180b0: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
-000180c0: 5f63 6f6f 7264 735f 616e 645f 6365 6c6c  _coords_and_cell
-000180d0: 7328 290a 0a20 2020 2020 2020 2023 2072  s()..        # r
-000180e0: 6573 6574 2074 6865 204b 4454 7265 6520  eset the KDTree 
-000180f0: 6166 7465 7220 6164 6469 6e67 2074 6865  after adding the
-00018100: 206e 6577 2069 6e64 6976 6964 7561 6c73   new individuals
-00018110: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-00018120: 6574 5f6b 645f 7472 6565 2829 0a0a 2020  et_kd_tree()..  
-00018130: 2020 2020 2020 2320 7265 7365 7420 7468        # reset th
-00018140: 6520 6465 6e73 6974 7920 6772 6964 730a  e density grids.
-00018150: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-00018160: 745f 6465 6e73 5f67 7269 6473 286c 616e  t_dens_grids(lan
-00018170: 6429 0a0a 2020 2020 2020 2020 2320 7265  d)..        # re
-00018180: 7365 742f 7365 7420 736f 7572 6365 2049  set/set source I
-00018190: 6e64 6976 6964 7561 6c73 2720 656e 7669  ndividuals' envi
-000181a0: 726f 6e6d 656e 7461 6c20 616e 6420 6669  ronmental and fi
-000181b0: 746e 6573 7320 7661 6c75 6573 0a20 2020  tness values.   
-000181c0: 2020 2020 2073 656c 662e 5f73 6574 5f65       self._set_e
-000181d0: 286c 616e 6429 0a0a 2020 2020 2020 2020  (land)..        
-000181e0: 2372 6573 6574 2070 6865 6e6f 7479 7065  #reset phenotype
-000181f0: 7320 616e 6420 6669 746e 6573 7365 730a  s and fitnesses.
-00018200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00018210: 6765 6e5f 6172 6368 2069 7320 6e6f 7420  gen_arch is not 
-00018220: 4e6f 6e65 2061 6e64 2073 656c 662e 6765  None and self.ge
-00018230: 6e5f 6172 6368 2e74 7261 6974 7320 6973  n_arch.traits is
-00018240: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00018250: 2020 2020 2020 205b 696e 642e 5f73 6574         [ind._set
-00018260: 5f7a 2873 656c 662e 6765 6e5f 6172 6368  _z(self.gen_arch
-00018270: 2920 666f 7220 696e 6420 696e 2073 656c  ) for ind in sel
-00018280: 662e 7661 6c75 6573 2829 5d0a 2020 2020  f.values()].    
-00018290: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
-000182a0: 6c63 5f66 6974 6e65 7373 2873 6574 5f66  lc_fitness(set_f
-000182b0: 6974 3d54 7275 6529 0a0a 2020 2020 2020  it=True)..      
-000182c0: 2020 2320 7072 696e 7420 696e 666f 726d    # print inform
-000182d0: 6174 6976 6520 6f75 7470 7574 0a20 2020  ative output.   
-000182e0: 2020 2020 2070 7269 6e74 2866 225c 6e7b       print(f"\n{
-000182f0: 6c65 6e28 696e 6469 7669 6473 297d 2049  len(individs)} I
-00018300: 6e64 6976 6964 7561 6c73 2073 7563 6365  ndividuals succe
-00018310: 7373 6675 6c6c 7920 220a 2020 2020 2020  ssfully ".      
-00018320: 2020 2020 2020 2020 6622 6164 6465 6420          f"added 
-00018330: 746f 2053 7065 6369 6573 207b 7365 6c66  to Species {self
-00018340: 2e69 6478 7d20 2827 7b73 656c 662e 6e61  .idx} ('{self.na
-00018350: 6d65 7d27 292e 5c6e 2229 0a0a 0a20 2020  me}').\n")...   
-00018360: 2064 6566 205f 696e 6974 5f6d 7370 7269   def _init_mspri
-00018370: 6d65 5f70 6f70 2873 656c 662c 206c 616e  me_pop(self, lan
-00018380: 642c 206d 7370 7269 6d65 5f69 6e69 745f  d, msprime_init_
-00018390: 7061 7261 6d73 293a 0a20 2020 2020 2020  params):.       
-000183a0: 2023 2067 6574 2069 6e74 656e 6465 6420   # get intended 
-000183b0: 746f 7461 6c20 696e 6974 6961 6c20 706f  total initial po
-000183c0: 7020 7369 7a65 0a20 2020 2020 2020 2074  p size.        t
-000183d0: 6172 6765 745f 7369 7a65 203d 206e 702e  arget_size = np.
-000183e0: 7375 6d28 5b5b 2a76 2e6b 6579 7328 295d  sum([[*v.keys()]
-000183f0: 5b30 5d20 666f 720a 2020 2020 2020 2020  [0] for.        
-00018400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018420: 2020 2020 7620 696e 206d 7370 7269 6d65      v in msprime
-00018430: 5f69 6e69 745f 7061 7261 6d73 2e76 616c  _init_params.val
-00018440: 7565 7328 295d 290a 2020 2020 2020 2020  ues()]).        
-00018450: 2320 7265 6d6f 7665 2061 6c6c 2063 7572  # remove all cur
-00018460: 7265 6e74 2069 6e64 6976 6964 730a 2020  rent individs.  
-00018470: 2020 2020 2020 7365 6c66 2e5f 7265 6d6f        self._remo
-00018480: 7665 5f69 6e64 6976 6964 7561 6c73 286e  ve_individuals(n
-00018490: 3d6c 656e 2873 656c 6629 2c0a 2020 2020  =len(self),.    
-000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184b0: 2020 2020 2020 2020 2020 2020 206b 6565               kee
-000184c0: 705f 7369 7465 735f 7461 623d 4661 6c73  p_sites_tab=Fals
-000184d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00017690: 2020 2020 2022 7468 6520 7265 6369 7069       "the recipi
+000176a0: 656e 7420 616e 6420 736f 7572 6365 2053  ent and source S
+000176b0: 7065 6369 6573 2720 220a 2020 2020 2020  pecies' ".      
+000176c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176d0: 2020 2020 2020 2020 2020 2022 5461 626c             "Tabl
+000176e0: 6543 6f6c 6c65 6374 696f 6e73 2069 6e64  eCollections ind
+000176f0: 6976 6964 7561 6c73 2074 6162 6c65 732e  ividuals tables.
+00017700: 2229 0a0a 2020 2020 2020 2020 2320 6164  ")..        # ad
+00017710: 6420 696e 2074 6865 2049 6e64 6976 6964  d in the Individ
+00017720: 7561 6c73 2c20 6b65 7965 6420 6279 2069  uals, keyed by i
+00017730: 6478 0a20 2020 2020 2020 2070 6f70 5f73  dx.        pop_s
+00017740: 697a 655f 6234 203d 206c 656e 2873 656c  ize_b4 = len(sel
+00017750: 6629 0a20 2020 2020 2020 2066 6f72 2069  f).        for i
+00017760: 6e64 2069 6e20 696e 6469 7669 6473 3a0a  nd in individs:.
+00017770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017780: 5b69 6e64 2e69 6478 5d20 3d20 696e 640a  [ind.idx] = ind.
+00017790: 2020 2020 2020 2020 706f 705f 7369 7a65          pop_size
+000177a0: 5f61 6620 3d20 6c65 6e28 7365 6c66 290a  _af = len(self).
+000177b0: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+000177c0: 706f 705f 7369 7a65 5f61 6620 2d20 706f  pop_size_af - po
+000177d0: 705f 7369 7a65 5f62 3429 203d 3d20 6c65  p_size_b4) == le
+000177e0: 6e28 696e 6469 7669 6473 292c 2028 2249  n(individs), ("I
+000177f0: 6e63 6f72 7265 6374 206e 756d 6265 7222  ncorrect number"
+00017800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 2022 206f 6620 496e 6469 7669 6475 616c   " of Individual
+00017830: 7320 6164 6465 6420 746f 2072 6563 6970  s added to recip
+00017840: 6965 6e74 2053 7065 6369 6573 2e22 290a  ient Species.").
+00017850: 0a20 2020 2020 2020 2023 2075 7064 6174  .        # updat
+00017860: 6520 6561 6368 2049 6e64 6976 6964 7561  e each Individua
+00017870: 6c27 7320 5f69 6e64 6976 6964 7561 6c73  l's _individuals
+00017880: 5f74 6162 5f69 6420 616e 6420 5f6e 6f64  _tab_id and _nod
+00017890: 6573 5f74 6162 5f69 6473 0a20 2020 2020  es_tab_ids.     
+000178a0: 2020 2023 2074 6f20 6d61 7463 6820 7468     # to match th
+000178b0: 6520 6e65 772c 2075 6e69 6f6e 6564 2054  e new, unioned T
+000178c0: 6162 6c65 436f 6c6c 6563 7469 6f6e 0a20  ableCollection. 
+000178d0: 2020 2020 2020 206e 6f64 6573 5f74 6162         nodes_tab
+000178e0: 5f69 6e64 6976 6964 7561 6c73 203d 2073  _individuals = s
+000178f0: 656c 662e 5f74 632e 6e6f 6465 732e 696e  elf._tc.nodes.in
+00017900: 6469 7669 6475 616c 0a20 2020 2020 2020  dividual.       
+00017910: 2066 6f72 2069 6478 2c20 696e 6420 696e   for idx, ind in
+00017920: 2073 656c 662e 6974 656d 7328 293a 0a20   self.items():. 
+00017930: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
+00017940: 6964 7561 6c73 5f74 6162 5f69 6420 3d20  iduals_tab_id = 
+00017950: 6e70 2e61 7267 7768 6572 6528 0a20 2020  np.argwhere(.   
+00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017970: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
+00017980: 7928 7265 6369 705f 7463 5f69 6e64 6976  y(recip_tc_indiv
+00017990: 6964 7561 6c73 5f69 6473 2920 3d3d 2069  iduals_ids) == i
+000179a0: 6478 292e 7261 7665 6c28 290a 2020 2020  dx).ravel().    
+000179b0: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+000179c0: 656e 2869 6e64 6976 6964 7561 6c73 5f74  en(individuals_t
+000179d0: 6162 5f69 6429 203d 3d20 310a 2020 2020  ab_id) == 1.    
+000179e0: 2020 2020 2020 2020 696e 6469 7669 6475          individu
+000179f0: 616c 735f 7461 625f 6964 203d 2069 6e64  als_tab_id = ind
+00017a00: 6976 6964 7561 6c73 5f74 6162 5f69 645b  ividuals_tab_id[
+00017a10: 305d 0a20 2020 2020 2020 2020 2020 2069  0].            i
+00017a20: 6e64 2e5f 696e 6469 7669 6475 616c 735f  nd._individuals_
+00017a30: 7461 625f 6964 203d 2069 6e64 6976 6964  tab_id = individ
+00017a40: 7561 6c73 5f74 6162 5f69 640a 2020 2020  uals_tab_id.    
+00017a50: 2020 2020 2020 2020 6e6f 6465 735f 7461          nodes_ta
+00017a60: 625f 6964 7320 3d20 6e70 2e61 7267 7768  b_ids = np.argwh
+00017a70: 6572 6528 6e6f 6465 735f 7461 625f 696e  ere(nodes_tab_in
+00017a80: 6469 7669 6475 616c 7320 3d3d 0a20 2020  dividuals ==.   
+00017a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ab0: 2020 2020 2069 6e64 6976 6964 7561 6c73       individuals
+00017ac0: 5f74 6162 5f69 6429 2e72 6176 656c 2829  _tab_id).ravel()
+00017ad0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00017ae0: 6572 7420 6c65 6e28 6e6f 6465 735f 7461  ert len(nodes_ta
+00017af0: 625f 6964 7329 203d 3d20 320a 2020 2020  b_ids) == 2.    
+00017b00: 2020 2020 2020 2020 696e 642e 5f6e 6f64          ind._nod
+00017b10: 6573 5f74 6162 5f69 6473 203d 207b 693a  es_tab_ids = {i:
+00017b20: 2069 6420 666f 7220 692c 2069 6420 696e   id for i, id in
+00017b30: 2065 6e75 6d65 7261 7465 286e 6f64 6573   enumerate(nodes
+00017b40: 5f74 6162 5f69 6473 297d 0a0a 2020 2020  _tab_ids)}..    
+00017b50: 2020 2020 2320 6669 6e61 6c20 6368 6563      # final chec
+00017b60: 6b20 7468 6174 2069 6e64 6963 6573 2063  k that indices c
+00017b70: 6865 636b 206f 7574 2069 6e20 7468 6520  heck out in the 
+00017b80: 6f74 6865 7220 6469 7265 6374 696f 6e0a  other direction.
+00017b90: 2020 2020 2020 2020 2320 2869 2e65 2e2c          # (i.e.,
+00017ba0: 2066 726f 6d20 6e6f 6465 7320 7461 6220   from nodes tab 
+00017bb0: 746f 2069 6e64 6976 6964 7561 6c73 2074  to individuals t
+00017bc0: 6162 2074 6f20 676e 7820 496e 6469 7669  ab to gnx Indivi
+00017bd0: 6475 616c 730a 2020 2020 2020 2020 2320  duals.        # 
+00017be0: 616e 6420 7468 6174 206e 6f64 6573 2069  and that nodes i
+00017bf0: 6473 2063 6865 636b 206f 7574 2074 6f6f  ds check out too
+00017c00: 0a20 2020 2020 2020 2063 7572 725f 6e6f  .        curr_no
+00017c10: 6465 5f63 7420 3d20 300a 2020 2020 2020  de_ct = 0.      
+00017c20: 2020 666f 7220 6e6f 6465 5f69 642c 206e    for node_id, n
+00017c30: 6f64 6520 696e 2065 6e75 6d65 7261 7465  ode in enumerate
+00017c40: 2873 656c 662e 5f74 632e 6e6f 6465 7329  (self._tc.nodes)
+00017c50: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00017c60: 4e4f 5445 3a20 6967 6e6f 7265 202d 3173  NOTE: ignore -1s
+00017c70: 3b20 7468 6579 2061 7265 206d 7370 7269  ; they are mspri
+00017c80: 6d65 2066 6c61 6773 2066 6f72 206e 6f6e  me flags for non
+00017c90: 2d73 616d 706c 6520 6e6f 6465 7320 6275  -sample nodes bu
+00017ca0: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
+00017cb0: 2020 2020 2020 6265 6168 7665 2061 7320        beahve as 
+00017cc0: 6120 5079 7468 6f6e 2069 6e64 6578 6572  a Python indexer
+00017cd0: 206f 6620 7468 6520 6c61 7374 2049 6e64   of the last Ind
+00017ce0: 6976 6964 7561 6c20 696e 2074 6865 0a20  ividual in the. 
+00017cf0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00017d00: 2020 2053 7065 6369 6573 2061 6e64 2074     Species and t
+00017d10: 6875 7320 7468 726f 7720 616e 2065 7272  hus throw an err
+00017d20: 6f72 0a20 2020 2020 2020 2020 2020 2069  or.            i
+00017d30: 6620 6e6f 6465 2e69 6e64 6976 6964 7561  f node.individua
+00017d40: 6c20 213d 202d 313a 0a20 2020 2020 2020  l != -1:.       
+00017d50: 2020 2020 2020 2020 2067 6e78 5f69 6e64           gnx_ind
+00017d60: 6976 6964 7561 6c5f 6964 203d 2069 6e74  ividual_id = int
+00017d70: 2e66 726f 6d5f 6279 7465 7328 7365 6c66  .from_bytes(self
+00017d80: 2e5f 7463 2e69 6e64 6976 6964 7561 6c73  ._tc.individuals
+00017d90: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017db0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017dc0: 6465 2e69 6e64 6976 6964 7561 6c5d 2e6d  de.individual].m
+00017dd0: 6574 6164 6174 612c 2027 6c69 7474 6c65  etadata, 'little
+00017de0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00017df0: 2020 2069 6620 676e 785f 696e 6469 7669     if gnx_indivi
+00017e00: 6475 616c 5f69 6420 696e 205b 2a73 656c  dual_id in [*sel
+00017e10: 665d 3a0a 2020 2020 2020 2020 2020 2020  f]:.            
+00017e20: 2020 2020 2020 2020 6375 7272 5f6e 6f64          curr_nod
+00017e30: 655f 6374 202b 3d20 310a 2020 2020 2020  e_ct += 1.      
+00017e40: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00017e50: 7365 7274 2028 7365 6c66 5b67 6e78 5f69  sert (self[gnx_i
+00017e60: 6e64 6976 6964 7561 6c5f 6964 5d2e 5f69  ndividual_id]._i
+00017e70: 6e64 6976 6964 7561 6c73 5f74 6162 5f69  ndividuals_tab_i
+00017e80: 6420 3d3d 0a20 2020 2020 2020 2020 2020  d ==.           
+00017e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ea0: 206e 6f64 652e 696e 6469 7669 6475 616c   node.individual
+00017eb0: 2061 6e64 206e 6f64 655f 6964 2069 6e0a   and node_id in.
+00017ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017ee0: 5b67 6e78 5f69 6e64 6976 6964 7561 6c5f  [gnx_individual_
+00017ef0: 6964 5d2e 5f6e 6f64 6573 5f74 6162 5f69  id]._nodes_tab_i
+00017f00: 6473 2e76 616c 7565 7328 2929 0a20 2020  ds.values()).   
+00017f10: 2020 2020 2061 7373 6572 7420 6375 7272       assert curr
+00017f20: 5f6e 6f64 655f 6374 203d 3d20 322a 6c65  _node_ct == 2*le
+00017f30: 6e28 7365 6c66 292c 2028 224e 756d 6265  n(self), ("Numbe
+00017f40: 7220 6f66 2063 7572 7265 6e74 2049 6e64  r of current Ind
+00017f50: 6976 6964 7561 6c73 2022 0a20 2020 2020  ividuals ".     
+00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 2020 2020 2020 2020 2020 2269 6e20 7468            "in th
+00017f90: 6520 7265 6369 7069 656e 7420 5370 6563  e recipient Spec
+00017fa0: 6965 7320 646f 6573 206e 6f74 2022 0a20  ies does not ". 
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fd0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00017fe0: 6174 6368 2074 6865 206e 756d 6265 7220  atch the number 
+00017ff0: 6578 7065 6374 6564 2062 6173 6564 206f  expected based o
+00018000: 6e20 220a 2020 2020 2020 2020 2020 2020  n ".            
+00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018030: 2020 2022 5461 626c 6543 6f6c 6c65 6374     "TableCollect
+00018040: 696f 6e20 636f 6e74 656e 7473 2e22 290a  ion contents.").
+00018050: 0a20 2020 2020 2020 2023 2073 6f72 7420  .        # sort 
+00018060: 616e 6420 7369 6d70 6c69 6679 2074 6865  and simplify the
+00018070: 2074 736b 6974 2e54 6162 6c65 436f 6c6c   tskit.TableColl
+00018080: 6563 7469 6f6e 2061 6761 696e 0a20 2020  ection again.   
+00018090: 2020 2020 2073 656c 662e 5f73 6f72 745f       self._sort_
+000180a0: 616e 645f 7369 6d70 6c69 6679 5f74 6162  and_simplify_tab
+000180b0: 6c65 5f63 6f6c 6c65 6374 696f 6e28 290a  le_collection().
+000180c0: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
+000180d0: 2074 6865 2063 6f6f 7264 7320 616e 6420   the coords and 
+000180e0: 6365 6c6c 7320 6174 7472 730a 2020 2020  cells attrs.    
+000180f0: 2020 2020 7365 6c66 2e5f 7365 745f 636f      self._set_co
+00018100: 6f72 6473 5f61 6e64 5f63 656c 6c73 2829  ords_and_cells()
+00018110: 0a0a 2020 2020 2020 2020 2320 7265 7365  ..        # rese
+00018120: 7420 7468 6520 4b44 5472 6565 2061 6674  t the KDTree aft
+00018130: 6572 2061 6464 696e 6720 7468 6520 6e65  er adding the ne
+00018140: 7720 696e 6469 7669 6475 616c 730a 2020  w individuals.  
+00018150: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
+00018160: 6b64 5f74 7265 6528 290a 0a20 2020 2020  kd_tree()..     
+00018170: 2020 2023 2072 6573 6574 2074 6865 2064     # reset the d
+00018180: 656e 7369 7479 2067 7269 6473 0a20 2020  ensity grids.   
+00018190: 2020 2020 2073 656c 662e 5f73 6574 5f64       self._set_d
+000181a0: 656e 735f 6772 6964 7328 6c61 6e64 290a  ens_grids(land).
+000181b0: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
+000181c0: 2f73 6574 2073 6f75 7263 6520 496e 6469  /set source Indi
+000181d0: 7669 6475 616c 7327 2065 6e76 6972 6f6e  viduals' environ
+000181e0: 6d65 6e74 616c 2061 6e64 2066 6974 6e65  mental and fitne
+000181f0: 7373 2076 616c 7565 730a 2020 2020 2020  ss values.      
+00018200: 2020 7365 6c66 2e5f 7365 745f 6528 6c61    self._set_e(la
+00018210: 6e64 290a 0a20 2020 2020 2020 2023 7265  nd)..        #re
+00018220: 7365 7420 7068 656e 6f74 7970 6573 2061  set phenotypes a
+00018230: 6e64 2066 6974 6e65 7373 6573 0a20 2020  nd fitnesses.   
+00018240: 2020 2020 2069 6620 7365 6c66 2e67 656e       if self.gen
+00018250: 5f61 7263 6820 6973 206e 6f74 204e 6f6e  _arch is not Non
+00018260: 6520 616e 6420 7365 6c66 2e67 656e 5f61  e and self.gen_a
+00018270: 7263 682e 7472 6169 7473 2069 7320 6e6f  rch.traits is no
+00018280: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00018290: 2020 2020 5b69 6e64 2e5f 7365 745f 7a28      [ind._set_z(
+000182a0: 7365 6c66 2e67 656e 5f61 7263 6829 2066  self.gen_arch) f
+000182b0: 6f72 2069 6e64 2069 6e20 7365 6c66 2e76  or ind in self.v
+000182c0: 616c 7565 7328 295d 0a20 2020 2020 2020  alues()].       
+000182d0: 2020 2020 2073 656c 662e 5f63 616c 635f       self._calc_
+000182e0: 6669 746e 6573 7328 7365 745f 6669 743d  fitness(set_fit=
+000182f0: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
+00018300: 2070 7269 6e74 2069 6e66 6f72 6d61 7469   print informati
+00018310: 7665 206f 7574 7075 740a 2020 2020 2020  ve output.      
+00018320: 2020 7072 696e 7428 6622 5c6e 7b6c 656e    print(f"\n{len
+00018330: 2869 6e64 6976 6964 7329 7d20 496e 6469  (individs)} Indi
+00018340: 7669 6475 616c 7320 7375 6363 6573 7366  viduals successf
+00018350: 756c 6c79 2022 0a20 2020 2020 2020 2020  ully ".         
+00018360: 2020 2020 2066 2261 6464 6564 2074 6f20       f"added to 
+00018370: 5370 6563 6965 7320 7b73 656c 662e 6964  Species {self.id
+00018380: 787d 2028 277b 7365 6c66 2e6e 616d 657d  x} ('{self.name}
+00018390: 2729 2e5c 6e22 290a 0a0a 2020 2020 6465  ').\n")...    de
+000183a0: 6620 5f69 6e69 745f 6d73 7072 696d 655f  f _init_msprime_
+000183b0: 706f 7028 7365 6c66 2c20 6c61 6e64 2c20  pop(self, land, 
+000183c0: 6d73 7072 696d 655f 696e 6974 5f70 6172  msprime_init_par
+000183d0: 616d 7329 3a0a 2020 2020 2020 2020 2320  ams):.        # 
+000183e0: 6765 7420 696e 7465 6e64 6564 2074 6f74  get intended tot
+000183f0: 616c 2069 6e69 7469 616c 2070 6f70 2073  al initial pop s
+00018400: 697a 650a 2020 2020 2020 2020 7461 7267  ize.        targ
+00018410: 6574 5f73 697a 6520 3d20 6e70 2e73 756d  et_size = np.sum
+00018420: 285b 5b2a 762e 6b65 7973 2829 5d5b 305d  ([[*v.keys()][0]
+00018430: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
+00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018460: 2076 2069 6e20 6d73 7072 696d 655f 696e   v in msprime_in
+00018470: 6974 5f70 6172 616d 732e 7661 6c75 6573  it_params.values
+00018480: 2829 5d29 0a20 2020 2020 2020 2023 2072  ()]).        # r
+00018490: 656d 6f76 6520 616c 6c20 6375 7272 656e  emove all curren
+000184a0: 7420 696e 6469 7669 6473 0a20 2020 2020  t individs.     
+000184b0: 2020 2073 656c 662e 5f72 656d 6f76 655f     self._remove_
+000184c0: 696e 6469 7669 6475 616c 7328 6e3d 6c65  individuals(n=le
+000184d0: 6e28 7365 6c66 292c 0a20 2020 2020 2020  n(self),.       
 000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184f0: 2020 2029 0a20 2020 2020 2020 2061 7373     ).        ass
-00018500: 6572 7420 6c65 6e28 7365 6c66 2920 3d3d  ert len(self) ==
-00018510: 2030 0a20 2020 2020 2020 2023 206c 6f6f   0.        # loo
-00018520: 7020 6f76 6572 2073 6f75 7263 6520 706f  p over source po
-00018530: 7073 2061 6e64 2061 6464 2069 6e64 6976  ps and add indiv
-00018540: 6964 7561 6c73 2066 726f 6d20 6561 6368  iduals from each
-00018550: 206f 6e65 0a20 2020 2020 2020 2066 6f72   one.        for
-00018560: 2070 6f70 2069 6e20 6d73 7072 696d 655f   pop in msprime_
-00018570: 696e 6974 5f70 6172 616d 732e 7661 6c75  init_params.valu
-00018580: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
-00018590: 2020 6173 7365 7274 206c 656e 2870 6f70    assert len(pop
-000185a0: 2e6b 6579 7328 2929 203d 3d20 312c 2028  .keys()) == 1, (
-000185b0: 2245 6163 6820 6d73 7072 696d 6520 736f  "Each msprime so
-000185c0: 7572 6365 2070 6f70 756c 6174 696f 6e20  urce population 
-000185d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000185e0: 2020 2020 2020 2020 2020 2270 6172 616d            "param
-000185f0: 6574 6572 697a 6564 2069 6e20 6120 5370  eterized in a Sp
-00018600: 6563 6965 7327 2027 696e 6974 2720 7365  ecies' 'init' se
-00018610: 6374 696f 6e20 220a 2020 2020 2020 2020  ction ".        
-00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018630: 226f 6620 7468 6520 7061 7261 6d65 7465  "of the paramete
-00018640: 7273 2066 696c 6522 0a20 2020 2020 2020  rs file".       
-00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018660: 2022 6d75 7374 2062 6520 7265 7072 6573   "must be repres
-00018670: 656e 7465 6420 6279 2061 2064 6963 7420  ented by a dict 
-00018680: 7769 7468 2061 2073 696e 676c 6520 6b65  with a single ke
-00018690: 7920 2874 6865 2022 0a20 2020 2020 2020  y (the ".       
-000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186b0: 2022 6e75 6d62 6572 206f 6620 496e 6469   "number of Indi
-000186c0: 7669 6475 616c 7320 746f 2073 616d 706c  viduals to sampl
-000186d0: 6520 6672 6f6d 2074 6865 2070 6f70 756c  e from the popul
-000186e0: 6174 696f 6e29 2022 0a20 2020 2020 2020  ation) ".       
-000186f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018700: 2022 7768 6f73 6520 7661 6c75 6520 6973   "whose value is
-00018710: 2061 2064 6963 7420 636f 6e74 6169 6e69   a dict containi
-00018720: 6e67 2031 2e29 2061 2027 636f 6f72 6473  ng 1.) a 'coords
-00018730: 2720 6b65 7920 220a 2020 2020 2020 2020  ' key ".        
-00018740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018750: 2269 6e64 6963 6174 696e 6720 7468 6520  "indicating the 
-00018760: 6c6f 6361 7469 6f6e 2f73 2074 6f20 706c  location/s to pl
-00018770: 6163 6520 7468 6520 220a 2020 2020 2020  ace the ".      
-00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018790: 2020 2273 616d 706c 6564 2049 6e64 6976    "sampled Indiv
-000187a0: 6964 7561 6c73 2061 7420 616e 6420 322e  iduals at and 2.
-000187b0: 2920 220a 2020 2020 2020 2020 2020 2020  ) ".            
-000187c0: 2020 2020 2020 2020 2020 2020 2261 2073              "a s
-000187d0: 6574 206f 6620 7661 6c69 6420 6b65 7977  et of valid keyw
-000187e0: 6f72 6420 6172 6775 6d65 6e74 7320 7468  ord arguments th
-000187f0: 6174 2022 0a20 2020 2020 2020 2020 2020  at ".           
-00018800: 2020 2020 2020 2020 2020 2020 2022 6361               "ca
-00018810: 6e20 6265 2070 726f 7669 6465 6420 746f  n be provided to
-00018820: 204d 6f64 656c 2e61 6464 5f69 6e64 6976   Model.add_indiv
-00018830: 6964 7561 6c73 2022 0a20 2020 2020 2020  iduals ".       
-00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018850: 2022 6173 2074 6865 2027 736f 7572 6365   "as the 'source
-00018860: 5f6d 7370 7269 6d65 5f70 6172 616d 7327  _msprime_params'
-00018870: 2064 6963 742e 2229 0a20 2020 2020 2020   dict.").       
-00018880: 2020 2020 206e 203d 205b 2a70 6f70 2e6b       n = [*pop.k
-00018890: 6579 7328 295d 5b30 5d0a 2020 2020 2020  eys()][0].      
-000188a0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-000188b0: 6e73 7461 6e63 6528 6e2c 2069 6e74 292c  nstance(n, int),
-000188c0: 2028 2254 6865 206b 6579 206f 6620 6561   ("The key of ea
-000188d0: 6368 2022 0a20 2020 2020 2020 2020 2020  ch ".           
-000188e0: 2020 2020 2020 2020 2020 2020 2022 6d73               "ms
-000188f0: 7072 696d 6520 736f 7572 6365 2070 6f70  prime source pop
-00018900: 756c 6174 696f 6e20 696e 2061 2053 7065  ulation in a Spe
-00018910: 6369 6573 2720 2769 6e69 7427 2022 0a20  cies' 'init' ". 
-00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018930: 2020 2020 2020 2022 7365 6374 696f 6e20         "section 
-00018940: 6f66 2074 6865 2070 6172 616d 6574 6572  of the parameter
-00018950: 7320 6669 6c65 206d 7573 7420 6265 2061  s file must be a
-00018960: 6e20 696e 7420 220a 2020 2020 2020 2020  n int ".        
-00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018980: 2269 6e64 6963 6174 696e 6720 7468 6520  "indicating the 
-00018990: 6e75 6d62 6572 206f 6620 7374 6172 7469  number of starti
-000189a0: 6e67 2049 6e64 6976 6964 7561 6c73 2022  ng Individuals "
-000189b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189c0: 2020 2020 2020 2020 2022 746f 2062 6520           "to be 
-000189d0: 736f 7572 6365 6420 6672 6f6d 2074 6861  sourced from tha
-000189e0: 7420 706f 7075 6c61 7469 6f6e 2e22 290a  t population.").
-000189f0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00018a00: 7274 2027 636f 6f72 6473 2720 696e 2070  rt 'coords' in p
-00018a10: 6f70 5b6e 5d2c 2028 2245 6163 6820 6d73  op[n], ("Each ms
-00018a20: 7072 696d 6520 736f 7572 6365 2070 6f70  prime source pop
-00018a30: 756c 6174 696f 6e27 7320 220a 2020 2020  ulation's ".    
-00018a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a60: 2020 2020 2269 6e69 7420 7061 7261 6d65      "init parame
-00018a70: 7465 7273 2064 6963 7420 6d75 7374 2069  ters dict must i
-00018a80: 6e63 6c75 6465 2022 0a20 2020 2020 2020  nclude ".       
+000184f0: 2020 2020 2020 2020 2020 6b65 6570 5f73            keep_s
+00018500: 6974 6573 5f74 6162 3d46 616c 7365 2c0a  ites_tab=False,.
+00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018530: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00018540: 206c 656e 2873 656c 6629 203d 3d20 300a   len(self) == 0.
+00018550: 2020 2020 2020 2020 2320 6c6f 6f70 206f          # loop o
+00018560: 7665 7220 736f 7572 6365 2070 6f70 7320  ver source pops 
+00018570: 616e 6420 6164 6420 696e 6469 7669 6475  and add individu
+00018580: 616c 7320 6672 6f6d 2065 6163 6820 6f6e  als from each on
+00018590: 650a 2020 2020 2020 2020 666f 7220 706f  e.        for po
+000185a0: 7020 696e 206d 7370 7269 6d65 5f69 6e69  p in msprime_ini
+000185b0: 745f 7061 7261 6d73 2e76 616c 7565 7328  t_params.values(
+000185c0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+000185d0: 7373 6572 7420 6c65 6e28 706f 702e 6b65  ssert len(pop.ke
+000185e0: 7973 2829 2920 3d3d 2031 2c20 2822 4561  ys()) == 1, ("Ea
+000185f0: 6368 206d 7370 7269 6d65 2073 6f75 7263  ch msprime sourc
+00018600: 6520 706f 7075 6c61 7469 6f6e 2022 0a20  e population ". 
+00018610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018620: 2020 2020 2020 2022 7061 7261 6d65 7465         "paramete
+00018630: 7269 7a65 6420 696e 2061 2053 7065 6369  rized in a Speci
+00018640: 6573 2720 2769 6e69 7427 2073 6563 7469  es' 'init' secti
+00018650: 6f6e 2022 0a20 2020 2020 2020 2020 2020  on ".           
+00018660: 2020 2020 2020 2020 2020 2020 2022 6f66               "of
+00018670: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+00018680: 6669 6c65 220a 2020 2020 2020 2020 2020  file".          
+00018690: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+000186a0: 7573 7420 6265 2072 6570 7265 7365 6e74  ust be represent
+000186b0: 6564 2062 7920 6120 6469 6374 2077 6974  ed by a dict wit
+000186c0: 6820 6120 7369 6e67 6c65 206b 6579 2028  h a single key (
+000186d0: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
+000186e0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+000186f0: 756d 6265 7220 6f66 2049 6e64 6976 6964  umber of Individ
+00018700: 7561 6c73 2074 6f20 7361 6d70 6c65 2066  uals to sample f
+00018710: 726f 6d20 7468 6520 706f 7075 6c61 7469  rom the populati
+00018720: 6f6e 2920 220a 2020 2020 2020 2020 2020  on) ".          
+00018730: 2020 2020 2020 2020 2020 2020 2020 2277                "w
+00018740: 686f 7365 2076 616c 7565 2069 7320 6120  hose value is a 
+00018750: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
+00018760: 312e 2920 6120 2763 6f6f 7264 7327 206b  1.) a 'coords' k
+00018770: 6579 2022 0a20 2020 2020 2020 2020 2020  ey ".           
+00018780: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+00018790: 6469 6361 7469 6e67 2074 6865 206c 6f63  dicating the loc
+000187a0: 6174 696f 6e2f 7320 746f 2070 6c61 6365  ation/s to place
+000187b0: 2074 6865 2022 0a20 2020 2020 2020 2020   the ".         
+000187c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000187d0: 7361 6d70 6c65 6420 496e 6469 7669 6475  sampled Individu
+000187e0: 616c 7320 6174 2061 6e64 2032 2e29 2022  als at and 2.) "
+000187f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018800: 2020 2020 2020 2020 2022 6120 7365 7420           "a set 
+00018810: 6f66 2076 616c 6964 206b 6579 776f 7264  of valid keyword
+00018820: 2061 7267 756d 656e 7473 2074 6861 7420   arguments that 
+00018830: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018840: 2020 2020 2020 2020 2020 2263 616e 2062            "can b
+00018850: 6520 7072 6f76 6964 6564 2074 6f20 4d6f  e provided to Mo
+00018860: 6465 6c2e 6164 645f 696e 6469 7669 6475  del.add_individu
+00018870: 616c 7320 220a 2020 2020 2020 2020 2020  als ".          
+00018880: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00018890: 7320 7468 6520 2773 6f75 7263 655f 6d73  s the 'source_ms
+000188a0: 7072 696d 655f 7061 7261 6d73 2720 6469  prime_params' di
+000188b0: 6374 2e22 290a 2020 2020 2020 2020 2020  ct.").          
+000188c0: 2020 6e20 3d20 5b2a 706f 702e 6b65 7973    n = [*pop.keys
+000188d0: 2829 5d5b 305d 0a20 2020 2020 2020 2020  ()][0].         
+000188e0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+000188f0: 616e 6365 286e 2c20 696e 7429 2c20 2822  ance(n, int), ("
+00018900: 5468 6520 6b65 7920 6f66 2065 6163 6820  The key of each 
+00018910: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018920: 2020 2020 2020 2020 2020 226d 7370 7269            "mspri
+00018930: 6d65 2073 6f75 7263 6520 706f 7075 6c61  me source popula
+00018940: 7469 6f6e 2069 6e20 6120 5370 6563 6965  tion in a Specie
+00018950: 7327 2027 696e 6974 2720 220a 2020 2020  s' 'init' ".    
+00018960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018970: 2020 2020 2273 6563 7469 6f6e 206f 6620      "section of 
+00018980: 7468 6520 7061 7261 6d65 7465 7273 2066  the parameters f
+00018990: 696c 6520 6d75 7374 2062 6520 616e 2069  ile must be an i
+000189a0: 6e74 2022 0a20 2020 2020 2020 2020 2020  nt ".           
+000189b0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+000189c0: 6469 6361 7469 6e67 2074 6865 206e 756d  dicating the num
+000189d0: 6265 7220 6f66 2073 7461 7274 696e 6720  ber of starting 
+000189e0: 496e 6469 7669 6475 616c 7320 220a 2020  Individuals ".  
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 2020 2020 2020 2274 6f20 6265 2073 6f75        "to be sou
+00018a10: 7263 6564 2066 726f 6d20 7468 6174 2070  rced from that p
+00018a20: 6f70 756c 6174 696f 6e2e 2229 0a20 2020  opulation.").   
+00018a30: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00018a40: 2763 6f6f 7264 7327 2069 6e20 706f 705b  'coords' in pop[
+00018a50: 6e5d 2c20 2822 4561 6368 206d 7370 7269  n], ("Each mspri
+00018a60: 6d65 2073 6f75 7263 6520 706f 7075 6c61  me source popula
+00018a70: 7469 6f6e 2773 2022 0a20 2020 2020 2020  tion's ".       
+00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ab0: 2022 6120 2763 6f6f 7264 7327 206b 6579   "a 'coords' key
-00018ac0: 2077 686f 7365 2076 616c 7565 2069 6e64   whose value ind
-00018ad0: 6963 6174 6573 2022 0a20 2020 2020 2020  icates ".       
-00018ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b00: 2022 7468 6520 6c6f 6361 7469 6f6e 2f73   "the location/s
-00018b10: 2077 6865 7265 2061 6c6c 2073 616d 706c   where all sampl
-00018b20: 6564 2022 0a20 2020 2020 2020 2020 2020  ed ".           
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b40: 2020 2020 2020 2020 2020 2020 2022 496e               "In
-00018b50: 6469 7669 6475 616c 7320 7368 6f75 6c64  dividuals should
-00018b60: 2062 6520 706c 6163 6564 2e22 290a 2020   be placed.").  
-00018b70: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
-00018b80: 203d 2070 6f70 5b6e 5d2e 706f 7028 2763   = pop[n].pop('c
-00018b90: 6f6f 7264 7327 290a 2020 2020 2020 2020  oords').        
-00018ba0: 2020 2020 6173 7365 7274 2028 6973 696e      assert (isin
-00018bb0: 7374 616e 6365 2863 6f6f 7264 732c 206c  stance(coords, l
-00018bc0: 6973 7429 206f 720a 2020 2020 2020 2020  ist) or.        
-00018bd0: 2020 2020 2020 2020 2020 2020 6973 696e              isin
-00018be0: 7374 616e 6365 2863 6f6f 7264 732c 2074  stance(coords, t
-00018bf0: 7570 6c65 2920 6f72 0a20 2020 2020 2020  uple) or.       
-00018c00: 2020 2020 2020 2020 2020 2020 2069 7369               isi
-00018c10: 6e73 7461 6e63 6528 636f 6f72 6473 2c20  nstance(coords, 
-00018c20: 6e70 2e6e 6461 7272 6179 2929 2c20 2822  np.ndarray)), ("
-00018c30: 5468 6520 2763 6f6f 7264 7327 206b 6579  The 'coords' key
-00018c40: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00018c50: 2020 2020 2020 2020 2020 2022 696e 2074             "in t
-00018c60: 6865 2069 6e69 7420 6469 6374 2066 6f72  he init dict for
-00018c70: 2061 6e20 6d73 7072 696d 6520 736f 7572   an msprime sour
-00018c80: 6365 2070 6f70 756c 6174 696f 6e20 220a  ce population ".
-00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ca0: 2020 2020 2020 2020 226d 7573 7420 6861          "must ha
-00018cb0: 7665 2061 206c 6973 742c 2074 7570 6c65  ve a list, tuple
-00018cc0: 2c20 6f72 206e 756d 7079 2e6e 6461 7272  , or numpy.ndarr
-00018cd0: 6179 2061 7320 220a 2020 2020 2020 2020  ay as ".        
-00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cf0: 2269 7473 2076 616c 7565 2e22 290a 2020  "its value.").  
-00018d00: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
-00018d10: 5f73 7472 7563 745f 6572 725f 6d73 6720  _struct_err_msg 
-00018d20: 3d20 2822 5468 6520 2763 6f6f 7264 7327  = ("The 'coords'
-00018d30: 2076 616c 7565 2066 6f72 2022 0a20 2020   value for ".   
-00018d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d50: 2020 2020 2022 616e 206d 7370 7269 6d65       "an msprime
-00018d60: 2073 6f75 7263 6520 706f 7075 6c61 746f   source populato
-00018d70: 6e20 6d75 7374 2062 6520 6f6e 6520 6f66  n must be one of
-00018d80: 3a20 220a 2020 2020 2020 2020 2020 2020  : ".            
-00018d90: 2020 2020 2020 2020 2020 2020 2231 2e29              "1.)
-00018da0: 2061 206c 6973 7420 6f72 2074 7570 6c65   a list or tuple
-00018db0: 206f 6620 6c65 6e67 7468 2032 2c20 6769   of length 2, gi
-00018dc0: 7669 6e67 2074 6865 2022 0a20 2020 2020  ving the ".     
-00018dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018de0: 2020 2022 636f 6f72 6469 6e61 7465 2070     "coordinate p
-00018df0: 6169 7220 6174 2077 6869 6368 2061 6c6c  air at which all
-00018e00: 2049 6e64 6976 6964 7561 6c73 2022 0a20   Individuals ". 
+00018aa0: 2022 696e 6974 2070 6172 616d 6574 6572   "init parameter
+00018ab0: 7320 6469 6374 206d 7573 7420 696e 636c  s dict must incl
+00018ac0: 7564 6520 220a 2020 2020 2020 2020 2020  ude ".          
+00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ae0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00018af0: 2027 636f 6f72 6473 2720 6b65 7920 7768   'coords' key wh
+00018b00: 6f73 6520 7661 6c75 6520 696e 6469 6361  ose value indica
+00018b10: 7465 7320 220a 2020 2020 2020 2020 2020  tes ".          
+00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b30: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00018b40: 6865 206c 6f63 6174 696f 6e2f 7320 7768  he location/s wh
+00018b50: 6572 6520 616c 6c20 7361 6d70 6c65 6420  ere all sampled 
+00018b60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b80: 2020 2020 2020 2020 2020 2249 6e64 6976            "Indiv
+00018b90: 6964 7561 6c73 2073 686f 756c 6420 6265  iduals should be
+00018ba0: 2070 6c61 6365 642e 2229 0a20 2020 2020   placed.").     
+00018bb0: 2020 2020 2020 2063 6f6f 7264 7320 3d20         coords = 
+00018bc0: 706f 705b 6e5d 2e70 6f70 2827 636f 6f72  pop[n].pop('coor
+00018bd0: 6473 2729 0a20 2020 2020 2020 2020 2020  ds').           
+00018be0: 2061 7373 6572 7420 2869 7369 6e73 7461   assert (isinsta
+00018bf0: 6e63 6528 636f 6f72 6473 2c20 6c69 7374  nce(coords, list
+00018c00: 2920 6f72 0a20 2020 2020 2020 2020 2020  ) or.           
+00018c10: 2020 2020 2020 2020 2069 7369 6e73 7461           isinsta
+00018c20: 6e63 6528 636f 6f72 6473 2c20 7475 706c  nce(coords, tupl
+00018c30: 6529 206f 720a 2020 2020 2020 2020 2020  e) or.          
+00018c40: 2020 2020 2020 2020 2020 6973 696e 7374            isinst
+00018c50: 616e 6365 2863 6f6f 7264 732c 206e 702e  ance(coords, np.
+00018c60: 6e64 6172 7261 7929 292c 2028 2254 6865  ndarray)), ("The
+00018c70: 2027 636f 6f72 6473 2720 6b65 7920 220a   'coords' key ".
+00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c90: 2020 2020 2020 2020 2269 6e20 7468 6520          "in the 
+00018ca0: 696e 6974 2064 6963 7420 666f 7220 616e  init dict for an
+00018cb0: 206d 7370 7269 6d65 2073 6f75 7263 6520   msprime source 
+00018cc0: 706f 7075 6c61 7469 6f6e 2022 0a20 2020  population ".   
+00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ce0: 2020 2020 2022 6d75 7374 2068 6176 6520       "must have 
+00018cf0: 6120 6c69 7374 2c20 7475 706c 652c 206f  a list, tuple, o
+00018d00: 7220 6e75 6d70 792e 6e64 6172 7261 7920  r numpy.ndarray 
+00018d10: 6173 2022 0a20 2020 2020 2020 2020 2020  as ".           
+00018d20: 2020 2020 2020 2020 2020 2020 2022 6974               "it
+00018d30: 7320 7661 6c75 652e 2229 0a20 2020 2020  s value.").     
+00018d40: 2020 2020 2020 2063 6f6f 7264 735f 7374         coords_st
+00018d50: 7275 6374 5f65 7272 5f6d 7367 203d 2028  ruct_err_msg = (
+00018d60: 2254 6865 2027 636f 6f72 6473 2720 7661  "The 'coords' va
+00018d70: 6c75 6520 666f 7220 220a 2020 2020 2020  lue for ".      
+00018d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d90: 2020 2261 6e20 6d73 7072 696d 6520 736f    "an msprime so
+00018da0: 7572 6365 2070 6f70 756c 6174 6f6e 206d  urce populaton m
+00018db0: 7573 7420 6265 206f 6e65 206f 663a 2022  ust be one of: "
+00018dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018dd0: 2020 2020 2020 2020 2022 312e 2920 6120           "1.) a 
+00018de0: 6c69 7374 206f 7220 7475 706c 6520 6f66  list or tuple of
+00018df0: 206c 656e 6774 6820 322c 2067 6976 696e   length 2, givin
+00018e00: 6720 7468 6520 220a 2020 2020 2020 2020  g the ".        
 00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e20: 2020 2020 2020 2022 7769 6c6c 2062 6567         "will beg
-00018e30: 696e 2074 6865 2073 696d 756c 6174 696f  in the simulatio
-00018e40: 6e3b 2032 2e29 2061 206c 6973 7420 6f72  n; 2.) a list or
-00018e50: 2074 7570 6c65 206f 6620 220a 2020 2020   tuple of ".    
-00018e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e70: 2020 2020 2263 6f6f 7264 696e 6174 6520      "coordinate 
-00018e80: 7061 6972 7320 666f 7220 616c 6c20 496e  pairs for all In
-00018e90: 6469 7669 6475 616c 7320 2873 7472 7563  dividuals (struc
-00018ea0: 7475 7265 6420 220a 2020 2020 2020 2020  tured ".        
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ec0: 2261 7320 6e20 7375 626c 6973 7473 206f  "as n sublists o
-00018ed0: 7220 7375 6274 7570 6c65 732c 2065 6163  r subtuples, eac
-00018ee0: 6820 6f66 206c 656e 6774 6820 3229 3b20  h of length 2); 
-00018ef0: 6f72 2022 0a20 2020 2020 2020 2020 2020  or ".           
-00018f00: 2020 2020 2020 2020 2020 2020 2022 332e               "3.
-00018f10: 2920 6120 6e75 6d70 792e 6e64 6172 7261  ) a numpy.ndarra
-00018f20: 7920 6f66 2074 6865 2073 616d 6520 7374  y of the same st
-00018f30: 7275 6374 7572 6520 2869 2e65 2e2c 2022  ructure (i.e., "
-00018f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f50: 2020 2020 2020 2020 2022 6569 7468 6572           "either
-00018f60: 2031 7832 2c20 6769 7669 6e67 2061 2073   1x2, giving a s
-00018f70: 696e 676c 6520 636f 6f72 6469 6e61 7465  ingle coordinate
-00018f80: 2070 6169 7220 666f 7220 220a 2020 2020   pair for ".    
-00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fa0: 2020 2020 2261 6c6c 2049 6e64 6976 6964      "all Individ
-00018fb0: 7561 6c73 2c20 6f72 206e 7832 2c20 7370  uals, or nx2, sp
-00018fc0: 6563 6966 7969 6e67 206c 6f63 6174 696f  ecifying locatio
-00018fd0: 6e73 2066 6f72 2022 0a20 2020 2020 2020  ns for ".       
-00018fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ff0: 2022 616c 6c20 6e20 496e 6469 7669 6475   "all n Individu
-00019000: 616c 7329 2e22 290a 2020 2020 2020 2020  als).").        
-00019010: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00019020: 6528 636f 6f72 6473 2c20 6c69 7374 2920  e(coords, list) 
-00019030: 6f72 2069 7369 6e73 7461 6e63 6528 636f  or isinstance(co
-00019040: 6f72 6473 2c20 7475 706c 6529 3a0a 2020  ords, tuple):.  
-00019050: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00019060: 2069 7369 6e73 7461 6e63 6528 636f 6f72   isinstance(coor
-00019070: 6473 5b30 5d2c 206c 6973 7429 206f 7220  ds[0], list) or 
-00019080: 6973 696e 7374 616e 6365 2863 6f6f 7264  isinstance(coord
-00019090: 735b 305d 2c20 7475 706c 6529 3a0a 2020  s[0], tuple):.  
-000190a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190b0: 2020 6173 7365 7274 2028 6e70 2e61 6c6c    assert (np.all
-000190c0: 285b 6c65 6e28 6329 203d 3d20 3220 666f  ([len(c) == 2 fo
-000190d0: 7220 6320 696e 2063 6f6f 7264 735d 2920  r c in coords]) 
-000190e0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019100: 6c65 6e28 636f 6f72 6473 2920 3d3d 206e  len(coords) == n
-00019110: 292c 2063 6f6f 7264 735f 7374 7275 6374  ), coords_struct
-00019120: 5f65 7272 5f6d 7367 0a20 2020 2020 2020  _err_msg.       
-00019130: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00019140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019150: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
-00019160: 6f72 6473 2920 3d3d 2032 2c20 636f 6f72  ords) == 2, coor
-00019170: 6473 5f73 7472 7563 745f 6572 725f 6d73  ds_struct_err_ms
-00019180: 670a 2020 2020 2020 2020 2020 2020 656c  g.            el
-00019190: 6966 2069 7369 6e73 7461 6e63 6528 636f  if isinstance(co
-000191a0: 6f72 6473 2c20 6e70 2e6e 6461 7272 6179  ords, np.ndarray
-000191b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000191c0: 2020 2061 7373 6572 7420 2863 6f6f 7264     assert (coord
-000191d0: 732e 7368 6170 6520 3d3d 2028 312c 2032  s.shape == (1, 2
-000191e0: 2920 6f72 0a20 2020 2020 2020 2020 2020  ) or.           
-000191f0: 2020 2020 2020 2020 2020 2020 2063 6f6f               coo
-00019200: 7264 732e 7368 6170 6520 3d3d 2028 6e2c  rds.shape == (n,
-00019210: 2032 2929 2c20 636f 6f72 6473 5f73 7472   2)), coords_str
-00019220: 7573 745f 6572 725f 6d73 670a 2020 2020  ust_err_msg.    
-00019230: 2020 2020 2020 2020 2320 7369 6d75 6c61          # simula
-00019240: 7465 2074 6865 2069 6e64 6976 6964 7561  te the individua
-00019250: 6c73 2061 6e64 2061 6464 2074 6865 6d20  ls and add them 
-00019260: 746f 2074 6865 2053 7065 6369 6573 0a20  to the Species. 
-00019270: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019280: 5f61 6464 5f69 6e64 6976 6964 7561 6c73  _add_individuals
-00019290: 286e 3d6e 2c0a 2020 2020 2020 2020 2020  (n=n,.          
-000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192b0: 2020 2020 2020 2020 636f 6f72 6473 3d63          coords=c
-000192c0: 6f6f 7264 732c 0a20 2020 2020 2020 2020  oords,.         
-000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192e0: 2020 2020 2020 2020 206c 616e 643d 6c61           land=la
-000192f0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-00019300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019310: 2020 2020 2020 736f 7572 6365 5f6d 7370        source_msp
-00019320: 7269 6d65 5f70 6172 616d 733d 706f 705b  rime_params=pop[
-00019330: 6e5d 2c0a 2020 2020 2020 2020 2020 2020  n],.            
+00018e20: 2263 6f6f 7264 696e 6174 6520 7061 6972  "coordinate pair
+00018e30: 2061 7420 7768 6963 6820 616c 6c20 496e   at which all In
+00018e40: 6469 7669 6475 616c 7320 220a 2020 2020  dividuals ".    
+00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e60: 2020 2020 2277 696c 6c20 6265 6769 6e20      "will begin 
+00018e70: 7468 6520 7369 6d75 6c61 7469 6f6e 3b20  the simulation; 
+00018e80: 322e 2920 6120 6c69 7374 206f 7220 7475  2.) a list or tu
+00018e90: 706c 6520 6f66 2022 0a20 2020 2020 2020  ple of ".       
+00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018eb0: 2022 636f 6f72 6469 6e61 7465 2070 6169   "coordinate pai
+00018ec0: 7273 2066 6f72 2061 6c6c 2049 6e64 6976  rs for all Indiv
+00018ed0: 6964 7561 6c73 2028 7374 7275 6374 7572  iduals (structur
+00018ee0: 6564 2022 0a20 2020 2020 2020 2020 2020  ed ".           
+00018ef0: 2020 2020 2020 2020 2020 2020 2022 6173               "as
+00018f00: 206e 2073 7562 6c69 7374 7320 6f72 2073   n sublists or s
+00018f10: 7562 7475 706c 6573 2c20 6561 6368 206f  ubtuples, each o
+00018f20: 6620 6c65 6e67 7468 2032 293b 206f 7220  f length 2); or 
+00018f30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018f40: 2020 2020 2020 2020 2020 2233 2e29 2061            "3.) a
+00018f50: 206e 756d 7079 2e6e 6461 7272 6179 206f   numpy.ndarray o
+00018f60: 6620 7468 6520 7361 6d65 2073 7472 7563  f the same struc
+00018f70: 7475 7265 2028 692e 652e 2c20 220a 2020  ture (i.e., ".  
+00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f90: 2020 2020 2020 2265 6974 6865 7220 3178        "either 1x
+00018fa0: 322c 2067 6976 696e 6720 6120 7369 6e67  2, giving a sing
+00018fb0: 6c65 2063 6f6f 7264 696e 6174 6520 7061  le coordinate pa
+00018fc0: 6972 2066 6f72 2022 0a20 2020 2020 2020  ir for ".       
+00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fe0: 2022 616c 6c20 496e 6469 7669 6475 616c   "all Individual
+00018ff0: 732c 206f 7220 6e78 322c 2073 7065 6369  s, or nx2, speci
+00019000: 6679 696e 6720 6c6f 6361 7469 6f6e 7320  fying locations 
+00019010: 666f 7220 220a 2020 2020 2020 2020 2020  for ".          
+00019020: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00019030: 6c6c 206e 2049 6e64 6976 6964 7561 6c73  ll n Individuals
+00019040: 292e 2229 0a20 2020 2020 2020 2020 2020  ).").           
+00019050: 2069 6620 6973 696e 7374 616e 6365 2863   if isinstance(c
+00019060: 6f6f 7264 732c 206c 6973 7429 206f 7220  oords, list) or 
+00019070: 6973 696e 7374 616e 6365 2863 6f6f 7264  isinstance(coord
+00019080: 732c 2074 7570 6c65 293a 0a20 2020 2020  s, tuple):.     
+00019090: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000190a0: 696e 7374 616e 6365 2863 6f6f 7264 735b  instance(coords[
+000190b0: 305d 2c20 6c69 7374 2920 6f72 2069 7369  0], list) or isi
+000190c0: 6e73 7461 6e63 6528 636f 6f72 6473 5b30  nstance(coords[0
+000190d0: 5d2c 2074 7570 6c65 293a 0a20 2020 2020  ], tuple):.     
+000190e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000190f0: 7373 6572 7420 286e 702e 616c 6c28 5b6c  ssert (np.all([l
+00019100: 656e 2863 2920 3d3d 2032 2066 6f72 2063  en(c) == 2 for c
+00019110: 2069 6e20 636f 6f72 6473 5d29 2061 6e64   in coords]) and
+00019120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019130: 2020 2020 2020 2020 2020 2020 206c 656e               len
+00019140: 2863 6f6f 7264 7329 203d 3d20 6e29 2c20  (coords) == n), 
+00019150: 636f 6f72 6473 5f73 7472 7563 745f 6572  coords_struct_er
+00019160: 725f 6d73 670a 2020 2020 2020 2020 2020  r_msg.          
+00019170: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019190: 6173 7365 7274 206c 656e 2863 6f6f 7264  assert len(coord
+000191a0: 7329 203d 3d20 322c 2063 6f6f 7264 735f  s) == 2, coords_
+000191b0: 7374 7275 6374 5f65 7272 5f6d 7367 0a20  struct_err_msg. 
+000191c0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000191d0: 6973 696e 7374 616e 6365 2863 6f6f 7264  isinstance(coord
+000191e0: 732c 206e 702e 6e64 6172 7261 7929 3a0a  s, np.ndarray):.
+000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019200: 6173 7365 7274 2028 636f 6f72 6473 2e73  assert (coords.s
+00019210: 6861 7065 203d 3d20 2831 2c20 3229 206f  hape == (1, 2) o
+00019220: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00019230: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
+00019240: 2e73 6861 7065 203d 3d20 286e 2c20 3229  .shape == (n, 2)
+00019250: 292c 2063 6f6f 7264 735f 7374 7275 7374  ), coords_strust
+00019260: 5f65 7272 5f6d 7367 0a20 2020 2020 2020  _err_msg.       
+00019270: 2020 2020 2023 2073 696d 756c 6174 6520       # simulate 
+00019280: 7468 6520 696e 6469 7669 6475 616c 7320  the individuals 
+00019290: 616e 6420 6164 6420 7468 656d 2074 6f20  and add them to 
+000192a0: 7468 6520 5370 6563 6965 730a 2020 2020  the Species.    
+000192b0: 2020 2020 2020 2020 7365 6c66 2e5f 6164          self._ad
+000192c0: 645f 696e 6469 7669 6475 616c 7328 6e3d  d_individuals(n=
+000192d0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+000192e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192f0: 2020 2020 2063 6f6f 7264 733d 636f 6f72       coords=coor
+00019300: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+00019310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019320: 2020 2020 2020 6c61 6e64 3d6c 616e 642c        land=land,
+00019330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
-00019360: 2063 6865 636b 2074 6861 7420 7468 6520   check that the 
-00019370: 5370 6563 6965 7320 776f 756e 6420 7570  Species wound up
-00019380: 2068 6176 696e 6720 7468 6520 636f 7272   having the corr
-00019390: 6563 7420 706f 7075 6c61 7469 6f6e 2073  ect population s
-000193a0: 697a 650a 2020 2020 2020 2020 6173 7365  ize.        asse
-000193b0: 7274 206c 656e 2873 656c 6629 203d 3d20  rt len(self) == 
-000193c0: 7461 7267 6574 5f73 697a 652c 2028 2241  target_size, ("A
-000193d0: 6674 6572 2061 6c6c 206d 7370 7269 6d65  fter all msprime
-000193e0: 2073 6f75 7263 6520 220a 2020 2020 2020   source ".      
-000193f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019400: 2020 2270 6f70 756c 6174 696f 6e73 2077    "populations w
-00019410: 6572 6520 7361 6d70 6c65 642c 2074 6865  ere sampled, the
-00019420: 2072 6573 756c 7469 6e67 2022 0a20 2020   resulting ".   
-00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2020 2020 2022 706f 7075 6c61 7469 6f6e       "population
-00019450: 2073 697a 6520 646f 6573 206e 6f74 2061   size does not a
-00019460: 6772 6565 2077 6974 6820 220a 2020 2020  gree with ".    
+00019350: 2020 2073 6f75 7263 655f 6d73 7072 696d     source_msprim
+00019360: 655f 7061 7261 6d73 3d70 6f70 5b6e 5d2c  e_params=pop[n],
+00019370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019390: 2020 290a 2020 2020 2020 2020 2320 6368    ).        # ch
+000193a0: 6563 6b20 7468 6174 2074 6865 2053 7065  eck that the Spe
+000193b0: 6369 6573 2077 6f75 6e64 2075 7020 6861  cies wound up ha
+000193c0: 7669 6e67 2074 6865 2063 6f72 7265 6374  ving the correct
+000193d0: 2070 6f70 756c 6174 696f 6e20 7369 7a65   population size
+000193e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000193f0: 6c65 6e28 7365 6c66 2920 3d3d 2074 6172  len(self) == tar
+00019400: 6765 745f 7369 7a65 2c20 2822 4166 7465  get_size, ("Afte
+00019410: 7220 616c 6c20 6d73 7072 696d 6520 736f  r all msprime so
+00019420: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+00019430: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019440: 706f 7075 6c61 7469 6f6e 7320 7765 7265  populations were
+00019450: 2073 616d 706c 6564 2c20 7468 6520 7265   sampled, the re
+00019460: 7375 6c74 696e 6720 220a 2020 2020 2020  sulting ".      
 00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019480: 2020 2020 2274 6865 2073 756d 206f 6620      "the sum of 
-00019490: 7468 6520 736f 7572 6365 2070 6f70 756c  the source popul
-000194a0: 6174 696f 6e20 7361 6d70 6c65 7320 220a  ation samples ".
+00019480: 2020 2270 6f70 756c 6174 696f 6e20 7369    "population si
+00019490: 7a65 2064 6f65 7320 6e6f 7420 6167 7265  ze does not agre
+000194a0: 6520 7769 7468 2022 0a20 2020 2020 2020  e with ".       
 000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194c0: 2020 2020 2020 2020 2273 7469 7075 6c61          "stipula
-000194d0: 7465 6420 696e 2074 6865 2070 6172 616d  ted in the param
-000194e0: 6574 6572 7320 6669 6c65 2e22 290a 0a0a  eters file.")...
-000194f0: 2020 2020 2375 7365 2074 6865 206b 645f      #use the kd_
-00019500: 7472 6565 2061 7474 7269 6275 7465 2074  tree attribute t
-00019510: 6f20 6669 6e64 206d 6174 696e 6720 7061  o find mating pa
-00019520: 6972 7320 6569 7468 6572 0a20 2020 2023  irs either.    #
-00019530: 7769 7468 696e 2074 6865 2073 7065 6369  within the speci
-00019540: 6573 2c20 6966 2077 6974 6869 6e20 3d3d  es, if within ==
-00019550: 2054 7275 652c 206f 7220 6265 7477 6565   True, or betwee
-00019560: 6e20 7468 6520 7370 6563 6965 730a 2020  n the species.  
-00019570: 2020 2361 6e64 2074 6865 2070 6f69 6e74    #and the point
-00019580: 7320 7072 6f76 6964 6564 2c20 6966 2077  s provided, if w
-00019590: 6974 6869 6e20 3d3d 2046 616c 7365 2061  ithin == False a
-000195a0: 6e64 2070 6f69 6e74 7320 6973 206e 6f74  nd points is not
-000195b0: 204e 6f6e 650a 2020 2020 6465 6620 5f67   None.    def _g
-000195c0: 6574 5f6d 6174 696e 675f 7061 6972 7328  et_mating_pairs(
-000195d0: 7365 6c66 2c20 7769 7468 696e 3d54 7275  self, within=Tru
-000195e0: 652c 2063 6f6f 7264 733d 4e6f 6e65 2c0a  e, coords=None,.
-000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019600: 2020 2020 2020 2020 2020 6368 6f6f 7365            choose
-00019610: 5f6e 6561 7265 7374 3d46 616c 7365 2c20  _nearest=False, 
-00019620: 696e 7665 7273 655f 6469 7374 5f6d 6174  inverse_dist_mat
-00019630: 696e 673d 4661 6c73 6529 3a0a 2020 2020  ing=False):.    
-00019640: 2020 2020 234e 4f54 453a 2049 6e20 6c69      #NOTE: In li
-00019650: 6575 206f 6620 6120 6d6f 7265 2073 6f70  eu of a more sop
-00019660: 6869 7374 6963 6174 6564 2077 6179 206f  histicated way o
-00019670: 660a 2020 2020 2020 2020 2364 6574 6572  f.        #deter
-00019680: 6d69 6e69 6e67 2077 6865 7468 6572 2074  mining whether t
-00019690: 6865 206b 645f 7472 6565 206e 6565 6473  he kd_tree needs
-000196a0: 2074 6f20 6265 2075 7064 6174 6564 200a   to be updated .
-000196b0: 2020 2020 2020 2020 2328 692e 652e 2069          #(i.e. i
-000196c0: 6620 7468 6520 7370 6563 6965 7320 6861  f the species ha
-000196d0: 7665 2075 6e64 6572 676f 6e65 206d 6f76  ve undergone mov
-000196e0: 656d 656e 742c 206d 6174 696e 672c 0a20  ement, mating,. 
-000196f0: 2020 2020 2020 2023 6f72 206d 6f72 7461         #or morta
-00019700: 6c69 7479 2073 696e 6365 2074 6865 206c  lity since the l
-00019710: 6173 7420 7469 6d65 2069 7420 7761 7320  ast time it was 
-00019720: 0a20 2020 2020 2020 2023 636f 6e73 7472  .        #constr
-00019730: 7563 7465 6429 2c20 616e 6420 696e 2061  ucted), and in a
-00019740: 6e20 6566 666f 7274 2074 6f20 6d69 6e69  n effort to mini
-00019750: 6d69 7a65 2074 6865 206e 756d 6265 720a  mize the number.
-00019760: 2020 2020 2020 2020 236f 6620 7469 6d65          #of time
-00019770: 7320 6974 2069 7320 636f 6e73 7472 7563  s it is construc
-00019780: 7465 6420 6561 6368 2074 696d 6520 2873  ted each time (s
-00019790: 696e 6365 0a20 2020 2020 2020 2023 6974  ince.        #it
-000197a0: 2773 206e 6f74 2061 6e20 696e 636f 6e73  's not an incons
-000197b0: 6571 7565 6e74 6961 6c20 7275 6e74 696d  equential runtim
-000197c0: 652c 2073 6f20 7465 6c6c 696e 6720 7468  e, so telling th
-000197d0: 650a 2020 2020 2020 2020 236d 6f64 656c  e.        #model
-000197e0: 2074 6f20 7265 6275 696c 6420 6974 2061   to rebuild it a
-000197f0: 6674 6572 2065 6163 6820 6d6f 7665 2c20  fter each move, 
-00019800: 6269 7274 682c 206f 720a 2020 2020 2020  birth, or.      
-00019810: 2020 2364 6561 7468 2073 7465 7020 636f    #death step co
-00019820: 756c 6420 6265 2075 6e6e 6365 7373 6172  uld be unncessar
-00019830: 696c 7920 636f 7374 6c79 292c 2066 6f72  ily costly), for
-00019840: 206e 6f77 2049 0a20 2020 2020 2020 2023   now I.        #
-00019850: 616d 206a 7573 7420 7465 6c6c 696e 6720  am just telling 
-00019860: 7468 6520 7472 6565 2074 6f20 6265 2072  the tree to be r
-00019870: 6562 7569 6c74 2065 6163 6820 7469 6d65  ebuilt each time
-00019880: 200a 2020 2020 2020 2020 2374 6865 2073   .        #the s
-00019890: 7070 2e5f 6765 745f 6d61 7469 6e67 5f70  pp._get_mating_p
-000198a0: 6169 7273 2829 206d 6574 686f 6420 6973  airs() method is
-000198b0: 2063 616c 6c65 6421 0a20 2020 2020 2020   called!.       
-000198c0: 2073 656c 662e 5f73 6574 5f6b 645f 7472   self._set_kd_tr
-000198d0: 6565 2829 0a0a 2020 2020 2020 2020 2320  ee()..        # 
-000198e0: 6966 206d 6174 696e 675f 7261 6469 7573  if mating_radius
-000198f0: 2069 7320 4e6f 6e65 2c20 7468 656e 206a   is None, then j
-00019900: 7573 7420 7573 6520 5772 6967 6874 2d46  ust use Wright-F
-00019910: 6973 6865 720a 2020 2020 2020 2020 2320  isher.        # 
-00019920: 7374 796c 6520 7061 6e6d 6978 6961 2028  style panmixia (
-00019930: 6472 6177 2077 6974 6820 7265 706c 6163  draw with replac
-00019940: 656d 656e 7420 6120 7361 6d70 6c65 0a20  ement a sample. 
-00019950: 2020 2020 2020 2023 206f 6620 7369 7a65         # of size
-00019960: 203d 204e 742a 622c 2077 6865 7265 204e   = Nt*b, where N
-00019970: 7420 6973 2074 6865 200a 2020 2020 2020  t is the .      
-00019980: 2020 2320 6375 7272 656e 7420 706f 7020    # current pop 
-00019990: 7369 7a65 2061 6e64 2062 2069 7320 7468  size and b is th
-000199a0: 6520 6269 7274 6820 7261 7465 2028 692e  e birth rate (i.
-000199b0: 652e 206d 6174 696e 6720 7072 6f62 6162  e. mating probab
-000199c0: 696c 6974 7929 3b0a 2020 2020 2020 2020  ility);.        
-000199d0: 2320 7468 6174 2073 616d 706c 6520 7265  # that sample re
-000199e0: 7072 6573 656e 7473 2061 6c6c 206d 6174  presents all mat
-000199f0: 696e 6720 696e 6469 7669 6475 616c 732c  ing individuals,
-00019a00: 2061 6e64 2065 6163 6820 6f66 2074 686f   and each of tho
-00019a10: 7365 0a20 2020 2020 2020 2023 2069 6e64  se.        # ind
-00019a20: 6976 6964 7561 6c73 2072 616e 646f 6d6c  ividuals randoml
-00019a30: 7920 6368 6f6f 7365 7320 6974 7320 6d61  y chooses its ma
-00019a40: 7465 0a20 2020 2020 2020 2069 6620 7365  te.        if se
-00019a50: 6c66 2e6d 6174 696e 675f 7261 6469 7573  lf.mating_radius
-00019a60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00019a70: 2020 2020 2020 2320 6472 6177 2061 206e        # draw a n
-00019a80: 756d 6265 7220 6f66 206d 6174 696e 6720  umber of mating 
-00019a90: 696e 6469 7669 6475 616c 7320 6173 2061  individuals as a
-00019aa0: 2062 696e 6f6d 6961 6c20 7276 0a20 2020   binomial rv.   
-00019ab0: 2020 2020 2020 2020 2023 2077 6974 6820           # with 
-00019ac0: 6e75 6d20 7472 6961 6c73 2065 7175 616c  num trials equal
-00019ad0: 2074 6f20 706f 7020 7369 7a65 2061 6e64   to pop size and
-00019ae0: 2070 726f 6261 6269 6c69 7479 2065 7175   probability equ
-00019af0: 616c 2074 6f0a 2020 2020 2020 2020 2020  al to.          
-00019b00: 2020 2320 7468 6520 7370 6563 6965 7327    # the species'
-00019b10: 2062 6972 7468 2072 6174 650a 2020 2020   birth rate.    
-00019b20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00019b30: 6220 3c20 313a 0a20 2020 2020 2020 2020  b < 1:.         
-00019b40: 2020 2020 2020 206e 5f6d 6174 6573 203d         n_mates =
-00019b50: 206e 702e 7261 6e64 6f6d 2e62 696e 6f6d   np.random.binom
-00019b60: 6961 6c28 6e3d 6c65 6e28 7365 6c66 292c  ial(n=len(self),
-00019b70: 2070 3d73 656c 662e 6229 0a20 2020 2020   p=self.b).     
-00019b80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00019b90: 2020 2020 2020 2020 2020 2020 206e 5f6d               n_m
-00019ba0: 6174 6573 203d 206c 656e 2873 656c 6629  ates = len(self)
-00019bb0: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-00019bc0: 655f 696e 6473 203d 2073 656c 662e 5f6b  e_inds = self._k
-00019bd0: 645f 7472 6565 2e74 7265 652e 696e 6469  d_tree.tree.indi
-00019be0: 6365 730a 2020 2020 2020 2020 2020 2020  ces.            
-00019bf0: 2320 6472 6177 2032 2a6e 5f6d 6174 6573  # draw 2*n_mates
-00019c00: 206d 6174 696e 6720 696e 6469 7669 6475   mating individu
-00019c10: 616c 732c 2077 6974 6820 7265 706c 6163  als, with replac
-00019c20: 656d 656e 7420 2861 7320 696e 2057 460a  ement (as in WF.
-00019c30: 2020 2020 2020 2020 2020 2020 2320 6d6f              # mo
-00019c40: 6465 6c29 2c20 7468 656e 2066 6f6c 6420  del), then fold 
-00019c50: 696e 746f 2061 6e20 6e5f 6d61 7465 7320  into an n_mates 
-00019c60: 7820 3220 6d61 7465 2d70 6169 7273 2061  x 2 mate-pairs a
-00019c70: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-00019c80: 2070 6169 7273 203d 206e 702e 7261 6e64   pairs = np.rand
-00019c90: 6f6d 2e63 686f 6963 6528 7472 6565 5f69  om.choice(tree_i
-00019ca0: 6e64 732c 2072 6570 6c61 6365 3d54 7275  nds, replace=Tru
-00019cb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00019cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cd0: 2020 2020 2020 2020 7369 7a65 3d6e 5f6d          size=n_m
-00019ce0: 6174 6573 2a32 292e 7265 7368 6170 6528  ates*2).reshape(
-00019cf0: 286e 5f6d 6174 6573 2c20 3229 290a 2020  (n_mates, 2)).  
-00019d00: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-00019d10: 7269 6420 6f66 2073 656c 6669 6e67 2070  rid of selfing p
-00019d20: 6169 7273 0a20 2020 2020 2020 2020 2020  airs.           
-00019d30: 2070 6169 7273 203d 206e 702e 6172 7261   pairs = np.arra
-00019d40: 7928 5b6c 6973 7428 7061 6972 2920 666f  y([list(pair) fo
-00019d50: 7220 7061 6972 2069 6e20 6c69 7374 280a  r pair in list(.
-00019d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d80: 2020 2020 6d61 7028 7365 742c 2070 6169      map(set, pai
-00019d90: 7273 2929 2069 6620 6c65 6e28 7061 6972  rs)) if len(pair
-00019da0: 2920 3d3d 2032 5d29 0a20 2020 2020 2020  ) == 2]).       
-00019db0: 2020 2020 2070 6169 7273 203d 206e 702e       pairs = np.
-00019dc0: 6172 7261 7928 7061 6972 7329 0a0a 2020  array(pairs)..  
-00019dd0: 2020 2020 2020 2320 6f74 6865 7277 6973        # otherwis
-00019de0: 652c 2063 686f 6f73 6520 6d61 7465 7320  e, choose mates 
-00019df0: 7573 696e 6720 6d61 7469 6e67 2072 6164  using mating rad
-00019e00: 6975 730a 2020 2020 2020 2020 656c 7365  ius.        else
-00019e10: 3a0a 2020 2020 2020 2020 2020 2020 2369  :.            #i
-00019e20: 6620 6e65 6967 6862 6f72 7320 6172 6520  f neighbors are 
-00019e30: 746f 2062 6520 666f 756e 6420 7769 7468  to be found with
-00019e40: 696e 2074 6865 2073 7065 6369 6573 2c0a  in the species,.
-00019e50: 2020 2020 2020 2020 2020 2020 2373 6574              #set
-00019e60: 2063 6f6f 7264 7320 746f 2073 656c 662e   coords to self.
-00019e70: 5f63 6f6f 7264 7320 286f 7468 6572 7769  _coords (otherwi
-00019e80: 7365 2c20 7468 6520 636f 6f72 6473 2074  se, the coords t
-00019e90: 6f0a 2020 2020 2020 2020 2020 2020 2366  o.            #f
-00019ea0: 696e 6420 6e65 6172 6573 7420 6e65 6967  ind nearest neig
-00019eb0: 6862 6f72 7320 7769 7468 2073 686f 756c  hbors with shoul
-00019ec0: 6420 6861 7665 2062 6565 6e20 7072 6f76  d have been prov
-00019ed0: 6964 6564 290a 2020 2020 2020 2020 2020  ided).          
-00019ee0: 2020 6966 2077 6974 6869 6e3a 0a20 2020    if within:.   
-00019ef0: 2020 2020 2020 2020 2020 2020 2063 6f6f               coo
-00019f00: 7264 7320 3d20 7365 6c66 2e5f 636f 6f72  rds = self._coor
-00019f10: 6473 0a0a 2020 2020 2020 2020 2020 2020  ds..            
-00019f20: 2371 7565 7279 2074 6865 2074 7265 6520  #query the tree 
-00019f30: 746f 2067 6574 206d 6174 696e 6720 7061  to get mating pa
-00019f40: 6972 730a 2020 2020 2020 2020 2020 2020  irs.            
-00019f50: 7061 6972 7320 3d20 7365 6c66 2e5f 6b64  pairs = self._kd
-00019f60: 5f74 7265 652e 5f67 6574 5f6d 6174 696e  _tree._get_matin
-00019f70: 675f 7061 6972 7328 636f 6f72 6473 3d63  g_pairs(coords=c
-00019f80: 6f6f 7264 732c 0a20 2020 2020 2020 2020  oords,.         
-00019f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fb0: 2020 2020 2020 2064 6973 743d 7365 6c66         dist=self
-00019fc0: 2e6d 6174 696e 675f 7261 6469 7573 2c0a  .mating_radius,.
+000194c0: 2022 7468 6520 7375 6d20 6f66 2074 6865   "the sum of the
+000194d0: 2073 6f75 7263 6520 706f 7075 6c61 7469   source populati
+000194e0: 6f6e 2073 616d 706c 6573 2022 0a20 2020  on samples ".   
+000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019500: 2020 2020 2022 7374 6970 756c 6174 6564       "stipulated
+00019510: 2069 6e20 7468 6520 7061 7261 6d65 7465   in the paramete
+00019520: 7273 2066 696c 652e 2229 0a0a 0a20 2020  rs file.")...   
+00019530: 2023 7573 6520 7468 6520 6b64 5f74 7265   #use the kd_tre
+00019540: 6520 6174 7472 6962 7574 6520 746f 2066  e attribute to f
+00019550: 696e 6420 6d61 7469 6e67 2070 6169 7273  ind mating pairs
+00019560: 2065 6974 6865 720a 2020 2020 2377 6974   either.    #wit
+00019570: 6869 6e20 7468 6520 7370 6563 6965 732c  hin the species,
+00019580: 2069 6620 7769 7468 696e 203d 3d20 5472   if within == Tr
+00019590: 7565 2c20 6f72 2062 6574 7765 656e 2074  ue, or between t
+000195a0: 6865 2073 7065 6369 6573 0a20 2020 2023  he species.    #
+000195b0: 616e 6420 7468 6520 706f 696e 7473 2070  and the points p
+000195c0: 726f 7669 6465 642c 2069 6620 7769 7468  rovided, if with
+000195d0: 696e 203d 3d20 4661 6c73 6520 616e 6420  in == False and 
+000195e0: 706f 696e 7473 2069 7320 6e6f 7420 4e6f  points is not No
+000195f0: 6e65 0a20 2020 2064 6566 205f 6765 745f  ne.    def _get_
+00019600: 6d61 7469 6e67 5f70 6169 7273 2873 656c  mating_pairs(sel
+00019610: 662c 2077 6974 6869 6e3d 5472 7565 2c20  f, within=True, 
+00019620: 636f 6f72 6473 3d4e 6f6e 652c 0a20 2020  coords=None,.   
+00019630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019640: 2020 2020 2020 2063 686f 6f73 655f 6e65         choose_ne
+00019650: 6172 6573 743d 4661 6c73 652c 2069 6e76  arest=False, inv
+00019660: 6572 7365 5f64 6973 745f 6d61 7469 6e67  erse_dist_mating
+00019670: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
+00019680: 2023 4e4f 5445 3a20 496e 206c 6965 7520   #NOTE: In lieu 
+00019690: 6f66 2061 206d 6f72 6520 736f 7068 6973  of a more sophis
+000196a0: 7469 6361 7465 6420 7761 7920 6f66 0a20  ticated way of. 
+000196b0: 2020 2020 2020 2023 6465 7465 726d 696e         #determin
+000196c0: 696e 6720 7768 6574 6865 7220 7468 6520  ing whether the 
+000196d0: 6b64 5f74 7265 6520 6e65 6564 7320 746f  kd_tree needs to
+000196e0: 2062 6520 7570 6461 7465 6420 0a20 2020   be updated .   
+000196f0: 2020 2020 2023 2869 2e65 2e20 6966 2074       #(i.e. if t
+00019700: 6865 2073 7065 6369 6573 2068 6176 6520  he species have 
+00019710: 756e 6465 7267 6f6e 6520 6d6f 7665 6d65  undergone moveme
+00019720: 6e74 2c20 6d61 7469 6e67 2c0a 2020 2020  nt, mating,.    
+00019730: 2020 2020 236f 7220 6d6f 7274 616c 6974      #or mortalit
+00019740: 7920 7369 6e63 6520 7468 6520 6c61 7374  y since the last
+00019750: 2074 696d 6520 6974 2077 6173 200a 2020   time it was .  
+00019760: 2020 2020 2020 2363 6f6e 7374 7275 6374        #construct
+00019770: 6564 292c 2061 6e64 2069 6e20 616e 2065  ed), and in an e
+00019780: 6666 6f72 7420 746f 206d 696e 696d 697a  ffort to minimiz
+00019790: 6520 7468 6520 6e75 6d62 6572 0a20 2020  e the number.   
+000197a0: 2020 2020 2023 6f66 2074 696d 6573 2069       #of times i
+000197b0: 7420 6973 2063 6f6e 7374 7275 6374 6564  t is constructed
+000197c0: 2065 6163 6820 7469 6d65 2028 7369 6e63   each time (sinc
+000197d0: 650a 2020 2020 2020 2020 2369 7427 7320  e.        #it's 
+000197e0: 6e6f 7420 616e 2069 6e63 6f6e 7365 7175  not an inconsequ
+000197f0: 656e 7469 616c 2072 756e 7469 6d65 2c20  ential runtime, 
+00019800: 736f 2074 656c 6c69 6e67 2074 6865 0a20  so telling the. 
+00019810: 2020 2020 2020 2023 6d6f 6465 6c20 746f         #model to
+00019820: 2072 6562 7569 6c64 2069 7420 6166 7465   rebuild it afte
+00019830: 7220 6561 6368 206d 6f76 652c 2062 6972  r each move, bir
+00019840: 7468 2c20 6f72 0a20 2020 2020 2020 2023  th, or.        #
+00019850: 6465 6174 6820 7374 6570 2063 6f75 6c64  death step could
+00019860: 2062 6520 756e 6e63 6573 7361 7269 6c79   be unncessarily
+00019870: 2063 6f73 746c 7929 2c20 666f 7220 6e6f   costly), for no
+00019880: 7720 490a 2020 2020 2020 2020 2361 6d20  w I.        #am 
+00019890: 6a75 7374 2074 656c 6c69 6e67 2074 6865  just telling the
+000198a0: 2074 7265 6520 746f 2062 6520 7265 6275   tree to be rebu
+000198b0: 696c 7420 6561 6368 2074 696d 6520 0a20  ilt each time . 
+000198c0: 2020 2020 2020 2023 7468 6520 7370 702e         #the spp.
+000198d0: 5f67 6574 5f6d 6174 696e 675f 7061 6972  _get_mating_pair
+000198e0: 7328 2920 6d65 7468 6f64 2069 7320 6361  s() method is ca
+000198f0: 6c6c 6564 210a 2020 2020 2020 2020 7365  lled!.        se
+00019900: 6c66 2e5f 7365 745f 6b64 5f74 7265 6528  lf._set_kd_tree(
+00019910: 290a 0a20 2020 2020 2020 2023 2069 6620  )..        # if 
+00019920: 6d61 7469 6e67 5f72 6164 6975 7320 6973  mating_radius is
+00019930: 204e 6f6e 652c 2074 6865 6e20 6a75 7374   None, then just
+00019940: 2075 7365 2057 7269 6768 742d 4669 7368   use Wright-Fish
+00019950: 6572 0a20 2020 2020 2020 2023 2073 7479  er.        # sty
+00019960: 6c65 2070 616e 6d69 7869 6120 2864 7261  le panmixia (dra
+00019970: 7720 7769 7468 2072 6570 6c61 6365 6d65  w with replaceme
+00019980: 6e74 2061 2073 616d 706c 650a 2020 2020  nt a sample.    
+00019990: 2020 2020 2320 6f66 2073 697a 6520 3d20      # of size = 
+000199a0: 4e74 2a62 2c20 7768 6572 6520 4e74 2069  Nt*b, where Nt i
+000199b0: 7320 7468 6520 0a20 2020 2020 2020 2023  s the .        #
+000199c0: 2063 7572 7265 6e74 2070 6f70 2073 697a   current pop siz
+000199d0: 6520 616e 6420 6220 6973 2074 6865 2062  e and b is the b
+000199e0: 6972 7468 2072 6174 6520 2869 2e65 2e20  irth rate (i.e. 
+000199f0: 6d61 7469 6e67 2070 726f 6261 6269 6c69  mating probabili
+00019a00: 7479 293b 0a20 2020 2020 2020 2023 2074  ty);.        # t
+00019a10: 6861 7420 7361 6d70 6c65 2072 6570 7265  hat sample repre
+00019a20: 7365 6e74 7320 616c 6c20 6d61 7469 6e67  sents all mating
+00019a30: 2069 6e64 6976 6964 7561 6c73 2c20 616e   individuals, an
+00019a40: 6420 6561 6368 206f 6620 7468 6f73 650a  d each of those.
+00019a50: 2020 2020 2020 2020 2320 696e 6469 7669          # indivi
+00019a60: 6475 616c 7320 7261 6e64 6f6d 6c79 2063  duals randomly c
+00019a70: 686f 6f73 6573 2069 7473 206d 6174 650a  hooses its mate.
+00019a80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019a90: 6d61 7469 6e67 5f72 6164 6975 7320 6973  mating_radius is
+00019aa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00019ab0: 2020 2023 2064 7261 7720 6120 6e75 6d62     # draw a numb
+00019ac0: 6572 206f 6620 6d61 7469 6e67 2069 6e64  er of mating ind
+00019ad0: 6976 6964 7561 6c73 2061 7320 6120 6269  ividuals as a bi
+00019ae0: 6e6f 6d69 616c 2072 760a 2020 2020 2020  nomial rv.      
+00019af0: 2020 2020 2020 2320 7769 7468 206e 756d        # with num
+00019b00: 2074 7269 616c 7320 6571 7561 6c20 746f   trials equal to
+00019b10: 2070 6f70 2073 697a 6520 616e 6420 7072   pop size and pr
+00019b20: 6f62 6162 696c 6974 7920 6571 7561 6c20  obability equal 
+00019b30: 746f 0a20 2020 2020 2020 2020 2020 2023  to.            #
+00019b40: 2074 6865 2073 7065 6369 6573 2720 6269   the species' bi
+00019b50: 7274 6820 7261 7465 0a20 2020 2020 2020  rth rate.       
+00019b60: 2020 2020 2069 6620 7365 6c66 2e62 203c       if self.b <
+00019b70: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00019b80: 2020 2020 6e5f 6d61 7465 7320 3d20 6e70      n_mates = np
+00019b90: 2e72 616e 646f 6d2e 6269 6e6f 6d69 616c  .random.binomial
+00019ba0: 286e 3d6c 656e 2873 656c 6629 2c20 703d  (n=len(self), p=
+00019bb0: 7365 6c66 2e62 290a 2020 2020 2020 2020  self.b).        
+00019bc0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00019bd0: 2020 2020 2020 2020 2020 6e5f 6d61 7465            n_mate
+00019be0: 7320 3d20 6c65 6e28 7365 6c66 290a 2020  s = len(self).  
+00019bf0: 2020 2020 2020 2020 2020 7472 6565 5f69            tree_i
+00019c00: 6e64 7320 3d20 7365 6c66 2e5f 6b64 5f74  nds = self._kd_t
+00019c10: 7265 652e 7472 6565 2e69 6e64 6963 6573  ree.tree.indices
+00019c20: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+00019c30: 7261 7720 322a 6e5f 6d61 7465 7320 6d61  raw 2*n_mates ma
+00019c40: 7469 6e67 2069 6e64 6976 6964 7561 6c73  ting individuals
+00019c50: 2c20 7769 7468 2072 6570 6c61 6365 6d65  , with replaceme
+00019c60: 6e74 2028 6173 2069 6e20 5746 0a20 2020  nt (as in WF.   
+00019c70: 2020 2020 2020 2020 2023 206d 6f64 656c           # model
+00019c80: 292c 2074 6865 6e20 666f 6c64 2069 6e74  ), then fold int
+00019c90: 6f20 616e 206e 5f6d 6174 6573 2078 2032  o an n_mates x 2
+00019ca0: 206d 6174 652d 7061 6972 7320 6172 7261   mate-pairs arra
+00019cb0: 790a 2020 2020 2020 2020 2020 2020 7061  y.            pa
+00019cc0: 6972 7320 3d20 6e70 2e72 616e 646f 6d2e  irs = np.random.
+00019cd0: 6368 6f69 6365 2874 7265 655f 696e 6473  choice(tree_inds
+00019ce0: 2c20 7265 706c 6163 653d 5472 7565 2c0a  , replace=True,.
+00019cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d10: 2020 2020 2073 697a 653d 6e5f 6d61 7465       size=n_mate
+00019d20: 732a 3229 2e72 6573 6861 7065 2828 6e5f  s*2).reshape((n_
+00019d30: 6d61 7465 732c 2032 2929 0a20 2020 2020  mates, 2)).     
+00019d40: 2020 2020 2020 2023 2067 6574 2072 6964         # get rid
+00019d50: 206f 6620 7365 6c66 696e 6720 7061 6972   of selfing pair
+00019d60: 730a 2020 2020 2020 2020 2020 2020 7061  s.            pa
+00019d70: 6972 7320 3d20 6e70 2e61 7272 6179 285b  irs = np.array([
+00019d80: 6c69 7374 2870 6169 7229 2066 6f72 2070  list(pair) for p
+00019d90: 6169 7220 696e 206c 6973 7428 0a20 2020  air in list(.   
+00019da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019dc0: 206d 6170 2873 6574 2c20 7061 6972 7329   map(set, pairs)
+00019dd0: 2920 6966 206c 656e 2870 6169 7229 203d  ) if len(pair) =
+00019de0: 3d20 325d 290a 2020 2020 2020 2020 2020  = 2]).          
+00019df0: 2020 7061 6972 7320 3d20 6e70 2e61 7272    pairs = np.arr
+00019e00: 6179 2870 6169 7273 290a 0a20 2020 2020  ay(pairs)..     
+00019e10: 2020 2023 206f 7468 6572 7769 7365 2c20     # otherwise, 
+00019e20: 6368 6f6f 7365 206d 6174 6573 2075 7369  choose mates usi
+00019e30: 6e67 206d 6174 696e 6720 7261 6469 7573  ng mating radius
+00019e40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00019e50: 2020 2020 2020 2020 2020 2023 6966 206e             #if n
+00019e60: 6569 6768 626f 7273 2061 7265 2074 6f20  eighbors are to 
+00019e70: 6265 2066 6f75 6e64 2077 6974 6869 6e20  be found within 
+00019e80: 7468 6520 7370 6563 6965 732c 0a20 2020  the species,.   
+00019e90: 2020 2020 2020 2020 2023 7365 7420 636f           #set co
+00019ea0: 6f72 6473 2074 6f20 7365 6c66 2e5f 636f  ords to self._co
+00019eb0: 6f72 6473 2028 6f74 6865 7277 6973 652c  ords (otherwise,
+00019ec0: 2074 6865 2063 6f6f 7264 7320 746f 0a20   the coords to. 
+00019ed0: 2020 2020 2020 2020 2020 2023 6669 6e64             #find
+00019ee0: 206e 6561 7265 7374 206e 6569 6768 626f   nearest neighbo
+00019ef0: 7273 2077 6974 6820 7368 6f75 6c64 2068  rs with should h
+00019f00: 6176 6520 6265 656e 2070 726f 7669 6465  ave been provide
+00019f10: 6429 0a20 2020 2020 2020 2020 2020 2069  d).            i
+00019f20: 6620 7769 7468 696e 3a0a 2020 2020 2020  f within:.      
+00019f30: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
+00019f40: 203d 2073 656c 662e 5f63 6f6f 7264 730a   = self._coords.
+00019f50: 0a20 2020 2020 2020 2020 2020 2023 7175  .            #qu
+00019f60: 6572 7920 7468 6520 7472 6565 2074 6f20  ery the tree to 
+00019f70: 6765 7420 6d61 7469 6e67 2070 6169 7273  get mating pairs
+00019f80: 0a20 2020 2020 2020 2020 2020 2070 6169  .            pai
+00019f90: 7273 203d 2073 656c 662e 5f6b 645f 7472  rs = self._kd_tr
+00019fa0: 6565 2e5f 6765 745f 6d61 7469 6e67 5f70  ee._get_mating_p
+00019fb0: 6169 7273 2863 6f6f 7264 733d 636f 6f72  airs(coords=coor
+00019fc0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
 00019fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a000: 6368 6f6f 7365 5f6e 6561 7265 7374 3d63  choose_nearest=c
-0001a010: 686f 6f73 655f 6e65 6172 6573 742c 0a20  hoose_nearest,. 
+00019ff0: 2020 2020 6469 7374 3d73 656c 662e 6d61      dist=self.ma
+0001a000: 7469 6e67 5f72 6164 6975 732c 0a20 2020  ting_radius,.   
+0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a040: 2020 2020 2020 2069 6e76 6572 7365 5f64         inverse_d
-0001a050: 6973 745f 6d61 7469 6e67 3d69 6e76 6572  ist_mating=inver
-0001a060: 7365 5f64 6973 745f 6d61 7469 6e67 290a  se_dist_mating).
-0001a070: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
-0001a080: 7365 2074 6865 2073 7065 6369 6573 2720  se the species' 
-0001a090: 6269 7274 6820 7261 7465 2074 6f20 6465  birth rate to de
-0001a0a0: 6369 6465 2028 6173 2062 6572 6e6f 756c  cide (as bernoul
-0001a0b0: 6c69 2064 7261 7773 290a 2020 2020 2020  li draws).      
-0001a0c0: 2020 2020 2020 2320 7768 6574 6865 7220        # whether 
-0001a0d0: 6561 6368 2070 6169 7220 6361 6e20 6d61  each pair can ma
-0001a0e0: 7465 0a20 2020 2020 2020 2020 2020 2063  te.            c
-0001a0f0: 616e 5f6d 6174 6520 3d20 6e70 2e62 6f6f  an_mate = np.boo
-0001a100: 6c38 286e 702e 7261 6e64 6f6d 2e62 696e  l8(np.random.bin
-0001a110: 6f6d 6961 6c28 6e3d 312c 2070 3d73 656c  omial(n=1, p=sel
-0001a120: 662e 622c 0a20 2020 2020 2020 2020 2020  f.b,.           
-0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a150: 2020 2020 2020 2020 7369 7a65 3d70 6169          size=pai
-0001a160: 7273 2e73 6861 7065 5b30 5d29 290a 2020  rs.shape[0])).  
-0001a170: 2020 2020 2020 2020 2020 7061 6972 7320            pairs 
-0001a180: 3d20 7061 6972 735b 6361 6e5f 6d61 7465  = pairs[can_mate
-0001a190: 2c20 3a5d 0a20 2020 2020 2020 2072 6574  , :].        ret
-0001a1a0: 7572 6e20 7061 6972 730a 0a0a 2020 2020  urn pairs...    
-0001a1b0: 6465 6620 5f6d 616b 655f 6765 615f 6466  def _make_gea_df
-0001a1c0: 2873 656c 662c 206c 7972 5f6e 756d 3d31  (self, lyr_num=1
-0001a1d0: 293a 0a20 2020 2020 2020 2022 2222 0a0a  ):.        """..
-0001a1e0: 2020 2020 2020 2020 4d61 6b65 7320 6120          Makes a 
-0001a1f0: 6461 7461 6672 616d 6520 666f 7220 4745  dataframe for GE
-0001a200: 4120 616e 616c 7973 6973 2063 6f6e 7461  A analysis conta
-0001a210: 696e 696e 6720 6765 6e6f 7479 7065 732c  ining genotypes,
-0001a220: 2063 6f6f 7264 696e 6174 6573 2c0a 2020   coordinates,.  
-0001a230: 2020 2020 2020 616e 6420 656e 7620 7661        and env va
-0001a240: 6c75 6573 2066 6f72 2061 6c6c 2069 6e64  lues for all ind
-0001a250: 6976 6964 7561 6c73 2e0a 0a20 2020 2020  ividuals...     
-0001a260: 2020 204e 4f54 453a 2043 7572 7265 6e74     NOTE: Current
-0001a270: 6c79 206f 6e6c 7920 6163 6365 7074 7320  ly only accepts 
-0001a280: 6f6e 6520 4c61 6e64 7363 6170 6520 4c61  one Landscape La
-0001a290: 7965 7220 2869 2e65 2e20 656e 7669 726f  yer (i.e. enviro
-0001a2a0: 6e6d 656e 7461 6c0a 2020 2020 2020 2020  nmental.        
-0001a2b0: 2020 2020 2020 7661 7269 6162 6c65 290a        variable).
-0001a2c0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0001a2d0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0001a2e0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206c  ------.        l
-0001a2f0: 7972 5f6e 756d 203a 2069 6e74 0a20 2020  yr_num : int.   
-0001a300: 2020 2020 2020 2020 2054 6865 206e 756d           The num
-0001a310: 6265 7220 6f66 2074 6865 204c 616e 6473  ber of the Lands
-0001a320: 6361 7065 204c 6179 6572 2066 726f 6d20  cape Layer from 
-0001a330: 7768 6963 6820 746f 2065 7874 7261 6374  which to extract
-0001a340: 0a20 2020 2020 2020 2020 2020 2065 6e76  .            env
-0001a350: 6972 6f6e 6d65 6e74 616c 2076 616c 7565  ironmental value
-0001a360: 732e 2044 6566 6175 6c74 7320 746f 2031  s. Defaults to 1
-0001a370: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0001a380: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-0001a390: 2d2d 0a20 2020 2020 2020 206f 7574 203a  --.        out :
-0001a3a0: 2070 616e 6461 732e 4461 7461 4672 616d   pandas.DataFram
-0001a3b0: 650a 2020 2020 2020 2020 2020 2020 4120  e.            A 
-0001a3c0: 4461 7461 4672 616d 6520 696e 2077 6869  DataFrame in whi
-0001a3d0: 6368 2063 6f6c 756d 6e73 2061 7265 206c  ch columns are l
-0001a3e0: 6f63 6920 616e 6420 726f 7773 2061 7265  oci and rows are
-0001a3f0: 2069 6e64 6976 6964 7561 6c73 0a20 2020   individuals.   
-0001a400: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001a410: 2023 6765 7420 6172 7261 7920 6f66 205b   #get array of [
-0001a420: 307c 302e 357c 315d 2067 656e 6f74 7970  0|0.5|1] genotyp
-0001a430: 6573 0a20 2020 2020 2020 2022 2222 0a20  es.        """. 
-0001a440: 2020 2020 2020 2067 656e 203d 2073 656c         gen = sel
-0001a450: 662e 5f67 6574 5f67 656e 6f74 7970 6573  f._get_genotypes
-0001a460: 2829 0a0a 2020 2020 2020 2020 236c 6f6f  ()..        #loo
-0001a470: 7020 746f 2063 6f6e 7665 7274 2062 696e  p to convert bin
-0001a480: 6172 7920 616c 6c65 6c65 2067 656e 6f74  ary allele genot
-0001a490: 7970 6573 2028 307c 3129 0a20 2020 2020  ypes (0|1).     
-0001a4a0: 2020 2023 696e 746f 2073 696e 676c 6520     #into single 
-0001a4b0: 6469 6769 7420 6765 6e6f 7479 7065 7320  digit genotypes 
-0001a4c0: 2830 2c20 302e 352c 2031 290a 2020 2020  (0, 0.5, 1).    
-0001a4d0: 2020 2020 6765 6e6f 5f69 6e64 203d 205b      geno_ind = [
-0001a4e0: 5d0a 2020 2020 2020 2020 666f 7220 696e  ].        for in
-0001a4f0: 6420 696e 2072 616e 6765 286c 656e 2867  d in range(len(g
-0001a500: 656e 2929 3a0a 2020 2020 2020 2020 2020  en)):.          
-0001a510: 2020 6765 6e6f 5f6c 6f63 203d 205b 5d0a    geno_loc = [].
-0001a520: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001a530: 6c6f 6369 2069 6e20 7261 6e67 6528 6c65  loci in range(le
-0001a540: 6e28 6765 6e5b 696e 645d 2929 3a0a 2020  n(gen[ind])):.  
-0001a550: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-0001a560: 6e6f 7479 7065 203d 2067 656e 5b69 6e64  notype = gen[ind
-0001a570: 5d5b 6c6f 6369 5d2e 6d65 616e 2829 2023  ][loci].mean() #
-0001a580: 2063 6f64 6564 2061 7320 302f 302e 352f   coded as 0/0.5/
-0001a590: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-0001a5a0: 2020 6765 6e6f 5f6c 6f63 2e61 7070 656e    geno_loc.appen
-0001a5b0: 6428 6765 6e6f 7479 7065 290a 2020 2020  d(genotype).    
-0001a5c0: 2020 2020 2020 2020 6765 6e6f 5f69 6e64          geno_ind
-0001a5d0: 2e61 7070 656e 6428 6765 6e6f 5f6c 6f63  .append(geno_loc
-0001a5e0: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-0001a5f0: 2020 2020 2020 6774 7320 3d20 7365 6c66        gts = self
-0001a600: 2e5f 6765 745f 6765 6e6f 7479 7065 7328  ._get_genotypes(
-0001a610: 6269 616c 6c65 6c69 633d 4661 6c73 6529  biallelic=False)
-0001a620: 0a0a 2020 2020 2020 2020 2363 6f6e 7665  ..        #conve
-0001a630: 7274 2074 6f20 6461 7461 6672 616d 650a  rt to dataframe.
-0001a640: 2020 2020 2020 2020 6765 615f 6466 203d          gea_df =
-0001a650: 2070 642e 4461 7461 4672 616d 6528 6774   pd.DataFrame(gt
-0001a660: 7329 0a0a 2020 2020 2020 2020 2367 6574  s)..        #get
-0001a670: 2065 6e76 6972 6f6e 6d65 6e74 616c 2064   environmental d
-0001a680: 6174 610a 2020 2020 2020 2020 656e 7620  ata.        env 
-0001a690: 3d20 7365 6c66 2e5f 6765 745f 6528 290a  = self._get_e().
-0001a6a0: 2020 2020 2020 2020 6765 615f 6466 5b27          gea_df['
-0001a6b0: 656e 7627 5d20 3d20 6c69 7374 2865 6e76  env'] = list(env
-0001a6c0: 5b3a 2c6c 7972 5f6e 756d 5d29 0a0a 2020  [:,lyr_num])..  
-0001a6d0: 2020 2020 2020 2367 6574 2063 6f6f 7264        #get coord
-0001a6e0: 730a 2020 2020 2020 2020 636f 6f72 6420  s.        coord 
-0001a6f0: 3d20 7365 6c66 2e5f 6765 745f 636f 6f72  = self._get_coor
-0001a700: 6473 2829 0a20 2020 2020 2020 2067 6561  ds().        gea
-0001a710: 5f64 665b 276c 6174 275d 203d 206c 6973  _df['lat'] = lis
-0001a720: 7428 636f 6f72 645b 3a2c 305d 290a 2020  t(coord[:,0]).  
-0001a730: 2020 2020 2020 6765 615f 6466 5b27 6c6f        gea_df['lo
-0001a740: 6e67 275d 203d 206c 6973 7428 636f 6f72  ng'] = list(coor
-0001a750: 645b 3a2c 315d 290a 0a20 2020 2020 2020  d[:,1])..       
-0001a760: 2072 6574 7572 6e20 6765 615f 6466 0a0a   return gea_df..
-0001a770: 0a20 2020 2064 6566 205f 7275 6e5f 6363  .    def _run_cc
-0001a780: 6128 7365 6c66 2c20 7472 745f 6e75 6d3d  a(self, trt_num=
-0001a790: 302c 2073 6361 6c65 3d54 7275 652c 2070  0, scale=True, p
-0001a7a0: 6c6f 743d 5472 7565 2c20 706c 6f74 5f73  lot=True, plot_s
-0001a7b0: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
-0001a7c0: 2020 2020 2020 2020 2073 643d 3329 3a0a           sd=3):.
-0001a7d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001a7e0: 2020 2020 5275 6e73 2061 2063 616e 6f6e      Runs a canon
-0001a7f0: 6963 616c 2063 6f72 7265 6c61 7469 6f6e  ical correlation
-0001a800: 2061 6e61 6c79 7369 7320 2843 4341 2920   analysis (CCA) 
-0001a810: 6f6e 2074 6865 2063 7572 7265 6e74 2067  on the current g
-0001a820: 656e 6574 6963 2061 6e64 0a20 2020 2020  enetic and.     
-0001a830: 2020 2065 6e76 6972 6f6e 6d65 6e74 616c     environmental
-0001a840: 2064 6174 6120 666f 7220 7468 6520 5370   data for the Sp
-0001a850: 6563 6965 7327 2063 7572 7265 6e74 2070  ecies' current p
-0001a860: 6f70 756c 6174 696f 6e2c 2075 7369 6e67  opulation, using
-0001a870: 2074 6865 0a20 2020 2020 2020 2069 6e64   the.        ind
-0001a880: 6963 6174 6564 2054 7261 6974 2e20 506c  icated Trait. Pl
-0001a890: 6f74 7320 7468 6520 7265 7375 6c74 7320  ots the results 
-0001a8a0: 616e 6420 7265 7475 726e 7320 7468 656d  and returns them
-0001a8b0: 2069 6e20 6120 6469 6374 2e0a 0a20 2020   in a dict...   
-0001a8c0: 2020 2020 2043 4341 206d 6f64 656c 2066       CCA model f
-0001a8d0: 6f72 6d75 6c61 3a20 6765 6e6f 7479 7065  ormula: genotype
-0001a8e0: 207e 2065 6e76 202b 206c 6174 202b 206c   ~ env + lat + l
-0001a8f0: 6f6e 670a 0a20 2020 2020 2020 204e 4f54  ong..        NOT
-0001a900: 453a 2063 7572 7265 6e74 6c79 206f 6e6c  E: currently onl
-0001a910: 7920 706f 7373 6962 6c65 2074 6f20 646f  y possible to do
-0001a920: 2033 2063 6f6d 706f 6e65 6e74 732f 3320   3 components/3 
-0001a930: 7661 7269 6162 6c65 733b 0a20 2020 2020  variables;.     
-0001a940: 2020 2020 2020 2020 2077 696c 6c20 6164           will ad
-0001a950: 6420 6772 6561 7465 7220 6675 6e63 7469  d greater functi
-0001a960: 6f6e 616c 6974 7920 696e 2074 6865 2066  onality in the f
-0001a970: 7574 7572 650a 0a20 2020 2020 2020 2050  uture..        P
-0001a980: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0001a990: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001a9a0: 2020 2020 2074 7274 5f6e 756d 203a 2069       trt_num : i
-0001a9b0: 6e74 0a20 2020 2020 2020 2020 2020 2054  nt.            T
-0001a9c0: 6865 206e 756d 6265 7220 6f66 2074 6865  he number of the
-0001a9d0: 2054 7261 6974 2074 6f20 7275 6e20 7468   Trait to run th
-0001a9e0: 6520 4745 4120 6f6e 2e20 4465 6661 756c  e GEA on. Defaul
-0001a9f0: 7473 2074 6f20 302e 0a20 2020 2020 2020  ts to 0..       
-0001aa00: 2073 6361 6c65 203a 2062 6f6f 6c0a 2020   scale : bool.  
-0001aa10: 2020 2020 2020 2020 2020 4966 2054 7275            If Tru
-0001aa20: 652c 2073 6361 6c65 7320 7468 6520 7661  e, scales the va
-0001aa30: 7269 6162 6c65 2c20 696e 6469 7669 6475  riable, individu
-0001aa40: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-0001aa50: 616e 6420 6c6f 6375 7320 6c6f 6164 696e  and locus loadin
-0001aa60: 6773 2066 726f 6d20 2d31 2074 6f20 3120  gs from -1 to 1 
-0001aa70: 746f 206d 616b 6520 7468 656d 2065 6173  to make them eas
-0001aa80: 6965 720a 2020 2020 2020 2020 2020 2020  ier.            
-0001aa90: 746f 2076 6973 7561 6c69 7a65 2e20 4465  to visualize. De
-0001aaa0: 6661 756c 7473 2074 6f20 5472 7565 2e0a  faults to True..
-0001aab0: 2020 2020 2020 2020 706c 6f74 203a 2062          plot : b
-0001aac0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-0001aad0: 5768 6574 6865 7220 6f72 206e 6f74 2074  Whether or not t
-0001aae0: 6f20 706c 6f74 2074 6865 206d 6f64 656c  o plot the model
-0001aaf0: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
-0001ab00: 7565 2e0a 2020 2020 2020 2020 706c 6f74  ue..        plot
-0001ab10: 5f73 6420 3a20 626f 6f6c 0a20 2020 2020  _sd : bool.     
-0001ab20: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-0001ab30: 6120 7374 616e 6461 7264 2064 6576 6961  a standard devia
-0001ab40: 7469 6f6e 2065 6c6c 6970 7365 2069 7320  tion ellipse is 
-0001ab50: 706c 6f74 7465 642c 2075 7369 6e67 2074  plotted, using t
-0001ab60: 6865 206e 756d 6265 720a 2020 2020 2020  he number.      
-0001ab70: 2020 2020 2020 6f66 2073 7461 6e64 6172        of standar
-0001ab80: 6420 6465 7669 6174 696f 6e73 2069 6e64  d deviations ind
-0001ab90: 6963 6174 6564 2062 7920 7468 6520 6172  icated by the ar
-0001aba0: 6775 6d65 6e74 2027 7364 272e 2044 6566  gument 'sd'. Def
-0001abb0: 6175 6c74 7320 746f 0a20 2020 2020 2020  aults to.       
-0001abc0: 2020 2020 2054 7275 652e 0a20 2020 2020       True..     
-0001abd0: 2020 2073 6420 3a20 7b69 6e74 2c20 666c     sd : {int, fl
-0001abe0: 6f61 747d 0a20 2020 2020 2020 2020 2020  oat}.           
-0001abf0: 204e 756d 6265 7220 6f66 2073 7461 6e64   Number of stand
-0001ac00: 6172 6420 6465 7669 6174 696f 6e73 2074  ard deviations t
-0001ac10: 6f20 7573 6520 666f 7220 706c 6f74 7469  o use for plotti
-0001ac20: 6e67 2074 6865 2073 7461 6e64 6172 640a  ng the standard.
-0001ac30: 2020 2020 2020 2020 2020 2020 6465 7669              devi
-0001ac40: 6174 696f 6e20 656c 6c69 7073 652e 2044  ation ellipse. D
-0001ac50: 6566 6175 6c74 7320 746f 2033 2e0a 0a20  efaults to 3... 
-0001ac60: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0001ac70: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0001ac80: 2020 2020 2020 206f 7574 203a 2064 6963         out : dic
-0001ac90: 740a 2020 2020 2020 2020 2020 2020 4120  t.            A 
-0001aca0: 6469 6374 206f 6620 7468 6520 666f 6c6c  dict of the foll
-0001acb0: 6f77 696e 6720 6b65 792d 7661 6c75 6520  owing key-value 
-0001acc0: 7061 6972 733a 0a20 2020 2020 2020 2020  pairs:.         
-0001acd0: 2020 2020 2020 2022 6765 615f 6466 223a         "gea_df":
-0001ace0: 2061 2044 6174 6146 7261 6d65 206f 6620   a DataFrame of 
-0001acf0: 696e 6469 7669 6475 616c 7327 2067 656e  individuals' gen
-0001ad00: 6f74 7970 6573 2c20 656e 7669 726f 6e6d  otypes, environm
-0001ad10: 656e 7461 6c0a 2020 2020 2020 2020 2020  ental.          
-0001ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad30: 7661 6c75 6573 2c20 616e 6420 636f 6f72  values, and coor
-0001ad40: 6469 6e61 7465 730a 2020 2020 2020 2020  dinates.        
-0001ad50: 2020 2020 2020 2020 2269 6e64 5f43 4341          "ind_CCA
-0001ad60: 6466 223a 2069 6e64 6976 6964 7561 6c20  df": individual 
-0001ad70: 6c6f 6164 696e 6773 2028 636f 6c75 6d6e  loadings (column
-0001ad80: 7320 3d20 6178 6573 2c0a 2020 2020 2020  s = axes,.      
-0001ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ada0: 2020 2020 2020 2072 6f77 7320 3d20 696e         rows = in
-0001adb0: 6469 7669 6475 616c 7329 0a20 2020 2020  dividuals).     
-0001adc0: 2020 2020 2020 2020 2020 2022 6c6f 6369             "loci
-0001add0: 5f43 4341 6466 223a 206c 6f63 7573 206c  _CCAdf": locus l
-0001ade0: 6f61 6469 6e67 7320 2863 6f6c 756d 6e73  oadings (columns
-0001adf0: 203d 2061 7865 732c 2072 6f77 7320 3d20   = axes, rows = 
-0001ae00: 6c6f 6369 290a 2020 2020 2020 2020 2020  loci).          
-0001ae10: 2020 2020 2020 2276 6172 5f43 4341 6466        "var_CCAdf
-0001ae20: 223a 2076 6172 6961 626c 6520 6c6f 6164  ": variable load
-0001ae30: 696e 6773 2028 636f 6c75 6d6e 7320 3d20  ings (columns = 
-0001ae40: 6178 6573 2c0a 2020 2020 2020 2020 2020  axes,.          
-0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae60: 2020 2072 6f77 7320 3d20 7661 7269 6162     rows = variab
-0001ae70: 6c65 2028 656e 762c 206c 6174 2c20 6c6f  le (env, lat, lo
-0001ae80: 6e67 2929 0a20 2020 2020 2020 2020 2020  ng)).           
-0001ae90: 2020 2020 2022 7472 6169 745f 6c6f 6369       "trait_loci
-0001aea0: 223a 206c 6973 7420 6f66 2069 6e64 6578  ": list of index
-0001aeb0: 6573 2066 6f72 206c 6f63 6920 7468 6174  es for loci that
-0001aec0: 2075 6e64 6572 6c69 6520 7468 6520 7472   underlie the tr
-0001aed0: 6169 740a 2020 2020 2020 2020 2020 2020  ait.            
-0001aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aef0: 2020 666f 7220 7768 6963 6820 7468 6520    for which the 
-0001af00: 4343 4120 7761 7320 7275 6e0a 2020 2020  CCA was run.    
-0001af10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001af20: 236d 616b 6520 4446 0a20 2020 2020 2020  #make DF.       
-0001af30: 2067 6561 5f64 6620 3d73 656c 662e 5f6d   gea_df =self._m
-0001af40: 616b 655f 6765 615f 6466 286c 7972 5f6e  ake_gea_df(lyr_n
-0001af50: 756d 3d73 656c 662e 6765 6e5f 6172 6368  um=self.gen_arch
-0001af60: 2e74 7261 6974 735b 7472 745f 6e75 6d5d  .traits[trt_num]
-0001af70: 2e6c 7972 5f6e 756d 290a 0a20 2020 2020  .lyr_num)..     
-0001af80: 2020 2023 6765 7420 6164 6170 7469 7665     #get adaptive
-0001af90: 206c 6f63 6920 2875 7365 6420 6c61 7465   loci (used late
-0001afa0: 7220 696e 2070 6c6f 7474 696e 6729 0a20  r in plotting). 
-0001afb0: 2020 2020 2020 2074 7261 6974 5f6c 6f63         trait_loc
-0001afc0: 6920 3d20 7365 6c66 2e67 656e 5f61 7263  i = self.gen_arc
-0001afd0: 682e 7472 6169 7473 5b74 7274 5f6e 756d  h.traits[trt_num
-0001afe0: 5d2e 6c6f 6369 2023 6765 7473 2074 7261  ].loci #gets tra
-0001aff0: 6974 206c 6f63 6920 696e 6465 7865 730a  it loci indexes.
-0001b000: 0a20 2020 2020 2020 2023 6765 7420 6e75  .        #get nu
-0001b010: 6d62 6572 206f 6620 6c6f 6369 0a20 2020  mber of loci.   
-0001b020: 2020 2020 204c 203d 2073 656c 662e 6765       L = self.ge
-0001b030: 6e5f 6172 6368 2e4c 0a20 2020 2020 2020  n_arch.L.       
-0001b040: 2023 6465 6669 6e65 2078 2061 6e64 2079   #define x and y
-0001b050: 3a0a 2020 2020 2020 2020 2320 7075 6c6c  :.        # pull
-0001b060: 206f 7574 2067 656e 6f74 7970 6573 0a20   out genotypes. 
-0001b070: 2020 2020 2020 2059 203d 2067 6561 5f64         Y = gea_d
-0001b080: 662e 696c 6f63 5b3a 2c72 616e 6765 284c  f.iloc[:,range(L
-0001b090: 295d 0a20 2020 2020 2020 2023 2070 756c  )].        # pul
-0001b0a0: 6c20 6f75 7420 7072 6564 6963 746f 7220  l out predictor 
-0001b0b0: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
-0001b0c0: 2020 2320 544f 444f 3a20 6d61 6b65 2069    # TODO: make i
-0001b0d0: 7420 706f 7373 6962 6c65 2074 6f20 6368  t possible to ch
-0001b0e0: 6f6f 7365 206d 6f72 6520 7661 7273 2069  oose more vars i
-0001b0f0: 6e20 6675 7475 7265 0a20 2020 2020 2020  n future.       
-0001b100: 2058 203d 2067 6561 5f64 665b 5b27 656e   X = gea_df[['en
-0001b110: 7627 2c27 6c61 7427 2c27 6c6f 6e67 275d  v','lat','long']
-0001b120: 5d0a 0a20 2020 2020 2020 2023 6465 6669  ]..        #defi
-0001b130: 6e65 206e 5f63 6f6d 706f 6e65 6e74 730a  ne n_components.
-0001b140: 2020 2020 2020 2020 6e5f 636f 6d70 6f6e          n_compon
-0001b150: 656e 7473 203d 2033 0a20 2020 2020 2020  ents = 3.       
-0001b160: 2023 6372 6561 7465 2074 6865 2043 4341   #create the CCA
-0001b170: 206d 6f64 656c 2061 6e64 2066 6974 2069   model and fit i
-0001b180: 7420 746f 2074 6865 2064 6174 610a 2020  t to the data.  
-0001b190: 2020 2020 2020 6363 6120 3d20 4343 4128        cca = CCA(
-0001b1a0: 6e5f 636f 6d70 6f6e 656e 7473 203d 206e  n_components = n
-0001b1b0: 5f63 6f6d 706f 6e65 6e74 7329 0a20 2020  _components).   
-0001b1c0: 2020 2020 2063 6361 2e66 6974 2859 2c20       cca.fit(Y, 
-0001b1d0: 5829 0a0a 2020 2020 2020 2020 2374 7261  X)..        #tra
-0001b1e0: 6e73 666f 726d 2064 6174 610a 2020 2020  nsform data.    
-0001b1f0: 2020 2020 595f 6320 3d20 6363 612e 7472      Y_c = cca.tr
-0001b200: 616e 7366 6f72 6d28 5929 0a0a 2020 2020  ansform(Y)..    
-0001b210: 2020 2020 2363 7265 6174 6520 6466 2066      #create df f
-0001b220: 6f72 2069 6e64 6976 6964 7561 6c73 0a20  or individuals. 
-0001b230: 2020 2020 2020 2069 6e64 5f64 6620 3d20         ind_df = 
-0001b240: 7064 2e44 6174 6146 7261 6d65 2859 5f63  pd.DataFrame(Y_c
-0001b250: 290a 2020 2020 2020 2020 236e 616d 696e  ).        #namin
-0001b260: 6720 4343 4120 636f 6c75 6d6e 7320 7374  g CCA columns st
-0001b270: 6172 7469 6e67 2061 7420 310a 2020 2020  arting at 1.    
-0001b280: 2020 2020 696e 645f 6466 2e63 6f6c 756d      ind_df.colum
-0001b290: 6e73 203d 205b 7374 7228 7229 2066 6f72  ns = [str(r) for
-0001b2a0: 2072 2069 6e20 7261 6e67 6528 312c 206e   r in range(1, n
-0001b2b0: 5f63 6f6d 706f 6e65 6e74 7320 2b20 3129  _components + 1)
-0001b2c0: 5d0a 0a20 2020 2020 2020 2023 6372 6561  ]..        #crea
-0001b2d0: 7465 2064 6620 666f 7220 6c6f 6369 0a20  te df for loci. 
-0001b2e0: 2020 2020 2020 206c 6f63 695f 6466 203d         loci_df =
-0001b2f0: 2070 642e 4461 7461 4672 616d 6528 6363   pd.DataFrame(cc
-0001b300: 612e 785f 6c6f 6164 696e 6773 5f29 0a20  a.x_loadings_). 
-0001b310: 2020 2020 2020 206c 6f63 695f 6466 2e63         loci_df.c
-0001b320: 6f6c 756d 6e73 203d 2069 6e64 5f64 662e  olumns = ind_df.
-0001b330: 636f 6c75 6d6e 7320 2373 616d 6520 636f  columns #same co
-0001b340: 6c75 6d6e 206e 616d 6573 0a0a 2020 2020  lumn names..    
-0001b350: 2020 2020 2363 7265 6174 6520 6466 2066      #create df f
-0001b360: 6f72 2076 6172 6961 626c 6573 0a20 2020  or variables.   
-0001b370: 2020 2020 2076 6172 5f64 6620 3d20 7064       var_df = pd
-0001b380: 2e44 6174 6146 7261 6d65 2863 6361 2e79  .DataFrame(cca.y
-0001b390: 5f6c 6f61 6469 6e67 735f 290a 2020 2020  _loadings_).    
-0001b3a0: 2020 2020 7661 725f 6466 2e63 6f6c 756d      var_df.colum
-0001b3b0: 6e73 203d 2069 6e64 5f64 662e 636f 6c75  ns = ind_df.colu
-0001b3c0: 6d6e 7320 2373 616d 6520 636f 6c75 6d6e  mns #same column
-0001b3d0: 206e 616d 6573 0a0a 2020 2020 2020 2020   names..        
-0001b3e0: 236d 616b 6520 6469 6374 696f 6e61 7279  #make dictionary
-0001b3f0: 206f 6620 6461 7461 6672 616d 6573 2074   of dataframes t
-0001b400: 6f20 7265 7475 726e 0a20 2020 2020 2020  o return.       
-0001b410: 2063 6361 5f64 6963 7420 3d20 7b27 6765   cca_dict = {'ge
-0001b420: 615f 6466 273a 6765 615f 6466 2c0a 2020  a_df':gea_df,.  
-0001b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b440: 2020 2769 6e64 5f64 6627 3a69 6e64 5f64    'ind_df':ind_d
-0001b450: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-0001b460: 2020 2020 2020 2027 6c6f 6369 5f64 6627         'loci_df'
-0001b470: 3a6c 6f63 695f 6466 2c0a 2020 2020 2020  :loci_df,.      
-0001b480: 2020 2020 2020 2020 2020 2020 2020 2776                'v
-0001b490: 6172 5f64 6627 3a76 6172 5f64 662c 0a20  ar_df':var_df,. 
-0001b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4b0: 2020 2027 7472 6169 745f 6c6f 6369 273a     'trait_loci':
-0001b4c0: 7472 6169 745f 6c6f 6369 7d0a 0a20 2020  trait_loci}..   
-0001b4d0: 2020 2020 2023 204e 4f54 453a 2072 6967       # NOTE: rig
-0001b4e0: 6874 206e 6f77 2074 6869 7320 706c 6f74  ht now this plot
-0001b4f0: 7469 6e67 206c 6f6f 7020 6f6e 6c79 2077  ting loop only w
-0001b500: 6f72 6b73 2066 6f72 2061 206d 6178 696d  orks for a maxim
-0001b510: 756d 206f 6620 3320 6178 6573 3b0a 2020  um of 3 axes;.  
-0001b520: 2020 2020 2020 2320 2020 2020 2020 696e        #       in
-0001b530: 2074 6865 2066 7574 7572 6520 6173 206d   the future as m
-0001b540: 6f72 6520 656e 7620 7661 7273 2061 7265  ore env vars are
-0001b550: 2061 6464 6564 2c20 636f 756c 6420 6164   added, could ad
-0001b560: 6420 6d6f 7265 2061 7865 730a 2020 2020  d more axes.    
-0001b570: 2020 2020 6966 2070 6c6f 743a 0a20 2020      if plot:.   
-0001b580: 2020 2020 2020 2020 2023 5363 616c 6520           #Scale 
-0001b590: 6461 7461 6672 616d 6573 2066 726f 6d20  dataframes from 
-0001b5a0: 2d31 2074 6f20 3120 6966 2073 6361 6c65  -1 to 1 if scale
-0001b5b0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-0001b5c0: 2020 2020 6966 2073 6361 6c65 203d 3d20      if scale == 
-0001b5d0: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
-0001b5e0: 2020 2020 2020 726d 696e 203d 202d 310a        rmin = -1.
-0001b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b600: 726d 6178 203d 2031 0a20 2020 2020 2020  rmax = 1.       
-0001b610: 2020 2020 2020 2020 206c 6f63 695f 6466           loci_df
-0001b620: 203d 2072 6d69 6e20 2b20 286c 6f63 695f   = rmin + (loci_
-0001b630: 6466 202d 206c 6f63 695f 6466 2e76 616c  df - loci_df.val
-0001b640: 7565 732e 6d69 6e28 2929 202a 2028 726d  ues.min()) * (rm
-0001b650: 6178 202d 0a20 2020 2020 2020 2020 2020  ax -.           
-0001b660: 2020 2020 2020 2020 2020 2020 2028 726d               (rm
-0001b670: 696e 2929 202f 2028 6c6f 6369 5f64 662e  in)) / (loci_df.
-0001b680: 7661 6c75 6573 2e6d 6178 2829 202d 206c  values.max() - l
-0001b690: 6f63 695f 6466 2e76 616c 7565 732e 6d69  oci_df.values.mi
-0001b6a0: 6e28 2929 0a20 2020 2020 2020 2020 2020  n()).           
-0001b6b0: 2020 2020 2076 6172 5f64 6620 3d20 726d       var_df = rm
-0001b6c0: 696e 202b 2028 7661 725f 6466 202d 2076  in + (var_df - v
-0001b6d0: 6172 5f64 662e 7661 6c75 6573 2e6d 696e  ar_df.values.min
-0001b6e0: 2829 2920 2a20 2872 6d61 7820 2d0a 2020  ()) * (rmax -.  
-0001b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b700: 2020 2020 2020 2872 6d69 6e29 2920 2f20        (rmin)) / 
-0001b710: 2876 6172 5f64 662e 7661 6c75 6573 2e6d  (var_df.values.m
-0001b720: 6178 2829 202d 2076 6172 5f64 662e 7661  ax() - var_df.va
-0001b730: 6c75 6573 2e6d 696e 2829 290a 2020 2020  lues.min()).    
-0001b740: 2020 2020 2020 2020 2020 2020 696e 645f              ind_
-0001b750: 6466 203d 2072 6d69 6e20 2b20 2869 6e64  df = rmin + (ind
-0001b760: 5f64 6620 2d20 696e 645f 6466 2e76 616c  _df - ind_df.val
-0001b770: 7565 732e 6d69 6e28 2929 202a 2028 726d  ues.min()) * (rm
-0001b780: 6178 202d 0a20 2020 2020 2020 2020 2020  ax -.           
-0001b790: 2020 2020 2020 2020 2020 2020 2028 726d               (rm
-0001b7a0: 696e 2929 202f 2028 696e 645f 6466 2e76  in)) / (ind_df.v
-0001b7b0: 616c 7565 732e 6d61 7828 2920 2d20 696e  alues.max() - in
-0001b7c0: 645f 6466 2e76 616c 7565 732e 6d69 6e28  d_df.values.min(
-0001b7d0: 2929 0a0a 0a20 2020 2020 2020 2020 2020  ))...           
-0001b7e0: 2023 6765 7420 6d61 7820 616e 6420 6d69   #get max and mi
-0001b7f0: 6e73 2074 6f20 7365 7420 6178 6973 206c  ns to set axis l
-0001b800: 6174 6572 206f 6e0a 2020 2020 2020 2020  ater on.        
-0001b810: 2020 2020 6d61 7864 6620 3d20 6d61 7828      maxdf = max(
-0001b820: 696e 645f 6466 2e76 616c 7565 732e 6d61  ind_df.values.ma
-0001b830: 7828 292c 2076 6172 5f64 662e 7661 6c75  x(), var_df.valu
-0001b840: 6573 2e6d 6178 2829 2c0a 2020 2020 2020  es.max(),.      
-0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b860: 2020 6c6f 6369 5f64 662e 7661 6c75 6573    loci_df.values
-0001b870: 2e6d 6178 2829 290a 2020 2020 2020 2020  .max()).        
-0001b880: 2020 2020 6d69 6e64 6620 3d20 6162 7328      mindf = abs(
-0001b890: 6d69 6e28 696e 645f 6466 2e76 616c 7565  min(ind_df.value
-0001b8a0: 732e 6d69 6e28 292c 2076 6172 5f64 662e  s.min(), var_df.
-0001b8b0: 7661 6c75 6573 2e6d 696e 2829 2c0a 2020  values.min(),.  
-0001b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8d0: 2020 2020 2020 2020 2020 6c6f 6369 5f64            loci_d
-0001b8e0: 662e 7661 6c75 6573 2e6d 696e 2829 2929  f.values.min()))
-0001b8f0: 0a20 2020 2020 2020 2020 2020 2061 786d  .            axm
-0001b900: 6178 203d 206d 6178 286d 6178 6466 2c20  ax = max(maxdf, 
-0001b910: 6d69 6e64 6629 202a 2031 2e32 3020 2361  mindf) * 1.20 #a
-0001b920: 6464 696e 6720 6120 3230 2520 6275 6666  dding a 20% buff
-0001b930: 6572 0a0a 2020 2020 2020 2020 2020 2020  er..            
-0001b940: 2373 6574 2075 7020 6669 6775 7265 0a20  #set up figure. 
-0001b950: 2020 2020 2020 2020 2020 2066 6967 203d             fig =
-0001b960: 2070 6c74 2e66 6967 7572 6528 6669 6773   plt.figure(figs
-0001b970: 697a 653d 2832 302c 2031 3529 290a 2020  ize=(20, 15)).  
-0001b980: 2020 2020 2020 2020 2020 666f 7220 6e2c            for n,
-0001b990: 2063 635f 6178 6573 5f70 6169 7220 696e   cc_axes_pair in
-0001b9a0: 2065 6e75 6d65 7261 7465 285b 5b31 2c20   enumerate([[1, 
-0001b9b0: 325d 2c20 5b31 2c20 335d 2c20 5b32 2c20  2], [1, 3], [2, 
-0001b9c0: 335d 5d29 3a0a 2020 2020 2020 2020 2020  3]]):.          
-0001b9d0: 2020 2020 2020 2364 6566 696e 6520 636f        #define co
-0001b9e0: 6d70 6f6e 656e 7473 2066 6f72 2061 7869  mponents for axi
-0001b9f0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0001ba00: 2020 6363 5f61 7869 7331 203d 2063 635f    cc_axis1 = cc_
-0001ba10: 6178 6573 5f70 6169 725b 305d 2023 782d  axes_pair[0] #x-
-0001ba20: 6178 6973 2043 430a 2020 2020 2020 2020  axis CC.        
-0001ba30: 2020 2020 2020 2020 6363 5f61 7869 7332          cc_axis2
-0001ba40: 203d 2063 635f 6178 6573 5f70 6169 725b   = cc_axes_pair[
-0001ba50: 315d 2023 792d 6178 6973 2043 430a 0a20  1] #y-axis CC.. 
-0001ba60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001ba70: 7820 3d20 6669 672e 6164 645f 7375 6270  x = fig.add_subp
-0001ba80: 6c6f 7428 3133 312b 6e29 0a0a 2020 2020  lot(131+n)..    
-0001ba90: 2020 2020 2020 2020 2020 2020 2361 6464              #add
-0001baa0: 2063 656e 7465 7220 6c69 6e65 730a 2020   center lines.  
-0001bab0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0001bac0: 2e61 7868 6c69 6e65 2879 3d30 2c20 636f  .axhline(y=0, co
-0001bad0: 6c6f 723d 276c 6967 6874 6772 6179 272c  lor='lightgray',
-0001bae0: 206c 696e 6573 7479 6c65 3d27 646f 7474   linestyle='dott
-0001baf0: 6564 2729 0a20 2020 2020 2020 2020 2020  ed').           
-0001bb00: 2020 2020 2061 782e 6178 766c 696e 6528       ax.axvline(
-0001bb10: 783d 302c 2063 6f6c 6f72 3d27 6c69 6768  x=0, color='ligh
-0001bb20: 7467 7261 7927 2c20 6c69 6e65 7374 796c  tgray', linestyl
-0001bb30: 653d 2764 6f74 7465 6427 290a 0a20 2020  e='dotted')..   
-0001bb40: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-0001bb50: 6574 2061 7865 7320 7261 6e67 650a 2020  et axes range.  
-0001bb60: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0001bb70: 742e 786c 696d 282d 6178 6d61 782c 2061  t.xlim(-axmax, a
-0001bb80: 786d 6178 290a 2020 2020 2020 2020 2020  xmax).          
-0001bb90: 2020 2020 2020 706c 742e 796c 696d 282d        plt.ylim(-
-0001bba0: 6178 6d61 782c 2061 786d 6178 290a 0a20  axmax, axmax).. 
-0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001bbc0: 706c 6f74 206e 6575 7472 616c 2053 4e50  plot neutral SNP
-0001bbd0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0001bbe0: 2020 6178 2e73 6361 7474 6572 286c 6f63    ax.scatter(loc
-0001bbf0: 695f 6466 5b73 7472 2863 635f 6178 6973  i_df[str(cc_axis
-0001bc00: 3129 5d2c 206c 6f63 695f 6466 5b73 7472  1)], loci_df[str
-0001bc10: 2863 635f 6178 6973 3229 5d2c 0a20 2020  (cc_axis2)],.   
-0001bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc30: 2020 2020 2020 2020 6d61 726b 6572 203d          marker =
-0001bc40: 2027 2b27 2c20 636f 6c6f 7220 3d20 2767   '+', color = 'g
-0001bc50: 7261 7927 2c0a 2020 2020 2020 2020 2020  ray',.          
+0001a030: 2020 2020 2020 2020 2020 2020 2063 686f               cho
+0001a040: 6f73 655f 6e65 6172 6573 743d 6368 6f6f  ose_nearest=choo
+0001a050: 7365 5f6e 6561 7265 7374 2c0a 2020 2020  se_nearest,.    
+0001a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a080: 2020 2020 696e 7665 7273 655f 6469 7374      inverse_dist
+0001a090: 5f6d 6174 696e 673d 696e 7665 7273 655f  _mating=inverse_
+0001a0a0: 6469 7374 5f6d 6174 696e 6729 0a0a 2020  dist_mating)..  
+0001a0b0: 2020 2020 2020 2020 2020 2320 7573 6520            # use 
+0001a0c0: 7468 6520 7370 6563 6965 7327 2062 6972  the species' bir
+0001a0d0: 7468 2072 6174 6520 746f 2064 6563 6964  th rate to decid
+0001a0e0: 6520 2861 7320 6265 726e 6f75 6c6c 6920  e (as bernoulli 
+0001a0f0: 6472 6177 7329 0a20 2020 2020 2020 2020  draws).         
+0001a100: 2020 2023 2077 6865 7468 6572 2065 6163     # whether eac
+0001a110: 6820 7061 6972 2063 616e 206d 6174 650a  h pair can mate.
+0001a120: 2020 2020 2020 2020 2020 2020 6361 6e5f              can_
+0001a130: 6d61 7465 203d 206e 702e 626f 6f6c 3828  mate = np.bool8(
+0001a140: 6e70 2e72 616e 646f 6d2e 6269 6e6f 6d69  np.random.binomi
+0001a150: 616c 286e 3d31 2c20 703d 7365 6c66 2e62  al(n=1, p=self.b
+0001a160: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a190: 2020 2020 2073 697a 653d 7061 6972 732e       size=pairs.
+0001a1a0: 7368 6170 655b 305d 2929 0a20 2020 2020  shape[0])).     
+0001a1b0: 2020 2020 2020 2070 6169 7273 203d 2070         pairs = p
+0001a1c0: 6169 7273 5b63 616e 5f6d 6174 652c 203a  airs[can_mate, :
+0001a1d0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+0001a1e0: 2070 6169 7273 0a0a 0a20 2020 2064 6566   pairs...    def
+0001a1f0: 205f 6d61 6b65 5f67 6561 5f64 6628 7365   _make_gea_df(se
+0001a200: 6c66 2c20 6c79 725f 6e75 6d3d 3129 3a0a  lf, lyr_num=1):.
+0001a210: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0001a220: 2020 2020 204d 616b 6573 2061 2064 6174       Makes a dat
+0001a230: 6166 7261 6d65 2066 6f72 2047 4541 2061  aframe for GEA a
+0001a240: 6e61 6c79 7369 7320 636f 6e74 6169 6e69  nalysis containi
+0001a250: 6e67 2067 656e 6f74 7970 6573 2c20 636f  ng genotypes, co
+0001a260: 6f72 6469 6e61 7465 732c 0a20 2020 2020  ordinates,.     
+0001a270: 2020 2061 6e64 2065 6e76 2076 616c 7565     and env value
+0001a280: 7320 666f 7220 616c 6c20 696e 6469 7669  s for all indivi
+0001a290: 6475 616c 732e 0a0a 2020 2020 2020 2020  duals...        
+0001a2a0: 4e4f 5445 3a20 4375 7272 656e 746c 7920  NOTE: Currently 
+0001a2b0: 6f6e 6c79 2061 6363 6570 7473 206f 6e65  only accepts one
+0001a2c0: 204c 616e 6473 6361 7065 204c 6179 6572   Landscape Layer
+0001a2d0: 2028 692e 652e 2065 6e76 6972 6f6e 6d65   (i.e. environme
+0001a2e0: 6e74 616c 0a20 2020 2020 2020 2020 2020  ntal.           
+0001a2f0: 2020 2076 6172 6961 626c 6529 0a0a 2020     variable)..  
+0001a300: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0001a310: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0001a320: 2d2d 2d0a 2020 2020 2020 2020 6c79 725f  ---.        lyr_
+0001a330: 6e75 6d20 3a20 696e 740a 2020 2020 2020  num : int.      
+0001a340: 2020 2020 2020 5468 6520 6e75 6d62 6572        The number
+0001a350: 206f 6620 7468 6520 4c61 6e64 7363 6170   of the Landscap
+0001a360: 6520 4c61 7965 7220 6672 6f6d 2077 6869  e Layer from whi
+0001a370: 6368 2074 6f20 6578 7472 6163 740a 2020  ch to extract.  
+0001a380: 2020 2020 2020 2020 2020 656e 7669 726f            enviro
+0001a390: 6e6d 656e 7461 6c20 7661 6c75 6573 2e20  nmental values. 
+0001a3a0: 4465 6661 756c 7473 2074 6f20 312e 0a0a  Defaults to 1...
+0001a3b0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0001a3c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0001a3d0: 2020 2020 2020 2020 6f75 7420 3a20 7061          out : pa
+0001a3e0: 6e64 6173 2e44 6174 6146 7261 6d65 0a20  ndas.DataFrame. 
+0001a3f0: 2020 2020 2020 2020 2020 2041 2044 6174             A Dat
+0001a400: 6146 7261 6d65 2069 6e20 7768 6963 6820  aFrame in which 
+0001a410: 636f 6c75 6d6e 7320 6172 6520 6c6f 6369  columns are loci
+0001a420: 2061 6e64 2072 6f77 7320 6172 6520 696e   and rows are in
+0001a430: 6469 7669 6475 616c 730a 2020 2020 2020  dividuals.      
+0001a440: 2020 2222 220a 2020 2020 2020 2020 2367    """.        #g
+0001a450: 6574 2061 7272 6179 206f 6620 5b30 7c30  et array of [0|0
+0001a460: 2e35 7c31 5d20 6765 6e6f 7479 7065 730a  .5|1] genotypes.
+0001a470: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001a480: 2020 2020 6765 6e20 3d20 7365 6c66 2e5f      gen = self._
+0001a490: 6765 745f 6765 6e6f 7479 7065 7328 290a  get_genotypes().
+0001a4a0: 0a20 2020 2020 2020 2023 6c6f 6f70 2074  .        #loop t
+0001a4b0: 6f20 636f 6e76 6572 7420 6269 6e61 7279  o convert binary
+0001a4c0: 2061 6c6c 656c 6520 6765 6e6f 7479 7065   allele genotype
+0001a4d0: 7320 2830 7c31 290a 2020 2020 2020 2020  s (0|1).        
+0001a4e0: 2369 6e74 6f20 7369 6e67 6c65 2064 6967  #into single dig
+0001a4f0: 6974 2067 656e 6f74 7970 6573 2028 302c  it genotypes (0,
+0001a500: 2030 2e35 2c20 3129 0a20 2020 2020 2020   0.5, 1).       
+0001a510: 2067 656e 6f5f 696e 6420 3d20 5b5d 0a20   geno_ind = []. 
+0001a520: 2020 2020 2020 2066 6f72 2069 6e64 2069         for ind i
+0001a530: 6e20 7261 6e67 6528 6c65 6e28 6765 6e29  n range(len(gen)
+0001a540: 293a 0a20 2020 2020 2020 2020 2020 2067  ):.            g
+0001a550: 656e 6f5f 6c6f 6320 3d20 5b5d 0a20 2020  eno_loc = [].   
+0001a560: 2020 2020 2020 2020 2066 6f72 206c 6f63           for loc
+0001a570: 6920 696e 2072 616e 6765 286c 656e 2867  i in range(len(g
+0001a580: 656e 5b69 6e64 5d29 293a 0a20 2020 2020  en[ind])):.     
+0001a590: 2020 2020 2020 2020 2020 2067 656e 6f74             genot
+0001a5a0: 7970 6520 3d20 6765 6e5b 696e 645d 5b6c  ype = gen[ind][l
+0001a5b0: 6f63 695d 2e6d 6561 6e28 2920 2320 636f  oci].mean() # co
+0001a5c0: 6465 6420 6173 2030 2f30 2e35 2f31 0a20  ded as 0/0.5/1. 
+0001a5d0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0001a5e0: 656e 6f5f 6c6f 632e 6170 7065 6e64 2867  eno_loc.append(g
+0001a5f0: 656e 6f74 7970 6529 0a20 2020 2020 2020  enotype).       
+0001a600: 2020 2020 2067 656e 6f5f 696e 642e 6170       geno_ind.ap
+0001a610: 7065 6e64 2867 656e 6f5f 6c6f 6329 0a20  pend(geno_loc). 
+0001a620: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001a630: 2020 2067 7473 203d 2073 656c 662e 5f67     gts = self._g
+0001a640: 6574 5f67 656e 6f74 7970 6573 2862 6961  et_genotypes(bia
+0001a650: 6c6c 656c 6963 3d46 616c 7365 290a 0a20  llelic=False).. 
+0001a660: 2020 2020 2020 2023 636f 6e76 6572 7420         #convert 
+0001a670: 746f 2064 6174 6166 7261 6d65 0a20 2020  to dataframe.   
+0001a680: 2020 2020 2067 6561 5f64 6620 3d20 7064       gea_df = pd
+0001a690: 2e44 6174 6146 7261 6d65 2867 7473 290a  .DataFrame(gts).
+0001a6a0: 0a20 2020 2020 2020 2023 6765 7420 656e  .        #get en
+0001a6b0: 7669 726f 6e6d 656e 7461 6c20 6461 7461  vironmental data
+0001a6c0: 0a20 2020 2020 2020 2065 6e76 203d 2073  .        env = s
+0001a6d0: 656c 662e 5f67 6574 5f65 2829 0a20 2020  elf._get_e().   
+0001a6e0: 2020 2020 2067 6561 5f64 665b 2765 6e76       gea_df['env
+0001a6f0: 275d 203d 206c 6973 7428 656e 765b 3a2c  '] = list(env[:,
+0001a700: 6c79 725f 6e75 6d5d 290a 0a20 2020 2020  lyr_num])..     
+0001a710: 2020 2023 6765 7420 636f 6f72 6473 0a20     #get coords. 
+0001a720: 2020 2020 2020 2063 6f6f 7264 203d 2073         coord = s
+0001a730: 656c 662e 5f67 6574 5f63 6f6f 7264 7328  elf._get_coords(
+0001a740: 290a 2020 2020 2020 2020 6765 615f 6466  ).        gea_df
+0001a750: 5b27 6c61 7427 5d20 3d20 6c69 7374 2863  ['lat'] = list(c
+0001a760: 6f6f 7264 5b3a 2c30 5d29 0a20 2020 2020  oord[:,0]).     
+0001a770: 2020 2067 6561 5f64 665b 276c 6f6e 6727     gea_df['long'
+0001a780: 5d20 3d20 6c69 7374 2863 6f6f 7264 5b3a  ] = list(coord[:
+0001a790: 2c31 5d29 0a0a 2020 2020 2020 2020 7265  ,1])..        re
+0001a7a0: 7475 726e 2067 6561 5f64 660a 0a0a 2020  turn gea_df...  
+0001a7b0: 2020 6465 6620 5f72 756e 5f63 6361 2873    def _run_cca(s
+0001a7c0: 656c 662c 2074 7274 5f6e 756d 3d30 2c20  elf, trt_num=0, 
+0001a7d0: 7363 616c 653d 5472 7565 2c20 706c 6f74  scale=True, plot
+0001a7e0: 3d54 7275 652c 2070 6c6f 745f 7364 3d54  =True, plot_sd=T
+0001a7f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0001a800: 2020 2020 2020 7364 3d33 293a 0a20 2020        sd=3):.   
+0001a810: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001a820: 2052 756e 7320 6120 6361 6e6f 6e69 6361   Runs a canonica
+0001a830: 6c20 636f 7272 656c 6174 696f 6e20 616e  l correlation an
+0001a840: 616c 7973 6973 2028 4343 4129 206f 6e20  alysis (CCA) on 
+0001a850: 7468 6520 6375 7272 656e 7420 6765 6e65  the current gene
+0001a860: 7469 6320 616e 640a 2020 2020 2020 2020  tic and.        
+0001a870: 656e 7669 726f 6e6d 656e 7461 6c20 6461  environmental da
+0001a880: 7461 2066 6f72 2074 6865 2053 7065 6369  ta for the Speci
+0001a890: 6573 2720 6375 7272 656e 7420 706f 7075  es' current popu
+0001a8a0: 6c61 7469 6f6e 2c20 7573 696e 6720 7468  lation, using th
+0001a8b0: 650a 2020 2020 2020 2020 696e 6469 6361  e.        indica
+0001a8c0: 7465 6420 5472 6169 742e 2050 6c6f 7473  ted Trait. Plots
+0001a8d0: 2074 6865 2072 6573 756c 7473 2061 6e64   the results and
+0001a8e0: 2072 6574 7572 6e73 2074 6865 6d20 696e   returns them in
+0001a8f0: 2061 2064 6963 742e 0a0a 2020 2020 2020   a dict...      
+0001a900: 2020 4343 4120 6d6f 6465 6c20 666f 726d    CCA model form
+0001a910: 756c 613a 2067 656e 6f74 7970 6520 7e20  ula: genotype ~ 
+0001a920: 656e 7620 2b20 6c61 7420 2b20 6c6f 6e67  env + lat + long
+0001a930: 0a0a 2020 2020 2020 2020 4e4f 5445 3a20  ..        NOTE: 
+0001a940: 6375 7272 656e 746c 7920 6f6e 6c79 2070  currently only p
+0001a950: 6f73 7369 626c 6520 746f 2064 6f20 3320  ossible to do 3 
+0001a960: 636f 6d70 6f6e 656e 7473 2f33 2076 6172  components/3 var
+0001a970: 6961 626c 6573 3b0a 2020 2020 2020 2020  iables;.        
+0001a980: 2020 2020 2020 7769 6c6c 2061 6464 2067        will add g
+0001a990: 7265 6174 6572 2066 756e 6374 696f 6e61  reater functiona
+0001a9a0: 6c69 7479 2069 6e20 7468 6520 6675 7475  lity in the futu
+0001a9b0: 7265 0a0a 2020 2020 2020 2020 5061 7261  re..        Para
+0001a9c0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0001a9d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0001a9e0: 2020 7472 745f 6e75 6d20 3a20 696e 740a    trt_num : int.
+0001a9f0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0001aa00: 6e75 6d62 6572 206f 6620 7468 6520 5472  number of the Tr
+0001aa10: 6169 7420 746f 2072 756e 2074 6865 2047  ait to run the G
+0001aa20: 4541 206f 6e2e 2044 6566 6175 6c74 7320  EA on. Defaults 
+0001aa30: 746f 2030 2e0a 2020 2020 2020 2020 7363  to 0..        sc
+0001aa40: 616c 6520 3a20 626f 6f6c 0a20 2020 2020  ale : bool.     
+0001aa50: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+0001aa60: 7363 616c 6573 2074 6865 2076 6172 6961  scales the varia
+0001aa70: 626c 652c 2069 6e64 6976 6964 7561 6c2c  ble, individual,
+0001aa80: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001aa90: 206c 6f63 7573 206c 6f61 6469 6e67 7320   locus loadings 
+0001aaa0: 6672 6f6d 202d 3120 746f 2031 2074 6f20  from -1 to 1 to 
+0001aab0: 6d61 6b65 2074 6865 6d20 6561 7369 6572  make them easier
+0001aac0: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
+0001aad0: 7669 7375 616c 697a 652e 2044 6566 6175  visualize. Defau
+0001aae0: 6c74 7320 746f 2054 7275 652e 0a20 2020  lts to True..   
+0001aaf0: 2020 2020 2070 6c6f 7420 3a20 626f 6f6c       plot : bool
+0001ab00: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+0001ab10: 7468 6572 206f 7220 6e6f 7420 746f 2070  ther or not to p
+0001ab20: 6c6f 7420 7468 6520 6d6f 6465 6c2e 2044  lot the model. D
+0001ab30: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
+0001ab40: 0a20 2020 2020 2020 2070 6c6f 745f 7364  .        plot_sd
+0001ab50: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
+0001ab60: 2020 2020 4966 2054 7275 652c 2061 2073      If True, a s
+0001ab70: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
+0001ab80: 6e20 656c 6c69 7073 6520 6973 2070 6c6f  n ellipse is plo
+0001ab90: 7474 6564 2c20 7573 696e 6720 7468 6520  tted, using the 
+0001aba0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
+0001abb0: 2020 206f 6620 7374 616e 6461 7264 2064     of standard d
+0001abc0: 6576 6961 7469 6f6e 7320 696e 6469 6361  eviations indica
+0001abd0: 7465 6420 6279 2074 6865 2061 7267 756d  ted by the argum
+0001abe0: 656e 7420 2773 6427 2e20 4465 6661 756c  ent 'sd'. Defaul
+0001abf0: 7473 2074 6f0a 2020 2020 2020 2020 2020  ts to.          
+0001ac00: 2020 5472 7565 2e0a 2020 2020 2020 2020    True..        
+0001ac10: 7364 203a 207b 696e 742c 2066 6c6f 6174  sd : {int, float
+0001ac20: 7d0a 2020 2020 2020 2020 2020 2020 4e75  }.            Nu
+0001ac30: 6d62 6572 206f 6620 7374 616e 6461 7264  mber of standard
+0001ac40: 2064 6576 6961 7469 6f6e 7320 746f 2075   deviations to u
+0001ac50: 7365 2066 6f72 2070 6c6f 7474 696e 6720  se for plotting 
+0001ac60: 7468 6520 7374 616e 6461 7264 0a20 2020  the standard.   
+0001ac70: 2020 2020 2020 2020 2064 6576 6961 7469           deviati
+0001ac80: 6f6e 2065 6c6c 6970 7365 2e20 4465 6661  on ellipse. Defa
+0001ac90: 756c 7473 2074 6f20 332e 0a0a 2020 2020  ults to 3...    
+0001aca0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0001acb0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001acc0: 2020 2020 6f75 7420 3a20 6469 6374 0a20      out : dict. 
+0001acd0: 2020 2020 2020 2020 2020 2041 2064 6963             A dic
+0001ace0: 7420 6f66 2074 6865 2066 6f6c 6c6f 7769  t of the followi
+0001acf0: 6e67 206b 6579 2d76 616c 7565 2070 6169  ng key-value pai
+0001ad00: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+0001ad10: 2020 2020 2267 6561 5f64 6622 3a20 6120      "gea_df": a 
+0001ad20: 4461 7461 4672 616d 6520 6f66 2069 6e64  DataFrame of ind
+0001ad30: 6976 6964 7561 6c73 2720 6765 6e6f 7479  ividuals' genoty
+0001ad40: 7065 732c 2065 6e76 6972 6f6e 6d65 6e74  pes, environment
+0001ad50: 616c 0a20 2020 2020 2020 2020 2020 2020  al.             
+0001ad60: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0001ad70: 7565 732c 2061 6e64 2063 6f6f 7264 696e  ues, and coordin
+0001ad80: 6174 6573 0a20 2020 2020 2020 2020 2020  ates.           
+0001ad90: 2020 2020 2022 696e 645f 4343 4164 6622       "ind_CCAdf"
+0001ada0: 3a20 696e 6469 7669 6475 616c 206c 6f61  : individual loa
+0001adb0: 6469 6e67 7320 2863 6f6c 756d 6e73 203d  dings (columns =
+0001adc0: 2061 7865 732c 0a20 2020 2020 2020 2020   axes,.         
+0001add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ade0: 2020 2020 726f 7773 203d 2069 6e64 6976      rows = indiv
+0001adf0: 6964 7561 6c73 290a 2020 2020 2020 2020  iduals).        
+0001ae00: 2020 2020 2020 2020 226c 6f63 695f 4343          "loci_CC
+0001ae10: 4164 6622 3a20 6c6f 6375 7320 6c6f 6164  Adf": locus load
+0001ae20: 696e 6773 2028 636f 6c75 6d6e 7320 3d20  ings (columns = 
+0001ae30: 6178 6573 2c20 726f 7773 203d 206c 6f63  axes, rows = loc
+0001ae40: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
+0001ae50: 2020 2022 7661 725f 4343 4164 6622 3a20     "var_CCAdf": 
+0001ae60: 7661 7269 6162 6c65 206c 6f61 6469 6e67  variable loading
+0001ae70: 7320 2863 6f6c 756d 6e73 203d 2061 7865  s (columns = axe
+0001ae80: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0001ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aea0: 726f 7773 203d 2076 6172 6961 626c 6520  rows = variable 
+0001aeb0: 2865 6e76 2c20 6c61 742c 206c 6f6e 6729  (env, lat, long)
+0001aec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001aed0: 2020 2274 7261 6974 5f6c 6f63 6922 3a20    "trait_loci": 
+0001aee0: 6c69 7374 206f 6620 696e 6465 7865 7320  list of indexes 
+0001aef0: 666f 7220 6c6f 6369 2074 6861 7420 756e  for loci that un
+0001af00: 6465 726c 6965 2074 6865 2074 7261 6974  derlie the trait
+0001af10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001af20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001af30: 6f72 2077 6869 6368 2074 6865 2043 4341  or which the CCA
+0001af40: 2077 6173 2072 756e 0a20 2020 2020 2020   was run.       
+0001af50: 2022 2222 0a20 2020 2020 2020 2023 6d61   """.        #ma
+0001af60: 6b65 2044 460a 2020 2020 2020 2020 6765  ke DF.        ge
+0001af70: 615f 6466 203d 7365 6c66 2e5f 6d61 6b65  a_df =self._make
+0001af80: 5f67 6561 5f64 6628 6c79 725f 6e75 6d3d  _gea_df(lyr_num=
+0001af90: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
+0001afa0: 6169 7473 5b74 7274 5f6e 756d 5d2e 6c79  aits[trt_num].ly
+0001afb0: 725f 6e75 6d29 0a0a 2020 2020 2020 2020  r_num)..        
+0001afc0: 2367 6574 2061 6461 7074 6976 6520 6c6f  #get adaptive lo
+0001afd0: 6369 2028 7573 6564 206c 6174 6572 2069  ci (used later i
+0001afe0: 6e20 706c 6f74 7469 6e67 290a 2020 2020  n plotting).    
+0001aff0: 2020 2020 7472 6169 745f 6c6f 6369 203d      trait_loci =
+0001b000: 2073 656c 662e 6765 6e5f 6172 6368 2e74   self.gen_arch.t
+0001b010: 7261 6974 735b 7472 745f 6e75 6d5d 2e6c  raits[trt_num].l
+0001b020: 6f63 6920 2367 6574 7320 7472 6169 7420  oci #gets trait 
+0001b030: 6c6f 6369 2069 6e64 6578 6573 0a0a 2020  loci indexes..  
+0001b040: 2020 2020 2020 2367 6574 206e 756d 6265        #get numbe
+0001b050: 7220 6f66 206c 6f63 690a 2020 2020 2020  r of loci.      
+0001b060: 2020 4c20 3d20 7365 6c66 2e67 656e 5f61    L = self.gen_a
+0001b070: 7263 682e 4c0a 2020 2020 2020 2020 2364  rch.L.        #d
+0001b080: 6566 696e 6520 7820 616e 6420 793a 0a20  efine x and y:. 
+0001b090: 2020 2020 2020 2023 2070 756c 6c20 6f75         # pull ou
+0001b0a0: 7420 6765 6e6f 7479 7065 730a 2020 2020  t genotypes.    
+0001b0b0: 2020 2020 5920 3d20 6765 615f 6466 2e69      Y = gea_df.i
+0001b0c0: 6c6f 635b 3a2c 7261 6e67 6528 4c29 5d0a  loc[:,range(L)].
+0001b0d0: 2020 2020 2020 2020 2320 7075 6c6c 206f          # pull o
+0001b0e0: 7574 2070 7265 6469 6374 6f72 2076 6172  ut predictor var
+0001b0f0: 6961 626c 6573 0a20 2020 2020 2020 2023  iables.        #
+0001b100: 2054 4f44 4f3a 206d 616b 6520 6974 2070   TODO: make it p
+0001b110: 6f73 7369 626c 6520 746f 2063 686f 6f73  ossible to choos
+0001b120: 6520 6d6f 7265 2076 6172 7320 696e 2066  e more vars in f
+0001b130: 7574 7572 650a 2020 2020 2020 2020 5820  uture.        X 
+0001b140: 3d20 6765 615f 6466 5b5b 2765 6e76 272c  = gea_df[['env',
+0001b150: 276c 6174 272c 276c 6f6e 6727 5d5d 0a0a  'lat','long']]..
+0001b160: 2020 2020 2020 2020 2364 6566 696e 6520          #define 
+0001b170: 6e5f 636f 6d70 6f6e 656e 7473 0a20 2020  n_components.   
+0001b180: 2020 2020 206e 5f63 6f6d 706f 6e65 6e74       n_component
+0001b190: 7320 3d20 330a 2020 2020 2020 2020 2363  s = 3.        #c
+0001b1a0: 7265 6174 6520 7468 6520 4343 4120 6d6f  reate the CCA mo
+0001b1b0: 6465 6c20 616e 6420 6669 7420 6974 2074  del and fit it t
+0001b1c0: 6f20 7468 6520 6461 7461 0a20 2020 2020  o the data.     
+0001b1d0: 2020 2063 6361 203d 2043 4341 286e 5f63     cca = CCA(n_c
+0001b1e0: 6f6d 706f 6e65 6e74 7320 3d20 6e5f 636f  omponents = n_co
+0001b1f0: 6d70 6f6e 656e 7473 290a 2020 2020 2020  mponents).      
+0001b200: 2020 6363 612e 6669 7428 592c 2058 290a    cca.fit(Y, X).
+0001b210: 0a20 2020 2020 2020 2023 7472 616e 7366  .        #transf
+0001b220: 6f72 6d20 6461 7461 0a20 2020 2020 2020  orm data.       
+0001b230: 2059 5f63 203d 2063 6361 2e74 7261 6e73   Y_c = cca.trans
+0001b240: 666f 726d 2859 290a 0a20 2020 2020 2020  form(Y)..       
+0001b250: 2023 6372 6561 7465 2064 6620 666f 7220   #create df for 
+0001b260: 696e 6469 7669 6475 616c 730a 2020 2020  individuals.    
+0001b270: 2020 2020 696e 645f 6466 203d 2070 642e      ind_df = pd.
+0001b280: 4461 7461 4672 616d 6528 595f 6329 0a20  DataFrame(Y_c). 
+0001b290: 2020 2020 2020 2023 6e61 6d69 6e67 2043         #naming C
+0001b2a0: 4341 2063 6f6c 756d 6e73 2073 7461 7274  CA columns start
+0001b2b0: 696e 6720 6174 2031 0a20 2020 2020 2020  ing at 1.       
+0001b2c0: 2069 6e64 5f64 662e 636f 6c75 6d6e 7320   ind_df.columns 
+0001b2d0: 3d20 5b73 7472 2872 2920 666f 7220 7220  = [str(r) for r 
+0001b2e0: 696e 2072 616e 6765 2831 2c20 6e5f 636f  in range(1, n_co
+0001b2f0: 6d70 6f6e 656e 7473 202b 2031 295d 0a0a  mponents + 1)]..
+0001b300: 2020 2020 2020 2020 2363 7265 6174 6520          #create 
+0001b310: 6466 2066 6f72 206c 6f63 690a 2020 2020  df for loci.    
+0001b320: 2020 2020 6c6f 6369 5f64 6620 3d20 7064      loci_df = pd
+0001b330: 2e44 6174 6146 7261 6d65 2863 6361 2e78  .DataFrame(cca.x
+0001b340: 5f6c 6f61 6469 6e67 735f 290a 2020 2020  _loadings_).    
+0001b350: 2020 2020 6c6f 6369 5f64 662e 636f 6c75      loci_df.colu
+0001b360: 6d6e 7320 3d20 696e 645f 6466 2e63 6f6c  mns = ind_df.col
+0001b370: 756d 6e73 2023 7361 6d65 2063 6f6c 756d  umns #same colum
+0001b380: 6e20 6e61 6d65 730a 0a20 2020 2020 2020  n names..       
+0001b390: 2023 6372 6561 7465 2064 6620 666f 7220   #create df for 
+0001b3a0: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
+0001b3b0: 2020 7661 725f 6466 203d 2070 642e 4461    var_df = pd.Da
+0001b3c0: 7461 4672 616d 6528 6363 612e 795f 6c6f  taFrame(cca.y_lo
+0001b3d0: 6164 696e 6773 5f29 0a20 2020 2020 2020  adings_).       
+0001b3e0: 2076 6172 5f64 662e 636f 6c75 6d6e 7320   var_df.columns 
+0001b3f0: 3d20 696e 645f 6466 2e63 6f6c 756d 6e73  = ind_df.columns
+0001b400: 2023 7361 6d65 2063 6f6c 756d 6e20 6e61   #same column na
+0001b410: 6d65 730a 0a20 2020 2020 2020 2023 6d61  mes..        #ma
+0001b420: 6b65 2064 6963 7469 6f6e 6172 7920 6f66  ke dictionary of
+0001b430: 2064 6174 6166 7261 6d65 7320 746f 2072   dataframes to r
+0001b440: 6574 7572 6e0a 2020 2020 2020 2020 6363  eturn.        cc
+0001b450: 615f 6469 6374 203d 207b 2767 6561 5f64  a_dict = {'gea_d
+0001b460: 6627 3a67 6561 5f64 662c 0a20 2020 2020  f':gea_df,.     
+0001b470: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001b480: 696e 645f 6466 273a 696e 645f 6466 2c0a  ind_df':ind_df,.
+0001b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4a0: 2020 2020 276c 6f63 695f 6466 273a 6c6f      'loci_df':lo
+0001b4b0: 6369 5f64 662c 0a20 2020 2020 2020 2020  ci_df,.         
+0001b4c0: 2020 2020 2020 2020 2020 2027 7661 725f             'var_
+0001b4d0: 6466 273a 7661 725f 6466 2c0a 2020 2020  df':var_df,.    
+0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4f0: 2774 7261 6974 5f6c 6f63 6927 3a74 7261  'trait_loci':tra
+0001b500: 6974 5f6c 6f63 697d 0a0a 2020 2020 2020  it_loci}..      
+0001b510: 2020 2320 4e4f 5445 3a20 7269 6768 7420    # NOTE: right 
+0001b520: 6e6f 7720 7468 6973 2070 6c6f 7474 696e  now this plottin
+0001b530: 6720 6c6f 6f70 206f 6e6c 7920 776f 726b  g loop only work
+0001b540: 7320 666f 7220 6120 6d61 7869 6d75 6d20  s for a maximum 
+0001b550: 6f66 2033 2061 7865 733b 0a20 2020 2020  of 3 axes;.     
+0001b560: 2020 2023 2020 2020 2020 2069 6e20 7468     #       in th
+0001b570: 6520 6675 7475 7265 2061 7320 6d6f 7265  e future as more
+0001b580: 2065 6e76 2076 6172 7320 6172 6520 6164   env vars are ad
+0001b590: 6465 642c 2063 6f75 6c64 2061 6464 206d  ded, could add m
+0001b5a0: 6f72 6520 6178 6573 0a20 2020 2020 2020  ore axes.       
+0001b5b0: 2069 6620 706c 6f74 3a0a 2020 2020 2020   if plot:.      
+0001b5c0: 2020 2020 2020 2353 6361 6c65 2064 6174        #Scale dat
+0001b5d0: 6166 7261 6d65 7320 6672 6f6d 202d 3120  aframes from -1 
+0001b5e0: 746f 2031 2069 6620 7363 616c 6520 3d20  to 1 if scale = 
+0001b5f0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0001b600: 2069 6620 7363 616c 6520 3d3d 2054 7275   if scale == Tru
+0001b610: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001b620: 2020 2072 6d69 6e20 3d20 2d31 0a20 2020     rmin = -1.   
+0001b630: 2020 2020 2020 2020 2020 2020 2072 6d61               rma
+0001b640: 7820 3d20 310a 2020 2020 2020 2020 2020  x = 1.          
+0001b650: 2020 2020 2020 6c6f 6369 5f64 6620 3d20        loci_df = 
+0001b660: 726d 696e 202b 2028 6c6f 6369 5f64 6620  rmin + (loci_df 
+0001b670: 2d20 6c6f 6369 5f64 662e 7661 6c75 6573  - loci_df.values
+0001b680: 2e6d 696e 2829 2920 2a20 2872 6d61 7820  .min()) * (rmax 
+0001b690: 2d0a 2020 2020 2020 2020 2020 2020 2020  -.              
+0001b6a0: 2020 2020 2020 2020 2020 2872 6d69 6e29            (rmin)
+0001b6b0: 2920 2f20 286c 6f63 695f 6466 2e76 616c  ) / (loci_df.val
+0001b6c0: 7565 732e 6d61 7828 2920 2d20 6c6f 6369  ues.max() - loci
+0001b6d0: 5f64 662e 7661 6c75 6573 2e6d 696e 2829  _df.values.min()
+0001b6e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b6f0: 2020 7661 725f 6466 203d 2072 6d69 6e20    var_df = rmin 
+0001b700: 2b20 2876 6172 5f64 6620 2d20 7661 725f  + (var_df - var_
+0001b710: 6466 2e76 616c 7565 732e 6d69 6e28 2929  df.values.min())
+0001b720: 202a 2028 726d 6178 202d 0a20 2020 2020   * (rmax -.     
+0001b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b740: 2020 2028 726d 696e 2929 202f 2028 7661     (rmin)) / (va
+0001b750: 725f 6466 2e76 616c 7565 732e 6d61 7828  r_df.values.max(
+0001b760: 2920 2d20 7661 725f 6466 2e76 616c 7565  ) - var_df.value
+0001b770: 732e 6d69 6e28 2929 0a20 2020 2020 2020  s.min()).       
+0001b780: 2020 2020 2020 2020 2069 6e64 5f64 6620           ind_df 
+0001b790: 3d20 726d 696e 202b 2028 696e 645f 6466  = rmin + (ind_df
+0001b7a0: 202d 2069 6e64 5f64 662e 7661 6c75 6573   - ind_df.values
+0001b7b0: 2e6d 696e 2829 2920 2a20 2872 6d61 7820  .min()) * (rmax 
+0001b7c0: 2d0a 2020 2020 2020 2020 2020 2020 2020  -.              
+0001b7d0: 2020 2020 2020 2020 2020 2872 6d69 6e29            (rmin)
+0001b7e0: 2920 2f20 2869 6e64 5f64 662e 7661 6c75  ) / (ind_df.valu
+0001b7f0: 6573 2e6d 6178 2829 202d 2069 6e64 5f64  es.max() - ind_d
+0001b800: 662e 7661 6c75 6573 2e6d 696e 2829 290a  f.values.min()).
+0001b810: 0a0a 2020 2020 2020 2020 2020 2020 2367  ..            #g
+0001b820: 6574 206d 6178 2061 6e64 206d 696e 7320  et max and mins 
+0001b830: 746f 2073 6574 2061 7869 7320 6c61 7465  to set axis late
+0001b840: 7220 6f6e 0a20 2020 2020 2020 2020 2020  r on.           
+0001b850: 206d 6178 6466 203d 206d 6178 2869 6e64   maxdf = max(ind
+0001b860: 5f64 662e 7661 6c75 6573 2e6d 6178 2829  _df.values.max()
+0001b870: 2c20 7661 725f 6466 2e76 616c 7565 732e  , var_df.values.
+0001b880: 6d61 7828 292c 0a20 2020 2020 2020 2020  max(),.         
+0001b890: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001b8a0: 6f63 695f 6466 2e76 616c 7565 732e 6d61  oci_df.values.ma
+0001b8b0: 7828 2929 0a20 2020 2020 2020 2020 2020  x()).           
+0001b8c0: 206d 696e 6466 203d 2061 6273 286d 696e   mindf = abs(min
+0001b8d0: 2869 6e64 5f64 662e 7661 6c75 6573 2e6d  (ind_df.values.m
+0001b8e0: 696e 2829 2c20 7661 725f 6466 2e76 616c  in(), var_df.val
+0001b8f0: 7565 732e 6d69 6e28 292c 0a20 2020 2020  ues.min(),.     
+0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b910: 2020 2020 2020 206c 6f63 695f 6466 2e76         loci_df.v
+0001b920: 616c 7565 732e 6d69 6e28 2929 290a 2020  alues.min())).  
+0001b930: 2020 2020 2020 2020 2020 6178 6d61 7820            axmax 
+0001b940: 3d20 6d61 7828 6d61 7864 662c 206d 696e  = max(maxdf, min
+0001b950: 6466 2920 2a20 312e 3230 2023 6164 6469  df) * 1.20 #addi
+0001b960: 6e67 2061 2032 3025 2062 7566 6665 720a  ng a 20% buffer.
+0001b970: 0a20 2020 2020 2020 2020 2020 2023 7365  .            #se
+0001b980: 7420 7570 2066 6967 7572 650a 2020 2020  t up figure.    
+0001b990: 2020 2020 2020 2020 6669 6720 3d20 706c          fig = pl
+0001b9a0: 742e 6669 6775 7265 2866 6967 7369 7a65  t.figure(figsize
+0001b9b0: 3d28 3230 2c20 3135 2929 0a20 2020 2020  =(20, 15)).     
+0001b9c0: 2020 2020 2020 2066 6f72 206e 2c20 6363         for n, cc
+0001b9d0: 5f61 7865 735f 7061 6972 2069 6e20 656e  _axes_pair in en
+0001b9e0: 756d 6572 6174 6528 5b5b 312c 2032 5d2c  umerate([[1, 2],
+0001b9f0: 205b 312c 2033 5d2c 205b 322c 2033 5d5d   [1, 3], [2, 3]]
+0001ba00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001ba10: 2020 2023 6465 6669 6e65 2063 6f6d 706f     #define compo
+0001ba20: 6e65 6e74 7320 666f 7220 6178 6973 0a20  nents for axis. 
+0001ba30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001ba40: 635f 6178 6973 3120 3d20 6363 5f61 7865  c_axis1 = cc_axe
+0001ba50: 735f 7061 6972 5b30 5d20 2378 2d61 7869  s_pair[0] #x-axi
+0001ba60: 7320 4343 0a20 2020 2020 2020 2020 2020  s CC.           
+0001ba70: 2020 2020 2063 635f 6178 6973 3220 3d20       cc_axis2 = 
+0001ba80: 6363 5f61 7865 735f 7061 6972 5b31 5d20  cc_axes_pair[1] 
+0001ba90: 2379 2d61 7869 7320 4343 0a0a 2020 2020  #y-axis CC..    
+0001baa0: 2020 2020 2020 2020 2020 2020 6178 203d              ax =
+0001bab0: 2066 6967 2e61 6464 5f73 7562 706c 6f74   fig.add_subplot
+0001bac0: 2831 3331 2b6e 290a 0a20 2020 2020 2020  (131+n)..       
+0001bad0: 2020 2020 2020 2020 2023 6164 6420 6365           #add ce
+0001bae0: 6e74 6572 206c 696e 6573 0a20 2020 2020  nter lines.     
+0001baf0: 2020 2020 2020 2020 2020 2061 782e 6178             ax.ax
+0001bb00: 686c 696e 6528 793d 302c 2063 6f6c 6f72  hline(y=0, color
+0001bb10: 3d27 6c69 6768 7467 7261 7927 2c20 6c69  ='lightgray', li
+0001bb20: 6e65 7374 796c 653d 2764 6f74 7465 6427  nestyle='dotted'
+0001bb30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001bb40: 2020 6178 2e61 7876 6c69 6e65 2878 3d30    ax.axvline(x=0
+0001bb50: 2c20 636f 6c6f 723d 276c 6967 6874 6772  , color='lightgr
+0001bb60: 6179 272c 206c 696e 6573 7479 6c65 3d27  ay', linestyle='
+0001bb70: 646f 7474 6564 2729 0a0a 2020 2020 2020  dotted')..      
+0001bb80: 2020 2020 2020 2020 2020 2320 7365 7420            # set 
+0001bb90: 6178 6573 2072 616e 6765 0a20 2020 2020  axes range.     
+0001bba0: 2020 2020 2020 2020 2020 2070 6c74 2e78             plt.x
+0001bbb0: 6c69 6d28 2d61 786d 6178 2c20 6178 6d61  lim(-axmax, axma
+0001bbc0: 7829 0a20 2020 2020 2020 2020 2020 2020  x).             
+0001bbd0: 2020 2070 6c74 2e79 6c69 6d28 2d61 786d     plt.ylim(-axm
+0001bbe0: 6178 2c20 6178 6d61 7829 0a0a 2020 2020  ax, axmax)..    
+0001bbf0: 2020 2020 2020 2020 2020 2020 2370 6c6f              #plo
+0001bc00: 7420 6e65 7574 7261 6c20 534e 5073 0a20  t neutral SNPs. 
+0001bc10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001bc20: 782e 7363 6174 7465 7228 6c6f 6369 5f64  x.scatter(loci_d
+0001bc30: 665b 7374 7228 6363 5f61 7869 7331 295d  f[str(cc_axis1)]
+0001bc40: 2c20 6c6f 6369 5f64 665b 7374 7228 6363  , loci_df[str(cc
+0001bc50: 5f61 7869 7332 295d 2c0a 2020 2020 2020  _axis2)],.      
 0001bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc70: 206c 6162 656c 203d 2027 4e65 7574 7261   label = 'Neutra
-0001bc80: 6c20 534e 5073 272c 2061 6c70 6861 203d  l SNPs', alpha =
-0001bc90: 2030 2e37 290a 2020 2020 2020 2020 2020   0.7).          
-0001bca0: 2020 2020 2020 2370 6c6f 7420 696e 6469        #plot indi
-0001bcb0: 7669 6475 616c 730a 2020 2020 2020 2020  viduals.        
-0001bcc0: 2020 2020 2020 2020 636d 6170 5f73 6361          cmap_sca
-0001bcd0: 7420 3d20 6178 2e73 6361 7474 6572 2869  t = ax.scatter(i
-0001bce0: 6e64 5f64 665b 7374 7228 6363 5f61 7869  nd_df[str(cc_axi
-0001bcf0: 7331 295d 2c0a 2020 2020 2020 2020 2020  s1)],.          
-0001bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd10: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-0001bd20: 5f64 665b 7374 7228 6363 5f61 7869 7332  _df[str(cc_axis2
-0001bd30: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+0001bc70: 2020 2020 206d 6172 6b65 7220 3d20 272b       marker = '+
+0001bc80: 272c 2063 6f6c 6f72 203d 2027 6772 6179  ', color = 'gray
+0001bc90: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0001bca0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0001bcb0: 6265 6c20 3d20 274e 6575 7472 616c 2053  bel = 'Neutral S
+0001bcc0: 4e50 7327 2c20 616c 7068 6120 3d20 302e  NPs', alpha = 0.
+0001bcd0: 3729 0a20 2020 2020 2020 2020 2020 2020  7).             
+0001bce0: 2020 2023 706c 6f74 2069 6e64 6976 6964     #plot individ
+0001bcf0: 7561 6c73 0a20 2020 2020 2020 2020 2020  uals.           
+0001bd00: 2020 2020 2063 6d61 705f 7363 6174 203d       cmap_scat =
+0001bd10: 2061 782e 7363 6174 7465 7228 696e 645f   ax.scatter(ind_
+0001bd20: 6466 5b73 7472 2863 635f 6178 6973 3129  df[str(cc_axis1)
+0001bd30: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
 0001bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd50: 2020 2020 2020 2020 2020 2063 203d 2067             c = g
-0001bd60: 6561 5f64 662e 656e 762c 2063 6d61 703d  ea_df.env, cmap=
-0001bd70: 2776 6972 6964 6973 272c 0a20 2020 2020  'viridis',.     
+0001bd50: 2020 2020 2020 2020 2020 696e 645f 6466            ind_df
+0001bd60: 5b73 7472 2863 635f 6178 6973 3229 5d2c  [str(cc_axis2)],
+0001bd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bda0: 2020 6c61 6265 6c20 3d20 2249 6e64 6976    label = "Indiv
-0001bdb0: 6964 7561 6c73 222c 2061 6c70 6861 203d  iduals", alpha =
-0001bdc0: 2030 2e35 290a 2020 2020 2020 2020 2020   0.5).          
-0001bdd0: 2020 2020 2020 2370 6c6f 7420 6164 6170        #plot adap
-0001bde0: 7469 7665 2053 4e50 730a 2020 2020 2020  tive SNPs.      
-0001bdf0: 2020 2020 2020 2020 2020 6178 2e73 6361            ax.sca
-0001be00: 7474 6572 286c 6f63 695f 6466 5b73 7472  tter(loci_df[str
-0001be10: 2863 635f 6178 6973 3129 5d5b 7472 6169  (cc_axis1)][trai
-0001be20: 745f 6c6f 6369 5d2c 0a20 2020 2020 2020  t_loci],.       
-0001be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be40: 2020 2020 6c6f 6369 5f64 665b 7374 7228      loci_df[str(
-0001be50: 6363 5f61 7869 7332 295d 5b74 7261 6974  cc_axis2)][trait
-0001be60: 5f6c 6f63 695d 2c0a 2020 2020 2020 2020  _loci],.        
+0001bd90: 2020 2020 2020 2020 6320 3d20 6765 615f          c = gea_
+0001bda0: 6466 2e65 6e76 2c20 636d 6170 3d27 7669  df.env, cmap='vi
+0001bdb0: 7269 6469 7327 2c0a 2020 2020 2020 2020  ridis',.        
+0001bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bdd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001bde0: 6162 656c 203d 2022 496e 6469 7669 6475  abel = "Individu
+0001bdf0: 616c 7322 2c20 616c 7068 6120 3d20 302e  als", alpha = 0.
+0001be00: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+0001be10: 2020 2023 706c 6f74 2061 6461 7074 6976     #plot adaptiv
+0001be20: 6520 534e 5073 0a20 2020 2020 2020 2020  e SNPs.         
+0001be30: 2020 2020 2020 2061 782e 7363 6174 7465         ax.scatte
+0001be40: 7228 6c6f 6369 5f64 665b 7374 7228 6363  r(loci_df[str(cc
+0001be50: 5f61 7869 7331 295d 5b74 7261 6974 5f6c  _axis1)][trait_l
+0001be60: 6f63 695d 2c0a 2020 2020 2020 2020 2020  oci],.          
 0001be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be80: 2020 206d 6172 6b65 723d 222b 222c 2063     marker="+", c
-0001be90: 6f6c 6f72 203d 2022 7265 6422 2c20 733d  olor = "red", s=
-0001bea0: 3130 302c 0a20 2020 2020 2020 2020 2020  100,.           
+0001be80: 206c 6f63 695f 6466 5b73 7472 2863 635f   loci_df[str(cc_
+0001be90: 6178 6973 3229 5d5b 7472 6169 745f 6c6f  axis2)][trait_lo
+0001bea0: 6369 5d2c 0a20 2020 2020 2020 2020 2020  ci],.           
 0001beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bec0: 6c61 6265 6c20 3d20 2741 6461 7074 6976  label = 'Adaptiv
-0001bed0: 6520 534e 5073 2729 0a0a 2020 2020 2020  e SNPs')..      
-0001bee0: 2020 2020 2020 2020 2020 2370 6c6f 7420            #plot 
-0001bef0: 7661 7269 6162 6c65 2076 6563 746f 7273  variable vectors
-0001bf00: 2061 7320 6172 726f 7773 0a20 2020 2020   as arrows.     
-0001bf10: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0001bf20: 2069 6e20 7261 6e67 6528 7661 725f 6466   in range(var_df
-0001bf30: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
-0001bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf50: 7820 3d20 7661 725f 6466 5b73 7472 2863  x = var_df[str(c
-0001bf60: 635f 6178 6973 3129 5d5b 695d 0a20 2020  c_axis1)][i].   
-0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf80: 2079 203d 2076 6172 5f64 665b 7374 7228   y = var_df[str(
-0001bf90: 6363 5f61 7869 7332 295d 5b69 5d0a 2020  cc_axis2)][i].  
-0001bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfb0: 2020 706c 742e 6172 726f 7728 302c 2030    plt.arrow(0, 0
-0001bfc0: 2c20 782c 2079 2c20 7769 6474 6820 3d20  , x, y, width = 
-0001bfd0: 302e 3031 2c0a 2020 2020 2020 2020 2020  0.01,.          
-0001bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bff0: 2020 2020 6865 6164 5f77 6964 7468 203d      head_width =
-0001c000: 2030 2e30 352c 2063 6f6c 6f72 203d 2027   0.05, color = '
-0001c010: 626c 6163 6b27 290a 2020 2020 2020 2020  black').        
-0001c020: 2020 2020 2020 2020 2020 2020 7378 203d              sx =
-0001c030: 2030 2e31 0a20 2020 2020 2020 2020 2020   0.1.           
-0001c040: 2020 2020 2020 2020 2073 7920 3d20 302e           sy = 0.
-0001c050: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-0001c060: 2020 2020 2020 2320 7468 6973 206d 6573        # this mes
-0001c070: 7320 6973 206a 7573 7420 746f 2061 7272  s is just to arr
-0001c080: 616e 6765 2074 6865 2074 6578 740a 2020  ange the text.  
+0001bec0: 6d61 726b 6572 3d22 2b22 2c20 636f 6c6f  marker="+", colo
+0001bed0: 7220 3d20 2272 6564 222c 2073 3d31 3030  r = "red", s=100
+0001bee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001bef0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+0001bf00: 656c 203d 2027 4164 6170 7469 7665 2053  el = 'Adaptive S
+0001bf10: 4e50 7327 290a 0a20 2020 2020 2020 2020  NPs')..         
+0001bf20: 2020 2020 2020 2023 706c 6f74 2076 6172         #plot var
+0001bf30: 6961 626c 6520 7665 6374 6f72 7320 6173  iable vectors as
+0001bf40: 2061 7272 6f77 730a 2020 2020 2020 2020   arrows.        
+0001bf50: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0001bf60: 2072 616e 6765 2876 6172 5f64 662e 7368   range(var_df.sh
+0001bf70: 6170 655b 305d 293a 0a20 2020 2020 2020  ape[0]):.       
+0001bf80: 2020 2020 2020 2020 2020 2020 2078 203d               x =
+0001bf90: 2076 6172 5f64 665b 7374 7228 6363 5f61   var_df[str(cc_a
+0001bfa0: 7869 7331 295d 5b69 5d0a 2020 2020 2020  xis1)][i].      
+0001bfb0: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+0001bfc0: 3d20 7661 725f 6466 5b73 7472 2863 635f  = var_df[str(cc_
+0001bfd0: 6178 6973 3229 5d5b 695d 0a20 2020 2020  axis2)][i].     
+0001bfe0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001bff0: 6c74 2e61 7272 6f77 2830 2c20 302c 2078  lt.arrow(0, 0, x
+0001c000: 2c20 792c 2077 6964 7468 203d 2030 2e30  , y, width = 0.0
+0001c010: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+0001c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c030: 2068 6561 645f 7769 6474 6820 3d20 302e   head_width = 0.
+0001c040: 3035 2c20 636f 6c6f 7220 3d20 2762 6c61  05, color = 'bla
+0001c050: 636b 2729 0a20 2020 2020 2020 2020 2020  ck').           
+0001c060: 2020 2020 2020 2020 2073 7820 3d20 302e           sx = 0.
+0001c070: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+0001c080: 2020 2020 2020 7379 203d 2030 2e31 0a20        sy = 0.1. 
 0001c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0a0: 2020 2320 6e65 7874 2074 6f20 6172 726f    # next to arro
-0001c0b0: 7773 2062 7574 2069 7420 6973 2061 2057  ws but it is a W
-0001c0c0: 4950 0a20 2020 2020 2020 2020 2020 2020  IP.             
-0001c0d0: 2020 2020 2020 2069 6620 2878 203c 2030         if (x < 0
-0001c0e0: 2061 6e64 2079 203c 2030 293a 0a20 2020   and y < 0):.   
-0001c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c100: 2020 2020 706c 742e 7465 7874 2878 202d      plt.text(x -
-0001c110: 2073 782c 2079 202d 2073 792c 2058 2e63   sx, y - sy, X.c
-0001c120: 6f6c 756d 6e73 5b69 5d29 0a20 2020 2020  olumns[i]).     
-0001c130: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001c140: 6620 2878 203c 2030 2061 6e64 2079 203e  f (x < 0 and y >
-0001c150: 2030 293a 0a20 2020 2020 2020 2020 2020   0):.           
-0001c160: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0001c170: 7465 7874 2878 202d 2073 782c 2079 202b  text(x - sx, y +
-0001c180: 2073 792c 2058 2e63 6f6c 756d 6e73 5b69   sy, X.columns[i
-0001c190: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0001c1a0: 2020 2020 2020 2069 6620 2878 203e 2030         if (x > 0
-0001c1b0: 2061 6e64 2079 203e 2030 293a 0a20 2020   and y > 0):.   
-0001c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1d0: 2020 2020 706c 742e 7465 7874 2878 202b      plt.text(x +
-0001c1e0: 2073 782c 2079 202b 2073 792c 2058 2e63   sx, y + sy, X.c
-0001c1f0: 6f6c 756d 6e73 5b69 5d29 0a20 2020 2020  olumns[i]).     
-0001c200: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001c210: 6620 2878 203e 2030 2061 6e64 2079 203c  f (x > 0 and y <
-0001c220: 2030 293a 0a20 2020 2020 2020 2020 2020   0):.           
-0001c230: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0001c240: 7465 7874 2878 202b 2073 782c 2079 202d  text(x + sx, y -
-0001c250: 2073 792c 2058 2e63 6f6c 756d 6e73 5b69   sy, X.columns[i
-0001c260: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
-0001c270: 2020 2020 2370 6c6f 7420 5344 2065 6c6c      #plot SD ell
-0001c280: 6970 7365 2066 6f72 2053 4e50 2064 6174  ipse for SNP dat
-0001c290: 6120 6966 2070 6c6f 745f 7364 203d 2054  a if plot_sd = T
-0001c2a0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0001c2b0: 2020 2020 6966 2070 6c6f 745f 7364 3a0a      if plot_sd:.
-0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c2d0: 2020 2020 7231 203d 206e 702e 7374 6428      r1 = np.std(
-0001c2e0: 6c6f 6369 5f64 665b 7374 7228 6363 5f61  loci_df[str(cc_a
-0001c2f0: 7869 7331 295d 2920 2a20 7364 0a20 2020  xis1)]) * sd.   
+0001c0a0: 2020 2023 2074 6869 7320 6d65 7373 2069     # this mess i
+0001c0b0: 7320 6a75 7374 2074 6f20 6172 7261 6e67  s just to arrang
+0001c0c0: 6520 7468 6520 7465 7874 0a20 2020 2020  e the text.     
+0001c0d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001c0e0: 206e 6578 7420 746f 2061 7272 6f77 7320   next to arrows 
+0001c0f0: 6275 7420 6974 2069 7320 6120 5749 500a  but it is a WIP.
+0001c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c110: 2020 2020 6966 2028 7820 3c20 3020 616e      if (x < 0 an
+0001c120: 6420 7920 3c20 3029 3a0a 2020 2020 2020  d y < 0):.      
+0001c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c140: 2070 6c74 2e74 6578 7428 7820 2d20 7378   plt.text(x - sx
+0001c150: 2c20 7920 2d20 7379 2c20 582e 636f 6c75  , y - sy, X.colu
+0001c160: 6d6e 735b 695d 290a 2020 2020 2020 2020  mns[i]).        
+0001c170: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0001c180: 7820 3c20 3020 616e 6420 7920 3e20 3029  x < 0 and y > 0)
+0001c190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001c1a0: 2020 2020 2020 2020 2070 6c74 2e74 6578           plt.tex
+0001c1b0: 7428 7820 2d20 7378 2c20 7920 2b20 7379  t(x - sx, y + sy
+0001c1c0: 2c20 582e 636f 6c75 6d6e 735b 695d 290a  , X.columns[i]).
+0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1e0: 2020 2020 6966 2028 7820 3e20 3020 616e      if (x > 0 an
+0001c1f0: 6420 7920 3e20 3029 3a0a 2020 2020 2020  d y > 0):.      
+0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c210: 2070 6c74 2e74 6578 7428 7820 2b20 7378   plt.text(x + sx
+0001c220: 2c20 7920 2b20 7379 2c20 582e 636f 6c75  , y + sy, X.colu
+0001c230: 6d6e 735b 695d 290a 2020 2020 2020 2020  mns[i]).        
+0001c240: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0001c250: 7820 3e20 3020 616e 6420 7920 3c20 3029  x > 0 and y < 0)
+0001c260: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001c270: 2020 2020 2020 2020 2070 6c74 2e74 6578           plt.tex
+0001c280: 7428 7820 2b20 7378 2c20 7920 2d20 7379  t(x + sx, y - sy
+0001c290: 2c20 582e 636f 6c75 6d6e 735b 695d 290a  , X.columns[i]).
+0001c2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c2b0: 2023 706c 6f74 2053 4420 656c 6c69 7073   #plot SD ellips
+0001c2c0: 6520 666f 7220 534e 5020 6461 7461 2069  e for SNP data i
+0001c2d0: 6620 706c 6f74 5f73 6420 3d20 5472 7565  f plot_sd = True
+0001c2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c2f0: 2069 6620 706c 6f74 5f73 643a 0a20 2020   if plot_sd:.   
 0001c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c310: 2072 3220 3d20 6e70 2e73 7464 286c 6f63   r2 = np.std(loc
+0001c310: 2072 3120 3d20 6e70 2e73 7464 286c 6f63   r1 = np.std(loc
 0001c320: 695f 6466 5b73 7472 2863 635f 6178 6973  i_df[str(cc_axis
-0001c330: 3229 5d29 202a 2073 640a 2020 2020 2020  2)]) * sd.      
-0001c340: 2020 2020 2020 2020 2020 2020 2020 7420                t 
-0001c350: 3d20 6e70 2e6c 696e 7370 6163 6528 302c  = np.linspace(0,
-0001c360: 2032 2a6d 6174 685f 7069 2c20 3130 3029   2*math_pi, 100)
-0001c370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c380: 2020 2020 2061 782e 706c 6f74 2872 312a       ax.plot(r1*
-0001c390: 6e70 2e63 6f73 2874 2920 2c20 7232 2a6e  np.cos(t) , r2*n
-0001c3a0: 702e 7369 6e28 7429 2c20 6c69 6e65 7374  p.sin(t), linest
-0001c3b0: 796c 6520 3d20 2764 6173 6865 6427 2c0a  yle = 'dashed',.
-0001c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3d0: 2020 2020 2020 2020 2020 2020 6320 3d20              c = 
-0001c3e0: 2772 6564 272c 206c 6162 656c 203d 2073  'red', label = s
-0001c3f0: 7472 2873 6429 202b 2022 2053 7464 4465  tr(sd) + " StdDe
-0001c400: 7622 290a 0a20 2020 2020 2020 2020 2020  v")..           
-0001c410: 2020 2020 2023 4556 4552 5954 4849 4e47       #EVERYTHING
-0001c420: 2042 454c 4f57 2054 4849 5320 4c49 4e45   BELOW THIS LINE
-0001c430: 2049 4e20 5448 4520 4c4f 4f50 2049 5320   IN THE LOOP IS 
-0001c440: 4a55 5354 2050 4c4f 5420 464f 524d 4154  JUST PLOT FORMAT
-0001c450: 5449 4e47 200a 2020 2020 2020 2020 2020  TING .          
-0001c460: 2020 2020 2020 2378 6c61 6265 6c20 6973        #xlabel is
-0001c470: 2074 6865 206c 6162 656c 2061 7420 7468   the label at th
-0001c480: 6520 626f 7474 6f6d 2028 7665 7274 6963  e bottom (vertic
-0001c490: 616c 2061 7869 7320 6c61 6265 6c29 0a20  al axis label). 
-0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001c4b0: 2061 6e64 2079 6c61 6265 6c20 6973 206f   and ylabel is o
-0001c4c0: 6e20 7468 6520 6c65 6674 2073 6964 6520  n the left side 
-0001c4d0: 2868 6f72 697a 6f6e 7461 6c20 6178 6973  (horizontal axis
-0001c4e0: 206c 6162 656c 290a 2020 2020 2020 2020   label).        
-0001c4f0: 2020 2020 2020 2020 6c61 6265 6c20 3d20          label = 
-0001c500: 6178 2e73 6574 5f78 6c61 6265 6c28 2743  ax.set_xlabel('C
-0001c510: 4341 2720 2b20 7374 7228 6363 5f61 7869  CA' + str(cc_axi
-0001c520: 7332 292c 2066 6f6e 7473 697a 6520 3d20  s2), fontsize = 
-0001c530: 3929 0a20 2020 2020 2020 2020 2020 2020  9).             
-0001c540: 2020 2061 782e 7861 7869 732e 7365 745f     ax.xaxis.set_
-0001c550: 6c61 6265 6c5f 636f 6f72 6473 2830 2e35  label_coords(0.5
-0001c560: 2c20 2d30 2e30 3229 0a20 2020 2020 2020  , -0.02).       
-0001c570: 2020 2020 2020 2020 206c 6162 656c 203d           label =
-0001c580: 2061 782e 7365 745f 796c 6162 656c 2827   ax.set_ylabel('
-0001c590: 4343 4127 202b 2073 7472 2863 635f 6178  CCA' + str(cc_ax
-0001c5a0: 6973 3129 2c20 666f 6e74 7369 7a65 203d  is1), fontsize =
-0001c5b0: 2039 290a 2020 2020 2020 2020 2020 2020   9).            
-0001c5c0: 2020 2020 6178 2e79 6178 6973 2e73 6574      ax.yaxis.set
-0001c5d0: 5f6c 6162 656c 5f63 6f6f 7264 7328 2d30  _label_coords(-0
-0001c5e0: 2e30 322c 2030 2e35 3529 0a0a 2020 2020  .02, 0.55)..    
-0001c5f0: 2020 2020 2020 2020 2020 2020 236d 616b              #mak
-0001c600: 6520 696e 746f 2062 6f78 0a20 2020 2020  e into box.     
-0001c610: 2020 2020 2020 2020 2020 2061 782e 7365             ax.se
-0001c620: 745f 6173 7065 6374 2827 6571 7561 6c27  t_aspect('equal'
-0001c630: 2c20 6164 6a75 7374 6162 6c65 3d27 626f  , adjustable='bo
-0001c640: 7827 290a 0a20 2020 2020 2020 2020 2020  x')..           
-0001c650: 2020 2020 2023 4d6f 7665 206c 6566 7420       #Move left 
-0001c660: 792d 6178 6973 2026 2062 6f74 746f 6d20  y-axis & bottom 
-0001c670: 782d 6178 6973 2074 6f20 6365 6e74 6572  x-axis to center
-0001c680: 2c20 7061 7373 696e 6720 7468 7275 2028  , passing thru (
-0001c690: 302c 3029 0a20 2020 2020 2020 2020 2020  0,0).           
-0001c6a0: 2020 2020 2061 782e 7370 696e 6573 5b27       ax.spines['
-0001c6b0: 6c65 6674 275d 2e73 6574 5f70 6f73 6974  left'].set_posit
-0001c6c0: 696f 6e28 2763 656e 7465 7227 290a 2020  ion('center').  
-0001c6d0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0001c6e0: 2e73 7069 6e65 735b 2762 6f74 746f 6d27  .spines['bottom'
-0001c6f0: 5d2e 7365 745f 706f 7369 7469 6f6e 2827  ].set_position('
-0001c700: 6365 6e74 6572 2729 0a0a 2020 2020 2020  center')..      
-0001c710: 2020 2020 2020 2020 2020 2363 6861 6e67            #chang
-0001c720: 6520 636f 6c6f 7273 2f72 656d 6f76 6520  e colors/remove 
-0001c730: 6465 6661 756c 7420 6178 6973 0a20 2020  default axis.   
-0001c740: 2020 2020 2020 2020 2020 2020 2061 7863               axc
-0001c750: 6f6c 6f72 203d 2027 6e6f 6e65 270a 2020  olor = 'none'.  
-0001c760: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0001c770: 2e73 7069 6e65 735b 276c 6566 7427 5d2e  .spines['left'].
-0001c780: 7365 745f 636f 6c6f 7228 6178 636f 6c6f  set_color(axcolo
-0001c790: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-0001c7a0: 2020 2061 782e 7370 696e 6573 5b27 626f     ax.spines['bo
-0001c7b0: 7474 6f6d 275d 2e73 6574 5f63 6f6c 6f72  ttom'].set_color
-0001c7c0: 2861 7863 6f6c 6f72 290a 2020 2020 2020  (axcolor).      
-0001c7d0: 2020 2020 2020 2020 2020 6178 2e73 7069            ax.spi
-0001c7e0: 6e65 735b 2772 6967 6874 275d 2e73 6574  nes['right'].set
-0001c7f0: 5f63 6f6c 6f72 2861 7863 6f6c 6f72 290a  _color(axcolor).
-0001c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c810: 6178 2e73 7069 6e65 735b 2774 6f70 275d  ax.spines['top']
-0001c820: 2e73 6574 5f63 6f6c 6f72 2861 7863 6f6c  .set_color(axcol
-0001c830: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
-0001c840: 2020 2020 6178 2e74 6963 6b5f 7061 7261      ax.tick_para
-0001c850: 6d73 2861 7869 7320 3d20 2778 272c 2063  ms(axis = 'x', c
-0001c860: 6f6c 6f72 733d 6178 636f 6c6f 7229 0a20  olors=axcolor). 
-0001c870: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001c880: 782e 7469 636b 5f70 6172 616d 7328 6178  x.tick_params(ax
-0001c890: 6973 203d 2027 7927 2c20 636f 6c6f 7273  is = 'y', colors
-0001c8a0: 3d61 7863 6f6c 6f72 290a 0a20 2020 2020  =axcolor)..     
-0001c8b0: 2020 2020 2020 2020 2020 2061 782e 7961             ax.ya
-0001c8c0: 7869 732e 6c61 6265 6c2e 7365 745f 636f  xis.label.set_co
-0001c8d0: 6c6f 7228 2767 7261 7927 290a 2020 2020  lor('gray').    
-0001c8e0: 2020 2020 2020 2020 2020 2020 6178 2e78              ax.x
-0001c8f0: 6178 6973 2e6c 6162 656c 2e73 6574 5f63  axis.label.set_c
-0001c900: 6f6c 6f72 2827 6772 6179 2729 0a0a 2020  olor('gray')..  
-0001c910: 2020 2020 2020 2020 2020 2020 2020 236c                #l
-0001c920: 6567 656e 6473 0a20 2020 2020 2020 2020  egends.         
-0001c930: 2020 2020 2020 2069 6620 6e20 3d3d 2032         if n == 2
-0001c940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c950: 2020 2020 2020 6178 2e6c 6567 656e 6428        ax.legend(
-0001c960: 6c6f 6320 3d20 2275 7070 6572 206c 6566  loc = "upper lef
-0001c970: 7422 2c20 6262 6f78 5f74 6f5f 616e 6368  t", bbox_to_anch
-0001c980: 6f72 3d28 312e 332c 2031 2e30 3529 290a  or=(1.3, 1.05)).
-0001c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9a0: 2020 2020 706c 742e 636f 6c6f 7262 6172      plt.colorbar
-0001c9b0: 2863 6d61 705f 7363 6174 2c20 6c61 6265  (cmap_scat, labe
-0001c9c0: 6c3d 2265 6e76 2229 0a20 2020 2020 2020  l="env").       
-0001c9d0: 2020 2020 2066 6967 2e73 686f 7728 290a       fig.show().
-0001c9e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001c9f0: 6363 615f 6469 6374 0a0a 0a20 2020 2023  cca_dict...    #
-0001ca00: 206d 6574 686f 6420 666f 7220 706c 6f74   method for plot
-0001ca10: 7469 6e67 2074 6865 2073 7065 6369 6573  ting the species
-0001ca20: 2028 6f72 2061 2073 7562 7365 7420 6f66   (or a subset of
-0001ca30: 2069 7473 2069 6e64 6976 6964 7561 6c73   its individuals
-0001ca40: 2c20 6279 2049 4429 0a20 2020 2023 206f  , by ID).    # o
-0001ca50: 6e20 746f 7020 6f66 2061 206c 6179 6572  n top of a layer
-0001ca60: 2028 6f72 206c 616e 6473 6361 7065 290a   (or landscape).
-0001ca70: 2020 2020 6465 6620 5f70 6c6f 7428 7365      def _plot(se
-0001ca80: 6c66 2c20 6c79 725f 6e75 6d3d 4e6f 6e65  lf, lyr_num=None
-0001ca90: 2c20 6c61 6e64 3d4e 6f6e 652c 2068 6964  , land=None, hid
-0001caa0: 655f 6c61 6e64 3d46 616c 7365 2c20 696e  e_land=False, in
-0001cab0: 6469 7669 6473 3d4e 6f6e 652c 0a20 2020  divids=None,.   
-0001cac0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
-0001cad0: 4661 6c73 652c 2063 6f6c 6f72 3d27 626c  False, color='bl
-0001cae0: 6163 6b27 2c20 6564 6765 5f63 6f6c 6f72  ack', edge_color
-0001caf0: 3d27 6661 6365 272c 2074 6578 745f 636f  ='face', text_co
-0001cb00: 6c6f 723d 2762 6c61 636b 272c 0a20 2020  lor='black',.   
-0001cb10: 2020 2020 2020 2020 2020 2063 6261 723d             cbar=
-0001cb20: 5472 7565 2c20 7369 7a65 3d32 352c 2074  True, size=25, t
-0001cb30: 6578 745f 7369 7a65 3d39 2c20 6c61 6e64  ext_size=9, land
-0001cb40: 5f63 6d61 703d 4e6f 6e65 2c20 7074 5f63  _cmap=None, pt_c
-0001cb50: 6d61 703d 4e6f 6e65 2c0a 2020 2020 2020  map=None,.      
-0001cb60: 2020 2020 2020 2020 616c 7068 613d 4661          alpha=Fa
-0001cb70: 6c73 652c 207a 6f6f 6d5f 7769 6474 683d  lse, zoom_width=
-0001cb80: 4e6f 6e65 2c20 783d 4e6f 6e65 2c20 793d  None, x=None, y=
-0001cb90: 4e6f 6e65 2c20 766d 696e 3d4e 6f6e 652c  None, vmin=None,
-0001cba0: 0a20 2020 2020 2020 2020 2020 2020 2076  .              v
-0001cbb0: 6d61 783d 4e6f 6e65 2c20 7469 636b 733d  max=None, ticks=
-0001cbc0: 4e6f 6e65 2c20 6d61 736b 5f72 6173 743d  None, mask_rast=
-0001cbd0: 4e6f 6e65 2c20 616e 696d 6174 653d 4661  None, animate=Fa
-0001cbe0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-0001cbf0: 2020 2063 656c 6c5f 636f 6f72 6473 3d46     cell_coords=F
-0001cc00: 616c 7365 293a 0a20 2020 2020 2020 2023  alse):.        #
-0001cc10: 2063 6f6e 7665 7274 2069 6e64 6976 6964   convert individ
-0001cc20: 7320 746f 2061 206c 6973 7420 2869 6e20  s to a list (in 
-0001cc30: 6361 7365 2063 6f6d 6573 2069 6e20 6173  case comes in as
-0001cc40: 2061 206e 756d 7079 2061 7272 6179 290a   a numpy array).
-0001cc50: 2020 2020 2020 2020 6966 2069 6e64 6976          if indiv
-0001cc60: 6964 7320 6973 206e 6f74 204e 6f6e 6520  ids is not None 
-0001cc70: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-0001cc80: 6365 2869 6e64 6976 6964 732c 206c 6973  ce(individs, lis
-0001cc90: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0001cca0: 696e 6469 7669 6473 203d 206c 6973 7428  individs = list(
-0001ccb0: 696e 6469 7669 6473 290a 2020 2020 2020  individs).      
-0001ccc0: 2020 2320 6765 7420 636f 6f72 6473 0a20    # get coords. 
-0001ccd0: 2020 2020 2020 2063 6f6f 7264 7320 3d20         coords = 
-0001cce0: 7365 6c66 2e5f 6765 745f 706c 6f74 5f63  self._get_plot_c
-0001ccf0: 6f6f 7264 7328 696e 6469 7669 6473 3d69  oords(individs=i
-0001cd00: 6e64 6976 6964 732c 0a20 2020 2020 2020  ndivids,.       
-0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd30: 6365 6c6c 5f63 6f6f 7264 733d 6365 6c6c  cell_coords=cell
-0001cd40: 5f63 6f6f 7264 7329 0a20 2020 2020 2020  _coords).       
-0001cd50: 2023 2067 6574 2074 6578 740a 2020 2020   # get text.    
-0001cd60: 2020 2020 6966 2074 6578 743a 0a20 2020      if text:.   
-0001cd70: 2020 2020 2020 2020 2069 6620 696e 6469           if indi
-0001cd80: 7669 6473 2069 7320 4e6f 6e65 3a0a 2020  vids is None:.  
-0001cd90: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0001cda0: 7874 203d 205b 2a73 656c 665d 0a20 2020  xt = [*self].   
-0001cdb0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001cdc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001cdd0: 6578 7420 3d20 696e 6469 7669 6473 0a20  ext = individs. 
-0001cde0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001cdf0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-0001ce00: 4e6f 6e65 0a20 2020 2020 2020 2023 2073  None.        # s
-0001ce10: 6574 2074 6865 2070 6c74 5f6c 696d 730a  et the plt_lims.
-0001ce20: 2020 2020 2020 2020 706c 745f 6c69 6d73          plt_lims
-0001ce30: 203d 2076 697a 2e5f 6765 745f 706c 745f   = viz._get_plt_
-0001ce40: 6c69 6d73 286c 616e 642c 2078 2c20 792c  lims(land, x, y,
-0001ce50: 207a 6f6f 6d5f 7769 6474 6829 0a20 2020   zoom_width).   
-0001ce60: 2020 2020 2023 2070 6c6f 7420 7468 6520       # plot the 
-0001ce70: 6c61 7965 7228 7329 0a20 2020 2020 2020  layer(s).       
-0001ce80: 2069 6620 6869 6465 5f6c 616e 643a 0a20   if hide_land:. 
-0001ce90: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-0001cea0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001ceb0: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-0001cec0: 7468 6520 6c61 7965 7273 2720 766d 696e  the layers' vmin
-0001ced0: 2061 6e64 2076 6d61 7820 7661 6c75 6573   and vmax values
-0001cee0: 2c20 6966 2061 6e79 206f 6620 7468 6520  , if any of the 
-0001cef0: 6c61 7965 7273 2074 6f0a 2020 2020 2020  layers to.      
-0001cf00: 2020 2020 2020 2320 6265 2070 6c6f 7474        # be plott
-0001cf10: 6564 2068 6173 2061 2063 6861 6e67 6520  ed has a change 
-0001cf20: 6576 656e 740a 2020 2020 2020 2020 2020  event.          
-0001cf30: 2020 6966 2028 286c 7972 5f6e 756d 2069    if ((lyr_num i
-0001cf40: 7320 4e6f 6e65 2061 6e64 206c 616e 642e  s None and land.
-0001cf50: 5f63 6861 6e67 6572 2069 7320 6e6f 7420  _changer is not 
-0001cf60: 4e6f 6e65 2920 6f72 0a20 2020 2020 2020  None) or.       
-0001cf70: 2020 2020 2020 2020 2028 6c61 6e64 2e5f           (land._
-0001cf80: 6368 616e 6765 7220 6973 206e 6f74 204e  changer is not N
-0001cf90: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0001cfa0: 2020 2020 2061 6e64 206c 7972 5f6e 756d       and lyr_num
-0001cfb0: 2069 6e20 5b2a 6c61 6e64 2e5f 6368 616e   in [*land._chan
-0001cfc0: 6765 722e 6368 616e 6765 5f69 6e66 6f5d  ger.change_info]
-0001cfd0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0001cfe0: 2020 2020 6966 206c 7972 5f6e 756d 2069      if lyr_num i
-0001cff0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0001d000: 2020 2020 2020 2020 2020 2020 6c61 6e64              land
-0001d010: 5f76 6d69 6e20 3d20 5b6c 7972 2e5f 7363  _vmin = [lyr._sc
-0001d020: 616c 655f 6d69 6e20 666f 7220 6c79 7220  ale_min for lyr 
-0001d030: 696e 206c 616e 642e 7661 6c75 6573 2829  in land.values()
-0001d040: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001d050: 2020 2020 2020 6c61 6e64 5f76 6d61 7820        land_vmax 
-0001d060: 3d20 5b6c 7972 2e5f 7363 616c 655f 6d61  = [lyr._scale_ma
-0001d070: 7820 666f 7220 6c79 7220 696e 206c 616e  x for lyr in lan
-0001d080: 642e 7661 6c75 6573 2829 5d0a 2020 2020  d.values()].    
-0001d090: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001d0a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d0b0: 2020 2020 2020 6c61 6e64 5f76 6d69 6e20        land_vmin 
-0001d0c0: 3d20 5b6c 616e 645b 6c79 725f 6e75 6d5d  = [land[lyr_num]
-0001d0d0: 2e5f 7363 616c 655f 6d69 6e5d 0a20 2020  ._scale_min].   
+0001c330: 3129 5d29 202a 2073 640a 2020 2020 2020  1)]) * sd.      
+0001c340: 2020 2020 2020 2020 2020 2020 2020 7232                r2
+0001c350: 203d 206e 702e 7374 6428 6c6f 6369 5f64   = np.std(loci_d
+0001c360: 665b 7374 7228 6363 5f61 7869 7332 295d  f[str(cc_axis2)]
+0001c370: 2920 2a20 7364 0a20 2020 2020 2020 2020  ) * sd.         
+0001c380: 2020 2020 2020 2020 2020 2074 203d 206e             t = n
+0001c390: 702e 6c69 6e73 7061 6365 2830 2c20 322a  p.linspace(0, 2*
+0001c3a0: 6d61 7468 5f70 692c 2031 3030 290a 2020  math_pi, 100).  
+0001c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3c0: 2020 6178 2e70 6c6f 7428 7231 2a6e 702e    ax.plot(r1*np.
+0001c3d0: 636f 7328 7429 202c 2072 322a 6e70 2e73  cos(t) , r2*np.s
+0001c3e0: 696e 2874 292c 206c 696e 6573 7479 6c65  in(t), linestyle
+0001c3f0: 203d 2027 6461 7368 6564 272c 0a20 2020   = 'dashed',.   
+0001c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c410: 2020 2020 2020 2020 2063 203d 2027 7265           c = 're
+0001c420: 6427 2c20 6c61 6265 6c20 3d20 7374 7228  d', label = str(
+0001c430: 7364 2920 2b20 2220 5374 6444 6576 2229  sd) + " StdDev")
+0001c440: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c450: 2020 2345 5645 5259 5448 494e 4720 4245    #EVERYTHING BE
+0001c460: 4c4f 5720 5448 4953 204c 494e 4520 494e  LOW THIS LINE IN
+0001c470: 2054 4845 204c 4f4f 5020 4953 204a 5553   THE LOOP IS JUS
+0001c480: 5420 504c 4f54 2046 4f52 4d41 5454 494e  T PLOT FORMATTIN
+0001c490: 4720 0a20 2020 2020 2020 2020 2020 2020  G .             
+0001c4a0: 2020 2023 786c 6162 656c 2069 7320 7468     #xlabel is th
+0001c4b0: 6520 6c61 6265 6c20 6174 2074 6865 2062  e label at the b
+0001c4c0: 6f74 746f 6d20 2876 6572 7469 6361 6c20  ottom (vertical 
+0001c4d0: 6178 6973 206c 6162 656c 290a 2020 2020  axis label).    
+0001c4e0: 2020 2020 2020 2020 2020 2020 2320 616e              # an
+0001c4f0: 6420 796c 6162 656c 2069 7320 6f6e 2074  d ylabel is on t
+0001c500: 6865 206c 6566 7420 7369 6465 2028 686f  he left side (ho
+0001c510: 7269 7a6f 6e74 616c 2061 7869 7320 6c61  rizontal axis la
+0001c520: 6265 6c29 0a20 2020 2020 2020 2020 2020  bel).           
+0001c530: 2020 2020 206c 6162 656c 203d 2061 782e       label = ax.
+0001c540: 7365 745f 786c 6162 656c 2827 4343 4127  set_xlabel('CCA'
+0001c550: 202b 2073 7472 2863 635f 6178 6973 3229   + str(cc_axis2)
+0001c560: 2c20 666f 6e74 7369 7a65 203d 2039 290a  , fontsize = 9).
+0001c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c580: 6178 2e78 6178 6973 2e73 6574 5f6c 6162  ax.xaxis.set_lab
+0001c590: 656c 5f63 6f6f 7264 7328 302e 352c 202d  el_coords(0.5, -
+0001c5a0: 302e 3032 290a 2020 2020 2020 2020 2020  0.02).          
+0001c5b0: 2020 2020 2020 6c61 6265 6c20 3d20 6178        label = ax
+0001c5c0: 2e73 6574 5f79 6c61 6265 6c28 2743 4341  .set_ylabel('CCA
+0001c5d0: 2720 2b20 7374 7228 6363 5f61 7869 7331  ' + str(cc_axis1
+0001c5e0: 292c 2066 6f6e 7473 697a 6520 3d20 3929  ), fontsize = 9)
+0001c5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c600: 2061 782e 7961 7869 732e 7365 745f 6c61   ax.yaxis.set_la
+0001c610: 6265 6c5f 636f 6f72 6473 282d 302e 3032  bel_coords(-0.02
+0001c620: 2c20 302e 3535 290a 0a20 2020 2020 2020  , 0.55)..       
+0001c630: 2020 2020 2020 2020 2023 6d61 6b65 2069           #make i
+0001c640: 6e74 6f20 626f 780a 2020 2020 2020 2020  nto box.        
+0001c650: 2020 2020 2020 2020 6178 2e73 6574 5f61          ax.set_a
+0001c660: 7370 6563 7428 2765 7175 616c 272c 2061  spect('equal', a
+0001c670: 646a 7573 7461 626c 653d 2762 6f78 2729  djustable='box')
+0001c680: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c690: 2020 234d 6f76 6520 6c65 6674 2079 2d61    #Move left y-a
+0001c6a0: 7869 7320 2620 626f 7474 6f6d 2078 2d61  xis & bottom x-a
+0001c6b0: 7869 7320 746f 2063 656e 7465 722c 2070  xis to center, p
+0001c6c0: 6173 7369 6e67 2074 6872 7520 2830 2c30  assing thru (0,0
+0001c6d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001c6e0: 2020 6178 2e73 7069 6e65 735b 276c 6566    ax.spines['lef
+0001c6f0: 7427 5d2e 7365 745f 706f 7369 7469 6f6e  t'].set_position
+0001c700: 2827 6365 6e74 6572 2729 0a20 2020 2020  ('center').     
+0001c710: 2020 2020 2020 2020 2020 2061 782e 7370             ax.sp
+0001c720: 696e 6573 5b27 626f 7474 6f6d 275d 2e73  ines['bottom'].s
+0001c730: 6574 5f70 6f73 6974 696f 6e28 2763 656e  et_position('cen
+0001c740: 7465 7227 290a 0a20 2020 2020 2020 2020  ter')..         
+0001c750: 2020 2020 2020 2023 6368 616e 6765 2063         #change c
+0001c760: 6f6c 6f72 732f 7265 6d6f 7665 2064 6566  olors/remove def
+0001c770: 6175 6c74 2061 7869 730a 2020 2020 2020  ault axis.      
+0001c780: 2020 2020 2020 2020 2020 6178 636f 6c6f            axcolo
+0001c790: 7220 3d20 276e 6f6e 6527 0a20 2020 2020  r = 'none'.     
+0001c7a0: 2020 2020 2020 2020 2020 2061 782e 7370             ax.sp
+0001c7b0: 696e 6573 5b27 6c65 6674 275d 2e73 6574  ines['left'].set
+0001c7c0: 5f63 6f6c 6f72 2861 7863 6f6c 6f72 290a  _color(axcolor).
+0001c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7e0: 6178 2e73 7069 6e65 735b 2762 6f74 746f  ax.spines['botto
+0001c7f0: 6d27 5d2e 7365 745f 636f 6c6f 7228 6178  m'].set_color(ax
+0001c800: 636f 6c6f 7229 0a20 2020 2020 2020 2020  color).         
+0001c810: 2020 2020 2020 2061 782e 7370 696e 6573         ax.spines
+0001c820: 5b27 7269 6768 7427 5d2e 7365 745f 636f  ['right'].set_co
+0001c830: 6c6f 7228 6178 636f 6c6f 7229 0a20 2020  lor(axcolor).   
+0001c840: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
+0001c850: 7370 696e 6573 5b27 746f 7027 5d2e 7365  spines['top'].se
+0001c860: 745f 636f 6c6f 7228 6178 636f 6c6f 7229  t_color(axcolor)
+0001c870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c880: 2061 782e 7469 636b 5f70 6172 616d 7328   ax.tick_params(
+0001c890: 6178 6973 203d 2027 7827 2c20 636f 6c6f  axis = 'x', colo
+0001c8a0: 7273 3d61 7863 6f6c 6f72 290a 2020 2020  rs=axcolor).    
+0001c8b0: 2020 2020 2020 2020 2020 2020 6178 2e74              ax.t
+0001c8c0: 6963 6b5f 7061 7261 6d73 2861 7869 7320  ick_params(axis 
+0001c8d0: 3d20 2779 272c 2063 6f6c 6f72 733d 6178  = 'y', colors=ax
+0001c8e0: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
+0001c8f0: 2020 2020 2020 2020 6178 2e79 6178 6973          ax.yaxis
+0001c900: 2e6c 6162 656c 2e73 6574 5f63 6f6c 6f72  .label.set_color
+0001c910: 2827 6772 6179 2729 0a20 2020 2020 2020  ('gray').       
+0001c920: 2020 2020 2020 2020 2061 782e 7861 7869           ax.xaxi
+0001c930: 732e 6c61 6265 6c2e 7365 745f 636f 6c6f  s.label.set_colo
+0001c940: 7228 2767 7261 7927 290a 0a20 2020 2020  r('gray')..     
+0001c950: 2020 2020 2020 2020 2020 2023 6c65 6765             #lege
+0001c960: 6e64 730a 2020 2020 2020 2020 2020 2020  nds.            
+0001c970: 2020 2020 6966 206e 203d 3d20 323a 0a20      if n == 2:. 
+0001c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c990: 2020 2061 782e 6c65 6765 6e64 286c 6f63     ax.legend(loc
+0001c9a0: 203d 2022 7570 7065 7220 6c65 6674 222c   = "upper left",
+0001c9b0: 2062 626f 785f 746f 5f61 6e63 686f 723d   bbox_to_anchor=
+0001c9c0: 2831 2e33 2c20 312e 3035 2929 0a20 2020  (1.3, 1.05)).   
+0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9e0: 2070 6c74 2e63 6f6c 6f72 6261 7228 636d   plt.colorbar(cm
+0001c9f0: 6170 5f73 6361 742c 206c 6162 656c 3d22  ap_scat, label="
+0001ca00: 656e 7622 290a 2020 2020 2020 2020 2020  env").          
+0001ca10: 2020 6669 672e 7368 6f77 2829 0a0a 2020    fig.show()..  
+0001ca20: 2020 2020 2020 7265 7475 726e 2063 6361        return cca
+0001ca30: 5f64 6963 740a 0a0a 2020 2020 2320 6d65  _dict...    # me
+0001ca40: 7468 6f64 2066 6f72 2070 6c6f 7474 696e  thod for plottin
+0001ca50: 6720 7468 6520 7370 6563 6965 7320 286f  g the species (o
+0001ca60: 7220 6120 7375 6273 6574 206f 6620 6974  r a subset of it
+0001ca70: 7320 696e 6469 7669 6475 616c 732c 2062  s individuals, b
+0001ca80: 7920 4944 290a 2020 2020 2320 6f6e 2074  y ID).    # on t
+0001ca90: 6f70 206f 6620 6120 6c61 7965 7220 286f  op of a layer (o
+0001caa0: 7220 6c61 6e64 7363 6170 6529 0a20 2020  r landscape).   
+0001cab0: 2064 6566 205f 706c 6f74 2873 656c 662c   def _plot(self,
+0001cac0: 206c 7972 5f6e 756d 3d4e 6f6e 652c 206c   lyr_num=None, l
+0001cad0: 616e 643d 4e6f 6e65 2c20 6869 6465 5f6c  and=None, hide_l
+0001cae0: 616e 643d 4661 6c73 652c 2069 6e64 6976  and=False, indiv
+0001caf0: 6964 733d 4e6f 6e65 2c0a 2020 2020 2020  ids=None,.      
+0001cb00: 2020 2020 2020 2020 7465 7874 3d46 616c          text=Fal
+0001cb10: 7365 2c20 636f 6c6f 723d 2762 6c61 636b  se, color='black
+0001cb20: 272c 2065 6467 655f 636f 6c6f 723d 2766  ', edge_color='f
+0001cb30: 6163 6527 2c20 7465 7874 5f63 6f6c 6f72  ace', text_color
+0001cb40: 3d27 626c 6163 6b27 2c0a 2020 2020 2020  ='black',.      
+0001cb50: 2020 2020 2020 2020 6362 6172 3d54 7275          cbar=Tru
+0001cb60: 652c 2073 697a 653d 3235 2c20 7465 7874  e, size=25, text
+0001cb70: 5f73 697a 653d 392c 206c 616e 645f 636d  _size=9, land_cm
+0001cb80: 6170 3d4e 6f6e 652c 2070 745f 636d 6170  ap=None, pt_cmap
+0001cb90: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0001cba0: 2020 2020 2061 6c70 6861 3d46 616c 7365       alpha=False
+0001cbb0: 2c20 7a6f 6f6d 5f77 6964 7468 3d4e 6f6e  , zoom_width=Non
+0001cbc0: 652c 2078 3d4e 6f6e 652c 2079 3d4e 6f6e  e, x=None, y=Non
+0001cbd0: 652c 2076 6d69 6e3d 4e6f 6e65 2c0a 2020  e, vmin=None,.  
+0001cbe0: 2020 2020 2020 2020 2020 2020 766d 6178              vmax
+0001cbf0: 3d4e 6f6e 652c 2074 6963 6b73 3d4e 6f6e  =None, ticks=Non
+0001cc00: 652c 206d 6173 6b5f 7261 7374 3d4e 6f6e  e, mask_rast=Non
+0001cc10: 652c 2061 6e69 6d61 7465 3d46 616c 7365  e, animate=False
+0001cc20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001cc30: 6365 6c6c 5f63 6f6f 7264 733d 4661 6c73  cell_coords=Fals
+0001cc40: 6529 3a0a 2020 2020 2020 2020 2320 636f  e):.        # co
+0001cc50: 6e76 6572 7420 696e 6469 7669 6473 2074  nvert individs t
+0001cc60: 6f20 6120 6c69 7374 2028 696e 2063 6173  o a list (in cas
+0001cc70: 6520 636f 6d65 7320 696e 2061 7320 6120  e comes in as a 
+0001cc80: 6e75 6d70 7920 6172 7261 7929 0a20 2020  numpy array).   
+0001cc90: 2020 2020 2069 6620 696e 6469 7669 6473       if individs
+0001cca0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0001ccb0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0001ccc0: 696e 6469 7669 6473 2c20 6c69 7374 293a  individs, list):
+0001ccd0: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+0001cce0: 6976 6964 7320 3d20 6c69 7374 2869 6e64  ivids = list(ind
+0001ccf0: 6976 6964 7329 0a20 2020 2020 2020 2023  ivids).        #
+0001cd00: 2067 6574 2063 6f6f 7264 730a 2020 2020   get coords.    
+0001cd10: 2020 2020 636f 6f72 6473 203d 2073 656c      coords = sel
+0001cd20: 662e 5f67 6574 5f70 6c6f 745f 636f 6f72  f._get_plot_coor
+0001cd30: 6473 2869 6e64 6976 6964 733d 696e 6469  ds(individs=indi
+0001cd40: 7669 6473 2c0a 2020 2020 2020 2020 2020  vids,.          
+0001cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd60: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0001cd70: 6c5f 636f 6f72 6473 3d63 656c 6c5f 636f  l_coords=cell_co
+0001cd80: 6f72 6473 290a 2020 2020 2020 2020 2320  ords).        # 
+0001cd90: 6765 7420 7465 7874 0a20 2020 2020 2020  get text.       
+0001cda0: 2069 6620 7465 7874 3a0a 2020 2020 2020   if text:.      
+0001cdb0: 2020 2020 2020 6966 2069 6e64 6976 6964        if individ
+0001cdc0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+0001cdd0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+0001cde0: 3d20 5b2a 7365 6c66 5d0a 2020 2020 2020  = [*self].      
+0001cdf0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001ce00: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0001ce10: 203d 2069 6e64 6976 6964 730a 2020 2020   = individs.    
+0001ce20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001ce30: 2020 2020 2020 7465 7874 203d 204e 6f6e        text = Non
+0001ce40: 650a 2020 2020 2020 2020 2320 7365 7420  e.        # set 
+0001ce50: 7468 6520 706c 745f 6c69 6d73 0a20 2020  the plt_lims.   
+0001ce60: 2020 2020 2070 6c74 5f6c 696d 7320 3d20       plt_lims = 
+0001ce70: 7669 7a2e 5f67 6574 5f70 6c74 5f6c 696d  viz._get_plt_lim
+0001ce80: 7328 6c61 6e64 2c20 782c 2079 2c20 7a6f  s(land, x, y, zo
+0001ce90: 6f6d 5f77 6964 7468 290a 2020 2020 2020  om_width).      
+0001cea0: 2020 2320 706c 6f74 2074 6865 206c 6179    # plot the lay
+0001ceb0: 6572 2873 290a 2020 2020 2020 2020 6966  er(s).        if
+0001cec0: 2068 6964 655f 6c61 6e64 3a0a 2020 2020   hide_land:.    
+0001ced0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+0001cee0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001cef0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+0001cf00: 206c 6179 6572 7327 2076 6d69 6e20 616e   layers' vmin an
+0001cf10: 6420 766d 6178 2076 616c 7565 732c 2069  d vmax values, i
+0001cf20: 6620 616e 7920 6f66 2074 6865 206c 6179  f any of the lay
+0001cf30: 6572 7320 746f 0a20 2020 2020 2020 2020  ers to.         
+0001cf40: 2020 2023 2062 6520 706c 6f74 7465 6420     # be plotted 
+0001cf50: 6861 7320 6120 6368 616e 6765 2065 7665  has a change eve
+0001cf60: 6e74 0a20 2020 2020 2020 2020 2020 2069  nt.            i
+0001cf70: 6620 2828 6c79 725f 6e75 6d20 6973 204e  f ((lyr_num is N
+0001cf80: 6f6e 6520 616e 6420 6c61 6e64 2e5f 6368  one and land._ch
+0001cf90: 616e 6765 7220 6973 206e 6f74 204e 6f6e  anger is not Non
+0001cfa0: 6529 206f 720a 2020 2020 2020 2020 2020  e) or.          
+0001cfb0: 2020 2020 2020 286c 616e 642e 5f63 6861        (land._cha
+0001cfc0: 6e67 6572 2069 7320 6e6f 7420 4e6f 6e65  nger is not None
+0001cfd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cfe0: 2020 616e 6420 6c79 725f 6e75 6d20 696e    and lyr_num in
+0001cff0: 205b 2a6c 616e 642e 5f63 6861 6e67 6572   [*land._changer
+0001d000: 2e63 6861 6e67 655f 696e 666f 5d29 293a  .change_info])):
+0001d010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d020: 2069 6620 6c79 725f 6e75 6d20 6973 204e   if lyr_num is N
+0001d030: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001d040: 2020 2020 2020 2020 206c 616e 645f 766d           land_vm
+0001d050: 696e 203d 205b 6c79 722e 5f73 6361 6c65  in = [lyr._scale
+0001d060: 5f6d 696e 2066 6f72 206c 7972 2069 6e20  _min for lyr in 
+0001d070: 6c61 6e64 2e76 616c 7565 7328 295d 0a20  land.values()]. 
+0001d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d090: 2020 206c 616e 645f 766d 6178 203d 205b     land_vmax = [
+0001d0a0: 6c79 722e 5f73 6361 6c65 5f6d 6178 2066  lyr._scale_max f
+0001d0b0: 6f72 206c 7972 2069 6e20 6c61 6e64 2e76  or lyr in land.v
+0001d0c0: 616c 7565 7328 295d 0a20 2020 2020 2020  alues()].       
+0001d0d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 0001d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0f0: 206c 616e 645f 766d 6178 203d 205b 6c61   land_vmax = [la
-0001d100: 6e64 5b6c 7972 5f6e 756d 5d2e 5f73 6361  nd[lyr_num]._sca
-0001d110: 6c65 5f6d 6178 5d0a 2020 2020 2020 2020  le_max].        
-0001d120: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001d130: 2020 2020 2020 2020 2020 6c61 6e64 5f76            land_v
-0001d140: 6d69 6e20 3d20 6c61 6e64 5f76 6d61 7820  min = land_vmax 
-0001d150: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0001d160: 2020 2076 697a 2e5f 706c 6f74 5f72 6173     viz._plot_ras
-0001d170: 7465 7273 286c 616e 642c 206c 7972 5f6e  ters(land, lyr_n
-0001d180: 756d 3d6c 7972 5f6e 756d 2c0a 2020 2020  um=lyr_num,.    
-0001d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1a0: 2020 2020 2020 2020 2020 6362 6172 3d63            cbar=c
-0001d1b0: 6261 722c 2063 6d61 703d 6c61 6e64 5f63  bar, cmap=land_c
-0001d1c0: 6d61 702c 2070 6c74 5f6c 696d 733d 706c  map, plt_lims=pl
-0001d1d0: 745f 6c69 6d73 2c0a 2020 2020 2020 2020  t_lims,.        
-0001d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1f0: 2020 2020 2020 7469 636b 733d 7469 636b        ticks=tick
-0001d200: 732c 206d 6173 6b5f 7261 7374 3d6d 6173  s, mask_rast=mas
-0001d210: 6b5f 7261 7374 2c0a 2020 2020 2020 2020  k_rast,.        
+0001d0f0: 2020 206c 616e 645f 766d 696e 203d 205b     land_vmin = [
+0001d100: 6c61 6e64 5b6c 7972 5f6e 756d 5d2e 5f73  land[lyr_num]._s
+0001d110: 6361 6c65 5f6d 696e 5d0a 2020 2020 2020  cale_min].      
+0001d120: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0001d130: 6e64 5f76 6d61 7820 3d20 5b6c 616e 645b  nd_vmax = [land[
+0001d140: 6c79 725f 6e75 6d5d 2e5f 7363 616c 655f  lyr_num]._scale_
+0001d150: 6d61 785d 0a20 2020 2020 2020 2020 2020  max].           
+0001d160: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001d170: 2020 2020 2020 206c 616e 645f 766d 696e         land_vmin
+0001d180: 203d 206c 616e 645f 766d 6178 203d 204e   = land_vmax = N
+0001d190: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0001d1a0: 7669 7a2e 5f70 6c6f 745f 7261 7374 6572  viz._plot_raster
+0001d1b0: 7328 6c61 6e64 2c20 6c79 725f 6e75 6d3d  s(land, lyr_num=
+0001d1c0: 6c79 725f 6e75 6d2c 0a20 2020 2020 2020  lyr_num,.       
+0001d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d1e0: 2020 2020 2020 2063 6261 723d 6362 6172         cbar=cbar
+0001d1f0: 2c20 636d 6170 3d6c 616e 645f 636d 6170  , cmap=land_cmap
+0001d200: 2c20 706c 745f 6c69 6d73 3d70 6c74 5f6c  , plt_lims=plt_l
+0001d210: 696d 732c 0a20 2020 2020 2020 2020 2020  ims,.           
 0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d230: 2020 2020 2020 766d 696e 3d6c 616e 645f        vmin=land_
-0001d240: 766d 696e 2c20 766d 6178 3d6c 616e 645f  vmin, vmax=land_
-0001d250: 766d 6178 290a 2020 2020 2020 2020 2320  vmax).        # 
-0001d260: 616e 6420 706c 6f74 2074 6865 2069 6e64  and plot the ind
-0001d270: 6976 6964 7561 6c73 0a20 2020 2020 2020  ividuals.       
-0001d280: 2070 6f69 6e74 7320 3d20 7669 7a2e 5f70   points = viz._p
-0001d290: 6c6f 745f 706f 696e 7473 2863 6f6f 7264  lot_points(coord
-0001d2a0: 732c 206c 7972 5f6e 756d 3d6c 7972 5f6e  s, lyr_num=lyr_n
-0001d2b0: 756d 2c20 636f 6c6f 723d 636f 6c6f 722c  um, color=color,
-0001d2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2e0: 2020 2065 6467 655f 636f 6c6f 723d 6564     edge_color=ed
-0001d2f0: 6765 5f63 6f6c 6f72 2c0a 2020 2020 2020  ge_color,.      
+0001d230: 2020 2074 6963 6b73 3d74 6963 6b73 2c20     ticks=ticks, 
+0001d240: 6d61 736b 5f72 6173 743d 6d61 736b 5f72  mask_rast=mask_r
+0001d250: 6173 742c 0a20 2020 2020 2020 2020 2020  ast,.           
+0001d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d270: 2020 2076 6d69 6e3d 6c61 6e64 5f76 6d69     vmin=land_vmi
+0001d280: 6e2c 2076 6d61 783d 6c61 6e64 5f76 6d61  n, vmax=land_vma
+0001d290: 7829 0a20 2020 2020 2020 2023 2061 6e64  x).        # and
+0001d2a0: 2070 6c6f 7420 7468 6520 696e 6469 7669   plot the indivi
+0001d2b0: 6475 616c 730a 2020 2020 2020 2020 706f  duals.        po
+0001d2c0: 696e 7473 203d 2076 697a 2e5f 706c 6f74  ints = viz._plot
+0001d2d0: 5f70 6f69 6e74 7328 636f 6f72 6473 2c20  _points(coords, 
+0001d2e0: 6c79 725f 6e75 6d3d 6c79 725f 6e75 6d2c  lyr_num=lyr_num,
+0001d2f0: 2063 6f6c 6f72 3d63 6f6c 6f72 2c0a 2020   color=color,.  
 0001d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d310: 2020 2020 2020 2020 2020 2020 7465 7874              text
-0001d320: 5f63 6f6c 6f72 3d74 6578 745f 636f 6c6f  _color=text_colo
-0001d330: 722c 2073 697a 653d 7369 7a65 2c0a 2020  r, size=size,.  
+0001d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d320: 6564 6765 5f63 6f6c 6f72 3d65 6467 655f  edge_color=edge_
+0001d330: 636f 6c6f 722c 0a20 2020 2020 2020 2020  color,.         
 0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d360: 7465 7874 5f73 697a 653d 7465 7874 5f73  text_size=text_s
-0001d370: 697a 652c 2061 6c70 6861 3d61 6c70 6861  ize, alpha=alpha
-0001d380: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3a0: 2020 2020 7465 7874 3d74 6578 742c 2070      text=text, p
-0001d3b0: 6c74 5f6c 696d 733d 706c 745f 6c69 6d73  lt_lims=plt_lims
-0001d3c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001d350: 2020 2020 2020 2020 2074 6578 745f 636f           text_co
+0001d360: 6c6f 723d 7465 7874 5f63 6f6c 6f72 2c20  lor=text_color, 
+0001d370: 7369 7a65 3d73 697a 652c 0a20 2020 2020  size=size,.     
+0001d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d390: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0001d3a0: 745f 7369 7a65 3d74 6578 745f 7369 7a65  t_size=text_size
+0001d3b0: 2c20 616c 7068 613d 616c 7068 612c 0a20  , alpha=alpha,. 
+0001d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3e0: 2020 2020 7074 5f63 6d61 703d 7074 5f63      pt_cmap=pt_c
-0001d3f0: 6d61 702c 2076 6d69 6e3d 766d 696e 2c20  map, vmin=vmin, 
-0001d400: 766d 6178 3d76 6d61 782c 0a20 2020 2020  vmax=vmax,.     
+0001d3e0: 2074 6578 743d 7465 7874 2c20 706c 745f   text=text, plt_
+0001d3f0: 6c69 6d73 3d70 6c74 5f6c 696d 732c 0a20  lims=plt_lims,. 
+0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d420: 2020 2020 2020 2020 2020 2020 2061 6e69               ani
-0001d430: 6d61 7465 3d61 6e69 6d61 7465 290a 2020  mate=animate).  
-0001d440: 2020 2020 2020 7265 7475 726e 2070 6f69        return poi
-0001d450: 6e74 730a 0a0a 2020 2020 236d 6574 686f  nts...    #metho
-0001d460: 6420 666f 7220 706c 6f74 7469 6e67 2074  d for plotting t
-0001d470: 6865 2073 7065 6369 6573 206f 6e20 746f  he species on to
-0001d480: 7020 6f66 2069 7473 2065 7374 696d 6174  p of its estimat
-0001d490: 6564 0a20 2020 2023 7370 6563 6965 732d  ed.    #species-
-0001d4a0: 6465 6e73 6974 7920 7261 7374 6572 0a20  density raster. 
-0001d4b0: 2020 2064 6566 205f 706c 6f74 5f64 656e     def _plot_den
-0001d4c0: 7369 7479 2873 656c 662c 206c 616e 642c  sity(self, land,
-0001d4d0: 206e 6f72 6d61 6c69 7a65 3d46 616c 7365   normalize=False
-0001d4e0: 2c20 696e 6469 7669 6473 3d4e 6f6e 652c  , individs=None,
-0001d4f0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-0001d500: 743d 4661 6c73 652c 2063 6f6c 6f72 3d27  t=False, color='
-0001d510: 626c 6163 6b27 2c20 6564 6765 5f63 6f6c  black', edge_col
-0001d520: 6f72 3d27 6661 6365 272c 0a20 2020 2020  or='face',.     
-0001d530: 2020 2020 2020 2074 6578 745f 636f 6c6f         text_colo
-0001d540: 723d 2762 6c61 636b 272c 2073 697a 653d  r='black', size=
-0001d550: 3235 2c20 7465 7874 5f73 697a 6520 3d20  25, text_size = 
-0001d560: 392c 0a20 2020 2020 2020 2020 2020 2061  9,.            a
-0001d570: 6c70 6861 3d30 2e35 2c20 7a6f 6f6d 5f77  lpha=0.5, zoom_w
-0001d580: 6964 7468 3d4e 6f6e 652c 2078 3d4e 6f6e  idth=None, x=Non
-0001d590: 652c 2079 3d4e 6f6e 652c 2074 6963 6b73  e, y=None, ticks
-0001d5a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-0001d5b0: 2020 206d 6173 6b5f 7261 7374 3d4e 6f6e     mask_rast=Non
-0001d5c0: 6529 3a0a 2020 2020 2020 2020 6173 7365  e):.        asse
-0001d5d0: 7274 2074 7970 6528 6e6f 726d 616c 697a  rt type(normaliz
-0001d5e0: 6529 2069 7320 626f 6f6c 2c20 2822 5468  e) is bool, ("Th
-0001d5f0: 6520 276e 6f72 6d61 6c69 7a65 2720 6172  e 'normalize' ar
-0001d600: 6775 6d65 6e74 2074 616b 6573 2022 0a20  gument takes ". 
-0001d610: 2020 2020 2020 2020 2020 2022 6120 626f             "a bo
-0001d620: 6f6c 6561 6e20 7661 6c75 652e 5c6e 2229  olean value.\n")
-0001d630: 0a20 2020 2020 2020 2023 7570 6461 7465  .        #update
-0001d640: 2074 6865 2073 7065 6369 6573 2720 636f   the species' co
-0001d650: 6f72 6469 6e61 7465 7320 616e 6420 6365  ordinates and ce
-0001d660: 6c6c 732c 2069 6e20 6361 7365 2069 7420  lls, in case it 
-0001d670: 6861 736e 2774 0a20 2020 2020 2020 2023  hasn't.        #
-0001d680: 6265 656e 2075 7064 6174 6564 2073 696e  been updated sin
-0001d690: 6365 2073 6f6d 6520 696e 7465 726e 616c  ce some internal
-0001d6a0: 206f 7220 6d61 6e75 616c 2063 6861 6e67   or manual chang
-0001d6b0: 6573 2069 6e20 706f 7075 6c61 7469 6f6e  es in population
-0001d6c0: 2d73 697a 650a 2020 2020 2020 2020 2368  -size.        #h
-0001d6d0: 6176 6520 6f63 6375 7272 6564 0a20 2020  ave occurred.   
-0001d6e0: 2020 2020 2073 656c 662e 5f73 6574 5f63       self._set_c
-0001d6f0: 6f6f 7264 735f 616e 645f 6365 6c6c 7328  oords_and_cells(
-0001d700: 290a 2020 2020 2020 2020 6465 6e73 203d  ).        dens =
-0001d710: 2073 656c 662e 5f63 616c 635f 6465 6e73   self._calc_dens
-0001d720: 6974 7928 6e6f 726d 616c 697a 6520 3d20  ity(normalize = 
-0001d730: 6e6f 726d 616c 697a 6529 0a20 2020 2020  normalize).     
-0001d740: 2020 2070 6c74 5f6c 696d 7320 3d20 7669     plt_lims = vi
-0001d750: 7a2e 5f67 6574 5f70 6c74 5f6c 696d 7328  z._get_plt_lims(
-0001d760: 6c61 6e64 2c20 782c 2079 2c20 7a6f 6f6d  land, x, y, zoom
-0001d770: 5f77 6964 7468 290a 2020 2020 2020 2020  _width).        
-0001d780: 6966 206e 6f72 6d61 6c69 7a65 3a0a 2020  if normalize:.  
-0001d790: 2020 2020 2020 2020 2020 7669 7a2e 5f70            viz._p
-0001d7a0: 6c6f 745f 7261 7374 6572 7328 6465 6e73  lot_rasters(dens
-0001d7b0: 2c20 706c 745f 6c69 6d73 203d 2070 6c74  , plt_lims = plt
-0001d7c0: 5f6c 696d 732c 206c 7972 5f6e 616d 6520  _lims, lyr_name 
-0001d7d0: 3d20 2764 656e 7369 7479 272c 0a20 2020  = 'density',.   
-0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7f0: 2020 2020 2020 2020 2020 2074 6963 6b73             ticks
-0001d800: 3d74 6963 6b73 2c20 6d61 736b 5f72 6173  =ticks, mask_ras
-0001d810: 743d 6d61 736b 5f72 6173 7429 0a20 2020  t=mask_rast).   
-0001d820: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001d830: 2020 2020 2020 2076 697a 2e5f 706c 6f74         viz._plot
-0001d840: 5f72 6173 7465 7273 2864 656e 732c 2070  _rasters(dens, p
-0001d850: 6c74 5f6c 696d 7320 3d20 706c 745f 6c69  lt_lims = plt_li
-0001d860: 6d73 2c20 766d 6178 203d 2064 656e 732e  ms, vmax = dens.
-0001d870: 6d61 7828 292c 0a20 2020 2020 2020 2020  max(),.         
-0001d880: 2020 2020 2020 206c 7972 5f6e 616d 6520         lyr_name 
-0001d890: 3d20 2764 656e 7369 7479 272c 2074 6963  = 'density', tic
-0001d8a0: 6b73 3d74 6963 6b73 2c20 6d61 736b 5f72  ks=ticks, mask_r
-0001d8b0: 6173 743d 6d61 736b 5f72 6173 7429 0a20  ast=mask_rast). 
-0001d8c0: 2020 2020 2020 2073 656c 662e 5f70 6c6f         self._plo
-0001d8d0: 7428 6869 6465 5f6c 616e 643d 5472 7565  t(hide_land=True
-0001d8e0: 2c20 696e 6469 7669 6473 203d 2069 6e64  , individs = ind
-0001d8f0: 6976 6964 732c 2074 6578 7420 3d20 7465  ivids, text = te
-0001d900: 7874 2c0a 2020 2020 2020 2020 2020 2020  xt,.            
-0001d910: 636f 6c6f 723d 636f 6c6f 722c 2065 6467  color=color, edg
-0001d920: 655f 636f 6c6f 7220 3d20 6564 6765 5f63  e_color = edge_c
-0001d930: 6f6c 6f72 2c20 7465 7874 5f63 6f6c 6f72  olor, text_color
-0001d940: 203d 2074 6578 745f 636f 6c6f 722c 0a20   = text_color,. 
-0001d950: 2020 2020 2020 2020 2020 2073 697a 653d             size=
-0001d960: 7369 7a65 2c20 7465 7874 5f73 697a 6520  size, text_size 
-0001d970: 3d20 7465 7874 5f73 697a 652c 2061 6c70  = text_size, alp
-0001d980: 6861 3d61 6c70 6861 2c0a 2020 2020 2020  ha=alpha,.      
-0001d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9a0: 2020 2020 2020 2020 2020 2020 2020 7a6f                zo
-0001d9b0: 6f6d 5f77 6964 7468 203d 207a 6f6f 6d5f  om_width = zoom_
-0001d9c0: 7769 6474 682c 2078 203d 2078 2c20 7920  width, x = x, y 
-0001d9d0: 3d20 7929 0a0a 0a20 2020 2023 206d 6574  = y)...    # met
-0001d9e0: 686f 6420 666f 7220 706c 6f74 7469 6e67  hod for plotting
-0001d9f0: 2069 6e64 6976 6964 7561 6c73 2063 6f6c   individuals col
-0001da00: 6f72 6564 2062 7920 7468 6569 7220 6765  ored by their ge
-0001da10: 6e6f 7479 7065 2061 7420 6120 6c6f 6375  notype at a locu
-0001da20: 730a 2020 2020 6465 6620 5f70 6c6f 745f  s.    def _plot_
-0001da30: 6765 6e6f 7479 7065 2873 656c 662c 206c  genotype(self, l
-0001da40: 6f63 7573 2c20 6c79 725f 6e75 6d3d 4e6f  ocus, lyr_num=No
-0001da50: 6e65 2c20 6c61 6e64 3d4e 6f6e 652c 2069  ne, land=None, i
-0001da60: 6e64 6976 6964 733d 4e6f 6e65 2c0a 2020  ndivids=None,.  
-0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da80: 2020 2020 2074 6578 743d 4661 6c73 652c       text=False,
-0001da90: 2073 697a 653d 3235 2c20 7465 7874 5f73   size=25, text_s
-0001daa0: 697a 6520 3d20 392c 2065 6467 655f 636f  ize = 9, edge_co
-0001dab0: 6c6f 723d 2762 6c61 636b 272c 0a20 2020  lor='black',.   
-0001dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dad0: 2020 2020 7465 7874 5f63 6f6c 6f72 3d27      text_color='
-0001dae0: 626c 6163 6b27 2c20 6362 6172 3d54 7275  black', cbar=Tru
-0001daf0: 652c 2061 6c70 6861 3d31 2c0a 2020 2020  e, alpha=1,.    
+0001d420: 2070 745f 636d 6170 3d70 745f 636d 6170   pt_cmap=pt_cmap
+0001d430: 2c20 766d 696e 3d76 6d69 6e2c 2076 6d61  , vmin=vmin, vma
+0001d440: 783d 766d 6178 2c0a 2020 2020 2020 2020  x=vmax,.        
+0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d460: 2020 2020 2020 2020 2020 616e 696d 6174            animat
+0001d470: 653d 616e 696d 6174 6529 0a20 2020 2020  e=animate).     
+0001d480: 2020 2072 6574 7572 6e20 706f 696e 7473     return points
+0001d490: 0a0a 0a20 2020 2023 6d65 7468 6f64 2066  ...    #method f
+0001d4a0: 6f72 2070 6c6f 7474 696e 6720 7468 6520  or plotting the 
+0001d4b0: 7370 6563 6965 7320 6f6e 2074 6f70 206f  species on top o
+0001d4c0: 6620 6974 7320 6573 7469 6d61 7465 640a  f its estimated.
+0001d4d0: 2020 2020 2373 7065 6369 6573 2d64 656e      #species-den
+0001d4e0: 7369 7479 2072 6173 7465 720a 2020 2020  sity raster.    
+0001d4f0: 6465 6620 5f70 6c6f 745f 6465 6e73 6974  def _plot_densit
+0001d500: 7928 7365 6c66 2c20 6c61 6e64 2c20 6e6f  y(self, land, no
+0001d510: 726d 616c 697a 653d 4661 6c73 652c 2069  rmalize=False, i
+0001d520: 6e64 6976 6964 733d 4e6f 6e65 2c0a 2020  ndivids=None,.  
+0001d530: 2020 2020 2020 2020 2020 7465 7874 3d46            text=F
+0001d540: 616c 7365 2c20 636f 6c6f 723d 2762 6c61  alse, color='bla
+0001d550: 636b 272c 2065 6467 655f 636f 6c6f 723d  ck', edge_color=
+0001d560: 2766 6163 6527 2c0a 2020 2020 2020 2020  'face',.        
+0001d570: 2020 2020 7465 7874 5f63 6f6c 6f72 3d27      text_color='
+0001d580: 626c 6163 6b27 2c20 7369 7a65 3d32 352c  black', size=25,
+0001d590: 2074 6578 745f 7369 7a65 203d 2039 2c0a   text_size = 9,.
+0001d5a0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+0001d5b0: 613d 302e 352c 207a 6f6f 6d5f 7769 6474  a=0.5, zoom_widt
+0001d5c0: 683d 4e6f 6e65 2c20 783d 4e6f 6e65 2c20  h=None, x=None, 
+0001d5d0: 793d 4e6f 6e65 2c20 7469 636b 733d 4e6f  y=None, ticks=No
+0001d5e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0001d5f0: 6d61 736b 5f72 6173 743d 4e6f 6e65 293a  mask_rast=None):
+0001d600: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0001d610: 7479 7065 286e 6f72 6d61 6c69 7a65 2920  type(normalize) 
+0001d620: 6973 2062 6f6f 6c2c 2028 2254 6865 2027  is bool, ("The '
+0001d630: 6e6f 726d 616c 697a 6527 2061 7267 756d  normalize' argum
+0001d640: 656e 7420 7461 6b65 7320 220a 2020 2020  ent takes ".    
+0001d650: 2020 2020 2020 2020 2261 2062 6f6f 6c65          "a boole
+0001d660: 616e 2076 616c 7565 2e5c 6e22 290a 2020  an value.\n").  
+0001d670: 2020 2020 2020 2375 7064 6174 6520 7468        #update th
+0001d680: 6520 7370 6563 6965 7327 2063 6f6f 7264  e species' coord
+0001d690: 696e 6174 6573 2061 6e64 2063 656c 6c73  inates and cells
+0001d6a0: 2c20 696e 2063 6173 6520 6974 2068 6173  , in case it has
+0001d6b0: 6e27 740a 2020 2020 2020 2020 2362 6565  n't.        #bee
+0001d6c0: 6e20 7570 6461 7465 6420 7369 6e63 6520  n updated since 
+0001d6d0: 736f 6d65 2069 6e74 6572 6e61 6c20 6f72  some internal or
+0001d6e0: 206d 616e 7561 6c20 6368 616e 6765 7320   manual changes 
+0001d6f0: 696e 2070 6f70 756c 6174 696f 6e2d 7369  in population-si
+0001d700: 7a65 0a20 2020 2020 2020 2023 6861 7665  ze.        #have
+0001d710: 206f 6363 7572 7265 640a 2020 2020 2020   occurred.      
+0001d720: 2020 7365 6c66 2e5f 7365 745f 636f 6f72    self._set_coor
+0001d730: 6473 5f61 6e64 5f63 656c 6c73 2829 0a20  ds_and_cells(). 
+0001d740: 2020 2020 2020 2064 656e 7320 3d20 7365         dens = se
+0001d750: 6c66 2e5f 6361 6c63 5f64 656e 7369 7479  lf._calc_density
+0001d760: 286e 6f72 6d61 6c69 7a65 203d 206e 6f72  (normalize = nor
+0001d770: 6d61 6c69 7a65 290a 2020 2020 2020 2020  malize).        
+0001d780: 706c 745f 6c69 6d73 203d 2076 697a 2e5f  plt_lims = viz._
+0001d790: 6765 745f 706c 745f 6c69 6d73 286c 616e  get_plt_lims(lan
+0001d7a0: 642c 2078 2c20 792c 207a 6f6f 6d5f 7769  d, x, y, zoom_wi
+0001d7b0: 6474 6829 0a20 2020 2020 2020 2069 6620  dth).        if 
+0001d7c0: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
+0001d7d0: 2020 2020 2020 2076 697a 2e5f 706c 6f74         viz._plot
+0001d7e0: 5f72 6173 7465 7273 2864 656e 732c 2070  _rasters(dens, p
+0001d7f0: 6c74 5f6c 696d 7320 3d20 706c 745f 6c69  lt_lims = plt_li
+0001d800: 6d73 2c20 6c79 725f 6e61 6d65 203d 2027  ms, lyr_name = '
+0001d810: 6465 6e73 6974 7927 2c0a 2020 2020 2020  density',.      
+0001d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d830: 2020 2020 2020 2020 7469 636b 733d 7469          ticks=ti
+0001d840: 636b 732c 206d 6173 6b5f 7261 7374 3d6d  cks, mask_rast=m
+0001d850: 6173 6b5f 7261 7374 290a 2020 2020 2020  ask_rast).      
+0001d860: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001d870: 2020 2020 7669 7a2e 5f70 6c6f 745f 7261      viz._plot_ra
+0001d880: 7374 6572 7328 6465 6e73 2c20 706c 745f  sters(dens, plt_
+0001d890: 6c69 6d73 203d 2070 6c74 5f6c 696d 732c  lims = plt_lims,
+0001d8a0: 2076 6d61 7820 3d20 6465 6e73 2e6d 6178   vmax = dens.max
+0001d8b0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0001d8c0: 2020 2020 6c79 725f 6e61 6d65 203d 2027      lyr_name = '
+0001d8d0: 6465 6e73 6974 7927 2c20 7469 636b 733d  density', ticks=
+0001d8e0: 7469 636b 732c 206d 6173 6b5f 7261 7374  ticks, mask_rast
+0001d8f0: 3d6d 6173 6b5f 7261 7374 290a 2020 2020  =mask_rast).    
+0001d900: 2020 2020 7365 6c66 2e5f 706c 6f74 2868      self._plot(h
+0001d910: 6964 655f 6c61 6e64 3d54 7275 652c 2069  ide_land=True, i
+0001d920: 6e64 6976 6964 7320 3d20 696e 6469 7669  ndivids = indivi
+0001d930: 6473 2c20 7465 7874 203d 2074 6578 742c  ds, text = text,
+0001d940: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+0001d950: 6f72 3d63 6f6c 6f72 2c20 6564 6765 5f63  or=color, edge_c
+0001d960: 6f6c 6f72 203d 2065 6467 655f 636f 6c6f  olor = edge_colo
+0001d970: 722c 2074 6578 745f 636f 6c6f 7220 3d20  r, text_color = 
+0001d980: 7465 7874 5f63 6f6c 6f72 2c0a 2020 2020  text_color,.    
+0001d990: 2020 2020 2020 2020 7369 7a65 3d73 697a          size=siz
+0001d9a0: 652c 2074 6578 745f 7369 7a65 203d 2074  e, text_size = t
+0001d9b0: 6578 745f 7369 7a65 2c20 616c 7068 613d  ext_size, alpha=
+0001d9c0: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
+0001d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9e0: 2020 2020 2020 2020 2020 207a 6f6f 6d5f             zoom_
+0001d9f0: 7769 6474 6820 3d20 7a6f 6f6d 5f77 6964  width = zoom_wid
+0001da00: 7468 2c20 7820 3d20 782c 2079 203d 2079  th, x = x, y = y
+0001da10: 290a 0a0a 2020 2020 2320 6d65 7468 6f64  )...    # method
+0001da20: 2066 6f72 2070 6c6f 7474 696e 6720 696e   for plotting in
+0001da30: 6469 7669 6475 616c 7320 636f 6c6f 7265  dividuals colore
+0001da40: 6420 6279 2074 6865 6972 2067 656e 6f74  d by their genot
+0001da50: 7970 6520 6174 2061 206c 6f63 7573 0a20  ype at a locus. 
+0001da60: 2020 2064 6566 205f 706c 6f74 5f67 656e     def _plot_gen
+0001da70: 6f74 7970 6528 7365 6c66 2c20 6c6f 6375  otype(self, locu
+0001da80: 732c 206c 7972 5f6e 756d 3d4e 6f6e 652c  s, lyr_num=None,
+0001da90: 206c 616e 643d 4e6f 6e65 2c20 696e 6469   land=None, indi
+0001daa0: 7669 6473 3d4e 6f6e 652c 0a20 2020 2020  vids=None,.     
+0001dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dac0: 2020 7465 7874 3d46 616c 7365 2c20 7369    text=False, si
+0001dad0: 7a65 3d32 352c 2074 6578 745f 7369 7a65  ze=25, text_size
+0001dae0: 203d 2039 2c20 6564 6765 5f63 6f6c 6f72   = 9, edge_color
+0001daf0: 3d27 626c 6163 6b27 2c0a 2020 2020 2020  ='black',.      
 0001db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db10: 2020 2062 795f 646f 6d69 6e61 6e63 653d     by_dominance=
-0001db20: 4661 6c73 652c 207a 6f6f 6d5f 7769 6474  False, zoom_widt
-0001db30: 683d 4e6f 6e65 2c20 783d 4e6f 6e65 2c20  h=None, x=None, 
-0001db40: 793d 4e6f 6e65 2c0a 2020 2020 2020 2020  y=None,.        
-0001db50: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001db60: 6963 6b73 3d4e 6f6e 652c 206d 6173 6b5f  icks=None, mask_
-0001db70: 7261 7374 3d4e 6f6e 6529 3a0a 0a20 2020  rast=None):..   
-0001db80: 2020 2020 2067 656e 6f74 7970 6573 203d       genotypes =
-0001db90: 2073 656c 662e 5f67 6574 5f67 656e 6f74   self._get_genot
-0001dba0: 7970 6573 286c 6f63 693d 5b6c 6f63 7573  ypes(loci=[locus
-0001dbb0: 5d2c 2069 6e64 6976 6964 733d 696e 6469  ], individs=indi
-0001dbc0: 7669 6473 2c0a 2020 2020 2020 2020 2020  vids,.          
-0001dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbe0: 2020 2020 2020 2020 2020 2020 2020 6269                bi
-0001dbf0: 616c 6c65 6c69 633d 4661 6c73 652c 2061  allelic=False, a
-0001dc00: 735f 6469 6374 3d54 7275 6529 0a20 2020  s_dict=True).   
-0001dc10: 2020 2020 2069 6620 6279 5f64 6f6d 696e       if by_domin
-0001dc20: 616e 6365 203d 3d20 5472 7565 3a0a 2020  ance == True:.  
-0001dc30: 2020 2020 2020 2020 2020 6966 206c 6f63            if loc
-0001dc40: 7573 2069 6e20 7365 6c66 2e67 656e 5f61  us in self.gen_a
-0001dc50: 7263 682e 6e6f 6e6e 6575 745f 6c6f 6369  rch.nonneut_loci
-0001dc60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001dc70: 2020 646f 6d20 3d20 7365 6c66 2e67 656e    dom = self.gen
-0001dc80: 5f61 7263 682e 646f 6d5b 6c6f 6375 735d  _arch.dom[locus]
-0001dc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dca0: 2023 204e 4f54 453a 2077 6f75 6c64 2062   # NOTE: would b
-0001dcb0: 6520 7369 6d70 6c65 7220 746f 206a 7573  e simpler to jus
-0001dcc0: 7420 7573 6520 6e70 2e63 6569 6c20 6865  t use np.ceil he
-0001dcd0: 7265 2e2e 2e0a 2020 2020 2020 2020 2020  re....          
-0001dce0: 2020 2020 2020 2320 2020 2020 2020 646f        #       do
-0001dcf0: 6e27 7420 7365 6520 7768 7920 4920 6469  n't see why I di
-0001dd00: 646e 2774 2e2e 2e3f 0a20 2020 2020 2020  dn't...?.       
-0001dd10: 2020 2020 2020 2020 2067 656e 6f74 7970           genotyp
-0001dd20: 6573 203d 207b 693a 6e70 2e63 6c69 7028  es = {i:np.clip(
-0001dd30: 6774 202a 2028 3120 2b20 646f 6d29 2c0a  gt * (1 + dom),.
-0001dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd60: 2020 2020 2020 2061 5f6d 696e 3d4e 6f6e         a_min=Non
-0001dd70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001db10: 2074 6578 745f 636f 6c6f 723d 2762 6c61   text_color='bla
+0001db20: 636b 272c 2063 6261 723d 5472 7565 2c20  ck', cbar=True, 
+0001db30: 616c 7068 613d 312c 0a20 2020 2020 2020  alpha=1,.       
+0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db50: 6279 5f64 6f6d 696e 616e 6365 3d46 616c  by_dominance=Fal
+0001db60: 7365 2c20 7a6f 6f6d 5f77 6964 7468 3d4e  se, zoom_width=N
+0001db70: 6f6e 652c 2078 3d4e 6f6e 652c 2079 3d4e  one, x=None, y=N
+0001db80: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001db90: 2020 2020 2020 2020 2020 2020 7469 636b              tick
+0001dba0: 733d 4e6f 6e65 2c20 6d61 736b 5f72 6173  s=None, mask_ras
+0001dbb0: 743d 4e6f 6e65 293a 0a0a 2020 2020 2020  t=None):..      
+0001dbc0: 2020 6765 6e6f 7479 7065 7320 3d20 7365    genotypes = se
+0001dbd0: 6c66 2e5f 6765 745f 6765 6e6f 7479 7065  lf._get_genotype
+0001dbe0: 7328 6c6f 6369 3d5b 6c6f 6375 735d 2c20  s(loci=[locus], 
+0001dbf0: 696e 6469 7669 6473 3d69 6e64 6976 6964  individs=individ
+0001dc00: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0001dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc20: 2020 2020 2020 2020 2020 2062 6961 6c6c             biall
+0001dc30: 656c 6963 3d46 616c 7365 2c20 6173 5f64  elic=False, as_d
+0001dc40: 6963 743d 5472 7565 290a 2020 2020 2020  ict=True).      
+0001dc50: 2020 6966 2062 795f 646f 6d69 6e61 6e63    if by_dominanc
+0001dc60: 6520 3d3d 2054 7275 653a 0a20 2020 2020  e == True:.     
+0001dc70: 2020 2020 2020 2069 6620 6c6f 6375 7320         if locus 
+0001dc80: 696e 2073 656c 662e 6765 6e5f 6172 6368  in self.gen_arch
+0001dc90: 2e6e 6f6e 6e65 7574 5f6c 6f63 693a 0a20  .nonneut_loci:. 
+0001dca0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001dcb0: 6f6d 203d 2073 656c 662e 6765 6e5f 6172  om = self.gen_ar
+0001dcc0: 6368 2e64 6f6d 5b6c 6f63 7573 5d0a 2020  ch.dom[locus].  
+0001dcd0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001dce0: 4e4f 5445 3a20 776f 756c 6420 6265 2073  NOTE: would be s
+0001dcf0: 696d 706c 6572 2074 6f20 6a75 7374 2075  impler to just u
+0001dd00: 7365 206e 702e 6365 696c 2068 6572 652e  se np.ceil here.
+0001dd10: 2e2e 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001dd20: 2020 2023 2020 2020 2020 2064 6f6e 2774     #       don't
+0001dd30: 2073 6565 2077 6879 2049 2064 6964 6e27   see why I didn'
+0001dd40: 742e 2e2e 3f0a 2020 2020 2020 2020 2020  t...?.          
+0001dd50: 2020 2020 2020 6765 6e6f 7479 7065 7320        genotypes 
+0001dd60: 3d20 7b69 3a6e 702e 636c 6970 2867 7420  = {i:np.clip(gt 
+0001dd70: 2a20 2831 202b 2064 6f6d 292c 0a20 2020  * (1 + dom),.   
 0001dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd90: 2020 2020 2020 2020 2020 615f 6d61 783d            a_max=
-0001dda0: 3129 2066 6f72 2069 2c20 6774 2069 6e20  1) for i, gt in 
-0001ddb0: 6765 6e6f 7479 7065 732e 6974 656d 7328  genotypes.items(
-0001ddc0: 297d 0a20 2020 2020 2020 2020 2020 2065  )}.            e
-0001ddd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001dde0: 2020 2020 2070 7269 6e74 2828 275c 6e5c       print(('\n\
-0001ddf0: 7457 4152 4e49 4e47 3a20 5468 6520 6279  tWARNING: The by
-0001de00: 5f64 6f6d 696e 616e 6365 2061 7267 756d  _dominance argum
-0001de10: 656e 7420 6973 2054 7275 652c 2027 0a20  ent is True, '. 
-0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de30: 2020 2020 2020 2762 7574 2061 206e 6575        'but a neu
-0001de40: 7472 616c 206c 6f63 7573 2077 6173 2063  tral locus was c
-0001de50: 686f 7365 6e2c 2027 0a20 2020 2020 2020  hosen, '.       
+0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dda0: 2020 2020 615f 6d69 6e3d 4e6f 6e65 2c0a      a_min=None,.
+0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddd0: 2020 2020 2020 2061 5f6d 6178 3d31 2920         a_max=1) 
+0001dde0: 666f 7220 692c 2067 7420 696e 2067 656e  for i, gt in gen
+0001ddf0: 6f74 7970 6573 2e69 7465 6d73 2829 7d0a  otypes.items()}.
+0001de00: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001de10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001de20: 2020 7072 696e 7428 2827 5c6e 5c74 5741    print(('\n\tWA
+0001de30: 524e 494e 473a 2054 6865 2062 795f 646f  RNING: The by_do
+0001de40: 6d69 6e61 6e63 6520 6172 6775 6d65 6e74  minance argument
+0001de50: 2069 7320 5472 7565 2c20 270a 2020 2020   is True, '.    
 0001de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de70: 2773 6f20 7468 6520 6172 6775 6d65 6e74  'so the argument
-0001de80: 2077 6173 206e 6f74 2075 7365 642e 5c6e   was not used.\n
-0001de90: 2729 290a 0a20 2020 2020 2020 2023 206a  '))..        # j
-0001dea0: 7573 7420 6173 7369 676e 2062 6c61 636b  ust assign black
-0001deb0: 2c20 6772 6179 2c20 616e 6420 7768 6974  , gray, and whit
-0001dec0: 6520 2873 696e 6365 2074 6865 7265 2773  e (since there's
-0001ded0: 206e 6f20 7265 6173 6f6e 0a20 2020 2020   no reason.     
-0001dee0: 2020 2023 206e 6563 6573 7361 7269 6c79     # necessarily
-0001def0: 2074 6861 7420 7468 6573 6520 7368 6f75   that these shou
-0001df00: 6c64 2062 6520 6d61 7070 6564 2074 6f20  ld be mapped to 
-0001df10: 6120 6365 7274 6169 6e20 6c61 7965 722c  a certain layer,
-0001df20: 2074 6865 2077 6179 0a20 2020 2020 2020   the way.       
-0001df30: 2023 2070 6865 6e6f 7479 7065 2073 686f   # phenotype sho
-0001df40: 756c 640a 2020 2020 2020 2020 636f 6c6f  uld.        colo
-0001df50: 7273 203d 205b 2723 3030 3030 3030 272c  rs = ['#000000',
-0001df60: 2027 2338 3038 3038 3027 2c20 2723 4646   '#808080', '#FF
-0001df70: 4646 4646 275d 0a0a 2020 2020 2020 2020  FFFF']..        
-0001df80: 666f 7220 6e2c 2067 656e 6f74 7970 6520  for n, genotype 
-0001df90: 696e 2065 6e75 6d65 7261 7465 285b 302e  in enumerate([0.
-0001dfa0: 302c 2030 2e35 2c20 312e 305d 293a 0a20  0, 0.5, 1.0]):. 
-0001dfb0: 2020 2020 2020 2020 2020 2067 656e 6f74             genot
-0001dfc0: 7970 655f 696e 6469 7669 6473 203d 205b  ype_individs = [
-0001dfd0: 6920 666f 7220 692c 2067 2069 6e20 6765  i for i, g in ge
-0001dfe0: 6e6f 7479 7065 732e 6974 656d 7328 0a20  notypes.items(. 
-0001dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e010: 2020 2020 2020 2029 2069 6620 6e70 2e61         ) if np.a
-0001e020: 746c 6561 7374 5f31 6428 6729 5b30 5d20  tleast_1d(g)[0] 
-0001e030: 3d3d 2067 656e 6f74 7970 655d 0a20 2020  == genotype].   
-0001e040: 2020 2020 2020 2020 2023 2077 696c 6c20           # will 
-0001e050: 6869 6465 2074 6865 206c 616e 6420 6966  hide the land if
-0001e060: 2074 6869 7320 6973 206e 6f74 2074 6865   this is not the
-0001e070: 2066 6972 7374 2070 6c6f 7420 6d61 6465   first plot made
-0001e080: 0a20 2020 2020 2020 2020 2020 2068 6964  .            hid
-0001e090: 655f 6c61 6e64 203d 206e 203e 2030 0a20  e_land = n > 0. 
-0001e0a0: 2020 2020 2020 2020 2020 2023 2070 6c6f             # plo
-0001e0b0: 7420 6966 2074 6865 7265 2061 7265 2061  t if there are a
-0001e0c0: 6e79 2069 6e64 6976 6964 7561 6c73 206f  ny individuals o
-0001e0d0: 6620 7468 6973 2067 656e 6f74 7970 650a  f this genotype.
-0001e0e0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0001e0f0: 656e 2867 656e 6f74 7970 655f 696e 6469  en(genotype_indi
-0001e100: 7669 6473 2920 3e3d 2031 3a0a 2020 2020  vids) >= 1:.    
-0001e110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e120: 2e5f 706c 6f74 286c 7972 5f6e 756d 3d6c  ._plot(lyr_num=l
-0001e130: 7972 5f6e 756d 2c20 6c61 6e64 3d6c 616e  yr_num, land=lan
-0001e140: 642c 2068 6964 655f 6c61 6e64 3d68 6964  d, hide_land=hid
-0001e150: 655f 6c61 6e64 2c0a 2020 2020 2020 2020  e_land,.        
-0001e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e170: 2020 2069 6e64 6976 6964 733d 6765 6e6f     individs=geno
-0001e180: 7479 7065 5f69 6e64 6976 6964 732c 0a20  type_individs,. 
-0001e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1a0: 2020 2020 2020 2020 2020 7465 7874 3d74            text=t
-0001e1b0: 6578 742c 2063 6f6c 6f72 3d63 6f6c 6f72  ext, color=color
-0001e1c0: 735b 6e5d 2c20 6564 6765 5f63 6f6c 6f72  s[n], edge_color
-0001e1d0: 3d65 6467 655f 636f 6c6f 722c 0a20 2020  =edge_color,.   
-0001e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1f0: 2020 2020 2020 2020 7465 7874 5f63 6f6c          text_col
-0001e200: 6f72 3d74 6578 745f 636f 6c6f 722c 2063  or=text_color, c
-0001e210: 6261 723d 6362 6172 2c0a 2020 2020 2020  bar=cbar,.      
+0001de70: 2020 2027 6275 7420 6120 6e65 7574 7261     'but a neutra
+0001de80: 6c20 6c6f 6375 7320 7761 7320 6368 6f73  l locus was chos
+0001de90: 656e 2c20 270a 2020 2020 2020 2020 2020  en, '.          
+0001dea0: 2020 2020 2020 2020 2020 2020 2027 736f               'so
+0001deb0: 2074 6865 2061 7267 756d 656e 7420 7761   the argument wa
+0001dec0: 7320 6e6f 7420 7573 6564 2e5c 6e27 2929  s not used.\n'))
+0001ded0: 0a0a 2020 2020 2020 2020 2320 6a75 7374  ..        # just
+0001dee0: 2061 7373 6967 6e20 626c 6163 6b2c 2067   assign black, g
+0001def0: 7261 792c 2061 6e64 2077 6869 7465 2028  ray, and white (
+0001df00: 7369 6e63 6520 7468 6572 6527 7320 6e6f  since there's no
+0001df10: 2072 6561 736f 6e0a 2020 2020 2020 2020   reason.        
+0001df20: 2320 6e65 6365 7373 6172 696c 7920 7468  # necessarily th
+0001df30: 6174 2074 6865 7365 2073 686f 756c 6420  at these should 
+0001df40: 6265 206d 6170 7065 6420 746f 2061 2063  be mapped to a c
+0001df50: 6572 7461 696e 206c 6179 6572 2c20 7468  ertain layer, th
+0001df60: 6520 7761 790a 2020 2020 2020 2020 2320  e way.        # 
+0001df70: 7068 656e 6f74 7970 6520 7368 6f75 6c64  phenotype should
+0001df80: 0a20 2020 2020 2020 2063 6f6c 6f72 7320  .        colors 
+0001df90: 3d20 5b27 2330 3030 3030 3027 2c20 2723  = ['#000000', '#
+0001dfa0: 3830 3830 3830 272c 2027 2346 4646 4646  808080', '#FFFFF
+0001dfb0: 4627 5d0a 0a20 2020 2020 2020 2066 6f72  F']..        for
+0001dfc0: 206e 2c20 6765 6e6f 7479 7065 2069 6e20   n, genotype in 
+0001dfd0: 656e 756d 6572 6174 6528 5b30 2e30 2c20  enumerate([0.0, 
+0001dfe0: 302e 352c 2031 2e30 5d29 3a0a 2020 2020  0.5, 1.0]):.    
+0001dff0: 2020 2020 2020 2020 6765 6e6f 7479 7065          genotype
+0001e000: 5f69 6e64 6976 6964 7320 3d20 5b69 2066  _individs = [i f
+0001e010: 6f72 2069 2c20 6720 696e 2067 656e 6f74  or i, g in genot
+0001e020: 7970 6573 2e69 7465 6d73 280a 2020 2020  ypes.items(.    
+0001e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e050: 2020 2020 2920 6966 206e 702e 6174 6c65      ) if np.atle
+0001e060: 6173 745f 3164 2867 295b 305d 203d 3d20  ast_1d(g)[0] == 
+0001e070: 6765 6e6f 7479 7065 5d0a 2020 2020 2020  genotype].      
+0001e080: 2020 2020 2020 2320 7769 6c6c 2068 6964        # will hid
+0001e090: 6520 7468 6520 6c61 6e64 2069 6620 7468  e the land if th
+0001e0a0: 6973 2069 7320 6e6f 7420 7468 6520 6669  is is not the fi
+0001e0b0: 7273 7420 706c 6f74 206d 6164 650a 2020  rst plot made.  
+0001e0c0: 2020 2020 2020 2020 2020 6869 6465 5f6c            hide_l
+0001e0d0: 616e 6420 3d20 6e20 3e20 300a 2020 2020  and = n > 0.    
+0001e0e0: 2020 2020 2020 2020 2320 706c 6f74 2069          # plot i
+0001e0f0: 6620 7468 6572 6520 6172 6520 616e 7920  f there are any 
+0001e100: 696e 6469 7669 6475 616c 7320 6f66 2074  individuals of t
+0001e110: 6869 7320 6765 6e6f 7479 7065 0a20 2020  his genotype.   
+0001e120: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+0001e130: 6765 6e6f 7479 7065 5f69 6e64 6976 6964  genotype_individ
+0001e140: 7329 203e 3d20 313a 0a20 2020 2020 2020  s) >= 1:.       
+0001e150: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+0001e160: 6c6f 7428 6c79 725f 6e75 6d3d 6c79 725f  lot(lyr_num=lyr_
+0001e170: 6e75 6d2c 206c 616e 643d 6c61 6e64 2c20  num, land=land, 
+0001e180: 6869 6465 5f6c 616e 643d 6869 6465 5f6c  hide_land=hide_l
+0001e190: 616e 642c 0a20 2020 2020 2020 2020 2020  and,.           
+0001e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1b0: 696e 6469 7669 6473 3d67 656e 6f74 7970  individs=genotyp
+0001e1c0: 655f 696e 6469 7669 6473 2c0a 2020 2020  e_individs,.    
+0001e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1e0: 2020 2020 2020 2074 6578 743d 7465 7874         text=text
+0001e1f0: 2c20 636f 6c6f 723d 636f 6c6f 7273 5b6e  , color=colors[n
+0001e200: 5d2c 2065 6467 655f 636f 6c6f 723d 6564  ], edge_color=ed
+0001e210: 6765 5f63 6f6c 6f72 2c0a 2020 2020 2020  ge_color,.      
 0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e230: 2020 2020 2073 697a 653d 7369 7a65 2c20       size=size, 
-0001e240: 7465 7874 5f73 697a 653d 7465 7874 5f73  text_size=text_s
-0001e250: 697a 652c 2061 6c70 6861 3d61 6c70 6861  ize, alpha=alpha
-0001e260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e270: 2020 2020 2020 2020 2020 2020 207a 6f6f               zoo
-0001e280: 6d5f 7769 6474 683d 7a6f 6f6d 5f77 6964  m_width=zoom_wid
-0001e290: 7468 2c20 783d 782c 2079 3d79 2c20 766d  th, x=x, y=y, vm
-0001e2a0: 696e 3d30 2c20 766d 6178 3d31 2c0a 2020  in=0, vmax=1,.  
-0001e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2c0: 2020 2020 2020 2020 2074 6963 6b73 3d74           ticks=t
-0001e2d0: 6963 6b73 2c20 6d61 736b 5f72 6173 743d  icks, mask_rast=
-0001e2e0: 6d61 736b 5f72 6173 7429 0a0a 0a20 2020  mask_rast)...   
-0001e2f0: 2023 206d 6574 686f 6420 666f 7220 706c   # method for pl
-0001e300: 6f74 7469 6e67 2069 6e64 6976 6964 7561  otting individua
-0001e310: 6c73 2063 6f6c 6f72 6564 2062 7920 7468  ls colored by th
-0001e320: 6569 7220 7068 656e 6f74 7970 6573 0a20  eir phenotypes. 
-0001e330: 2020 2023 666f 7220 6120 6769 7665 6e20     #for a given 
-0001e340: 7472 6169 740a 2020 2020 6465 6620 5f70  trait.    def _p
-0001e350: 6c6f 745f 7068 656e 6f74 7970 6528 7365  lot_phenotype(se
-0001e360: 6c66 2c20 7472 6169 742c 206c 7972 5f6e  lf, trait, lyr_n
-0001e370: 756d 3d4e 6f6e 652c 206c 616e 643d 4e6f  um=None, land=No
-0001e380: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0001e390: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-0001e3a0: 7669 6473 3d4e 6f6e 652c 2074 6578 743d  vids=None, text=
-0001e3b0: 4661 6c73 652c 2073 697a 653d 3235 2c20  False, size=25, 
-0001e3c0: 7465 7874 5f73 697a 653d 392c 0a20 2020  text_size=9,.   
-0001e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3e0: 2020 2020 2065 6467 655f 636f 6c6f 723d       edge_color=
-0001e3f0: 2762 6c61 636b 272c 2074 6578 745f 636f  'black', text_co
-0001e400: 6c6f 723d 2762 6c61 636b 272c 2063 6261  lor='black', cba
-0001e410: 723d 5472 7565 2c0a 2020 2020 2020 2020  r=True,.        
-0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e430: 616c 7068 613d 312c 207a 6f6f 6d5f 7769  alpha=1, zoom_wi
-0001e440: 6474 683d 4e6f 6e65 2c20 783d 4e6f 6e65  dth=None, x=None
-0001e450: 2c20 793d 4e6f 6e65 2c0a 2020 2020 2020  , y=None,.      
-0001e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e470: 2020 7469 636b 733d 4e6f 6e65 2c20 6d61    ticks=None, ma
-0001e480: 736b 5f72 6173 743d 4e6f 6e65 2c20 616e  sk_rast=None, an
-0001e490: 696d 6174 653d 4661 6c73 6529 3a0a 0a20  imate=False):.. 
-0001e4a0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
-0001e4b0: 2074 7261 6974 2773 206c 7972 5f6e 756d   trait's lyr_num
-0001e4c0: 2c20 6966 206e 6f20 6c79 725f 6e75 6d20  , if no lyr_num 
-0001e4d0: 7072 6f76 6964 6564 0a20 2020 2020 2020  provided.       
-0001e4e0: 206c 7972 5f6e 756d 203d 2073 656c 662e   lyr_num = self.
-0001e4f0: 6765 6e5f 6172 6368 2e74 7261 6974 735b  gen_arch.traits[
-0001e500: 7472 6169 745d 2e6c 7972 5f6e 756d 0a0a  trait].lyr_num..
-0001e510: 2020 2020 2020 2020 7a20 3d20 4f44 287a          z = OD(z
-0001e520: 6970 285b 2a73 656c 665d 2c20 7365 6c66  ip([*self], self
-0001e530: 2e5f 6765 745f 7a28 295b 3a2c 2074 7261  ._get_z()[:, tra
-0001e540: 6974 5d29 290a 2020 2020 2020 2020 6966  it])).        if
-0001e550: 2069 6e64 6976 6964 7320 6973 206e 6f74   individs is not
-0001e560: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001e570: 2020 207a 203d 207b 693a 2076 2066 6f72     z = {i: v for
-0001e580: 2069 2c20 7620 696e 207a 2e69 7465 6d73   i, v in z.items
-0001e590: 2829 2069 6620 6920 696e 2069 6e64 6976  () if i in indiv
-0001e5a0: 6964 737d 0a0a 2020 2020 2020 2020 2320  ids}..        # 
-0001e5b0: 6765 7420 7468 6520 636f 7272 6563 7420  get the correct 
-0001e5c0: 636d 6170 2066 6f72 2074 6869 7320 7472  cmap for this tr
-0001e5d0: 6169 7427 7320 6c61 7965 720a 2020 2020  ait's layer.    
-0001e5e0: 2020 2020 7074 5f63 6d61 7020 3d20 7669      pt_cmap = vi
-0001e5f0: 7a2e 5f63 686f 6f73 655f 636d 6170 2873  z._choose_cmap(s
-0001e600: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
-0001e610: 6974 735b 7472 6169 745d 2e6c 7972 5f6e  its[trait].lyr_n
-0001e620: 756d 290a 0a20 2020 2020 2020 2070 6f69  um)..        poi
-0001e630: 6e74 7320 3d20 7365 6c66 2e5f 706c 6f74  nts = self._plot
-0001e640: 286c 7972 5f6e 756d 203d 206c 7972 5f6e  (lyr_num = lyr_n
-0001e650: 756d 2c20 6c61 6e64 203d 206c 616e 642c  um, land = land,
-0001e660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e670: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-0001e680: 6976 6964 7320 3d20 696e 6469 7669 6473  ivids = individs
-0001e690: 2c20 7465 7874 203d 2074 6578 742c 0a20  , text = text,. 
+0001e230: 2020 2020 2074 6578 745f 636f 6c6f 723d       text_color=
+0001e240: 7465 7874 5f63 6f6c 6f72 2c20 6362 6172  text_color, cbar
+0001e250: 3d63 6261 722c 0a20 2020 2020 2020 2020  =cbar,.         
+0001e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e270: 2020 7369 7a65 3d73 697a 652c 2074 6578    size=size, tex
+0001e280: 745f 7369 7a65 3d74 6578 745f 7369 7a65  t_size=text_size
+0001e290: 2c20 616c 7068 613d 616c 7068 612c 0a20  , alpha=alpha,. 
+0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2b0: 2020 2020 2020 2020 2020 7a6f 6f6d 5f77            zoom_w
+0001e2c0: 6964 7468 3d7a 6f6f 6d5f 7769 6474 682c  idth=zoom_width,
+0001e2d0: 2078 3d78 2c20 793d 792c 2076 6d69 6e3d   x=x, y=y, vmin=
+0001e2e0: 302c 2076 6d61 783d 312c 0a20 2020 2020  0, vmax=1,.     
+0001e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e300: 2020 2020 2020 7469 636b 733d 7469 636b        ticks=tick
+0001e310: 732c 206d 6173 6b5f 7261 7374 3d6d 6173  s, mask_rast=mas
+0001e320: 6b5f 7261 7374 290a 0a0a 2020 2020 2320  k_rast)...    # 
+0001e330: 6d65 7468 6f64 2066 6f72 2070 6c6f 7474  method for plott
+0001e340: 696e 6720 696e 6469 7669 6475 616c 7320  ing individuals 
+0001e350: 636f 6c6f 7265 6420 6279 2074 6865 6972  colored by their
+0001e360: 2070 6865 6e6f 7479 7065 730a 2020 2020   phenotypes.    
+0001e370: 2366 6f72 2061 2067 6976 656e 2074 7261  #for a given tra
+0001e380: 6974 0a20 2020 2064 6566 205f 706c 6f74  it.    def _plot
+0001e390: 5f70 6865 6e6f 7479 7065 2873 656c 662c  _phenotype(self,
+0001e3a0: 2074 7261 6974 2c20 6c79 725f 6e75 6d3d   trait, lyr_num=
+0001e3b0: 4e6f 6e65 2c20 6c61 6e64 3d4e 6f6e 652c  None, land=None,
+0001e3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e3d0: 2020 2020 2020 2020 2069 6e64 6976 6964           individ
+0001e3e0: 733d 4e6f 6e65 2c20 7465 7874 3d46 616c  s=None, text=Fal
+0001e3f0: 7365 2c20 7369 7a65 3d32 352c 2074 6578  se, size=25, tex
+0001e400: 745f 7369 7a65 3d39 2c0a 2020 2020 2020  t_size=9,.      
+0001e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e420: 2020 6564 6765 5f63 6f6c 6f72 3d27 626c    edge_color='bl
+0001e430: 6163 6b27 2c20 7465 7874 5f63 6f6c 6f72  ack', text_color
+0001e440: 3d27 626c 6163 6b27 2c20 6362 6172 3d54  ='black', cbar=T
+0001e450: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0001e460: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
+0001e470: 6861 3d31 2c20 7a6f 6f6d 5f77 6964 7468  ha=1, zoom_width
+0001e480: 3d4e 6f6e 652c 2078 3d4e 6f6e 652c 2079  =None, x=None, y
+0001e490: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0001e4a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001e4b0: 6963 6b73 3d4e 6f6e 652c 206d 6173 6b5f  icks=None, mask_
+0001e4c0: 7261 7374 3d4e 6f6e 652c 2061 6e69 6d61  rast=None, anima
+0001e4d0: 7465 3d46 616c 7365 293a 0a0a 2020 2020  te=False):..    
+0001e4e0: 2020 2020 2320 6765 7420 7468 6520 7472      # get the tr
+0001e4f0: 6169 7427 7320 6c79 725f 6e75 6d2c 2069  ait's lyr_num, i
+0001e500: 6620 6e6f 206c 7972 5f6e 756d 2070 726f  f no lyr_num pro
+0001e510: 7669 6465 640a 2020 2020 2020 2020 6c79  vided.        ly
+0001e520: 725f 6e75 6d20 3d20 7365 6c66 2e67 656e  r_num = self.gen
+0001e530: 5f61 7263 682e 7472 6169 7473 5b74 7261  _arch.traits[tra
+0001e540: 6974 5d2e 6c79 725f 6e75 6d0a 0a20 2020  it].lyr_num..   
+0001e550: 2020 2020 207a 203d 204f 4428 7a69 7028       z = OD(zip(
+0001e560: 5b2a 7365 6c66 5d2c 2073 656c 662e 5f67  [*self], self._g
+0001e570: 6574 5f7a 2829 5b3a 2c20 7472 6169 745d  et_z()[:, trait]
+0001e580: 2929 0a20 2020 2020 2020 2069 6620 696e  )).        if in
+0001e590: 6469 7669 6473 2069 7320 6e6f 7420 4e6f  divids is not No
+0001e5a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001e5b0: 7a20 3d20 7b69 3a20 7620 666f 7220 692c  z = {i: v for i,
+0001e5c0: 2076 2069 6e20 7a2e 6974 656d 7328 2920   v in z.items() 
+0001e5d0: 6966 2069 2069 6e20 696e 6469 7669 6473  if i in individs
+0001e5e0: 7d0a 0a20 2020 2020 2020 2023 2067 6574  }..        # get
+0001e5f0: 2074 6865 2063 6f72 7265 6374 2063 6d61   the correct cma
+0001e600: 7020 666f 7220 7468 6973 2074 7261 6974  p for this trait
+0001e610: 2773 206c 6179 6572 0a20 2020 2020 2020  's layer.       
+0001e620: 2070 745f 636d 6170 203d 2076 697a 2e5f   pt_cmap = viz._
+0001e630: 6368 6f6f 7365 5f63 6d61 7028 7365 6c66  choose_cmap(self
+0001e640: 2e67 656e 5f61 7263 682e 7472 6169 7473  .gen_arch.traits
+0001e650: 5b74 7261 6974 5d2e 6c79 725f 6e75 6d29  [trait].lyr_num)
+0001e660: 0a0a 2020 2020 2020 2020 706f 696e 7473  ..        points
+0001e670: 203d 2073 656c 662e 5f70 6c6f 7428 6c79   = self._plot(ly
+0001e680: 725f 6e75 6d20 3d20 6c79 725f 6e75 6d2c  r_num = lyr_num,
+0001e690: 206c 616e 6420 3d20 6c61 6e64 2c0a 2020   land = land,.  
 0001e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6b0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-0001e6c0: 203d 206c 6973 7428 7a2e 7661 6c75 6573   = list(z.values
-0001e6d0: 2829 292c 2070 745f 636d 6170 203d 2070  ()), pt_cmap = p
-0001e6e0: 745f 636d 6170 2c0a 2020 2020 2020 2020  t_cmap,.        
-0001e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e700: 2020 2020 6564 6765 5f63 6f6c 6f72 203d      edge_color =
-0001e710: 2065 6467 655f 636f 6c6f 722c 2074 6578   edge_color, tex
-0001e720: 745f 636f 6c6f 7220 3d20 7465 7874 5f63  t_color = text_c
-0001e730: 6f6c 6f72 2c0a 2020 2020 2020 2020 2020  olor,.          
-0001e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e750: 2020 6362 6172 203d 2063 6261 722c 2073    cbar = cbar, s
-0001e760: 697a 6520 3d20 7369 7a65 2c20 7465 7874  ize = size, text
-0001e770: 5f73 697a 6520 3d20 7465 7874 5f73 697a  _size = text_siz
-0001e780: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001e790: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001e7a0: 6c70 6861 203d 2061 6c70 6861 2c20 7a6f  lpha = alpha, zo
-0001e7b0: 6f6d 5f77 6964 7468 203d 207a 6f6f 6d5f  om_width = zoom_
-0001e7c0: 7769 6474 682c 2078 203d 2078 2c0a 2020  width, x = x,.  
-0001e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7e0: 2020 2020 2020 2020 2020 7920 3d20 792c            y = y,
-0001e7f0: 2076 6d69 6e20 3d20 302c 2076 6d61 7820   vmin = 0, vmax 
-0001e800: 3d20 312c 2074 6963 6b73 3d74 6963 6b73  = 1, ticks=ticks
-0001e810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e820: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001e830: 736b 5f72 6173 743d 6d61 736b 5f72 6173  sk_rast=mask_ras
-0001e840: 742c 2061 6e69 6d61 7465 3d61 6e69 6d61  t, animate=anima
-0001e850: 7465 290a 0a20 2020 2020 2020 2072 6574  te)..        ret
-0001e860: 7572 6e20 706f 696e 7473 0a0a 0a20 2020  urn points...   
-0001e870: 2023 206d 6574 686f 6420 666f 7220 706c   # method for pl
-0001e880: 6f74 7469 6e67 2069 6e64 6976 6964 7561  otting individua
-0001e890: 6c73 2063 6f6c 6f72 6564 2062 7920 7468  ls colored by th
-0001e8a0: 6569 7220 6f76 6572 616c 6c20 6669 746e  eir overall fitn
-0001e8b0: 6573 7365 732c 0a20 2020 2023 6f72 2062  esses,.    #or b
-0001e8c0: 7920 7468 6569 7220 6669 746e 6573 7365  y their fitnesse
-0001e8d0: 7320 666f 7220 6120 7369 6e67 6c65 2074  s for a single t
-0001e8e0: 7261 6974 2028 6966 2074 7261 6974 2069  rait (if trait i
-0001e8f0: 7320 6e6f 7420 4e6f 6e65 290a 2020 2020  s not None).    
-0001e900: 6465 6620 5f70 6c6f 745f 6669 746e 6573  def _plot_fitnes
-0001e910: 7328 7365 6c66 2c20 7472 745f 6e75 6d3d  s(self, trt_num=
-0001e920: 4e6f 6e65 2c20 6c79 725f 6e75 6d3d 4e6f  None, lyr_num=No
-0001e930: 6e65 2c20 6c61 6e64 3d4e 6f6e 652c 0a20  ne, land=None,. 
-0001e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e950: 2020 2020 2069 6e64 6976 6964 733d 4e6f       individs=No
-0001e960: 6e65 2c20 7465 7874 3d46 616c 7365 2c20  ne, text=False, 
-0001e970: 7068 656e 6f74 7970 655f 7465 7874 3d46  phenotype_text=F
-0001e980: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0001e990: 2020 2020 2020 2020 2020 2020 7068 656e              phen
-0001e9a0: 6f74 7970 655f 7465 7874 5f63 6f6c 6f72  otype_text_color
-0001e9b0: 3d27 626c 6163 6b27 2c20 6669 746e 6573  ='black', fitnes
-0001e9c0: 735f 7465 7874 3d46 616c 7365 2c0a 2020  s_text=False,.  
-0001e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9e0: 2020 2020 6669 746e 6573 735f 7465 7874      fitness_text
-0001e9f0: 5f63 6f6c 6f72 3d27 2333 3333 3333 3327  _color='#333333'
-0001ea00: 2c20 7369 7a65 3d31 3030 2c20 7465 7874  , size=100, text
-0001ea10: 5f73 697a 6520 3d20 392c 0a20 2020 2020  _size = 9,.     
-0001ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea30: 2065 6467 655f 636f 6c6f 723d 2762 6c61   edge_color='bla
-0001ea40: 636b 272c 2074 6578 745f 636f 6c6f 723d  ck', text_color=
-0001ea50: 2762 6c61 636b 272c 0a20 2020 2020 2020  'black',.       
-0001ea60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001ea70: 6974 5f63 6d61 7020 3d20 2752 6459 6c47  it_cmap = 'RdYlG
-0001ea80: 6e27 2c20 6362 6172 3d54 7275 652c 2066  n', cbar=True, f
-0001ea90: 6974 6e65 7373 5f63 6261 723d 5472 7565  itness_cbar=True
-0001eaa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001eab0: 2020 2020 2020 2020 616c 7068 613d 312c          alpha=1,
-0001eac0: 207a 6f6f 6d5f 7769 6474 683d 4e6f 6e65   zoom_width=None
-0001ead0: 2c20 783d 4e6f 6e65 2c20 793d 4e6f 6e65  , x=None, y=None
-0001eae0: 2c20 7469 636b 733d 4e6f 6e65 2c0a 2020  , ticks=None,.  
-0001eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb00: 2020 2020 6d61 736b 5f72 6173 743d 4e6f      mask_rast=No
-0001eb10: 6e65 293a 0a0a 2020 2020 2020 2020 2372  ne):..        #r
-0001eb20: 6574 7572 6e20 6d65 7373 6167 6573 2069  eturn messages i
-0001eb30: 6620 7370 6563 6965 7320 646f 6573 206e  f species does n
-0001eb40: 6f74 2068 6176 6520 6765 6e6f 6d65 7320  ot have genomes 
-0001eb50: 6f72 2074 7261 6974 730a 2020 2020 2020  or traits.      
-0001eb60: 2020 6966 2073 656c 662e 6765 6e5f 6172    if self.gen_ar
-0001eb70: 6368 2069 7320 4e6f 6e65 3a0a 2020 2020  ch is None:.    
-0001eb80: 2020 2020 2020 2020 7072 696e 7428 2822          print(("
-0001eb90: 5370 6563 6965 732e 5f70 6c6f 745f 6669  Species._plot_fi
-0001eba0: 746e 6573 7320 6973 206e 6f74 2076 616c  tness is not val
-0001ebb0: 6964 2066 6f72 2073 7065 6369 6573 2022  id for species "
-0001ebc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ebd0: 2020 2020 2277 6974 686f 7574 2067 656e      "without gen
-0001ebe0: 6f6d 6573 2e5c 6e22 2929 0a20 2020 2020  omes.\n")).     
-0001ebf0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0001ec00: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-0001ec10: 6765 6e5f 6172 6368 2e74 7261 6974 7320  gen_arch.traits 
-0001ec20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001ec30: 2020 2020 2070 7269 6e74 2828 2253 7065       print(("Spe
-0001ec40: 6369 6573 2e5f 706c 6f74 5f66 6974 6e65  cies._plot_fitne
-0001ec50: 7373 2069 7320 6e6f 7420 7661 6c69 6420  ss is not valid 
-0001ec60: 666f 7220 7370 6563 6965 7320 220a 2020  for species ".  
-0001ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec80: 2022 7769 7468 6f75 7420 7472 6169 7473   "without traits
-0001ec90: 2e5c 6e22 2929 0a20 2020 2020 2020 2020  .\n")).         
-0001eca0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
-0001ecb0: 2020 2023 2067 6574 2074 6865 2074 7261     # get the tra
-0001ecc0: 6974 2773 206c 7972 5f6e 756d 2c20 6966  it's lyr_num, if
-0001ecd0: 206c 7972 5f6e 756d 2077 6173 6e27 7420   lyr_num wasn't 
-0001ece0: 7072 6f76 6964 6564 2062 7574 2074 7274  provided but trt
-0001ecf0: 5f6e 756d 2077 6173 0a20 2020 2020 2020  _num was.       
-0001ed00: 2069 6620 7472 745f 6e75 6d20 6973 206e   if trt_num is n
-0001ed10: 6f74 204e 6f6e 6520 616e 6420 6c79 725f  ot None and lyr_
-0001ed20: 6e75 6d20 6973 204e 6f6e 653a 0a20 2020  num is None:.   
-0001ed30: 2020 2020 2020 2020 206c 7972 5f6e 756d           lyr_num
-0001ed40: 203d 2073 656c 662e 6765 6e5f 6172 6368   = self.gen_arch
-0001ed50: 2e74 7261 6974 735b 7472 745f 6e75 6d5d  .traits[trt_num]
-0001ed60: 2e6c 7972 5f6e 756d 0a0a 2020 2020 2020  .lyr_num..      
-0001ed70: 2020 2320 6765 7420 616c 6c20 696e 6469    # get all indi
-0001ed80: 7669 6473 2720 6669 746e 6573 7320 7661  vids' fitness va
-0001ed90: 6c75 6573 2c0a 2020 2020 2020 2020 2320  lues,.        # 
-0001eda0: 616e 6420 6765 7420 6170 7072 6f70 7269  and get appropri
-0001edb0: 6174 6520 636f 6c6f 726d 6170 0a20 2020  ate colormap.   
-0001edc0: 2020 2020 2069 6620 7472 745f 6e75 6d20       if trt_num 
-0001edd0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001ede0: 2020 2020 2077 203d 2073 656c 662e 5f63       w = self._c
-0001edf0: 616c 635f 6669 746e 6573 7328 290a 2020  alc_fitness().  
-0001ee00: 2020 2020 2020 2020 2020 7074 5f63 6d61            pt_cma
-0001ee10: 7020 3d20 2747 7265 7973 5f72 270a 2020  p = 'Greys_r'.  
-0001ee20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001ee30: 2020 2020 2020 2020 7720 3d20 7365 6c66          w = self
-0001ee40: 2e5f 6361 6c63 5f66 6974 6e65 7373 2874  ._calc_fitness(t
-0001ee50: 7261 6974 5f6e 756d 203d 2074 7274 5f6e  rait_num = trt_n
-0001ee60: 756d 290a 0a20 2020 2020 2020 2023 6669  um)..        #fi
-0001ee70: 6c74 6572 206f 7574 2075 6e77 616e 7465  lter out unwante
-0001ee80: 6420 696e 6469 7669 6473 2c20 6966 206e  d individs, if n
-0001ee90: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
-0001eea0: 2077 203d 204f 4428 7a69 7028 5b2a 7365   w = OD(zip([*se
-0001eeb0: 6c66 5d2c 2077 2929 0a20 2020 2020 2020  lf], w)).       
-0001eec0: 2069 6620 696e 6469 7669 6473 2069 7320   if individs is 
-0001eed0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0001eee0: 2020 2020 2020 7720 3d20 7b69 3a76 2066        w = {i:v f
-0001eef0: 6f72 2069 2c76 2069 6e20 772e 6974 656d  or i,v in w.item
-0001ef00: 7328 2920 6966 2069 2069 6e20 696e 6469  s() if i in indi
-0001ef10: 7669 6473 7d0a 0a20 2020 2020 2020 2023  vids}..        #
-0001ef20: 2063 616c 6320 6d69 6e69 6d75 6d20 706f   calc minimum po
-0001ef30: 7373 6962 6c65 2066 6974 6e65 7373 2028  ssible fitness (
-0001ef40: 666f 7220 7068 656e 6f74 7970 6573 2077  for phenotypes w
-0001ef50: 6974 6869 6e20 3020 3c3d 207a 203c 3d20  ithin 0 <= z <= 
-0001ef60: 312c 0a20 2020 2020 2020 2023 7768 6963  1,.        #whic
-0001ef70: 6820 696e 2072 6561 6c69 7479 2069 736e  h in reality isn
-0001ef80: 2774 2061 2063 6f6e 7374 7261 696e 742c  't a constraint,
-0001ef90: 2062 7574 2076 616c 7565 7320 6c6f 7765   but values lowe
-0001efa0: 7220 7468 616e 0a20 2020 2020 2020 2023  r than.        #
-0001efb0: 7468 6973 2077 696c 6c20 616c 736f 2062  this will also b
-0001efc0: 6520 636f 6e73 7472 6169 6e65 6420 746f  e constrained to
-0001efd0: 2074 6865 206d 696e 696d 756d 2d76 616c   the minimum-val
-0001efe0: 7565 2063 6f6c 6f72 2066 6f72 2070 6c6f  ue color for plo
-0001eff0: 7474 696e 6729 0a20 2020 2020 2020 2023  tting).        #
-0001f000: 4e4f 5445 3a20 7468 6520 6e70 2e61 746c  NOTE: the np.atl
-0001f010: 6561 7374 5f32 6428 2e2e 2e29 2e6d 696e  east_2d(...).min
-0001f020: 2829 2063 6f6e 7374 7275 6374 206d 616b  () construct mak
-0001f030: 6573 2074 6869 730a 2020 2020 2020 2020  es this.        
-0001f040: 2377 6f72 6b20 626f 7468 2066 6f72 2066  #work both for f
-0001f050: 6978 6564 2061 6e64 2073 7061 7469 616c  ixed and spatial
-0001f060: 6c79 2076 6172 7969 6e67 2070 6869 0a20  ly varying phi. 
-0001f070: 2020 2020 2020 2069 6620 7472 745f 6e75         if trt_nu
-0001f080: 6d20 6973 204e 6f6e 653a 0a20 2020 2020  m is None:.     
-0001f090: 2020 2020 2020 206d 696e 5f66 6974 203d         min_fit =
-0001f0a0: 206e 702e 7072 6f64 7563 7428 5b31 202d   np.product([1 -
-0001f0b0: 206e 702e 6174 6c65 6173 745f 3264 2874   np.atleast_2d(t
-0001f0c0: 2e70 6869 292e 6d69 6e28 0a20 2020 2020  .phi).min(.     
-0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0e0: 2020 2020 2020 2029 2066 6f72 2074 2069         ) for t i
-0001f0f0: 6e20 6c69 7374 2873 656c 662e 6765 6e5f  n list(self.gen_
-0001f100: 6172 6368 2e74 7261 6974 732e 7661 6c75  arch.traits.valu
-0001f110: 6573 2829 295d 290a 2020 2020 2020 2020  es())]).        
-0001f120: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001f130: 2020 6d69 6e5f 6669 7420 3d20 3120 2d20    min_fit = 1 - 
-0001f140: 6e70 2e61 746c 6561 7374 5f32 6428 7365  np.atleast_2d(se
-0001f150: 6c66 2e67 656e 5f61 7263 682e 7472 6169  lf.gen_arch.trai
-0001f160: 7473 5b0a 2020 2020 2020 2020 2020 2020  ts[.            
-0001f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f190: 2020 2020 2020 2020 2020 2020 7472 745f              trt_
-0001f1a0: 6e75 6d5d 2e70 6869 292e 6d69 6e28 290a  num].phi).min().
-0001f1b0: 0a20 2020 2020 2020 2023 7468 656e 2067  .        #then g
-0001f1c0: 6574 2075 6e65 7665 6e20 636d 6170 2061  et uneven cmap a
-0001f1d0: 6e64 2063 6261 722d 6d61 6b65 7220 286e  nd cbar-maker (n
-0001f1e0: 6565 6473 2074 6f20 6265 2075 6e65 7665  eeds to be uneve
-0001f1f0: 6e20 746f 0a20 2020 2020 2020 2023 6769  n to.        #gi
-0001f200: 7665 2063 6f6c 6f72 2d72 6573 6f6c 7574  ve color-resolut
-0001f210: 696f 6e20 746f 2076 616c 7565 7320 7661  ion to values va
-0001f220: 7279 696e 670a 2020 2020 2020 2020 2362  rying.        #b
-0001f230: 6574 7765 656e 2031 2061 6e64 2074 6865  etween 1 and the
-0001f240: 206d 696e 696d 756d 2d66 6974 6e65 7373   minimum-fitness
-0001f250: 2076 616c 7565 2061 7373 756d 696e 6720   value assuming 
-0001f260: 616c 6c0a 2020 2020 2020 2020 2370 6865  all.        #phe
-0001f270: 6e6f 7479 7065 7320 6172 6520 636f 6e73  notypes are cons
-0001f280: 7472 6169 6e65 6420 303c 3d7a 3c3d 312c  trained 0<=z<=1,
-0001f290: 2062 7574 2074 6865 6e20 616c 736f 0a20   but then also. 
-0001f2a0: 2020 2020 2020 2023 616c 6c6f 7720 6772         #allow gr
-0001f2b0: 6164 7561 6c6c 7920 6465 6570 656e 696e  adually deepenin
-0001f2c0: 6720 7265 6473 2066 6f72 2066 6974 6e65  g reds for fitne
-0001f2d0: 7373 2076 616c 7565 7320 6c6f 7765 720a  ss values lower.
-0001f2e0: 2020 2020 2020 2020 2374 6861 6e20 7468          #than th
-0001f2f0: 6174 206d 696e 696d 756d 2076 616c 7565  at minimum value
-0001f300: 292c 2075 7369 6e67 2074 6865 206d 696e  ), using the min
-0001f310: 5f66 6974 2076 616c 0a20 2020 2020 2020  _fit val.       
-0001f320: 2063 6d61 702c 206d 616b 655f 6362 6172   cmap, make_cbar
-0001f330: 5f66 6e20 3d20 7669 7a2e 5f6d 616b 655f  _fn = viz._make_
-0001f340: 6669 746e 6573 735f 636d 6170 5f61 6e64  fitness_cmap_and
-0001f350: 5f63 6261 725f 6d61 6b65 7228 0a20 2020  _cbar_maker(.   
-0001f360: 2020 2020 2020 2020 206d 696e 5f76 616c           min_val
-0001f370: 203d 206d 696e 5f66 6974 2c20 6d61 785f   = min_fit, max_
-0001f380: 7661 6c20 3d20 312c 2063 6d61 7020 3d20  val = 1, cmap = 
-0001f390: 6669 745f 636d 6170 2c0a 2020 2020 2020  fit_cmap,.      
-0001f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f3c0: 2020 2020 2020 2020 2020 7472 745f 6e75            trt_nu
-0001f3d0: 6d20 3d20 7472 745f 6e75 6d29 0a0a 2020  m = trt_num)..  
-0001f3e0: 2020 2020 2020 2370 6c6f 7420 7468 6520        #plot the 
-0001f3f0: 7472 6169 7420 7068 656e 6f74 7970 6520  trait phenotype 
-0001f400: 696e 206c 6172 6765 7220 6369 7263 6c65  in larger circle
-0001f410: 7320 6669 7273 742c 2069 6620 7472 6169  s first, if trai
-0001f420: 7420 6973 206e 6f74 204e 6f6e 650a 2020  t is not None.  
-0001f430: 2020 2020 2020 6966 2074 7274 5f6e 756d        if trt_num
-0001f440: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0001f450: 2020 2020 2020 2020 2020 2370 6c6f 7420            #plot 
-0001f460: 7468 6520 6f75 7465 7220 2870 6865 6e6f  the outer (pheno
-0001f470: 7479 7065 2920 6369 7263 6c65 730a 2020  type) circles.  
-0001f480: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0001f490: 706c 6f74 5f70 6865 6e6f 7479 7065 2874  plot_phenotype(t
-0001f4a0: 7261 6974 203d 2074 7274 5f6e 756d 2c20  rait = trt_num, 
-0001f4b0: 6c79 725f 6e75 6d20 3d20 6c79 725f 6e75  lyr_num = lyr_nu
-0001f4c0: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
-0001f4d0: 2020 206c 616e 6420 3d20 6c61 6e64 2c20     land = land, 
-0001f4e0: 696e 6469 7669 6473 203d 2069 6e64 6976  individs = indiv
-0001f4f0: 6964 732c 2074 6578 7420 3d20 4661 6c73  ids, text = Fals
-0001f500: 652c 2073 697a 6520 3d20 7369 7a65 2c0a  e, size = size,.
-0001f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f520: 7465 7874 5f73 697a 6520 3d20 7465 7874  text_size = text
-0001f530: 5f73 697a 652c 2065 6467 655f 636f 6c6f  _size, edge_colo
-0001f540: 723d 6564 6765 5f63 6f6c 6f72 2c0a 2020  r=edge_color,.  
-0001f550: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0001f560: 7874 5f63 6f6c 6f72 203d 2074 6578 745f  xt_color = text_
-0001f570: 636f 6c6f 722c 2063 6261 7220 3d20 6362  color, cbar = cb
-0001f580: 6172 2c20 616c 7068 6120 3d20 616c 7068  ar, alpha = alph
-0001f590: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-0001f5a0: 2020 207a 6f6f 6d5f 7769 6474 6820 3d20     zoom_width = 
-0001f5b0: 7a6f 6f6d 5f77 6964 7468 2c20 7820 3d20  zoom_width, x = 
-0001f5c0: 782c 2079 203d 2079 2c20 7469 636b 733d  x, y = y, ticks=
-0001f5d0: 7469 636b 732c 0a20 2020 2020 2020 2020  ticks,.         
-0001f5e0: 2020 2020 2020 206d 6173 6b5f 7261 7374         mask_rast
-0001f5f0: 3d6d 6173 6b5f 7261 7374 290a 2020 2020  =mask_rast).    
-0001f600: 2020 2020 2020 2020 236d 616b 6520 7369          #make si
-0001f610: 7a65 2073 6d61 6c6c 6572 2066 6f72 2074  ze smaller for t
-0001f620: 6865 206e 6578 7420 6c61 7965 7220 6f66  he next layer of
-0001f630: 2069 6e6e 6572 2028 6669 746e 6573 7329   inner (fitness)
-0001f640: 2063 6972 636c 6573 0a20 2020 2020 2020   circles.       
-0001f650: 2020 2020 2073 697a 6520 3d20 726f 756e       size = roun
-0001f660: 6428 302e 342a 7369 7a65 290a 2020 2020  d(0.4*size).    
-0001f670: 2020 2020 2020 2020 2320 6765 7420 7369          # get si
-0001f680: 7a65 7320 666f 7220 616c 6c20 696e 6469  zes for all indi
-0001f690: 7669 6475 616c 7327 2069 6e6e 6572 2d63  viduals' inner-c
-0001f6a0: 6972 636c 6520 6669 746e 6573 7320 706f  ircle fitness po
-0001f6b0: 696e 7473 2c20 6966 0a20 2020 2020 2020  ints, if.       
-0001f6c0: 2020 2020 2023 2074 7274 5f6e 756d 2069       # trt_num i
-0001f6d0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0001f6e0: 2020 2020 2020 2069 6620 7472 745f 6e75         if trt_nu
-0001f6f0: 6d20 6973 206e 6f74 204e 6f6e 653a 0a20  m is not None:. 
-0001f700: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001f710: 697a 6520 3d20 7369 7a65 202a 2028 3120  ize = size * (1 
-0001f720: 2d20 2828 6e70 2e61 7272 6179 285b 2a77  - ((np.array([*w
-0001f730: 2e76 616c 7565 7328 0a20 2020 2020 2020  .values(.       
-0001f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f760: 2020 2020 2029 5d29 202d 206d 696e 5f66       )]) - min_f
-0001f770: 6974 2920 2f20 2831 202d 206d 696e 5f66  it) / (1 - min_f
-0001f780: 6974 2929 290a 0a20 2020 2020 2020 2073  it)))..        s
-0001f790: 656c 662e 5f70 6c6f 7428 6c79 725f 6e75  elf._plot(lyr_nu
-0001f7a0: 6d3d 6c79 725f 6e75 6d2c 206c 616e 643d  m=lyr_num, land=
-0001f7b0: 6c61 6e64 2c20 6869 6465 5f6c 616e 643d  land, hide_land=
-0001f7c0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0001f7d0: 2020 2020 2020 2020 2069 6e64 6976 6964           individ
-0001f7e0: 733d 696e 6469 7669 6473 2c20 7465 7874  s=individs, text
-0001f7f0: 3d74 6578 742c 2063 6f6c 6f72 3d6c 6973  =text, color=lis
-0001f800: 7428 772e 7661 6c75 6573 2829 292c 0a20  t(w.values()),. 
-0001f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f820: 2020 7074 5f63 6d61 703d 636d 6170 2c20    pt_cmap=cmap, 
-0001f830: 7369 7a65 3d73 697a 652c 2065 6467 655f  size=size, edge_
-0001f840: 636f 6c6f 723d 6564 6765 5f63 6f6c 6f72  color=edge_color
-0001f850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f860: 2020 2020 2074 6578 745f 636f 6c6f 723d       text_color=
-0001f870: 7465 7874 5f63 6f6c 6f72 2c20 6362 6172  text_color, cbar
-0001f880: 3d63 6261 722c 2074 6578 745f 7369 7a65  =cbar, text_size
-0001f890: 3d74 6578 745f 7369 7a65 2c0a 2020 2020  =text_size,.    
-0001f8a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001f8b0: 6c70 6861 3d61 6c70 6861 2c20 7a6f 6f6d  lpha=alpha, zoom
-0001f8c0: 5f77 6964 7468 3d7a 6f6f 6d5f 7769 6474  _width=zoom_widt
-0001f8d0: 682c 2078 3d78 2c20 793d 792c 2074 6963  h, x=x, y=y, tic
-0001f8e0: 6b73 3d74 6963 6b73 2c0a 2020 2020 2020  ks=ticks,.      
-0001f8f0: 2020 2020 2020 2020 2020 2020 206d 6173               mas
-0001f900: 6b5f 7261 7374 3d6d 6173 6b5f 7261 7374  k_rast=mask_rast
-0001f910: 290a 0a20 2020 2020 2020 2023 706c 6f74  )..        #plot
-0001f920: 2070 6865 6e6f 7479 7065 2074 6578 7420   phenotype text 
-0001f930: 2877 6f72 6b73 206f 6e6c 7920 6966 2070  (works only if p
-0001f940: 6c6f 7474 696e 6720 6120 7370 6563 6966  lotting a specif
-0001f950: 6963 2074 7261 6974 290a 2020 2020 2020  ic trait).      
-0001f960: 2020 6966 2070 6865 6e6f 7479 7065 5f74    if phenotype_t
-0001f970: 6578 7420 616e 6420 7472 745f 6e75 6d20  ext and trt_num 
-0001f980: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0001f990: 2020 2020 2020 2020 2066 6f72 2069 6e64           for ind
-0001f9a0: 2069 6e20 7365 6c66 2e76 616c 7565 7328   in self.values(
-0001f9b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001f9c0: 2020 2070 6c74 2e74 6578 7428 696e 642e     plt.text(ind.
-0001f9d0: 782d 302e 352c 2069 6e64 2e79 2d30 2e35  x-0.5, ind.y-0.5
-0001f9e0: 2c20 2725 302e 3266 2720 2520 696e 642e  , '%0.2f' % ind.
-0001f9f0: 7a5b 7472 745f 6e75 6d5d 2c0a 2020 2020  z[trt_num],.    
-0001fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa10: 636f 6c6f 7220 3d20 7068 656e 6f74 7970  color = phenotyp
-0001fa20: 655f 7465 7874 5f63 6f6c 6f72 2c20 7369  e_text_color, si
-0001fa30: 7a65 203d 2074 6578 745f 7369 7a65 290a  ze = text_size).
-0001fa40: 0a20 2020 2020 2020 2023 706c 6f74 2066  .        #plot f
-0001fa50: 6974 6e65 7373 2074 6578 740a 2020 2020  itness text.    
-0001fa60: 2020 2020 6966 2066 6974 6e65 7373 5f74      if fitness_t
-0001fa70: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-0001fa80: 206f 6666 7365 745f 6672 6f6d 5f70 6865   offset_from_phe
-0001fa90: 6e6f 7479 7065 5f74 6578 7420 3d20 302e  notype_text = 0.
-0001faa0: 3030 312a 6d61 7828 7365 6c66 2e5f 6c61  001*max(self._la
-0001fab0: 6e64 5f64 696d 290a 2020 2020 2020 2020  nd_dim).        
-0001fac0: 2020 2020 666f 7220 696e 6420 696e 2073      for ind in s
-0001fad0: 656c 662e 7661 6c75 6573 2829 3a0a 2020  elf.values():.  
-0001fae0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0001faf0: 742e 7465 7874 2869 6e64 2e78 2d30 2e35  t.text(ind.x-0.5
-0001fb00: 2b6f 6666 7365 745f 6672 6f6d 5f70 6865  +offset_from_phe
-0001fb10: 6e6f 7479 7065 5f74 6578 742c 0a20 2020  notype_text,.   
-0001fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb30: 2020 2020 2020 696e 642e 792d 302e 352b        ind.y-0.5+
-0001fb40: 6f66 6673 6574 5f66 726f 6d5f 7068 656e  offset_from_phen
-0001fb50: 6f74 7970 655f 7465 7874 2c0a 2020 2020  otype_text,.    
+0001e6b0: 2020 2020 2020 2020 2020 696e 6469 7669            indivi
+0001e6c0: 6473 203d 2069 6e64 6976 6964 732c 2074  ds = individs, t
+0001e6d0: 6578 7420 3d20 7465 7874 2c0a 2020 2020  ext = text,.    
+0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6f0: 2020 2020 2020 2020 636f 6c6f 7220 3d20          color = 
+0001e700: 6c69 7374 287a 2e76 616c 7565 7328 2929  list(z.values())
+0001e710: 2c20 7074 5f63 6d61 7020 3d20 7074 5f63  , pt_cmap = pt_c
+0001e720: 6d61 702c 0a20 2020 2020 2020 2020 2020  map,.           
+0001e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e740: 2065 6467 655f 636f 6c6f 7220 3d20 6564   edge_color = ed
+0001e750: 6765 5f63 6f6c 6f72 2c20 7465 7874 5f63  ge_color, text_c
+0001e760: 6f6c 6f72 203d 2074 6578 745f 636f 6c6f  olor = text_colo
+0001e770: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0001e780: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001e790: 6261 7220 3d20 6362 6172 2c20 7369 7a65  bar = cbar, size
+0001e7a0: 203d 2073 697a 652c 2074 6578 745f 7369   = size, text_si
+0001e7b0: 7a65 203d 2074 6578 745f 7369 7a65 2c0a  ze = text_size,.
+0001e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7d0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+0001e7e0: 6120 3d20 616c 7068 612c 207a 6f6f 6d5f  a = alpha, zoom_
+0001e7f0: 7769 6474 6820 3d20 7a6f 6f6d 5f77 6964  width = zoom_wid
+0001e800: 7468 2c20 7820 3d20 782c 0a20 2020 2020  th, x = x,.     
+0001e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e820: 2020 2020 2020 2079 203d 2079 2c20 766d         y = y, vm
+0001e830: 696e 203d 2030 2c20 766d 6178 203d 2031  in = 0, vmax = 1
+0001e840: 2c20 7469 636b 733d 7469 636b 732c 0a20  , ticks=ticks,. 
+0001e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e860: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
+0001e870: 7261 7374 3d6d 6173 6b5f 7261 7374 2c20  rast=mask_rast, 
+0001e880: 616e 696d 6174 653d 616e 696d 6174 6529  animate=animate)
+0001e890: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001e8a0: 2070 6f69 6e74 730a 0a0a 2020 2020 2320   points...    # 
+0001e8b0: 6d65 7468 6f64 2066 6f72 2070 6c6f 7474  method for plott
+0001e8c0: 696e 6720 696e 6469 7669 6475 616c 7320  ing individuals 
+0001e8d0: 636f 6c6f 7265 6420 6279 2074 6865 6972  colored by their
+0001e8e0: 206f 7665 7261 6c6c 2066 6974 6e65 7373   overall fitness
+0001e8f0: 6573 2c0a 2020 2020 236f 7220 6279 2074  es,.    #or by t
+0001e900: 6865 6972 2066 6974 6e65 7373 6573 2066  heir fitnesses f
+0001e910: 6f72 2061 2073 696e 676c 6520 7472 6169  or a single trai
+0001e920: 7420 2869 6620 7472 6169 7420 6973 206e  t (if trait is n
+0001e930: 6f74 204e 6f6e 6529 0a20 2020 2064 6566  ot None).    def
+0001e940: 205f 706c 6f74 5f66 6974 6e65 7373 2873   _plot_fitness(s
+0001e950: 656c 662c 2074 7274 5f6e 756d 3d4e 6f6e  elf, trt_num=Non
+0001e960: 652c 206c 7972 5f6e 756d 3d4e 6f6e 652c  e, lyr_num=None,
+0001e970: 206c 616e 643d 4e6f 6e65 2c0a 2020 2020   land=None,.    
+0001e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e990: 2020 696e 6469 7669 6473 3d4e 6f6e 652c    individs=None,
+0001e9a0: 2074 6578 743d 4661 6c73 652c 2070 6865   text=False, phe
+0001e9b0: 6e6f 7479 7065 5f74 6578 743d 4661 6c73  notype_text=Fals
+0001e9c0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001e9d0: 2020 2020 2020 2020 2070 6865 6e6f 7479           phenoty
+0001e9e0: 7065 5f74 6578 745f 636f 6c6f 723d 2762  pe_text_color='b
+0001e9f0: 6c61 636b 272c 2066 6974 6e65 7373 5f74  lack', fitness_t
+0001ea00: 6578 743d 4661 6c73 652c 0a20 2020 2020  ext=False,.     
+0001ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea20: 2066 6974 6e65 7373 5f74 6578 745f 636f   fitness_text_co
+0001ea30: 6c6f 723d 2723 3333 3333 3333 272c 2073  lor='#333333', s
+0001ea40: 697a 653d 3130 302c 2074 6578 745f 7369  ize=100, text_si
+0001ea50: 7a65 203d 2039 2c0a 2020 2020 2020 2020  ze = 9,.        
+0001ea60: 2020 2020 2020 2020 2020 2020 2020 6564                ed
+0001ea70: 6765 5f63 6f6c 6f72 3d27 626c 6163 6b27  ge_color='black'
+0001ea80: 2c20 7465 7874 5f63 6f6c 6f72 3d27 626c  , text_color='bl
+0001ea90: 6163 6b27 2c0a 2020 2020 2020 2020 2020  ack',.          
+0001eaa0: 2020 2020 2020 2020 2020 2020 6669 745f              fit_
+0001eab0: 636d 6170 203d 2027 5264 596c 476e 272c  cmap = 'RdYlGn',
+0001eac0: 2063 6261 723d 5472 7565 2c20 6669 746e   cbar=True, fitn
+0001ead0: 6573 735f 6362 6172 3d54 7275 652c 0a20  ess_cbar=True,. 
+0001eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eaf0: 2020 2020 2061 6c70 6861 3d31 2c20 7a6f       alpha=1, zo
+0001eb00: 6f6d 5f77 6964 7468 3d4e 6f6e 652c 2078  om_width=None, x
+0001eb10: 3d4e 6f6e 652c 2079 3d4e 6f6e 652c 2074  =None, y=None, t
+0001eb20: 6963 6b73 3d4e 6f6e 652c 0a20 2020 2020  icks=None,.     
+0001eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb40: 206d 6173 6b5f 7261 7374 3d4e 6f6e 6529   mask_rast=None)
+0001eb50: 3a0a 0a20 2020 2020 2020 2023 7265 7475  :..        #retu
+0001eb60: 726e 206d 6573 7361 6765 7320 6966 2073  rn messages if s
+0001eb70: 7065 6369 6573 2064 6f65 7320 6e6f 7420  pecies does not 
+0001eb80: 6861 7665 2067 656e 6f6d 6573 206f 7220  have genomes or 
+0001eb90: 7472 6169 7473 0a20 2020 2020 2020 2069  traits.        i
+0001eba0: 6620 7365 6c66 2e67 656e 5f61 7263 6820  f self.gen_arch 
+0001ebb0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0001ebc0: 2020 2020 2070 7269 6e74 2828 2253 7065       print(("Spe
+0001ebd0: 6369 6573 2e5f 706c 6f74 5f66 6974 6e65  cies._plot_fitne
+0001ebe0: 7373 2069 7320 6e6f 7420 7661 6c69 6420  ss is not valid 
+0001ebf0: 666f 7220 7370 6563 6965 7320 220a 2020  for species ".  
+0001ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec10: 2022 7769 7468 6f75 7420 6765 6e6f 6d65   "without genome
+0001ec20: 732e 5c6e 2229 290a 2020 2020 2020 2020  s.\n")).        
+0001ec30: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0001ec40: 2020 2065 6c69 6620 7365 6c66 2e67 656e     elif self.gen
+0001ec50: 5f61 7263 682e 7472 6169 7473 2069 7320  _arch.traits is 
+0001ec60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001ec70: 2020 7072 696e 7428 2822 5370 6563 6965    print(("Specie
+0001ec80: 732e 5f70 6c6f 745f 6669 746e 6573 7320  s._plot_fitness 
+0001ec90: 6973 206e 6f74 2076 616c 6964 2066 6f72  is not valid for
+0001eca0: 2073 7065 6369 6573 2022 0a20 2020 2020   species ".     
+0001ecb0: 2020 2020 2020 2020 2020 2020 2020 2277                "w
+0001ecc0: 6974 686f 7574 2074 7261 6974 732e 5c6e  ithout traits.\n
+0001ecd0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+0001ece0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
+0001ecf0: 2320 6765 7420 7468 6520 7472 6169 7427  # get the trait'
+0001ed00: 7320 6c79 725f 6e75 6d2c 2069 6620 6c79  s lyr_num, if ly
+0001ed10: 725f 6e75 6d20 7761 736e 2774 2070 726f  r_num wasn't pro
+0001ed20: 7669 6465 6420 6275 7420 7472 745f 6e75  vided but trt_nu
+0001ed30: 6d20 7761 730a 2020 2020 2020 2020 6966  m was.        if
+0001ed40: 2074 7274 5f6e 756d 2069 7320 6e6f 7420   trt_num is not 
+0001ed50: 4e6f 6e65 2061 6e64 206c 7972 5f6e 756d  None and lyr_num
+0001ed60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001ed70: 2020 2020 2020 6c79 725f 6e75 6d20 3d20        lyr_num = 
+0001ed80: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
+0001ed90: 6169 7473 5b74 7274 5f6e 756d 5d2e 6c79  aits[trt_num].ly
+0001eda0: 725f 6e75 6d0a 0a20 2020 2020 2020 2023  r_num..        #
+0001edb0: 2067 6574 2061 6c6c 2069 6e64 6976 6964   get all individ
+0001edc0: 7327 2066 6974 6e65 7373 2076 616c 7565  s' fitness value
+0001edd0: 732c 0a20 2020 2020 2020 2023 2061 6e64  s,.        # and
+0001ede0: 2067 6574 2061 7070 726f 7072 6961 7465   get appropriate
+0001edf0: 2063 6f6c 6f72 6d61 700a 2020 2020 2020   colormap.      
+0001ee00: 2020 6966 2074 7274 5f6e 756d 2069 7320    if trt_num is 
+0001ee10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001ee20: 2020 7720 3d20 7365 6c66 2e5f 6361 6c63    w = self._calc
+0001ee30: 5f66 6974 6e65 7373 2829 0a20 2020 2020  _fitness().     
+0001ee40: 2020 2020 2020 2070 745f 636d 6170 203d         pt_cmap =
+0001ee50: 2027 4772 6579 735f 7227 0a20 2020 2020   'Greys_r'.     
+0001ee60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001ee70: 2020 2020 2077 203d 2073 656c 662e 5f63       w = self._c
+0001ee80: 616c 635f 6669 746e 6573 7328 7472 6169  alc_fitness(trai
+0001ee90: 745f 6e75 6d20 3d20 7472 745f 6e75 6d29  t_num = trt_num)
+0001eea0: 0a0a 2020 2020 2020 2020 2366 696c 7465  ..        #filte
+0001eeb0: 7220 6f75 7420 756e 7761 6e74 6564 2069  r out unwanted i
+0001eec0: 6e64 6976 6964 732c 2069 6620 6e65 6365  ndivids, if nece
+0001eed0: 7373 6172 790a 2020 2020 2020 2020 7720  ssary.        w 
+0001eee0: 3d20 4f44 287a 6970 285b 2a73 656c 665d  = OD(zip([*self]
+0001eef0: 2c20 7729 290a 2020 2020 2020 2020 6966  , w)).        if
+0001ef00: 2069 6e64 6976 6964 7320 6973 206e 6f74   individs is not
+0001ef10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001ef20: 2020 2077 203d 207b 693a 7620 666f 7220     w = {i:v for 
+0001ef30: 692c 7620 696e 2077 2e69 7465 6d73 2829  i,v in w.items()
+0001ef40: 2069 6620 6920 696e 2069 6e64 6976 6964   if i in individ
+0001ef50: 737d 0a0a 2020 2020 2020 2020 2320 6361  s}..        # ca
+0001ef60: 6c63 206d 696e 696d 756d 2070 6f73 7369  lc minimum possi
+0001ef70: 626c 6520 6669 746e 6573 7320 2866 6f72  ble fitness (for
+0001ef80: 2070 6865 6e6f 7479 7065 7320 7769 7468   phenotypes with
+0001ef90: 696e 2030 203c 3d20 7a20 3c3d 2031 2c0a  in 0 <= z <= 1,.
+0001efa0: 2020 2020 2020 2020 2377 6869 6368 2069          #which i
+0001efb0: 6e20 7265 616c 6974 7920 6973 6e27 7420  n reality isn't 
+0001efc0: 6120 636f 6e73 7472 6169 6e74 2c20 6275  a constraint, bu
+0001efd0: 7420 7661 6c75 6573 206c 6f77 6572 2074  t values lower t
+0001efe0: 6861 6e0a 2020 2020 2020 2020 2374 6869  han.        #thi
+0001eff0: 7320 7769 6c6c 2061 6c73 6f20 6265 2063  s will also be c
+0001f000: 6f6e 7374 7261 696e 6564 2074 6f20 7468  onstrained to th
+0001f010: 6520 6d69 6e69 6d75 6d2d 7661 6c75 6520  e minimum-value 
+0001f020: 636f 6c6f 7220 666f 7220 706c 6f74 7469  color for plotti
+0001f030: 6e67 290a 2020 2020 2020 2020 234e 4f54  ng).        #NOT
+0001f040: 453a 2074 6865 206e 702e 6174 6c65 6173  E: the np.atleas
+0001f050: 745f 3264 282e 2e2e 292e 6d69 6e28 2920  t_2d(...).min() 
+0001f060: 636f 6e73 7472 7563 7420 6d61 6b65 7320  construct makes 
+0001f070: 7468 6973 0a20 2020 2020 2020 2023 776f  this.        #wo
+0001f080: 726b 2062 6f74 6820 666f 7220 6669 7865  rk both for fixe
+0001f090: 6420 616e 6420 7370 6174 6961 6c6c 7920  d and spatially 
+0001f0a0: 7661 7279 696e 6720 7068 690a 2020 2020  varying phi.    
+0001f0b0: 2020 2020 6966 2074 7274 5f6e 756d 2069      if trt_num i
+0001f0c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0001f0d0: 2020 2020 6d69 6e5f 6669 7420 3d20 6e70      min_fit = np
+0001f0e0: 2e70 726f 6475 6374 285b 3120 2d20 6e70  .product([1 - np
+0001f0f0: 2e61 746c 6561 7374 5f32 6428 742e 7068  .atleast_2d(t.ph
+0001f100: 6929 2e6d 696e 280a 2020 2020 2020 2020  i).min(.        
+0001f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f120: 2020 2020 2920 666f 7220 7420 696e 206c      ) for t in l
+0001f130: 6973 7428 7365 6c66 2e67 656e 5f61 7263  ist(self.gen_arc
+0001f140: 682e 7472 6169 7473 2e76 616c 7565 7328  h.traits.values(
+0001f150: 2929 5d29 0a20 2020 2020 2020 2065 6c73  ))]).        els
+0001f160: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+0001f170: 696e 5f66 6974 203d 2031 202d 206e 702e  in_fit = 1 - np.
+0001f180: 6174 6c65 6173 745f 3264 2873 656c 662e  atleast_2d(self.
+0001f190: 6765 6e5f 6172 6368 2e74 7261 6974 735b  gen_arch.traits[
+0001f1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f1d0: 2020 2020 2020 2020 2074 7274 5f6e 756d           trt_num
+0001f1e0: 5d2e 7068 6929 2e6d 696e 2829 0a0a 2020  ].phi).min()..  
+0001f1f0: 2020 2020 2020 2374 6865 6e20 6765 7420        #then get 
+0001f200: 756e 6576 656e 2063 6d61 7020 616e 6420  uneven cmap and 
+0001f210: 6362 6172 2d6d 616b 6572 2028 6e65 6564  cbar-maker (need
+0001f220: 7320 746f 2062 6520 756e 6576 656e 2074  s to be uneven t
+0001f230: 6f0a 2020 2020 2020 2020 2367 6976 6520  o.        #give 
+0001f240: 636f 6c6f 722d 7265 736f 6c75 7469 6f6e  color-resolution
+0001f250: 2074 6f20 7661 6c75 6573 2076 6172 7969   to values varyi
+0001f260: 6e67 0a20 2020 2020 2020 2023 6265 7477  ng.        #betw
+0001f270: 6565 6e20 3120 616e 6420 7468 6520 6d69  een 1 and the mi
+0001f280: 6e69 6d75 6d2d 6669 746e 6573 7320 7661  nimum-fitness va
+0001f290: 6c75 6520 6173 7375 6d69 6e67 2061 6c6c  lue assuming all
+0001f2a0: 0a20 2020 2020 2020 2023 7068 656e 6f74  .        #phenot
+0001f2b0: 7970 6573 2061 7265 2063 6f6e 7374 7261  ypes are constra
+0001f2c0: 696e 6564 2030 3c3d 7a3c 3d31 2c20 6275  ined 0<=z<=1, bu
+0001f2d0: 7420 7468 656e 2061 6c73 6f0a 2020 2020  t then also.    
+0001f2e0: 2020 2020 2361 6c6c 6f77 2067 7261 6475      #allow gradu
+0001f2f0: 616c 6c79 2064 6565 7065 6e69 6e67 2072  ally deepening r
+0001f300: 6564 7320 666f 7220 6669 746e 6573 7320  eds for fitness 
+0001f310: 7661 6c75 6573 206c 6f77 6572 0a20 2020  values lower.   
+0001f320: 2020 2020 2023 7468 616e 2074 6861 7420       #than that 
+0001f330: 6d69 6e69 6d75 6d20 7661 6c75 6529 2c20  minimum value), 
+0001f340: 7573 696e 6720 7468 6520 6d69 6e5f 6669  using the min_fi
+0001f350: 7420 7661 6c0a 2020 2020 2020 2020 636d  t val.        cm
+0001f360: 6170 2c20 6d61 6b65 5f63 6261 725f 666e  ap, make_cbar_fn
+0001f370: 203d 2076 697a 2e5f 6d61 6b65 5f66 6974   = viz._make_fit
+0001f380: 6e65 7373 5f63 6d61 705f 616e 645f 6362  ness_cmap_and_cb
+0001f390: 6172 5f6d 616b 6572 280a 2020 2020 2020  ar_maker(.      
+0001f3a0: 2020 2020 2020 6d69 6e5f 7661 6c20 3d20        min_val = 
+0001f3b0: 6d69 6e5f 6669 742c 206d 6178 5f76 616c  min_fit, max_val
+0001f3c0: 203d 2031 2c20 636d 6170 203d 2066 6974   = 1, cmap = fit
+0001f3d0: 5f63 6d61 702c 0a20 2020 2020 2020 2020  _cmap,.         
+0001f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f400: 2020 2020 2020 2074 7274 5f6e 756d 203d         trt_num =
+0001f410: 2074 7274 5f6e 756d 290a 0a20 2020 2020   trt_num)..     
+0001f420: 2020 2023 706c 6f74 2074 6865 2074 7261     #plot the tra
+0001f430: 6974 2070 6865 6e6f 7479 7065 2069 6e20  it phenotype in 
+0001f440: 6c61 7267 6572 2063 6972 636c 6573 2066  larger circles f
+0001f450: 6972 7374 2c20 6966 2074 7261 6974 2069  irst, if trait i
+0001f460: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+0001f470: 2020 2069 6620 7472 745f 6e75 6d20 6973     if trt_num is
+0001f480: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001f490: 2020 2020 2020 2023 706c 6f74 2074 6865         #plot the
+0001f4a0: 206f 7574 6572 2028 7068 656e 6f74 7970   outer (phenotyp
+0001f4b0: 6529 2063 6972 636c 6573 0a20 2020 2020  e) circles.     
+0001f4c0: 2020 2020 2020 2073 656c 662e 5f70 6c6f         self._plo
+0001f4d0: 745f 7068 656e 6f74 7970 6528 7472 6169  t_phenotype(trai
+0001f4e0: 7420 3d20 7472 745f 6e75 6d2c 206c 7972  t = trt_num, lyr
+0001f4f0: 5f6e 756d 203d 206c 7972 5f6e 756d 2c0a  _num = lyr_num,.
+0001f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f510: 6c61 6e64 203d 206c 616e 642c 2069 6e64  land = land, ind
+0001f520: 6976 6964 7320 3d20 696e 6469 7669 6473  ivids = individs
+0001f530: 2c20 7465 7874 203d 2046 616c 7365 2c20  , text = False, 
+0001f540: 7369 7a65 203d 2073 697a 652c 0a20 2020  size = size,.   
+0001f550: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0001f560: 745f 7369 7a65 203d 2074 6578 745f 7369  t_size = text_si
+0001f570: 7a65 2c20 6564 6765 5f63 6f6c 6f72 3d65  ze, edge_color=e
+0001f580: 6467 655f 636f 6c6f 722c 0a20 2020 2020  dge_color,.     
+0001f590: 2020 2020 2020 2020 2020 2074 6578 745f             text_
+0001f5a0: 636f 6c6f 7220 3d20 7465 7874 5f63 6f6c  color = text_col
+0001f5b0: 6f72 2c20 6362 6172 203d 2063 6261 722c  or, cbar = cbar,
+0001f5c0: 2061 6c70 6861 203d 2061 6c70 6861 2c0a   alpha = alpha,.
+0001f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f5e0: 7a6f 6f6d 5f77 6964 7468 203d 207a 6f6f  zoom_width = zoo
+0001f5f0: 6d5f 7769 6474 682c 2078 203d 2078 2c20  m_width, x = x, 
+0001f600: 7920 3d20 792c 2074 6963 6b73 3d74 6963  y = y, ticks=tic
+0001f610: 6b73 2c0a 2020 2020 2020 2020 2020 2020  ks,.            
+0001f620: 2020 2020 6d61 736b 5f72 6173 743d 6d61      mask_rast=ma
+0001f630: 736b 5f72 6173 7429 0a20 2020 2020 2020  sk_rast).       
+0001f640: 2020 2020 2023 6d61 6b65 2073 697a 6520       #make size 
+0001f650: 736d 616c 6c65 7220 666f 7220 7468 6520  smaller for the 
+0001f660: 6e65 7874 206c 6179 6572 206f 6620 696e  next layer of in
+0001f670: 6e65 7220 2866 6974 6e65 7373 2920 6369  ner (fitness) ci
+0001f680: 7263 6c65 730a 2020 2020 2020 2020 2020  rcles.          
+0001f690: 2020 7369 7a65 203d 2072 6f75 6e64 2830    size = round(0
+0001f6a0: 2e34 2a73 697a 6529 0a20 2020 2020 2020  .4*size).       
+0001f6b0: 2020 2020 2023 2067 6574 2073 697a 6573       # get sizes
+0001f6c0: 2066 6f72 2061 6c6c 2069 6e64 6976 6964   for all individ
+0001f6d0: 7561 6c73 2720 696e 6e65 722d 6369 7263  uals' inner-circ
+0001f6e0: 6c65 2066 6974 6e65 7373 2070 6f69 6e74  le fitness point
+0001f6f0: 732c 2069 660a 2020 2020 2020 2020 2020  s, if.          
+0001f700: 2020 2320 7472 745f 6e75 6d20 6973 206e    # trt_num is n
+0001f710: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0001f720: 2020 2020 6966 2074 7274 5f6e 756d 2069      if trt_num i
+0001f730: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0001f740: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+0001f750: 203d 2073 697a 6520 2a20 2831 202d 2028   = size * (1 - (
+0001f760: 286e 702e 6172 7261 7928 5b2a 772e 7661  (np.array([*w.va
+0001f770: 6c75 6573 280a 2020 2020 2020 2020 2020  lues(.          
+0001f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f7a0: 2020 295d 2920 2d20 6d69 6e5f 6669 7429    )]) - min_fit)
+0001f7b0: 202f 2028 3120 2d20 6d69 6e5f 6669 7429   / (1 - min_fit)
+0001f7c0: 2929 0a0a 2020 2020 2020 2020 7365 6c66  ))..        self
+0001f7d0: 2e5f 706c 6f74 286c 7972 5f6e 756d 3d6c  ._plot(lyr_num=l
+0001f7e0: 7972 5f6e 756d 2c20 6c61 6e64 3d6c 616e  yr_num, land=lan
+0001f7f0: 642c 2068 6964 655f 6c61 6e64 3d54 7275  d, hide_land=Tru
+0001f800: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001f810: 2020 2020 2020 696e 6469 7669 6473 3d69        individs=i
+0001f820: 6e64 6976 6964 732c 2074 6578 743d 7465  ndivids, text=te
+0001f830: 7874 2c20 636f 6c6f 723d 6c69 7374 2877  xt, color=list(w
+0001f840: 2e76 616c 7565 7328 2929 2c0a 2020 2020  .values()),.    
+0001f850: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001f860: 745f 636d 6170 3d63 6d61 702c 2073 697a  t_cmap=cmap, siz
+0001f870: 653d 7369 7a65 2c20 6564 6765 5f63 6f6c  e=size, edge_col
+0001f880: 6f72 3d65 6467 655f 636f 6c6f 722c 0a20  or=edge_color,. 
+0001f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f8a0: 2020 7465 7874 5f63 6f6c 6f72 3d74 6578    text_color=tex
+0001f8b0: 745f 636f 6c6f 722c 2063 6261 723d 6362  t_color, cbar=cb
+0001f8c0: 6172 2c20 7465 7874 5f73 697a 653d 7465  ar, text_size=te
+0001f8d0: 7874 5f73 697a 652c 0a20 2020 2020 2020  xt_size,.       
+0001f8e0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+0001f8f0: 613d 616c 7068 612c 207a 6f6f 6d5f 7769  a=alpha, zoom_wi
+0001f900: 6474 683d 7a6f 6f6d 5f77 6964 7468 2c20  dth=zoom_width, 
+0001f910: 783d 782c 2079 3d79 2c20 7469 636b 733d  x=x, y=y, ticks=
+0001f920: 7469 636b 732c 0a20 2020 2020 2020 2020  ticks,.         
+0001f930: 2020 2020 2020 2020 2020 6d61 736b 5f72            mask_r
+0001f940: 6173 743d 6d61 736b 5f72 6173 7429 0a0a  ast=mask_rast)..
+0001f950: 2020 2020 2020 2020 2370 6c6f 7420 7068          #plot ph
+0001f960: 656e 6f74 7970 6520 7465 7874 2028 776f  enotype text (wo
+0001f970: 726b 7320 6f6e 6c79 2069 6620 706c 6f74  rks only if plot
+0001f980: 7469 6e67 2061 2073 7065 6369 6669 6320  ting a specific 
+0001f990: 7472 6169 7429 0a20 2020 2020 2020 2069  trait).        i
+0001f9a0: 6620 7068 656e 6f74 7970 655f 7465 7874  f phenotype_text
+0001f9b0: 2061 6e64 2074 7274 5f6e 756d 2069 7320   and trt_num is 
+0001f9c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001f9d0: 2020 2020 2020 666f 7220 696e 6420 696e        for ind in
+0001f9e0: 2073 656c 662e 7661 6c75 6573 2829 3a0a   self.values():.
+0001f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fa00: 706c 742e 7465 7874 2869 6e64 2e78 2d30  plt.text(ind.x-0
+0001fa10: 2e35 2c20 696e 642e 792d 302e 352c 2027  .5, ind.y-0.5, '
+0001fa20: 2530 2e32 6627 2025 2069 6e64 2e7a 5b74  %0.2f' % ind.z[t
+0001fa30: 7274 5f6e 756d 5d2c 0a20 2020 2020 2020  rt_num],.       
+0001fa40: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+0001fa50: 6f72 203d 2070 6865 6e6f 7479 7065 5f74  or = phenotype_t
+0001fa60: 6578 745f 636f 6c6f 722c 2073 697a 6520  ext_color, size 
+0001fa70: 3d20 7465 7874 5f73 697a 6529 0a0a 2020  = text_size)..  
+0001fa80: 2020 2020 2020 2370 6c6f 7420 6669 746e        #plot fitn
+0001fa90: 6573 7320 7465 7874 0a20 2020 2020 2020  ess text.       
+0001faa0: 2069 6620 6669 746e 6573 735f 7465 7874   if fitness_text
+0001fab0: 3a0a 2020 2020 2020 2020 2020 2020 6f66  :.            of
+0001fac0: 6673 6574 5f66 726f 6d5f 7068 656e 6f74  fset_from_phenot
+0001fad0: 7970 655f 7465 7874 203d 2030 2e30 3031  ype_text = 0.001
+0001fae0: 2a6d 6178 2873 656c 662e 5f6c 616e 645f  *max(self._land_
+0001faf0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+0001fb00: 2066 6f72 2069 6e64 2069 6e20 7365 6c66   for ind in self
+0001fb10: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
+0001fb20: 2020 2020 2020 2020 2020 2070 6c74 2e74             plt.t
+0001fb30: 6578 7428 696e 642e 782d 302e 352b 6f66  ext(ind.x-0.5+of
+0001fb40: 6673 6574 5f66 726f 6d5f 7068 656e 6f74  fset_from_phenot
+0001fb50: 7970 655f 7465 7874 2c0a 2020 2020 2020  ype_text,.      
 0001fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb70: 2020 2020 2027 2530 2e32 6627 2025 2069       '%0.2f' % i
-0001fb80: 6e64 2e66 6974 2c20 636f 6c6f 7220 3d20  nd.fit, color = 
-0001fb90: 6669 746e 6573 735f 7465 7874 5f63 6f6c  fitness_text_col
-0001fba0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-0001fbb0: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-0001fbc0: 6520 3d20 7465 7874 5f73 697a 6529 0a0a  e = text_size)..
-0001fbd0: 2020 2020 2020 2020 2361 6e64 206d 616b          #and mak
-0001fbe0: 6520 6120 636f 6c6f 7262 6172 2066 6f72  e a colorbar for
-0001fbf0: 2074 6865 2066 6974 6e65 7373 2076 616c   the fitness val
-0001fc00: 7565 7320 0a20 2020 2020 2020 2069 6620  ues .        if 
-0001fc10: 6669 746e 6573 735f 6362 6172 3a0a 2020  fitness_cbar:.  
-0001fc20: 2020 2020 2020 2020 2020 7669 7a2e 5f6d            viz._m
-0001fc30: 616b 655f 6669 746e 6573 735f 6362 6172  ake_fitness_cbar
-0001fc40: 286d 616b 655f 6362 6172 5f66 6e2c 206d  (make_cbar_fn, m
-0001fc50: 696e 5f66 6974 290a 0a20 2020 2023 6d65  in_fit)..    #me
-0001fc60: 7468 6f64 2074 6f20 706c 6f74 2061 2073  thod to plot a s
-0001fc70: 7065 6369 6573 2720 616c 6c65 6c65 2066  pecies' allele f
-0001fc80: 7265 7175 656e 6369 6573 0a20 2020 2064  requencies.    d
-0001fc90: 6566 205f 706c 6f74 5f61 6c6c 656c 655f  ef _plot_allele_
-0001fca0: 6672 6571 7565 6e63 6965 7328 7365 6c66  frequencies(self
-0001fcb0: 2c20 636f 6c6f 723d 2772 6564 2729 3a0a  , color='red'):.
-0001fcc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001fcd0: 6765 6e5f 6172 6368 2069 7320 4e6f 6e65  gen_arch is None
-0001fce0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0001fcf0: 696e 7428 2822 5370 6563 6965 732e 5f70  int(("Species._p
-0001fd00: 6c6f 745f 616c 6c65 6c65 5f66 7265 7175  lot_allele_frequ
-0001fd10: 656e 6369 6573 2069 7320 6e6f 7420 7661  encies is not va
-0001fd20: 6c69 6420 666f 7220 220a 2020 2020 2020  lid for ".      
-0001fd30: 2020 2020 2020 2020 2020 2020 2022 7370               "sp
-0001fd40: 6563 6965 7320 7769 7468 6f75 7420 6765  ecies without ge
-0001fd50: 6e6f 6d65 732e 5c6e 2229 290a 2020 2020  nomes.\n")).    
-0001fd60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001fd70: 2020 2020 2020 7365 6c66 2e67 656e 5f61        self.gen_a
-0001fd80: 7263 682e 5f70 6c6f 745f 616c 6c65 6c65  rch._plot_allele
-0001fd90: 5f66 7265 7175 656e 6369 6573 2873 656c  _frequencies(sel
-0001fda0: 662c 2063 6f6c 6f72 3d63 6f6c 6f72 290a  f, color=color).
-0001fdb0: 0a20 2020 2023 206d 6574 686f 6420 666f  .    # method fo
-0001fdc0: 7220 706c 6f74 7469 6e67 2061 2068 6973  r plotting a his
-0001fdd0: 746f 6772 616d 206f 6620 7468 6520 6375  togram of the cu
-0001fde0: 7272 656e 7420 6669 746e 6573 7320 7661  rrent fitness va
-0001fdf0: 6c75 6573 0a20 2020 2064 6566 205f 706c  lues.    def _pl
-0001fe00: 6f74 5f68 6973 745f 6669 746e 6573 7328  ot_hist_fitness(
-0001fe10: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0001fe20: 6c74 2e68 6973 7428 6c69 7374 2873 656c  lt.hist(list(sel
-0001fe30: 662e 5f63 616c 635f 6669 746e 6573 7328  f._calc_fitness(
-0001fe40: 2929 290a 2020 2020 2020 2020 706c 742e  ))).        plt.
-0001fe50: 786c 6162 656c 2827 4669 746e 6573 7327  xlabel('Fitness'
-0001fe60: 290a 2020 2020 2020 2020 706c 742e 796c  ).        plt.yl
-0001fe70: 6162 656c 2827 436f 756e 7427 290a 0a20  abel('Count').. 
-0001fe80: 2020 2023 206d 6574 686f 6420 666f 7220     # method for 
-0001fe90: 706c 6f74 7469 6e67 2074 6865 206d 6f76  plotting the mov
-0001fea0: 656d 656e 7420 7375 7266 6163 6520 2869  ement surface (i
-0001feb0: 6e20 7661 7269 6f75 7320 666f 726d 6174  n various format
-0001fec0: 7329 0a20 2020 2064 6566 205f 706c 6f74  s).    def _plot
-0001fed0: 5f64 6972 6563 7469 6f6e 5f73 7572 6661  _direction_surfa
-0001fee0: 6365 2873 656c 662c 206c 616e 642c 2073  ce(self, land, s
-0001fef0: 7572 665f 7479 7065 2c20 7374 796c 652c  urf_type, style,
-0001ff00: 2078 3d4e 6f6e 652c 2079 3d4e 6f6e 652c   x=None, y=None,
-0001ff10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff30: 207a 6f6f 6d5f 7769 6474 683d 4e6f 6e65   zoom_width=None
-0001ff40: 2c20 7363 616c 655f 6661 6374 3d34 2e35  , scale_fact=4.5
-0001ff50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff70: 2020 636f 6c6f 723d 2762 6c61 636b 272c    color='black',
-0001ff80: 2063 6261 723d 5472 7565 2c20 7469 636b   cbar=True, tick
-0001ff90: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffb0: 2020 2020 2020 2020 636d 6170 3d27 706c          cmap='pl
-0001ffc0: 6173 6d61 272c 206d 6173 6b5f 7261 7374  asma', mask_rast
-0001ffd0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0001ffe0: 2320 6765 7420 7468 6520 636f 7272 6563  # get the correc
-0001fff0: 7420 7375 7266 6163 650a 2020 2020 2020  t surface.      
-00020000: 2020 6966 2073 7572 665f 7479 7065 203d    if surf_type =
-00020010: 3d20 276d 6f76 6527 3a0a 2020 2020 2020  = 'move':.      
-00020020: 2020 2020 2020 7375 7266 203d 2073 656c        surf = sel
-00020030: 662e 5f6d 6f76 655f 7375 7266 0a20 2020  f._move_surf.   
-00020040: 2020 2020 2065 6c69 6620 7375 7266 5f74       elif surf_t
-00020050: 7970 6520 3d3d 2027 6469 7370 273a 0a20  ype == 'disp':. 
-00020060: 2020 2020 2020 2020 2020 2073 7572 6620             surf 
-00020070: 3d3d 2073 656c 662e 5f64 6973 705f 7375  == self._disp_su
-00020080: 7266 0a0a 2020 2020 2020 2020 2320 6765  rf..        # ge
-00020090: 7420 616c 6c20 7827 7320 616e 6420 7927  t all x's and y'
-000200a0: 732c 2069 6620 7820 616e 6420 7920 6172  s, if x and y ar
-000200b0: 6520 4e6f 6e65 0a20 2020 2020 2020 2069  e None.        i
-000200c0: 6620 7820 6973 204e 6f6e 6520 616e 6420  f x is None and 
-000200d0: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
-000200e0: 2020 2020 2020 2078 203d 205b 2a72 616e         x = [*ran
-000200f0: 6765 286c 616e 642e 6469 6d5b 305d 295d  ge(land.dim[0])]
-00020100: 0a20 2020 2020 2020 2020 2020 2079 203d  .            y =
-00020110: 205b 2a72 616e 6765 286c 616e 642e 6469   [*range(land.di
-00020120: 6d5b 315d 295d 0a20 2020 2020 2020 2065  m[1])].        e
-00020130: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00020140: 2078 203d 205b 785d 0a20 2020 2020 2020   x = [x].       
-00020150: 2020 2020 2079 203d 205b 795d 0a20 2020       y = [y].   
-00020160: 2020 2020 2023 6368 6563 6b20 6966 2074       #check if t
-00020170: 6865 2073 7572 6661 6365 2069 7320 6e6f  he surface is no
-00020180: 6e65 0a20 2020 2020 2020 2069 6620 7375  ne.        if su
-00020190: 7266 2069 7320 4e6f 6e65 3a0a 2020 2020  rf is None:.    
-000201a0: 2020 2020 2020 2020 7072 696e 7428 2827          print(('
-000201b0: 4675 6e63 7469 6f6e 206e 6f74 2076 616c  Function not val
-000201c0: 6964 2066 6f72 2061 2053 7065 6369 6573  id for a Species
-000201d0: 2077 6974 6820 6e6f 2027 0a20 2020 2020   with no '.     
-000201e0: 2020 2020 2020 2020 2020 2020 2020 275f                '_
-000201f0: 2573 5375 7266 6163 652e 2729 2025 2028  %sSurface.') % (
-00020200: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00020210: 2020 276d 6f76 6527 3a20 274d 6f76 656d    'move': 'Movem
-00020220: 656e 7427 2c20 2764 6973 7027 3a20 2744  ent', 'disp': 'D
-00020230: 6973 7065 7273 616c 277d 5b73 7572 665f  ispersal'}[surf_
-00020240: 7479 7065 5d29 290a 2020 2020 2020 2020  type])).        
-00020250: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00020260: 2020 2065 6c69 6620 7374 796c 6520 6e6f     elif style no
-00020270: 7420 696e 205b 2768 6973 7427 2c20 2763  t in ['hist', 'c
-00020280: 6869 7374 272c 2027 7665 6374 272c 2027  hist', 'vect', '
-00020290: 6364 7261 7773 275d 3a0a 2020 2020 2020  cdraws']:.      
-000202a0: 2020 2020 2020 7072 696e 7428 2822 5468        print(("Th
-000202b0: 6520 2773 7479 6c65 2720 6172 6775 6d65  e 'style' argume
-000202c0: 6e74 206d 7573 7420 7461 6b65 206f 6e65  nt must take one
-000202d0: 206f 6620 7468 6520 220a 2020 2020 2020   of the ".      
-000202e0: 2020 2020 2020 2020 2020 2020 2022 666f               "fo
-000202f0: 6c6c 6f77 696e 6720 7661 6c75 6573 3a20  llowing values: 
-00020300: 2768 6973 7427 2c20 2763 6869 7374 272c  'hist', 'chist',
-00020310: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00020320: 2020 2020 2020 2227 7665 6374 272c 2027        "'vect', '
-00020330: 6364 7261 7773 2722 2929 0a20 2020 2020  cdraws'")).     
-00020340: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00020350: 2020 2020 2020 656c 6966 2073 7479 6c65        elif style
-00020360: 203d 3d20 2768 6973 7427 3a0a 2020 2020   == 'hist':.    
-00020370: 2020 2020 2020 2020 7820 3d20 785b 305d          x = x[0]
-00020380: 0a20 2020 2020 2020 2020 2020 2079 203d  .            y =
-00020390: 2079 5b30 5d0a 2020 2020 2020 2020 2020   y[0].          
-000203a0: 2020 706c 742e 6869 7374 2872 2e63 686f    plt.hist(r.cho
-000203b0: 6963 6528 7375 7266 2e73 7572 665b 792c  ice(surf.surf[y,
-000203c0: 782c 3a5d 2c20 7369 7a65 203d 2031 3030  x,:], size = 100
-000203d0: 3030 2c20 7265 706c 6163 6520 3d20 5472  00, replace = Tr
-000203e0: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-000203f0: 2020 2020 2020 2020 2020 6269 6e73 3d31            bins=1
-00020400: 3030 2c20 6465 6e73 6974 793d 5472 7565  00, density=True
-00020410: 2c20 616c 7068 613d 302e 352c 2063 6f6c  , alpha=0.5, col
-00020420: 6f72 3d63 6f6c 6f72 290a 0a20 2020 2020  or=color)..     
-00020430: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00020440: 2020 2020 2023 6469 7370 6c61 7920 7468       #display th
-00020450: 6520 6d6f 7665 6d65 6e74 2d73 7572 6661  e movement-surfa
-00020460: 6365 2072 6173 7465 720a 2020 2020 2020  ce raster.      
-00020470: 2020 2020 2020 6c79 725f 6e75 6d20 3d20        lyr_num = 
-00020480: 7375 7266 2e6c 7972 5f6e 756d 0a20 2020  surf.lyr_num.   
-00020490: 2020 2020 2020 2020 206c 616e 645b 6c79           land[ly
-000204a0: 725f 6e75 6d5d 2e5f 706c 6f74 287a 6f6f  r_num]._plot(zoo
-000204b0: 6d5f 7769 6474 6820 3d20 7a6f 6f6d 5f77  m_width = zoom_w
-000204c0: 6964 7468 2c20 783d 6e70 2e6d 6561 6e28  idth, x=np.mean(
-000204d0: 7829 2c0a 2020 2020 2020 2020 2020 2020  x),.            
-000204e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000204f0: 2020 2020 793d 6e70 2e6d 6561 6e28 7929      y=np.mean(y)
-00020500: 2c20 7469 636b 733d 7469 636b 732c 2063  , ticks=ticks, c
-00020510: 6d61 703d 636d 6170 2c0a 2020 2020 2020  map=cmap,.      
+0001fb70: 2020 2069 6e64 2e79 2d30 2e35 2b6f 6666     ind.y-0.5+off
+0001fb80: 7365 745f 6672 6f6d 5f70 6865 6e6f 7479  set_from_phenoty
+0001fb90: 7065 5f74 6578 742c 0a20 2020 2020 2020  pe_text,.       
+0001fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fbb0: 2020 2725 302e 3266 2720 2520 696e 642e    '%0.2f' % ind.
+0001fbc0: 6669 742c 2063 6f6c 6f72 203d 2066 6974  fit, color = fit
+0001fbd0: 6e65 7373 5f74 6578 745f 636f 6c6f 722c  ness_text_color,
+0001fbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fbf0: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
+0001fc00: 2074 6578 745f 7369 7a65 290a 0a20 2020   text_size)..   
+0001fc10: 2020 2020 2023 616e 6420 6d61 6b65 2061       #and make a
+0001fc20: 2063 6f6c 6f72 6261 7220 666f 7220 7468   colorbar for th
+0001fc30: 6520 6669 746e 6573 7320 7661 6c75 6573  e fitness values
+0001fc40: 200a 2020 2020 2020 2020 6966 2066 6974   .        if fit
+0001fc50: 6e65 7373 5f63 6261 723a 0a20 2020 2020  ness_cbar:.     
+0001fc60: 2020 2020 2020 2076 697a 2e5f 6d61 6b65         viz._make
+0001fc70: 5f66 6974 6e65 7373 5f63 6261 7228 6d61  _fitness_cbar(ma
+0001fc80: 6b65 5f63 6261 725f 666e 2c20 6d69 6e5f  ke_cbar_fn, min_
+0001fc90: 6669 7429 0a0a 2020 2020 236d 6574 686f  fit)..    #metho
+0001fca0: 6420 746f 2070 6c6f 7420 6120 7370 6563  d to plot a spec
+0001fcb0: 6965 7327 2061 6c6c 656c 6520 6672 6571  ies' allele freq
+0001fcc0: 7565 6e63 6965 730a 2020 2020 6465 6620  uencies.    def 
+0001fcd0: 5f70 6c6f 745f 616c 6c65 6c65 5f66 7265  _plot_allele_fre
+0001fce0: 7175 656e 6369 6573 2873 656c 662c 2063  quencies(self, c
+0001fcf0: 6f6c 6f72 3d27 7265 6427 293a 0a20 2020  olor='red'):.   
+0001fd00: 2020 2020 2069 6620 7365 6c66 2e67 656e       if self.gen
+0001fd10: 5f61 7263 6820 6973 204e 6f6e 653a 0a20  _arch is None:. 
+0001fd20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0001fd30: 2828 2253 7065 6369 6573 2e5f 706c 6f74  (("Species._plot
+0001fd40: 5f61 6c6c 656c 655f 6672 6571 7565 6e63  _allele_frequenc
+0001fd50: 6965 7320 6973 206e 6f74 2076 616c 6964  ies is not valid
+0001fd60: 2066 6f72 2022 0a20 2020 2020 2020 2020   for ".         
+0001fd70: 2020 2020 2020 2020 2020 2273 7065 6369            "speci
+0001fd80: 6573 2077 6974 686f 7574 2067 656e 6f6d  es without genom
+0001fd90: 6573 2e5c 6e22 2929 0a20 2020 2020 2020  es.\n")).       
+0001fda0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001fdb0: 2020 2073 656c 662e 6765 6e5f 6172 6368     self.gen_arch
+0001fdc0: 2e5f 706c 6f74 5f61 6c6c 656c 655f 6672  ._plot_allele_fr
+0001fdd0: 6571 7565 6e63 6965 7328 7365 6c66 2c20  equencies(self, 
+0001fde0: 636f 6c6f 723d 636f 6c6f 7229 0a0a 2020  color=color)..  
+0001fdf0: 2020 2320 6d65 7468 6f64 2066 6f72 2070    # method for p
+0001fe00: 6c6f 7474 696e 6720 6120 6869 7374 6f67  lotting a histog
+0001fe10: 7261 6d20 6f66 2074 6865 2063 7572 7265  ram of the curre
+0001fe20: 6e74 2066 6974 6e65 7373 2076 616c 7565  nt fitness value
+0001fe30: 730a 2020 2020 6465 6620 5f70 6c6f 745f  s.    def _plot_
+0001fe40: 6869 7374 5f66 6974 6e65 7373 2873 656c  hist_fitness(sel
+0001fe50: 6629 3a0a 2020 2020 2020 2020 706c 742e  f):.        plt.
+0001fe60: 6869 7374 286c 6973 7428 7365 6c66 2e5f  hist(list(self._
+0001fe70: 6361 6c63 5f66 6974 6e65 7373 2829 2929  calc_fitness()))
+0001fe80: 0a20 2020 2020 2020 2070 6c74 2e78 6c61  .        plt.xla
+0001fe90: 6265 6c28 2746 6974 6e65 7373 2729 0a20  bel('Fitness'). 
+0001fea0: 2020 2020 2020 2070 6c74 2e79 6c61 6265         plt.ylabe
+0001feb0: 6c28 2743 6f75 6e74 2729 0a0a 2020 2020  l('Count')..    
+0001fec0: 2320 6d65 7468 6f64 2066 6f72 2070 6c6f  # method for plo
+0001fed0: 7474 696e 6720 7468 6520 6d6f 7665 6d65  tting the moveme
+0001fee0: 6e74 2073 7572 6661 6365 2028 696e 2076  nt surface (in v
+0001fef0: 6172 696f 7573 2066 6f72 6d61 7473 290a  arious formats).
+0001ff00: 2020 2020 6465 6620 5f70 6c6f 745f 6469      def _plot_di
+0001ff10: 7265 6374 696f 6e5f 7375 7266 6163 6528  rection_surface(
+0001ff20: 7365 6c66 2c20 6c61 6e64 2c20 7375 7266  self, land, surf
+0001ff30: 5f74 7970 652c 2073 7479 6c65 2c20 783d  _type, style, x=
+0001ff40: 4e6f 6e65 2c20 793d 4e6f 6e65 2c0a 2020  None, y=None,.  
+0001ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff60: 2020 2020 2020 2020 2020 2020 2020 7a6f                zo
+0001ff70: 6f6d 5f77 6964 7468 3d4e 6f6e 652c 2073  om_width=None, s
+0001ff80: 6361 6c65 5f66 6163 743d 342e 352c 0a20  cale_fact=4.5,. 
+0001ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001ffb0: 6f6c 6f72 3d27 626c 6163 6b27 2c20 6362  olor='black', cb
+0001ffc0: 6172 3d54 7275 652c 2074 6963 6b73 3d4e  ar=True, ticks=N
+0001ffd0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fff0: 2020 2020 2063 6d61 703d 2770 6c61 736d       cmap='plasm
+00020000: 6127 2c20 6d61 736b 5f72 6173 743d 4e6f  a', mask_rast=No
+00020010: 6e65 293a 0a20 2020 2020 2020 2023 2067  ne):.        # g
+00020020: 6574 2074 6865 2063 6f72 7265 6374 2073  et the correct s
+00020030: 7572 6661 6365 0a20 2020 2020 2020 2069  urface.        i
+00020040: 6620 7375 7266 5f74 7970 6520 3d3d 2027  f surf_type == '
+00020050: 6d6f 7665 273a 0a20 2020 2020 2020 2020  move':.         
+00020060: 2020 2073 7572 6620 3d20 7365 6c66 2e5f     surf = self._
+00020070: 6d6f 7665 5f73 7572 660a 2020 2020 2020  move_surf.      
+00020080: 2020 656c 6966 2073 7572 665f 7479 7065    elif surf_type
+00020090: 203d 3d20 2764 6973 7027 3a0a 2020 2020   == 'disp':.    
+000200a0: 2020 2020 2020 2020 7375 7266 203d 3d20          surf == 
+000200b0: 7365 6c66 2e5f 6469 7370 5f73 7572 660a  self._disp_surf.
+000200c0: 0a20 2020 2020 2020 2023 2067 6574 2061  .        # get a
+000200d0: 6c6c 2078 2773 2061 6e64 2079 2773 2c20  ll x's and y's, 
+000200e0: 6966 2078 2061 6e64 2079 2061 7265 204e  if x and y are N
+000200f0: 6f6e 650a 2020 2020 2020 2020 6966 2078  one.        if x
+00020100: 2069 7320 4e6f 6e65 2061 6e64 2079 2069   is None and y i
+00020110: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00020120: 2020 2020 7820 3d20 5b2a 7261 6e67 6528      x = [*range(
+00020130: 6c61 6e64 2e64 696d 5b30 5d29 5d0a 2020  land.dim[0])].  
+00020140: 2020 2020 2020 2020 2020 7920 3d20 5b2a            y = [*
+00020150: 7261 6e67 6528 6c61 6e64 2e64 696d 5b31  range(land.dim[1
+00020160: 5d29 5d0a 2020 2020 2020 2020 656c 7365  ])].        else
+00020170: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
+00020180: 3d20 5b78 5d0a 2020 2020 2020 2020 2020  = [x].          
+00020190: 2020 7920 3d20 5b79 5d0a 2020 2020 2020    y = [y].      
+000201a0: 2020 2363 6865 636b 2069 6620 7468 6520    #check if the 
+000201b0: 7375 7266 6163 6520 6973 206e 6f6e 650a  surface is none.
+000201c0: 2020 2020 2020 2020 6966 2073 7572 6620          if surf 
+000201d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000201e0: 2020 2020 2070 7269 6e74 2828 2746 756e       print(('Fun
+000201f0: 6374 696f 6e20 6e6f 7420 7661 6c69 6420  ction not valid 
+00020200: 666f 7220 6120 5370 6563 6965 7320 7769  for a Species wi
+00020210: 7468 206e 6f20 270a 2020 2020 2020 2020  th no '.        
+00020220: 2020 2020 2020 2020 2020 2027 5f25 7353             '_%sS
+00020230: 7572 6661 6365 2e27 2920 2520 287b 0a20  urface.') % ({. 
+00020240: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00020250: 6d6f 7665 273a 2027 4d6f 7665 6d65 6e74  move': 'Movement
+00020260: 272c 2027 6469 7370 273a 2027 4469 7370  ', 'disp': 'Disp
+00020270: 6572 7361 6c27 7d5b 7375 7266 5f74 7970  ersal'}[surf_typ
+00020280: 655d 2929 0a20 2020 2020 2020 2020 2020  e])).           
+00020290: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+000202a0: 656c 6966 2073 7479 6c65 206e 6f74 2069  elif style not i
+000202b0: 6e20 5b27 6869 7374 272c 2027 6368 6973  n ['hist', 'chis
+000202c0: 7427 2c20 2776 6563 7427 2c20 2763 6472  t', 'vect', 'cdr
+000202d0: 6177 7327 5d3a 0a20 2020 2020 2020 2020  aws']:.         
+000202e0: 2020 2070 7269 6e74 2828 2254 6865 2027     print(("The '
+000202f0: 7374 796c 6527 2061 7267 756d 656e 7420  style' argument 
+00020300: 6d75 7374 2074 616b 6520 6f6e 6520 6f66  must take one of
+00020310: 2074 6865 2022 0a20 2020 2020 2020 2020   the ".         
+00020320: 2020 2020 2020 2020 2020 2266 6f6c 6c6f            "follo
+00020330: 7769 6e67 2076 616c 7565 733a 2027 6869  wing values: 'hi
+00020340: 7374 272c 2027 6368 6973 7427 2c20 220a  st', 'chist', ".
+00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020360: 2020 2022 2776 6563 7427 2c20 2763 6472     "'vect', 'cdr
+00020370: 6177 7327 2229 290a 2020 2020 2020 2020  aws'")).        
+00020380: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00020390: 2020 2065 6c69 6620 7374 796c 6520 3d3d     elif style ==
+000203a0: 2027 6869 7374 273a 0a20 2020 2020 2020   'hist':.       
+000203b0: 2020 2020 2078 203d 2078 5b30 5d0a 2020       x = x[0].  
+000203c0: 2020 2020 2020 2020 2020 7920 3d20 795b            y = y[
+000203d0: 305d 0a20 2020 2020 2020 2020 2020 2070  0].            p
+000203e0: 6c74 2e68 6973 7428 722e 6368 6f69 6365  lt.hist(r.choice
+000203f0: 2873 7572 662e 7375 7266 5b79 2c78 2c3a  (surf.surf[y,x,:
+00020400: 5d2c 2073 697a 6520 3d20 3130 3030 302c  ], size = 10000,
+00020410: 2072 6570 6c61 6365 203d 2054 7275 6529   replace = True)
+00020420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00020430: 2020 2020 2020 2062 696e 733d 3130 302c         bins=100,
+00020440: 2064 656e 7369 7479 3d54 7275 652c 2061   density=True, a
+00020450: 6c70 6861 3d30 2e35 2c20 636f 6c6f 723d  lpha=0.5, color=
+00020460: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
+00020470: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00020480: 2020 2364 6973 706c 6179 2074 6865 206d    #display the m
+00020490: 6f76 656d 656e 742d 7375 7266 6163 6520  ovement-surface 
+000204a0: 7261 7374 6572 0a20 2020 2020 2020 2020  raster.         
+000204b0: 2020 206c 7972 5f6e 756d 203d 2073 7572     lyr_num = sur
+000204c0: 662e 6c79 725f 6e75 6d0a 2020 2020 2020  f.lyr_num.      
+000204d0: 2020 2020 2020 6c61 6e64 5b6c 7972 5f6e        land[lyr_n
+000204e0: 756d 5d2e 5f70 6c6f 7428 7a6f 6f6d 5f77  um]._plot(zoom_w
+000204f0: 6964 7468 203d 207a 6f6f 6d5f 7769 6474  idth = zoom_widt
+00020500: 682c 2078 3d6e 702e 6d65 616e 2878 292c  h, x=np.mean(x),
+00020510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00020520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020530: 2020 2020 2020 2020 2020 6d61 736b 5f72            mask_r
-00020540: 6173 743d 6d61 736b 5f72 6173 7429 0a0a  ast=mask_rast)..
-00020550: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00020560: 7479 6c65 203d 3d20 2763 6869 7374 273a  tyle == 'chist':
-00020570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020580: 2066 6f72 2078 5f76 616c 2069 6e20 783a   for x_val in x:
-00020590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000205a0: 2020 2020 2066 6f72 2079 5f76 616c 2069       for y_val i
-000205b0: 6e20 793a 0a20 2020 2020 2020 2020 2020  n y:.           
-000205c0: 2020 2020 2020 2020 2020 2020 2076 2c20               v, 
-000205d0: 6120 3d20 6e70 2e68 6973 746f 6772 616d  a = np.histogram
-000205e0: 2872 2e63 686f 6963 6528 7375 7266 2e73  (r.choice(surf.s
-000205f0: 7572 665b 795f 7661 6c2c 0a20 2020 2020  urf[y_val,.     
-00020600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020630: 2020 2020 2020 2020 2020 785f 7661 6c2c            x_val,
-00020640: 203a 5d2c 0a20 2020 2020 2020 2020 2020   :],.           
+00020530: 2079 3d6e 702e 6d65 616e 2879 292c 2074   y=np.mean(y), t
+00020540: 6963 6b73 3d74 6963 6b73 2c20 636d 6170  icks=ticks, cmap
+00020550: 3d63 6d61 702c 0a20 2020 2020 2020 2020  =cmap,.         
+00020560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020570: 2020 2020 2020 206d 6173 6b5f 7261 7374         mask_rast
+00020580: 3d6d 6173 6b5f 7261 7374 290a 0a20 2020  =mask_rast)..   
+00020590: 2020 2020 2020 2020 2069 6620 7374 796c           if styl
+000205a0: 6520 3d3d 2027 6368 6973 7427 3a0a 2020  e == 'chist':.  
+000205b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000205c0: 7220 785f 7661 6c20 696e 2078 3a0a 2020  r x_val in x:.  
+000205d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000205e0: 2020 666f 7220 795f 7661 6c20 696e 2079    for y_val in y
+000205f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020600: 2020 2020 2020 2020 2020 762c 2061 203d            v, a =
+00020610: 206e 702e 6869 7374 6f67 7261 6d28 722e   np.histogram(r.
+00020620: 6368 6f69 6365 2873 7572 662e 7375 7266  choice(surf.surf
+00020630: 5b79 5f76 616c 2c0a 2020 2020 2020 2020  [y_val,.        
+00020640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020670: 2020 2020 2020 2020 2020 7265 706c 6163            replac
-00020680: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+00020670: 2020 2020 2020 2078 5f76 616c 2c20 3a5d         x_val, :]
+00020680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00020690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000206a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206b0: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-000206c0: 653d 3735 3030 292c 2062 696e 733d 3135  e=7500), bins=15
-000206d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000206e0: 2020 2020 2020 2020 2020 7620 3d20 7620            v = v 
-000206f0: 2f20 666c 6f61 7428 762e 7375 6d28 2929  / float(v.sum())
-00020700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020710: 2020 2020 2020 2020 2061 203d 205b 2861           a = [(a
-00020720: 5b6e 5d20 2b20 615b 6e20 2b20 315d 2920  [n] + a[n + 1]) 
-00020730: 2f20 3220 666f 7220 6e20 696e 2072 616e  / 2 for n in ran
-00020740: 6765 286c 656e 2861 2920 2d20 3129 5d0a  ge(len(a) - 1)].
-00020750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020760: 2020 2020 2020 2020 7873 203d 205b 6e70          xs = [np
-00020770: 2e63 6f73 2861 5b6e 5d29 202a 2030 2e37  .cos(a[n]) * 0.7
-00020780: 3520 666f 7220 6e20 696e 2072 616e 6765  5 for n in range
-00020790: 286c 656e 2861 2929 5d0a 2020 2020 2020  (len(a))].      
-000207a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000207b0: 2020 7973 203d 205b 6e70 2e73 696e 2861    ys = [np.sin(a
-000207c0: 5b6e 5d29 202a 2030 2e37 3520 666f 7220  [n]) * 0.75 for 
-000207d0: 6e20 696e 2072 616e 6765 286c 656e 2861  n in range(len(a
-000207e0: 2929 5d0a 2020 2020 2020 2020 2020 2020  ))].            
-000207f0: 2020 2020 2020 2020 2020 2020 7873 203d              xs =
-00020800: 206e 702e 6172 7261 7928 7873 2920 2a20   np.array(xs) * 
-00020810: 7620 2a20 7363 616c 655f 6661 6374 0a20  v * scale_fact. 
-00020820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020830: 2020 2020 2020 2079 7320 3d20 6e70 2e61         ys = np.a
-00020840: 7272 6179 2879 7329 202a 2076 202a 2073  rray(ys) * v * s
-00020850: 6361 6c65 5f66 6163 740a 2020 2020 2020  cale_fact.      
+000206b0: 2020 2020 2020 2072 6570 6c61 6365 3d54         replace=T
+000206c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000206d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000206e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000206f0: 2020 2020 2020 2020 2020 7369 7a65 3d37            size=7
+00020700: 3530 3029 2c20 6269 6e73 3d31 3529 0a20  500), bins=15). 
+00020710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020720: 2020 2020 2020 2076 203d 2076 202f 2066         v = v / f
+00020730: 6c6f 6174 2876 2e73 756d 2829 290a 2020  loat(v.sum()).  
+00020740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020750: 2020 2020 2020 6120 3d20 5b28 615b 6e5d        a = [(a[n]
+00020760: 202b 2061 5b6e 202b 2031 5d29 202f 2032   + a[n + 1]) / 2
+00020770: 2066 6f72 206e 2069 6e20 7261 6e67 6528   for n in range(
+00020780: 6c65 6e28 6129 202d 2031 295d 0a20 2020  len(a) - 1)].   
+00020790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000207a0: 2020 2020 2078 7320 3d20 5b6e 702e 636f       xs = [np.co
+000207b0: 7328 615b 6e5d 2920 2a20 302e 3735 2066  s(a[n]) * 0.75 f
+000207c0: 6f72 206e 2069 6e20 7261 6e67 6528 6c65  or n in range(le
+000207d0: 6e28 6129 295d 0a20 2020 2020 2020 2020  n(a))].         
+000207e0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000207f0: 7320 3d20 5b6e 702e 7369 6e28 615b 6e5d  s = [np.sin(a[n]
+00020800: 2920 2a20 302e 3735 2066 6f72 206e 2069  ) * 0.75 for n i
+00020810: 6e20 7261 6e67 6528 6c65 6e28 6129 295d  n range(len(a))]
+00020820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020830: 2020 2020 2020 2020 2078 7320 3d20 6e70           xs = np
+00020840: 2e61 7272 6179 2878 7329 202a 2076 202a  .array(xs) * v *
+00020850: 2073 6361 6c65 5f66 6163 740a 2020 2020   scale_fact.    
 00020860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020870: 2020 5b70 6c74 2e70 6c6f 7428 2878 5f76    [plt.plot((x_v
-00020880: 616c 202b 2030 2e35 2c20 2878 5f76 616c  al + 0.5, (x_val
-00020890: 202b 2030 2e35 202b 2078 735b 6e5d 2929   + 0.5 + xs[n]))
-000208a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000208b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208c0: 2020 2020 2879 5f76 616c 202b 2030 2e35      (y_val + 0.5
-000208d0: 2c20 2879 5f76 616c 202b 2030 2e35 202b  , (y_val + 0.5 +
-000208e0: 2079 735b 6e5d 2929 2c0a 2020 2020 2020   ys[n])),.      
+00020870: 2020 2020 7973 203d 206e 702e 6172 7261      ys = np.arra
+00020880: 7928 7973 2920 2a20 7620 2a20 7363 616c  y(ys) * v * scal
+00020890: 655f 6661 6374 0a20 2020 2020 2020 2020  e_fact.         
+000208a0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000208b0: 706c 742e 706c 6f74 2828 785f 7661 6c20  plt.plot((x_val 
+000208c0: 2b20 302e 352c 2028 785f 7661 6c20 2b20  + 0.5, (x_val + 
+000208d0: 302e 3520 2b20 7873 5b6e 5d29 292c 0a20  0.5 + xs[n])),. 
+000208e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000208f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020900: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00020910: 7769 6474 683d 322c 0a20 2020 2020 2020  width=2,.       
-00020920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020930: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00020940: 3d63 6f6c 6f72 2920 666f 7220 6e20 696e  =color) for n in
-00020950: 2072 616e 6765 286c 656e 2878 7329 295d   range(len(xs))]
-00020960: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00020970: 6966 2073 7479 6c65 203d 3d20 2763 6472  if style == 'cdr
-00020980: 6177 7327 3a0a 2020 2020 2020 2020 2020  aws':.          
-00020990: 2020 2020 2020 666f 7220 785f 7661 6c20        for x_val 
-000209a0: 696e 2078 3a0a 2020 2020 2020 2020 2020  in x:.          
-000209b0: 2020 2020 2020 2020 2020 666f 7220 795f            for y_
-000209c0: 7661 6c20 696e 2079 3a0a 2020 2020 2020  val in y:.      
-000209d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000209e0: 2020 7074 7320 3d20 5b28 6e70 2e63 6f73    pts = [(np.cos
-000209f0: 2861 292c 206e 702e 7369 6e28 6129 2920  (a), np.sin(a)) 
-00020a00: 666f 7220 6120 696e 2072 2e63 686f 6963  for a in r.choic
-00020a10: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00020a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a30: 2020 2073 7572 662e 7375 7266 5b79 5f76     surf.surf[y_v
-00020a40: 616c 2c20 785f 7661 6c2c 203a 5d2c 2073  al, x_val, :], s
-00020a50: 697a 653d 3130 3030 2c0a 2020 2020 2020  ize=1000,.      
+00020900: 2028 795f 7661 6c20 2b20 302e 352c 2028   (y_val + 0.5, (
+00020910: 795f 7661 6c20 2b20 302e 3520 2b20 7973  y_val + 0.5 + ys
+00020920: 5b6e 5d29 292c 0a20 2020 2020 2020 2020  [n])),.         
+00020930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020940: 2020 2020 2020 2020 206c 696e 6577 6964           linewid
+00020950: 7468 3d32 2c0a 2020 2020 2020 2020 2020  th=2,.          
+00020960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020970: 2020 2020 2020 2020 636f 6c6f 723d 636f          color=co
+00020980: 6c6f 7229 2066 6f72 206e 2069 6e20 7261  lor) for n in ra
+00020990: 6e67 6528 6c65 6e28 7873 2929 5d0a 0a20  nge(len(xs))].. 
+000209a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000209b0: 7374 796c 6520 3d3d 2027 6364 7261 7773  style == 'cdraws
+000209c0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+000209d0: 2020 2066 6f72 2078 5f76 616c 2069 6e20     for x_val in 
+000209e0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
+000209f0: 2020 2020 2020 2066 6f72 2079 5f76 616c         for y_val
+00020a00: 2069 6e20 793a 0a20 2020 2020 2020 2020   in y:.         
+00020a10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00020a20: 7473 203d 205b 286e 702e 636f 7328 6129  ts = [(np.cos(a)
+00020a30: 2c20 6e70 2e73 696e 2861 2929 2066 6f72  , np.sin(a)) for
+00020a40: 2061 2069 6e20 722e 6368 6f69 6365 280a   a in r.choice(.
+00020a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a70: 2020 2020 2020 2020 2020 7265 706c 6163            replac
-00020a80: 653d 5472 7565 295d 0a20 2020 2020 2020  e=True)].       
-00020a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020aa0: 2070 6c74 2e73 6361 7474 6572 285b 7074   plt.scatter([pt
-00020ab0: 5b30 5d20 2a20 302e 3520 2b20 785f 7661  [0] * 0.5 + x_va
-00020ac0: 6c20 2b20 302e 3520 666f 7220 7074 2069  l + 0.5 for pt i
-00020ad0: 6e20 7074 735d 2c0a 2020 2020 2020 2020  n pts],.        
-00020ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020af0: 2020 2020 2020 2020 2020 2020 5b70 745b              [pt[
-00020b00: 315d 202a 2030 2e35 202b 2079 5f76 616c  1] * 0.5 + y_val
-00020b10: 202b 2030 2e35 2066 6f72 2070 7420 696e   + 0.5 for pt in
-00020b20: 2070 7473 5d2c 0a20 2020 2020 2020 2020   pts],.         
-00020b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b40: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00020b50: 3d63 6f6c 6f72 2c20 616c 7068 613d 302e  =color, alpha=0.
-00020b60: 312c 206d 6172 6b65 723d 272e 2729 0a0a  1, marker='.')..
-00020b70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00020b80: 2073 7479 6c65 203d 3d20 2776 6563 7427   style == 'vect'
-00020b90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00020ba0: 2020 6465 6620 706c 6f74 5f6f 6e65 5f63    def plot_one_c
-00020bb0: 656c 6c28 782c 2079 293a 0a20 2020 2020  ell(x, y):.     
-00020bc0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00020bd0: 2064 7261 7720 7361 6d70 6c65 206f 6620   draw sample of 
-00020be0: 616e 676c 6573 2066 726f 6d20 7468 6520  angles from the 
-00020bf0: 4761 7573 7369 616e 204b 4445 0a20 2020  Gaussian KDE.   
-00020c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c10: 2023 7265 7072 6573 656e 7469 6e67 2074   #representing t
-00020c20: 6865 2076 6f6e 206d 6973 6573 206d 6978  he von mises mix
-00020c30: 7475 7265 2064 6973 7472 6962 7574 696f  ture distributio
-00020c40: 6e20 284b 4445 290a 2020 2020 2020 2020  n (KDE).        
-00020c50: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
-00020c60: 203d 2073 7572 662e 7375 7266 5b79 2c78   = surf.surf[y,x
-00020c70: 2c3a 5d0a 2020 2020 2020 2020 2020 2020  ,:].            
-00020c80: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00020c90: 206c 6973 7473 206f 6620 7468 6520 7820   lists of the x 
-00020ca0: 616e 6420 7920 2869 2e65 2e20 636f 7320  and y (i.e. cos 
-00020cb0: 616e 6420 7369 6e29 0a20 2020 2020 2020  and sin).       
-00020cc0: 2020 2020 2020 2020 2020 2020 2023 636f               #co
-00020cd0: 6d70 6f6e 656e 7473 206f 6620 6561 6368  mponents of each
-00020ce0: 2061 6e67 6c65 2069 6e20 7468 6520 7361   angle in the sa
-00020cf0: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-00020d00: 2020 2020 2020 2020 2078 5f76 6563 7473           x_vects
-00020d10: 203d 206e 702e 636f 7328 7361 6d70 290a   = np.cos(samp).
-00020d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d30: 2020 2020 795f 7665 6374 7320 3d20 6e70      y_vects = np
-00020d40: 2e73 696e 2873 616d 7029 0a20 2020 2020  .sin(samp).     
-00020d50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00020d60: 2064 6566 696e 6520 7468 6520 6478 2061   define the dx a
-00020d70: 6e64 2064 7920 6469 7374 616e 6365 7320  nd dy distances 
-00020d80: 7573 6564 2074 6f20 7468 650a 2020 2020  used to the.    
-00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020da0: 2370 6f73 6974 696f 6e20 7468 6520 6172  #position the ar
-00020db0: 726f 7768 6561 6420 2864 6976 6964 6520  rowhead (divide 
-00020dc0: 6279 2073 7172 7428 3229 2f32 2c20 746f  by sqrt(2)/2, to
-00020dd0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00020de0: 2020 2020 2020 2373 6361 6c65 2074 6f20        #scale to 
-00020df0: 7468 6520 7369 7a65 206f 6620 6861 6c66  the size of half
-00020e00: 206f 6620 7468 6520 6469 6167 6f6e 616c   of the diagonal
-00020e10: 206f 6620 6120 6365 6c6c 290a 2020 2020   of a cell).    
-00020e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e30: 6478 203d 206e 702e 6d65 616e 2878 5f76  dx = np.mean(x_v
-00020e40: 6563 7473 2920 2f20 6e70 2e73 7172 7428  ects) / np.sqrt(
-00020e50: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
-00020e60: 2020 2020 2020 2064 7920 3d20 6e70 2e6d         dy = np.m
-00020e70: 6561 6e28 795f 7665 6374 7329 202f 206e  ean(y_vects) / n
-00020e80: 702e 7371 7274 2832 290a 2020 2020 2020  p.sqrt(2).      
-00020e90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020ea0: 6e6f 7720 706c 6f74 2074 6865 2061 7272  now plot the arr
-00020eb0: 6f77 0a20 2020 2020 2020 2020 2020 2020  ow.             
-00020ec0: 2020 2020 2020 2070 6c74 2e61 7272 6f77         plt.arrow
-00020ed0: 2878 202b 2030 2e35 2c20 7920 2b20 302e  (x + 0.5, y + 0.
-00020ee0: 352c 2064 782c 2064 792c 2061 6c70 6861  5, dx, dy, alpha
-00020ef0: 3d30 2e37 352c 0a20 2020 2020 2020 2020  =0.75,.         
-00020f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f10: 2020 2020 2063 6f6c 6f72 3d63 6f6c 6f72       color=color
-00020f20: 2c20 6865 6164 5f77 6964 7468 3d30 2e32  , head_width=0.2
-00020f30: 342c 2068 6561 645f 6c65 6e67 7468 3d30  4, head_length=0
-00020f40: 2e33 3229 0a0a 2020 2020 2020 2020 2020  .32)..          
-00020f50: 2020 2020 2020 2320 6361 6c6c 2074 6865        # call the
-00020f60: 2069 6e74 6572 6e61 6c6c 7920 6465 6669   internally defi
-00020f70: 6e65 6420 6675 6e63 7469 6f6e 2061 7320  ned function as 
-00020f80: 6120 6e65 7374 6564 206c 6973 740a 2020  a nested list.  
-00020f90: 2020 2020 2020 2020 2020 2020 2020 2363                #c
-00020fa0: 6f6d 7072 6568 656e 7369 6f6e 2066 6f72  omprehension for
-00020fb0: 2061 6c6c 2072 6173 7465 7220 6365 6c6c   all raster cell
-00020fc0: 732c 2077 6869 6368 2049 2062 656c 6965  s, which I belie
-00020fd0: 7665 0a20 2020 2020 2020 2020 2020 2020  ve.             
-00020fe0: 2020 2023 7368 6f75 6c64 2064 6f20 6974     #should do it
-00020ff0: 7320 6265 7374 2074 6f20 7665 6374 6f72  s best to vector
-00021000: 697a 6520 7468 6520 7768 6f6c 6520 6f70  ize the whole op
-00021010: 6572 6174 696f 6e0a 2020 2020 2020 2020  eration.        
-00021020: 2020 2020 2020 2020 5b5b 706c 6f74 5f6f          [[plot_o
-00021030: 6e65 5f63 656c 6c28 6a2c 2069 2920 666f  ne_cell(j, i) fo
-00021040: 7220 6920 696e 2072 616e 6765 280a 2020  r i in range(.  
-00021050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021060: 2020 7375 7266 2e73 7572 662e 7368 6170    surf.surf.shap
-00021070: 655b 305d 295d 2066 6f72 206a 2069 6e20  e[0])] for j in 
-00021080: 7261 6e67 6528 0a20 2020 2020 2020 2020  range(.         
-00021090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210a0: 2020 2020 2020 2020 2020 2073 7572 662e             surf.
-000210b0: 7375 7266 2e73 6861 7065 5b31 5d29 5d0a  surf.shape[1])].
-000210c0: 0a0a 2020 2020 2320 706c 6f74 2074 6865  ..    # plot the
-000210d0: 206c 696e 6561 6765 2066 6f72 2061 2067   lineage for a g
-000210e0: 6976 656e 206e 6f64 6520 616e 6420 6c6f  iven node and lo
-000210f0: 6375 730a 2020 2020 6465 6620 5f70 6c6f  cus.    def _plo
-00021100: 745f 6765 6e65 5f66 6c6f 7728 7365 6c66  t_gene_flow(self
-00021110: 2c20 6c6f 6375 732c 2073 7479 6c65 2c20  , locus, style, 
-00021120: 6c61 6e64 2c20 6e6f 6465 733d 4e6f 6e65  land, nodes=None
-00021130: 2c20 696e 6469 7669 6473 3d4e 6f6e 652c  , individs=None,
-00021140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021150: 2020 2020 2020 2020 636f 6c6f 723d 4e6f          color=No
-00021160: 6e65 2c20 7068 656e 6f74 7970 653d 4e6f  ne, phenotype=No
-00021170: 6e65 2c20 6c79 725f 6e75 6d3d 302c 206a  ne, lyr_num=0, j
-00021180: 6974 7465 723d 5472 7565 2c0a 2020 2020  itter=True,.    
-00021190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211a0: 2020 2061 6c70 6861 3d30 2e35 2c20 7369     alpha=0.5, si
-000211b0: 7a65 3d32 352c 2061 6464 5f72 6f6f 7473  ze=25, add_roots
-000211c0: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
-000211d0: 2069 6620 6e6f 7420 7365 6c66 2e67 656e   if not self.gen
-000211e0: 5f61 7263 682e 7573 655f 7473 6b69 743a  _arch.use_tskit:
-000211f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00021200: 7365 2045 7863 6570 7469 6f6e 2828 2247  se Exception(("G
-00021210: 656e 6520 666c 6f77 2063 616e 6e6f 7420  ene flow cannot 
-00021220: 6265 2070 6c6f 7474 6564 2066 6f72 2061  be plotted for a
-00021230: 2053 7065 6369 6573 2022 0a20 2020 2020   Species ".     
-00021240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021250: 2020 2020 2020 2020 2277 686f 7365 2073          "whose s
-00021260: 7061 7469 616c 2070 6564 6967 7265 6520  patial pedigree 
-00021270: 6973 206e 6f74 2062 6569 6e67 2074 7261  is not being tra
-00021280: 636b 6564 2022 0a20 2020 2020 2020 2020  cked ".         
-00021290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000212a0: 2020 2020 2262 7920 7473 6b69 742e 2229      "by tskit.")
-000212b0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-000212c0: 2073 7479 6c65 2069 6e20 5b27 6c69 6e65   style in ['line
-000212d0: 6167 6527 2c20 2776 6563 746f 7227 5d2c  age', 'vector'],
-000212e0: 2028 2254 6865 2073 7479 6c65 2061 7267   ("The style arg
-000212f0: 756d 656e 7420 6d75 7374 2062 6520 220a  ument must be ".
-00021300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021330: 2267 6976 656e 2065 6974 6865 7220 276c  "given either 'l
-00021340: 696e 6561 6765 2720 6f72 2022 0a20 2020  ineage' or ".   
+00020a70: 7375 7266 2e73 7572 665b 795f 7661 6c2c  surf.surf[y_val,
+00020a80: 2078 5f76 616c 2c20 3a5d 2c20 7369 7a65   x_val, :], size
+00020a90: 3d31 3030 302c 0a20 2020 2020 2020 2020  =1000,.         
+00020aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ab0: 2020 2020 2020 2072 6570 6c61 6365 3d54         replace=T
+00020ac0: 7275 6529 5d0a 2020 2020 2020 2020 2020  rue)].          
+00020ad0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00020ae0: 742e 7363 6174 7465 7228 5b70 745b 305d  t.scatter([pt[0]
+00020af0: 202a 2030 2e35 202b 2078 5f76 616c 202b   * 0.5 + x_val +
+00020b00: 2030 2e35 2066 6f72 2070 7420 696e 2070   0.5 for pt in p
+00020b10: 7473 5d2c 0a20 2020 2020 2020 2020 2020  ts],.           
+00020b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b30: 2020 2020 2020 2020 205b 7074 5b31 5d20           [pt[1] 
+00020b40: 2a20 302e 3520 2b20 795f 7661 6c20 2b20  * 0.5 + y_val + 
+00020b50: 302e 3520 666f 7220 7074 2069 6e20 7074  0.5 for pt in pt
+00020b60: 735d 2c0a 2020 2020 2020 2020 2020 2020  s],.            
+00020b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b80: 2020 2020 2020 2020 636f 6c6f 723d 636f          color=co
+00020b90: 6c6f 722c 2061 6c70 6861 3d30 2e31 2c20  lor, alpha=0.1, 
+00020ba0: 6d61 726b 6572 3d27 2e27 290a 0a20 2020  marker='.')..   
+00020bb0: 2020 2020 2020 2020 2065 6c69 6620 7374           elif st
+00020bc0: 796c 6520 3d3d 2027 7665 6374 273a 0a20  yle == 'vect':. 
+00020bd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00020be0: 6566 2070 6c6f 745f 6f6e 655f 6365 6c6c  ef plot_one_cell
+00020bf0: 2878 2c20 7929 3a0a 2020 2020 2020 2020  (x, y):.        
+00020c00: 2020 2020 2020 2020 2020 2020 2320 6472              # dr
+00020c10: 6177 2073 616d 706c 6520 6f66 2061 6e67  aw sample of ang
+00020c20: 6c65 7320 6672 6f6d 2074 6865 2047 6175  les from the Gau
+00020c30: 7373 6961 6e20 4b44 450a 2020 2020 2020  ssian KDE.      
+00020c40: 2020 2020 2020 2020 2020 2020 2020 2372                #r
+00020c50: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00020c60: 766f 6e20 6d69 7365 7320 6d69 7874 7572  von mises mixtur
+00020c70: 6520 6469 7374 7269 6275 7469 6f6e 2028  e distribution (
+00020c80: 4b44 4529 0a20 2020 2020 2020 2020 2020  KDE).           
+00020c90: 2020 2020 2020 2020 2073 616d 7020 3d20           samp = 
+00020ca0: 7375 7266 2e73 7572 665b 792c 782c 3a5d  surf.surf[y,x,:]
+00020cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020cc0: 2020 2020 2023 2063 7265 6174 6520 6c69       # create li
+00020cd0: 7374 7320 6f66 2074 6865 2078 2061 6e64  sts of the x and
+00020ce0: 2079 2028 692e 652e 2063 6f73 2061 6e64   y (i.e. cos and
+00020cf0: 2073 696e 290a 2020 2020 2020 2020 2020   sin).          
+00020d00: 2020 2020 2020 2020 2020 2363 6f6d 706f            #compo
+00020d10: 6e65 6e74 7320 6f66 2065 6163 6820 616e  nents of each an
+00020d20: 676c 6520 696e 2074 6865 2073 616d 706c  gle in the sampl
+00020d30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00020d40: 2020 2020 2020 785f 7665 6374 7320 3d20        x_vects = 
+00020d50: 6e70 2e63 6f73 2873 616d 7029 0a20 2020  np.cos(samp).   
+00020d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d70: 2079 5f76 6563 7473 203d 206e 702e 7369   y_vects = np.si
+00020d80: 6e28 7361 6d70 290a 2020 2020 2020 2020  n(samp).        
+00020d90: 2020 2020 2020 2020 2020 2020 2320 6465              # de
+00020da0: 6669 6e65 2074 6865 2064 7820 616e 6420  fine the dx and 
+00020db0: 6479 2064 6973 7461 6e63 6573 2075 7365  dy distances use
+00020dc0: 6420 746f 2074 6865 0a20 2020 2020 2020  d to the.       
+00020dd0: 2020 2020 2020 2020 2020 2020 2023 706f               #po
+00020de0: 7369 7469 6f6e 2074 6865 2061 7272 6f77  sition the arrow
+00020df0: 6865 6164 2028 6469 7669 6465 2062 7920  head (divide by 
+00020e00: 7371 7274 2832 292f 322c 2074 6f20 0a20  sqrt(2)/2, to . 
+00020e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e20: 2020 2023 7363 616c 6520 746f 2074 6865     #scale to the
+00020e30: 2073 697a 6520 6f66 2068 616c 6620 6f66   size of half of
+00020e40: 2074 6865 2064 6961 676f 6e61 6c20 6f66   the diagonal of
+00020e50: 2061 2063 656c 6c29 0a20 2020 2020 2020   a cell).       
+00020e60: 2020 2020 2020 2020 2020 2020 2064 7820               dx 
+00020e70: 3d20 6e70 2e6d 6561 6e28 785f 7665 6374  = np.mean(x_vect
+00020e80: 7329 202f 206e 702e 7371 7274 2832 290a  s) / np.sqrt(2).
+00020e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ea0: 2020 2020 6479 203d 206e 702e 6d65 616e      dy = np.mean
+00020eb0: 2879 5f76 6563 7473 2920 2f20 6e70 2e73  (y_vects) / np.s
+00020ec0: 7172 7428 3229 0a20 2020 2020 2020 2020  qrt(2).         
+00020ed0: 2020 2020 2020 2020 2020 2023 206e 6f77             # now
+00020ee0: 2070 6c6f 7420 7468 6520 6172 726f 770a   plot the arrow.
+00020ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f00: 2020 2020 706c 742e 6172 726f 7728 7820      plt.arrow(x 
+00020f10: 2b20 302e 352c 2079 202b 2030 2e35 2c20  + 0.5, y + 0.5, 
+00020f20: 6478 2c20 6479 2c20 616c 7068 613d 302e  dx, dy, alpha=0.
+00020f30: 3735 2c0a 2020 2020 2020 2020 2020 2020  75,.            
+00020f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f50: 2020 636f 6c6f 723d 636f 6c6f 722c 2068    color=color, h
+00020f60: 6561 645f 7769 6474 683d 302e 3234 2c20  ead_width=0.24, 
+00020f70: 6865 6164 5f6c 656e 6774 683d 302e 3332  head_length=0.32
+00020f80: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00020f90: 2020 2023 2063 616c 6c20 7468 6520 696e     # call the in
+00020fa0: 7465 726e 616c 6c79 2064 6566 696e 6564  ternally defined
+00020fb0: 2066 756e 6374 696f 6e20 6173 2061 206e   function as a n
+00020fc0: 6573 7465 6420 6c69 7374 0a20 2020 2020  ested list.     
+00020fd0: 2020 2020 2020 2020 2020 2023 636f 6d70             #comp
+00020fe0: 7265 6865 6e73 696f 6e20 666f 7220 616c  rehension for al
+00020ff0: 6c20 7261 7374 6572 2063 656c 6c73 2c20  l raster cells, 
+00021000: 7768 6963 6820 4920 6265 6c69 6576 650a  which I believe.
+00021010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021020: 2373 686f 756c 6420 646f 2069 7473 2062  #should do its b
+00021030: 6573 7420 746f 2076 6563 746f 7269 7a65  est to vectorize
+00021040: 2074 6865 2077 686f 6c65 206f 7065 7261   the whole opera
+00021050: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00021060: 2020 2020 205b 5b70 6c6f 745f 6f6e 655f       [[plot_one_
+00021070: 6365 6c6c 286a 2c20 6929 2066 6f72 2069  cell(j, i) for i
+00021080: 2069 6e20 7261 6e67 6528 0a20 2020 2020   in range(.     
+00021090: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000210a0: 7572 662e 7375 7266 2e73 6861 7065 5b30  urf.surf.shape[0
+000210b0: 5d29 5d20 666f 7220 6a20 696e 2072 616e  ])] for j in ran
+000210c0: 6765 280a 2020 2020 2020 2020 2020 2020  ge(.            
+000210d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210e0: 2020 2020 2020 2020 7375 7266 2e73 7572          surf.sur
+000210f0: 662e 7368 6170 655b 315d 295d 0a0a 0a20  f.shape[1])]... 
+00021100: 2020 2023 2070 6c6f 7420 7468 6520 6c69     # plot the li
+00021110: 6e65 6167 6520 666f 7220 6120 6769 7665  neage for a give
+00021120: 6e20 6e6f 6465 2061 6e64 206c 6f63 7573  n node and locus
+00021130: 0a20 2020 2064 6566 205f 706c 6f74 5f67  .    def _plot_g
+00021140: 656e 655f 666c 6f77 2873 656c 662c 206c  ene_flow(self, l
+00021150: 6f63 7573 2c20 7374 796c 652c 206c 616e  ocus, style, lan
+00021160: 642c 206e 6f64 6573 3d4e 6f6e 652c 2069  d, nodes=None, i
+00021170: 6e64 6976 6964 733d 4e6f 6e65 2c0a 2020  ndivids=None,.  
+00021180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021190: 2020 2020 2063 6f6c 6f72 3d4e 6f6e 652c       color=None,
+000211a0: 2070 6865 6e6f 7479 7065 3d4e 6f6e 652c   phenotype=None,
+000211b0: 206c 7972 5f6e 756d 3d30 2c20 6a69 7474   lyr_num=0, jitt
+000211c0: 6572 3d54 7275 652c 0a20 2020 2020 2020  er=True,.       
+000211d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211e0: 616c 7068 613d 302e 352c 2073 697a 653d  alpha=0.5, size=
+000211f0: 3235 2c20 6164 645f 726f 6f74 733d 4661  25, add_roots=Fa
+00021200: 6c73 6529 3a0a 2020 2020 2020 2020 6966  lse):.        if
+00021210: 206e 6f74 2073 656c 662e 6765 6e5f 6172   not self.gen_ar
+00021220: 6368 2e75 7365 5f74 736b 6974 3a0a 2020  ch.use_tskit:.  
+00021230: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00021240: 4578 6365 7074 696f 6e28 2822 4765 6e65  Exception(("Gene
+00021250: 2066 6c6f 7720 6361 6e6e 6f74 2062 6520   flow cannot be 
+00021260: 706c 6f74 7465 6420 666f 7220 6120 5370  plotted for a Sp
+00021270: 6563 6965 7320 220a 2020 2020 2020 2020  ecies ".        
+00021280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021290: 2020 2020 2022 7768 6f73 6520 7370 6174       "whose spat
+000212a0: 6961 6c20 7065 6469 6772 6565 2069 7320  ial pedigree is 
+000212b0: 6e6f 7420 6265 696e 6720 7472 6163 6b65  not being tracke
+000212c0: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
+000212d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000212e0: 2022 6279 2074 736b 6974 2e22 2929 0a20   "by tskit.")). 
+000212f0: 2020 2020 2020 2061 7373 6572 7420 7374         assert st
+00021300: 796c 6520 696e 205b 276c 696e 6561 6765  yle in ['lineage
+00021310: 272c 2027 7665 6374 6f72 275d 2c20 2822  ', 'vector'], ("
+00021320: 5468 6520 7374 796c 6520 6172 6775 6d65  The style argume
+00021330: 6e74 206d 7573 7420 6265 2022 0a20 2020  nt must be ".   
+00021340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021370: 2020 2020 2020 2020 2020 2020 2022 2776               "'v
-00021380: 6563 746f 7227 2061 7320 6120 7661 6c75  ector' as a valu
-00021390: 652e 2229 0a20 2020 2020 2020 2069 6620  e.").        if 
-000213a0: 6e6f 6465 7320 6973 204e 6f6e 653a 0a20  nodes is None:. 
-000213b0: 2020 2020 2020 2020 2020 2023 2067 6574             # get
-000213c0: 2061 2072 616e 646f 6d20 7365 6c65 6374   a random select
-000213d0: 696f 6e20 6f66 206e 2069 6e64 6976 6964  ion of n individ
-000213e0: 7561 6c73 2c20 6966 2069 6e64 6976 6964  uals, if individ
-000213f0: 7327 2076 616c 7565 2069 7320 696e 740a  s' value is int.
-00021400: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00021410: 7369 6e73 7461 6e63 6528 696e 6469 7669  sinstance(indivi
-00021420: 6473 2c20 696e 7429 3a0a 2020 2020 2020  ds, int):.      
-00021430: 2020 2020 2020 2020 2020 696e 6469 7669            indivi
-00021440: 6473 203d 206e 702e 7261 6e64 6f6d 2e63  ds = np.random.c
-00021450: 686f 6963 6528 5b2a 7365 6c66 5d2c 2069  hoice([*self], i
-00021460: 6e64 6976 6964 732c 2072 6570 6c61 6365  ndivids, replace
-00021470: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00021480: 2020 2020 2373 6f72 7420 616e 6420 7369      #sort and si
-00021490: 6d70 6c69 6679 2074 6865 2054 6162 6c65  mplify the Table
-000214a0: 436f 6c6c 6563 7469 6f6e 2c20 6966 206e  Collection, if n
-000214b0: 6565 6465 6420 0a20 2020 2020 2020 2020  eeded .         
-000214c0: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-000214d0: 7463 5f73 6f72 7465 645f 616e 645f 7369  tc_sorted_and_si
-000214e0: 6d70 6c69 6669 6564 3a0a 2020 2020 2020  mplified:.      
-000214f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00021500: 736f 7274 5f61 6e64 5f73 696d 706c 6966  sort_and_simplif
-00021510: 795f 7461 626c 655f 636f 6c6c 6563 7469  y_table_collecti
-00021520: 6f6e 2829 0a20 2020 2020 2020 2020 2020  on().           
-00021530: 206e 6f64 6573 203d 2073 656c 662e 5f67   nodes = self._g
-00021540: 6574 5f6e 6f64 6573 2869 6e64 6976 6964  et_nodes(individ
-00021550: 733d 696e 6469 7669 6473 290a 0a20 2020  s=individs)..   
-00021560: 2020 2020 2023 2073 6f72 7420 616e 6420       # sort and 
-00021570: 7369 6d70 6c69 6679 2074 6865 2054 6162  simplify the Tab
-00021580: 6c65 436f 6c6c 6563 7469 6f6e 2069 6620  leCollection if 
-00021590: 6e65 6564 6564 0a20 2020 2020 2020 2069  needed.        i
-000215a0: 6620 6e6f 7420 7365 6c66 2e5f 7463 5f73  f not self._tc_s
-000215b0: 6f72 7465 645f 616e 645f 7369 6d70 6c69  orted_and_simpli
-000215c0: 6669 6564 3a0a 2020 2020 2020 2020 2020  fied:.          
-000215d0: 2020 7365 6c66 2e5f 736f 7274 5f61 6e64    self._sort_and
-000215e0: 5f73 696d 706c 6966 795f 7461 626c 655f  _simplify_table_
-000215f0: 636f 6c6c 6563 7469 6f6e 2829 0a20 2020  collection().   
-00021600: 2020 2020 2023 2067 7261 6220 7468 6520       # grab the 
-00021610: 5461 626c 6543 6f6c 6c65 6374 696f 6e20  TableCollection 
-00021620: 616e 6420 6974 7320 5472 6565 5365 7175  and its TreeSequ
-00021630: 656e 6365 0a20 2020 2020 2020 2074 6320  ence.        tc 
-00021640: 3d20 7365 6c66 2e5f 7463 0a20 2020 2020  = self._tc.     
-00021650: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00021660: 2020 2020 7473 203d 2074 632e 7472 6565      ts = tc.tree
-00021670: 5f73 6571 7565 6e63 6528 290a 2020 2020  _sequence().    
-00021680: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00021690: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-000216a0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-000216b0: 6e28 2822 5468 6520 7370 6563 6965 7327  n(("The species'
-000216c0: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-000216d0: 206d 7573 7420 6265 2073 6f72 7465 6420   must be sorted 
-000216e0: 616e 6420 220a 2020 2020 2020 2020 2020  and ".          
-000216f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021700: 2020 2022 7369 6d70 6c69 6669 6564 2062     "simplified b
-00021710: 6566 6f72 6520 7468 6973 206d 6574 686f  efore this metho
-00021720: 6420 6973 2063 616c 6c65 642e 2229 290a  d is called.")).
-00021730: 0a20 2020 2020 2020 206e 6f64 655f 6375  .        node_cu
-00021740: 7272 5f6c 6f63 7320 3d20 5b5b 692e 782c  rr_locs = [[i.x,
-00021750: 2069 2e79 5d20 666f 7220 6e20 696e 206e   i.y] for n in n
-00021760: 6f64 6573 2066 6f72 2069 2069 6e20 7365  odes for i in se
-00021770: 6c66 2e76 616c 7565 7328 0a20 2020 2020  lf.values(.     
-00021780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021790: 2020 2029 2069 6620 6e20 696e 2069 2e5f     ) if n in i._
-000217a0: 6e6f 6465 735f 7461 625f 6964 732e 7661  nodes_tab_ids.va
-000217b0: 6c75 6573 2829 5d0a 0a20 2020 2020 2020  lues()]..       
-000217c0: 2023 2067 6574 2074 6865 2074 7265 6520   # get the tree 
-000217d0: 666f 7220 7468 6973 206c 6f63 7573 0a20  for this locus. 
-000217e0: 2020 2020 2020 2074 7265 6520 3d20 7473         tree = ts
-000217f0: 2e61 736c 6973 7428 295b 5f67 6574 5f74  .aslist()[_get_t
-00021800: 7265 656e 756d 7328 7473 2c20 5b6c 6f63  reenums(ts, [loc
-00021810: 7573 5d29 5b30 5d5d 0a20 2020 2020 2020  us])[0]].       
-00021820: 2023 2067 6574 2074 6865 206c 696e 6561   # get the linea
-00021830: 6765 5f64 6963 7420 2877 6974 6820 6269  ge_dict (with bi
-00021840: 7274 6820 7469 6d65 7320 616e 6420 6269  rth times and bi
-00021850: 7274 6820 6c6f 6361 7469 6f6e 7329 0a20  rth locations). 
-00021860: 2020 2020 2020 206c 696e 5f64 6963 7420         lin_dict 
-00021870: 3d20 5f67 6574 5f6c 696e 6561 6765 5f64  = _get_lineage_d
-00021880: 6963 7473 5f6f 6e65 5f74 7265 6528 7463  icts_one_tree(tc
-00021890: 2c20 7472 6565 2c20 6e6f 6465 732c 2073  , tree, nodes, s
-000218a0: 656c 662e 7429 0a20 2020 2020 2020 2069  elf.t).        i
-000218b0: 6620 636f 6c6f 7220 6973 204e 6f6e 653a  f color is None:
-000218c0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-000218d0: 7265 6174 6520 7374 6172 742d 636f 6c6f  reate start-colo
-000218e0: 7220 7661 6c75 6573 2066 6f72 206e 6f64  r values for nod
-000218f0: 6573 2720 7365 7061 7261 7465 206c 696e  es' separate lin
-00021900: 6561 6765 2074 7261 636b 730a 2020 2020  eage tracks.    
-00021910: 2020 2020 2020 2020 636f 6c6f 7273 203d          colors =
-00021920: 205b 6d70 6c2e 636f 6c6f 7273 2e74 6f5f   [mpl.colors.to_
-00021930: 6865 7828 706c 742e 636d 2e53 6574 315f  hex(plt.cm.Set1_
-00021940: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00021950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021960: 2020 2020 2020 2020 2020 206e 2929 2066             n)) f
-00021970: 6f72 206e 2069 6e20 6e70 2e6c 696e 7370  or n in np.linsp
-00021980: 6163 6528 302c 2030 2e38 352c 2038 295d  ace(0, 0.85, 8)]
-00021990: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000219a0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-000219b0: 7320 3d20 5b63 6f6c 6f72 2066 6f72 205f  s = [color for _
-000219c0: 2069 6e20 7261 6e67 6528 3829 5d0a 2020   in range(8)].  
-000219d0: 2020 2020 2020 2320 706c 6f74 2074 6865        # plot the
-000219e0: 2073 7065 6369 6573 2c20 6569 7468 6572   species, either
-000219f0: 2077 6974 6820 6f72 2077 6974 686f 7574   with or without
-00021a00: 2070 6865 6e6f 7479 7065 2d70 6169 6e74   phenotype-paint
-00021a10: 696e 670a 2020 2020 2020 2020 6966 2070  ing.        if p
-00021a20: 6865 6e6f 7479 7065 2069 7320 4e6f 6e65  henotype is None
-00021a30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00021a40: 6c66 2e5f 706c 6f74 286c 7972 5f6e 756d  lf._plot(lyr_num
-00021a50: 3d6c 7972 5f6e 756d 2c20 6c61 6e64 3d6c  =lyr_num, land=l
-00021a60: 616e 642c 2073 697a 653d 7369 7a65 290a  and, size=size).
-00021a70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00021a80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00021a90: 706c 6f74 5f70 6865 6e6f 7479 7065 2870  plot_phenotype(p
-00021aa0: 6865 6e6f 7479 7065 2c20 6c61 6e64 3d6c  henotype, land=l
-00021ab0: 616e 642c 2073 697a 653d 7369 7a65 290a  and, size=size).
-00021ac0: 2020 2020 2020 2020 6178 203d 2070 6c74          ax = plt
-00021ad0: 2e67 6361 2829 0a20 2020 2020 2020 2023  .gca().        #
-00021ae0: 2065 7874 7261 6374 2061 6e64 2070 6c6f   extract and plo
-00021af0: 7420 7468 6520 7365 7269 6573 206f 6620  t the series of 
-00021b00: 706f 696e 7473 2066 6f72 2065 6163 6820  points for each 
-00021b10: 6e6f 6465 0a20 2020 2020 2020 2066 6f72  node.        for
-00021b20: 2069 2c20 6e6f 6465 2069 6e20 656e 756d   i, node in enum
-00021b30: 6572 6174 6528 6e6f 6465 7329 3a0a 2020  erate(nodes):.  
-00021b40: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-00021b50: 636f 6c20 3d20 636f 6c6f 7273 5b69 2025  col = colors[i %
-00021b60: 206c 656e 2863 6f6c 6f72 7329 5d0a 2020   len(colors)].  
-00021b70: 2020 2020 2020 2020 2020 6966 2073 7479            if sty
-00021b80: 6c65 203d 3d20 276c 696e 6561 6765 273a  le == 'lineage':
-00021b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021ba0: 206c 6f63 7320 3d20 6e70 2e76 7374 6163   locs = np.vstac
-00021bb0: 6b28 5b76 5b31 5d20 666f 7220 7620 696e  k([v[1] for v in
-00021bc0: 206c 696e 5f64 6963 745b 6e6f 6465 5d2e   lin_dict[node].
-00021bd0: 7661 6c75 6573 2829 5d29 0a20 2020 2020  values()]).     
-00021be0: 2020 2020 2020 2020 2020 2069 6620 6a69             if ji
-00021bf0: 7474 6572 3a0a 2020 2020 2020 2020 2020  tter:.          
-00021c00: 2020 2020 2020 2020 2020 6c6f 6373 203d            locs =
-00021c10: 206c 6f63 7320 2b20 6e70 2e72 616e 646f   locs + np.rando
-00021c20: 6d2e 6e6f 726d 616c 2830 2c20 302e 3031  m.normal(0, 0.01
-00021c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021c50: 2020 2020 2020 2020 2020 2020 2020 7369                si
-00021c60: 7a65 3d6c 6f63 732e 7369 7a65 292e 7265  ze=locs.size).re
-00021c70: 7368 6170 6528 6c6f 6373 2e73 6861 7065  shape(locs.shape
-00021c80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00021c90: 2020 2320 6372 6561 7465 206c 6973 7420    # create list 
-00021ca0: 6f66 2063 6f6c 6f72 7320 666f 7220 706c  of colors for pl
-00021cb0: 6f74 7469 6e67 2c0a 2020 2020 2020 2020  otting,.        
-00021cc0: 2020 2020 2020 2020 2320 7573 696e 6720          # using 
-00021cd0: 6c69 6e65 6172 6c79 2069 6e74 6572 706f  linearly interpo
-00021ce0: 6c61 7465 6420 636f 6c6f 7273 0a20 2020  lated colors.   
-00021cf0: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-00021d00: 6620 7468 6520 636f 6c6f 7220 6172 6775  f the color argu
-00021d10: 6d65 6e74 2077 6173 206e 6f74 2070 726f  ment was not pro
-00021d20: 7669 6465 642c 200a 2020 2020 2020 2020  vided, .        
-00021d30: 2020 2020 2020 2020 2320 6f72 2065 6c73          # or els
-00021d40: 6520 6a75 7374 2075 7369 6e67 2074 6865  e just using the
-00021d50: 2073 6f6c 6964 2063 6f6c 6f72 0a20 2020   solid color.   
-00021d60: 2020 2020 2020 2020 2020 2020 2023 2070               # p
-00021d70: 726f 7669 6465 6420 746f 2074 6865 2063  rovided to the c
-00021d80: 6f6c 6f72 2061 7267 756d 656e 740a 2020  olor argument.  
-00021d90: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00021da0: 6c6f 725f 6e75 6d73 203d 206e 702e 696e  lor_nums = np.in
-00021db0: 7438 286e 702e 6c69 6e73 7061 6365 2830  t8(np.linspace(0
-00021dc0: 2c20 3130 302c 206c 6f63 732e 7368 6170  , 100, locs.shap
-00021dd0: 655b 305d 2d31 2929 0a20 2020 2020 2020  e[0]-1)).       
-00021de0: 2020 2020 2020 2020 2069 6620 636f 6c6f           if colo
-00021df0: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-00021e00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00021e10: 6c6f 745f 636f 6c6f 7273 203d 5b76 697a  lot_colors =[viz
-00021e20: 2e5f 6361 6c63 5f72 6573 6861 6465 645f  ._calc_reshaded_
-00021e30: 636f 6c6f 7228 7374 6172 745f 636f 6c2c  color(start_col,
-00021e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e70: 2020 206e 756d 2920 666f 7220 6e75 6d20     num) for num 
-00021e80: 696e 2063 6f6c 6f72 5f6e 756d 735d 0a20  in color_nums]. 
-00021e90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00021ea0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00021eb0: 2020 2020 2020 2020 2070 6c6f 745f 636f           plot_co
-00021ec0: 6c6f 7273 203d 205b 7374 6172 745f 636f  lors = [start_co
-00021ed0: 6c20 666f 7220 6e75 6d20 696e 2063 6f6c  l for num in col
-00021ee0: 6f72 5f6e 756d 735d 0a20 2020 2020 2020  or_nums].       
-00021ef0: 2020 2020 2020 2020 2023 2063 7265 6174           # creat
-00021f00: 6520 6120 6c69 6e65 6172 2069 6e74 6572  e a linear inter
-00021f10: 706f 6c61 7469 6f6e 206f 6620 6c69 6e65  polation of line
-00021f20: 7769 6474 6873 0a20 2020 2020 2020 2020  widths.         
-00021f30: 2020 2020 2020 206c 696e 6577 6964 7468         linewidth
-00021f40: 7320 3d20 6e70 2e6c 696e 7370 6163 6528  s = np.linspace(
-00021f50: 332c 2030 2e38 352c 206c 6f63 732e 7368  3, 0.85, locs.sh
-00021f60: 6170 655b 305d 2d31 290a 2020 2020 2020  ape[0]-1).      
-00021f70: 2020 2020 2020 2020 2020 666f 7220 6e2c            for n,
-00021f80: 2063 6f6c 2069 6e20 656e 756d 6572 6174   col in enumerat
-00021f90: 6528 706c 6f74 5f63 6f6c 6f72 7329 3a0a  e(plot_colors):.
-00021fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021fb0: 2020 2020 2320 4e4f 5445 206e 6565 6420      # NOTE need 
-00021fc0: 746f 2075 7365 206f 6e6c 7920 7468 6520  to use only the 
-00021fd0: 6669 7273 7420 3220 7661 6c75 6573 2069  first 2 values i
-00021fe0: 6e20 7468 6520 6c6f 6361 7469 6f6e 0a20  n the location. 
-00021ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022000: 2020 2023 2064 6174 6120 6265 6361 7573     # data becaus
-00022010: 6520 7375 6273 6571 7565 6e74 2076 616c  e subsequent val
-00022020: 7565 7320 6172 6520 7573 6564 0a20 2020  ues are used.   
+00021360: 2020 2020 2020 2020 2020 2020 2022 6769               "gi
+00021370: 7665 6e20 6569 7468 6572 2027 6c69 6e65  ven either 'line
+00021380: 6167 6527 206f 7220 220a 2020 2020 2020  age' or ".      
+00021390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213b0: 2020 2020 2020 2020 2020 2227 7665 6374            "'vect
+000213c0: 6f72 2720 6173 2061 2076 616c 7565 2e22  or' as a value."
+000213d0: 290a 2020 2020 2020 2020 6966 206e 6f64  ).        if nod
+000213e0: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+000213f0: 2020 2020 2020 2020 2320 6765 7420 6120          # get a 
+00021400: 7261 6e64 6f6d 2073 656c 6563 7469 6f6e  random selection
+00021410: 206f 6620 6e20 696e 6469 7669 6475 616c   of n individual
+00021420: 732c 2069 6620 696e 6469 7669 6473 2720  s, if individs' 
+00021430: 7661 6c75 6520 6973 2069 6e74 0a20 2020  value is int.   
+00021440: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00021450: 7374 616e 6365 2869 6e64 6976 6964 732c  stance(individs,
+00021460: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+00021470: 2020 2020 2020 2069 6e64 6976 6964 7320         individs 
+00021480: 3d20 6e70 2e72 616e 646f 6d2e 6368 6f69  = np.random.choi
+00021490: 6365 285b 2a73 656c 665d 2c20 696e 6469  ce([*self], indi
+000214a0: 7669 6473 2c20 7265 706c 6163 653d 4661  vids, replace=Fa
+000214b0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+000214c0: 2023 736f 7274 2061 6e64 2073 696d 706c   #sort and simpl
+000214d0: 6966 7920 7468 6520 5461 626c 6543 6f6c  ify the TableCol
+000214e0: 6c65 6374 696f 6e2c 2069 6620 6e65 6564  lection, if need
+000214f0: 6564 200a 2020 2020 2020 2020 2020 2020  ed .            
+00021500: 6966 206e 6f74 2073 656c 662e 5f74 635f  if not self._tc_
+00021510: 736f 7274 6564 5f61 6e64 5f73 696d 706c  sorted_and_simpl
+00021520: 6966 6965 643a 0a20 2020 2020 2020 2020  ified:.         
+00021530: 2020 2020 2020 2073 656c 662e 5f73 6f72         self._sor
+00021540: 745f 616e 645f 7369 6d70 6c69 6679 5f74  t_and_simplify_t
+00021550: 6162 6c65 5f63 6f6c 6c65 6374 696f 6e28  able_collection(
+00021560: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
+00021570: 6465 7320 3d20 7365 6c66 2e5f 6765 745f  des = self._get_
+00021580: 6e6f 6465 7328 696e 6469 7669 6473 3d69  nodes(individs=i
+00021590: 6e64 6976 6964 7329 0a0a 2020 2020 2020  ndivids)..      
+000215a0: 2020 2320 736f 7274 2061 6e64 2073 696d    # sort and sim
+000215b0: 706c 6966 7920 7468 6520 5461 626c 6543  plify the TableC
+000215c0: 6f6c 6c65 6374 696f 6e20 6966 206e 6565  ollection if nee
+000215d0: 6465 640a 2020 2020 2020 2020 6966 206e  ded.        if n
+000215e0: 6f74 2073 656c 662e 5f74 635f 736f 7274  ot self._tc_sort
+000215f0: 6564 5f61 6e64 5f73 696d 706c 6966 6965  ed_and_simplifie
+00021600: 643a 0a20 2020 2020 2020 2020 2020 2073  d:.            s
+00021610: 656c 662e 5f73 6f72 745f 616e 645f 7369  elf._sort_and_si
+00021620: 6d70 6c69 6679 5f74 6162 6c65 5f63 6f6c  mplify_table_col
+00021630: 6c65 6374 696f 6e28 290a 2020 2020 2020  lection().      
+00021640: 2020 2320 6772 6162 2074 6865 2054 6162    # grab the Tab
+00021650: 6c65 436f 6c6c 6563 7469 6f6e 2061 6e64  leCollection and
+00021660: 2069 7473 2054 7265 6553 6571 7565 6e63   its TreeSequenc
+00021670: 650a 2020 2020 2020 2020 7463 203d 2073  e.        tc = s
+00021680: 656c 662e 5f74 630a 2020 2020 2020 2020  elf._tc.        
+00021690: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000216a0: 2074 7320 3d20 7463 2e74 7265 655f 7365   ts = tc.tree_se
+000216b0: 7175 656e 6365 2829 0a20 2020 2020 2020  quence().       
+000216c0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000216d0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
+000216e0: 6169 7365 2045 7863 6570 7469 6f6e 2828  aise Exception((
+000216f0: 2254 6865 2073 7065 6369 6573 2720 5461  "The species' Ta
+00021700: 626c 6543 6f6c 6c65 6374 696f 6e20 6d75  bleCollection mu
+00021710: 7374 2062 6520 736f 7274 6564 2061 6e64  st be sorted and
+00021720: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00021730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021740: 2273 696d 706c 6966 6965 6420 6265 666f  "simplified befo
+00021750: 7265 2074 6869 7320 6d65 7468 6f64 2069  re this method i
+00021760: 7320 6361 6c6c 6564 2e22 2929 0a0a 2020  s called."))..  
+00021770: 2020 2020 2020 6e6f 6465 5f63 7572 725f        node_curr_
+00021780: 6c6f 6373 203d 205b 5b69 2e78 2c20 692e  locs = [[i.x, i.
+00021790: 795d 2066 6f72 206e 2069 6e20 6e6f 6465  y] for n in node
+000217a0: 7320 666f 7220 6920 696e 2073 656c 662e  s for i in self.
+000217b0: 7661 6c75 6573 280a 2020 2020 2020 2020  values(.        
+000217c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000217d0: 2920 6966 206e 2069 6e20 692e 5f6e 6f64  ) if n in i._nod
+000217e0: 6573 5f74 6162 5f69 6473 2e76 616c 7565  es_tab_ids.value
+000217f0: 7328 295d 0a0a 2020 2020 2020 2020 2320  s()]..        # 
+00021800: 6765 7420 7468 6520 7472 6565 2066 6f72  get the tree for
+00021810: 2074 6869 7320 6c6f 6375 730a 2020 2020   this locus.    
+00021820: 2020 2020 7472 6565 203d 2074 732e 6173      tree = ts.as
+00021830: 6c69 7374 2829 5b5f 6765 745f 7472 6565  list()[_get_tree
+00021840: 6e75 6d73 2874 732c 205b 6c6f 6375 735d  nums(ts, [locus]
+00021850: 295b 305d 5d0a 2020 2020 2020 2020 2320  )[0]].        # 
+00021860: 6765 7420 7468 6520 6c69 6e65 6167 655f  get the lineage_
+00021870: 6469 6374 2028 7769 7468 2062 6972 7468  dict (with birth
+00021880: 2074 696d 6573 2061 6e64 2062 6972 7468   times and birth
+00021890: 206c 6f63 6174 696f 6e73 290a 2020 2020   locations).    
+000218a0: 2020 2020 6c69 6e5f 6469 6374 203d 205f      lin_dict = _
+000218b0: 6765 745f 6c69 6e65 6167 655f 6469 6374  get_lineage_dict
+000218c0: 735f 6f6e 655f 7472 6565 2874 632c 2074  s_one_tree(tc, t
+000218d0: 7265 652c 206e 6f64 6573 2c20 7365 6c66  ree, nodes, self
+000218e0: 2e74 290a 2020 2020 2020 2020 6966 2063  .t).        if c
+000218f0: 6f6c 6f72 2069 7320 4e6f 6e65 3a0a 2020  olor is None:.  
+00021900: 2020 2020 2020 2020 2020 2320 6372 6561            # crea
+00021910: 7465 2073 7461 7274 2d63 6f6c 6f72 2076  te start-color v
+00021920: 616c 7565 7320 666f 7220 6e6f 6465 7327  alues for nodes'
+00021930: 2073 6570 6172 6174 6520 6c69 6e65 6167   separate lineag
+00021940: 6520 7472 6163 6b73 0a20 2020 2020 2020  e tracks.       
+00021950: 2020 2020 2063 6f6c 6f72 7320 3d20 5b6d       colors = [m
+00021960: 706c 2e63 6f6c 6f72 732e 746f 5f68 6578  pl.colors.to_hex
+00021970: 2870 6c74 2e63 6d2e 5365 7431 5f72 280a  (plt.cm.Set1_r(.
+00021980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000219a0: 2020 2020 2020 2020 6e29 2920 666f 7220          n)) for 
+000219b0: 6e20 696e 206e 702e 6c69 6e73 7061 6365  n in np.linspace
+000219c0: 2830 2c20 302e 3835 2c20 3829 5d0a 2020  (0, 0.85, 8)].  
+000219d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000219e0: 2020 2020 2020 2020 636f 6c6f 7273 203d          colors =
+000219f0: 205b 636f 6c6f 7220 666f 7220 5f20 696e   [color for _ in
+00021a00: 2072 616e 6765 2838 295d 0a20 2020 2020   range(8)].     
+00021a10: 2020 2023 2070 6c6f 7420 7468 6520 7370     # plot the sp
+00021a20: 6563 6965 732c 2065 6974 6865 7220 7769  ecies, either wi
+00021a30: 7468 206f 7220 7769 7468 6f75 7420 7068  th or without ph
+00021a40: 656e 6f74 7970 652d 7061 696e 7469 6e67  enotype-painting
+00021a50: 0a20 2020 2020 2020 2069 6620 7068 656e  .        if phen
+00021a60: 6f74 7970 6520 6973 204e 6f6e 653a 0a20  otype is None:. 
+00021a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00021a80: 5f70 6c6f 7428 6c79 725f 6e75 6d3d 6c79  _plot(lyr_num=ly
+00021a90: 725f 6e75 6d2c 206c 616e 643d 6c61 6e64  r_num, land=land
+00021aa0: 2c20 7369 7a65 3d73 697a 6529 0a20 2020  , size=size).   
+00021ab0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00021ac0: 2020 2020 2020 2073 656c 662e 5f70 6c6f         self._plo
+00021ad0: 745f 7068 656e 6f74 7970 6528 7068 656e  t_phenotype(phen
+00021ae0: 6f74 7970 652c 206c 616e 643d 6c61 6e64  otype, land=land
+00021af0: 2c20 7369 7a65 3d73 697a 6529 0a20 2020  , size=size).   
+00021b00: 2020 2020 2061 7820 3d20 706c 742e 6763       ax = plt.gc
+00021b10: 6128 290a 2020 2020 2020 2020 2320 6578  a().        # ex
+00021b20: 7472 6163 7420 616e 6420 706c 6f74 2074  tract and plot t
+00021b30: 6865 2073 6572 6965 7320 6f66 2070 6f69  he series of poi
+00021b40: 6e74 7320 666f 7220 6561 6368 206e 6f64  nts for each nod
+00021b50: 650a 2020 2020 2020 2020 666f 7220 692c  e.        for i,
+00021b60: 206e 6f64 6520 696e 2065 6e75 6d65 7261   node in enumera
+00021b70: 7465 286e 6f64 6573 293a 0a20 2020 2020  te(nodes):.     
+00021b80: 2020 2020 2020 2073 7461 7274 5f63 6f6c         start_col
+00021b90: 203d 2063 6f6c 6f72 735b 6920 2520 6c65   = colors[i % le
+00021ba0: 6e28 636f 6c6f 7273 295d 0a20 2020 2020  n(colors)].     
+00021bb0: 2020 2020 2020 2069 6620 7374 796c 6520         if style 
+00021bc0: 3d3d 2027 6c69 6e65 6167 6527 3a0a 2020  == 'lineage':.  
+00021bd0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00021be0: 6373 203d 206e 702e 7673 7461 636b 285b  cs = np.vstack([
+00021bf0: 765b 315d 2066 6f72 2076 2069 6e20 6c69  v[1] for v in li
+00021c00: 6e5f 6469 6374 5b6e 6f64 655d 2e76 616c  n_dict[node].val
+00021c10: 7565 7328 295d 290a 2020 2020 2020 2020  ues()]).        
+00021c20: 2020 2020 2020 2020 6966 206a 6974 7465          if jitte
+00021c30: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00021c40: 2020 2020 2020 206c 6f63 7320 3d20 6c6f         locs = lo
+00021c50: 6373 202b 206e 702e 7261 6e64 6f6d 2e6e  cs + np.random.n
+00021c60: 6f72 6d61 6c28 302c 2030 2e30 312c 0a20  ormal(0, 0.01,. 
+00021c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c90: 2020 2020 2020 2020 2020 2073 697a 653d             size=
+00021ca0: 6c6f 6373 2e73 697a 6529 2e72 6573 6861  locs.size).resha
+00021cb0: 7065 286c 6f63 732e 7368 6170 6529 0a20  pe(locs.shape). 
+00021cc0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00021cd0: 2063 7265 6174 6520 6c69 7374 206f 6620   create list of 
+00021ce0: 636f 6c6f 7273 2066 6f72 2070 6c6f 7474  colors for plott
+00021cf0: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+00021d00: 2020 2020 2023 2075 7369 6e67 206c 696e       # using lin
+00021d10: 6561 726c 7920 696e 7465 7270 6f6c 6174  early interpolat
+00021d20: 6564 2063 6f6c 6f72 730a 2020 2020 2020  ed colors.      
+00021d30: 2020 2020 2020 2020 2020 2320 6966 2074            # if t
+00021d40: 6865 2063 6f6c 6f72 2061 7267 756d 656e  he color argumen
+00021d50: 7420 7761 7320 6e6f 7420 7072 6f76 6964  t was not provid
+00021d60: 6564 2c20 0a20 2020 2020 2020 2020 2020  ed, .           
+00021d70: 2020 2020 2023 206f 7220 656c 7365 206a       # or else j
+00021d80: 7573 7420 7573 696e 6720 7468 6520 736f  ust using the so
+00021d90: 6c69 6420 636f 6c6f 720a 2020 2020 2020  lid color.      
+00021da0: 2020 2020 2020 2020 2020 2320 7072 6f76            # prov
+00021db0: 6964 6564 2074 6f20 7468 6520 636f 6c6f  ided to the colo
+00021dc0: 7220 6172 6775 6d65 6e74 0a20 2020 2020  r argument.     
+00021dd0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+00021de0: 5f6e 756d 7320 3d20 6e70 2e69 6e74 3828  _nums = np.int8(
+00021df0: 6e70 2e6c 696e 7370 6163 6528 302c 2031  np.linspace(0, 1
+00021e00: 3030 2c20 6c6f 6373 2e73 6861 7065 5b30  00, locs.shape[0
+00021e10: 5d2d 3129 290a 2020 2020 2020 2020 2020  ]-1)).          
+00021e20: 2020 2020 2020 6966 2063 6f6c 6f72 2069        if color i
+00021e30: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00021e40: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
+00021e50: 5f63 6f6c 6f72 7320 3d5b 7669 7a2e 5f63  _colors =[viz._c
+00021e60: 616c 635f 7265 7368 6164 6564 5f63 6f6c  alc_reshaded_col
+00021e70: 6f72 2873 7461 7274 5f63 6f6c 2c0a 2020  or(start_col,.  
+00021e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021eb0: 6e75 6d29 2066 6f72 206e 756d 2069 6e20  num) for num in 
+00021ec0: 636f 6c6f 725f 6e75 6d73 5d0a 2020 2020  color_nums].    
+00021ed0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00021ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021ef0: 2020 2020 2020 706c 6f74 5f63 6f6c 6f72        plot_color
+00021f00: 7320 3d20 5b73 7461 7274 5f63 6f6c 2066  s = [start_col f
+00021f10: 6f72 206e 756d 2069 6e20 636f 6c6f 725f  or num in color_
+00021f20: 6e75 6d73 5d0a 2020 2020 2020 2020 2020  nums].          
+00021f30: 2020 2020 2020 2320 6372 6561 7465 2061        # create a
+00021f40: 206c 696e 6561 7220 696e 7465 7270 6f6c   linear interpol
+00021f50: 6174 696f 6e20 6f66 206c 696e 6577 6964  ation of linewid
+00021f60: 7468 730a 2020 2020 2020 2020 2020 2020  ths.            
+00021f70: 2020 2020 6c69 6e65 7769 6474 6873 203d      linewidths =
+00021f80: 206e 702e 6c69 6e73 7061 6365 2833 2c20   np.linspace(3, 
+00021f90: 302e 3835 2c20 6c6f 6373 2e73 6861 7065  0.85, locs.shape
+00021fa0: 5b30 5d2d 3129 0a20 2020 2020 2020 2020  [0]-1).         
+00021fb0: 2020 2020 2020 2066 6f72 206e 2c20 636f         for n, co
+00021fc0: 6c20 696e 2065 6e75 6d65 7261 7465 2870  l in enumerate(p
+00021fd0: 6c6f 745f 636f 6c6f 7273 293a 0a20 2020  lot_colors):.   
+00021fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ff0: 2023 204e 4f54 4520 6e65 6564 2074 6f20   # NOTE need to 
+00022000: 7573 6520 6f6e 6c79 2074 6865 2066 6972  use only the fir
+00022010: 7374 2032 2076 616c 7565 7320 696e 2074  st 2 values in t
+00022020: 6865 206c 6f63 6174 696f 6e0a 2020 2020  he location.    
 00022030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022040: 2023 2074 6f20 7374 6f72 6520 696e 6469   # to store indi
-00022050: 7669 6475 616c 7327 2070 6865 6e6f 7479  viduals' phenoty
-00022060: 7065 7320 616e 6420 6669 746e 6573 730a  pes and fitness.
-00022070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022080: 2020 2020 6178 2e70 6c6f 7428 6c6f 6373      ax.plot(locs
-00022090: 5b6e 3a6e 2b32 2c20 305d 2c20 6c6f 6373  [n:n+2, 0], locs
-000220a0: 5b6e 3a6e 2b32 2c20 315d 2c20 6c69 6e65  [n:n+2, 1], line
-000220b0: 7374 796c 653d 2773 6f6c 6964 272c 0a20  style='solid',. 
-000220c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000220d0: 2020 2020 2020 2020 2020 206d 6172 6b65             marke
-000220e0: 723d 276f 272c 206d 6172 6b65 7273 697a  r='o', markersiz
-000220f0: 653d 7369 7a65 2a2a 2831 2f32 292c 2063  e=size**(1/2), c
-00022100: 6f6c 6f72 3d63 6f6c 2c0a 2020 2020 2020  olor=col,.      
-00022110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022120: 2020 2020 2020 6c69 6e65 7769 6474 683d        linewidth=
-00022130: 6c69 6e65 7769 6474 6873 5b6e 5d2c 2061  linewidths[n], a
-00022140: 6c70 6861 3d61 6c70 6861 290a 2020 2020  lpha=alpha).    
-00022150: 2020 2020 2020 2020 656c 6966 2073 7479          elif sty
-00022160: 6c65 203d 3d20 2776 6563 746f 7227 3a0a  le == 'vector':.
-00022170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022180: 2320 6765 7420 7468 6520 7374 6172 7420  # get the start 
-00022190: 616e 6420 656e 6420 6c6f 6361 7469 6f6e  and end location
-000221a0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000221b0: 2020 2320 4e4f 5445 206e 6565 6420 746f    # NOTE need to
-000221c0: 2074 616b 6520 6f6e 6c79 2074 6865 2066   take only the f
-000221d0: 6972 7374 2032 2076 616c 7565 7320 696e  irst 2 values in
-000221e0: 2074 6865 206c 6f63 6174 696f 6e0a 2020   the location.  
-000221f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00022200: 6461 7461 2062 6563 6175 7365 2073 7562  data because sub
-00022210: 7365 7175 656e 7420 7661 6c75 6573 2061  sequent values a
-00022220: 7265 2075 7365 6420 746f 2073 746f 7265  re used to store
-00022230: 2069 6e64 6976 6964 7561 6c73 2720 0a20   individuals' . 
-00022240: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00022250: 2070 6865 6e6f 7479 7065 7320 616e 6420   phenotypes and 
-00022260: 6669 746e 6573 730a 2020 2020 2020 2020  fitness.        
-00022270: 2020 2020 2020 2020 6265 675f 6c6f 6320          beg_loc 
-00022280: 3d20 5b2a 6c69 6e5f 6469 6374 5b6e 6f64  = [*lin_dict[nod
-00022290: 655d 2e76 616c 7565 7328 295d 5b2d 315d  e].values()][-1]
-000222a0: 5b31 5d5b 3a32 5d0a 2020 2020 2020 2020  [1][:2].        
-000222b0: 2020 2020 2020 2020 656e 645f 6c6f 6320          end_loc 
-000222c0: 3d20 5b2a 6c69 6e5f 6469 6374 5b6e 6f64  = [*lin_dict[nod
-000222d0: 655d 2e76 616c 7565 7328 295d 5b30 5d5b  e].values()][0][
-000222e0: 315d 5b3a 325d 0a20 2020 2020 2020 2020  1][:2].         
-000222f0: 2020 2020 2020 2064 782c 2064 7920 3d20         dx, dy = 
-00022300: 5b65 6e64 5f6c 6f63 5b69 5d20 2d20 6265  [end_loc[i] - be
-00022310: 675f 6c6f 635b 695d 2066 6f72 2069 2069  g_loc[i] for i i
-00022320: 6e20 7261 6e67 6528 3229 5d0a 2020 2020  n range(2)].    
-00022330: 2020 2020 2020 2020 2020 2020 2320 706c              # pl
-00022340: 6f74 2074 6865 2076 6563 746f 720a 2020  ot the vector.  
-00022350: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00022360: 4e4f 5445 3a20 5348 4f55 4c44 2049 2042  NOTE: SHOULD I B
-00022370: 4520 4649 5454 494e 4720 4120 5245 4752  E FITTING A REGR
-00022380: 4553 5349 4f4e 204c 494e 4520 544f 2054  ESSION LINE TO T
-00022390: 4845 2058 2041 4e44 2059 0a20 2020 2020  HE X AND Y.     
-000223a0: 2020 2020 2020 2020 2020 2023 204c 4f43             # LOC
-000223b0: 4154 494f 4e53 2c20 544f 2047 4554 2054  ATIONS, TO GET T
-000223c0: 4845 2027 4156 4552 4147 4527 2056 4543  HE 'AVERAGE' VEC
-000223d0: 544f 522c 2052 4154 4845 5220 5448 414e  TOR, RATHER THAN
-000223e0: 204a 5553 540a 2020 2020 2020 2020 2020   JUST.          
-000223f0: 2020 2020 2020 2320 504c 4f54 5449 4e47        # PLOTTING
-00022400: 2054 4845 2056 4543 544f 5220 4245 5457   THE VECTOR BETW
-00022410: 4545 4e20 5448 4520 4f4c 4445 5354 2041  EEN THE OLDEST A
-00022420: 4e44 2043 5552 5245 4e54 2050 4f53 4954  ND CURRENT POSIT
-00022430: 494f 4e53 0a20 2020 2020 2020 2020 2020  IONS.           
-00022440: 2020 2020 2023 2028 5748 4943 4820 434f       # (WHICH CO
-00022450: 554c 4420 4541 5349 4c59 204d 4953 5245  ULD EASILY MISRE
-00022460: 5052 4553 454e 5420 5448 4520 4f56 4552  PRESENT THE OVER
-00022470: 414c 4c20 5452 454e 4420 4245 4341 5553  ALL TREND BECAUS
-00022480: 4520 0a20 2020 2020 2020 2020 2020 2020  E .             
-00022490: 2020 2023 204f 4620 4348 414e 4345 2041     # OF CHANCE A
-000224a0: 5459 5049 4341 4c20 4c4f 4341 5449 4f4e  TYPICAL LOCATION
-000224b0: 5320 464f 5220 4549 5448 4552 204f 4620  S FOR EITHER OF 
-000224c0: 5448 4f53 4520 5457 4f20 504f 5349 5449  THOSE TWO POSITI
-000224d0: 4f4e 530a 2020 2020 2020 2020 2020 2020  ONS.            
-000224e0: 2020 2020 6178 2e61 7272 6f77 282a 6265      ax.arrow(*be
-000224f0: 675f 6c6f 632c 2064 782c 2064 792c 2063  g_loc, dx, dy, c
-00022500: 6f6c 6f72 3d73 7461 7274 5f63 6f6c 2c0a  olor=start_col,.
-00022510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022520: 2020 2020 2020 2020 2077 6964 7468 3d30           width=0
-00022530: 2e30 352c 2068 6561 645f 7769 6474 683d  .05, head_width=
-00022540: 302e 342c 206c 656e 6774 685f 696e 636c  0.4, length_incl
-00022550: 7564 6573 5f68 6561 643d 5472 7565 290a  udes_head=True).
-00022560: 2020 2020 2020 2020 2020 2020 2320 706c              # pl
-00022570: 6f74 2074 6865 206e 6f64 6573 2720 6375  ot the nodes' cu
-00022580: 7272 656e 7420 6c6f 6361 7469 6f6e 7320  rrent locations 
-00022590: 616e 6420 7468 6569 7220 6269 7274 6820  and their birth 
-000225a0: 6c6f 6361 7469 6f6e 732c 0a20 2020 2020  locations,.     
-000225b0: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-000225c0: 6564 2062 7920 6120 7468 696e 2062 6c61  ed by a thin bla
-000225d0: 636b 206c 696e 650a 2020 2020 2020 2020  ck line.        
-000225e0: 2020 2020 6e6f 6465 5f63 7572 725f 6c6f      node_curr_lo
-000225f0: 6320 3d20 6e6f 6465 5f63 7572 725f 6c6f  c = node_curr_lo
-00022600: 6373 5b69 5d0a 2020 2020 2020 2020 2020  cs[i].          
-00022610: 2020 6e6f 6465 5f62 6972 7468 5f6c 6f63    node_birth_loc
-00022620: 203d 205b 2a6c 696e 5f64 6963 745b 6e6f   = [*lin_dict[no
-00022630: 6465 5d2e 7661 6c75 6573 2829 5d5b 305d  de].values()][0]
-00022640: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-00022650: 706c 742e 706c 6f74 285b 6e6f 6465 5f62  plt.plot([node_b
-00022660: 6972 7468 5f6c 6f63 5b30 5d2c 206e 6f64  irth_loc[0], nod
-00022670: 655f 6375 7272 5f6c 6f63 5b30 5d5d 2c0a  e_curr_loc[0]],.
-00022680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022690: 2020 2020 205b 6e6f 6465 5f62 6972 7468       [node_birth
-000226a0: 5f6c 6f63 5b31 5d2c 206e 6f64 655f 6375  _loc[1], node_cu
-000226b0: 7272 5f6c 6f63 5b31 5d5d 2c0a 2020 2020  rr_loc[1]],.    
+00022040: 2320 6461 7461 2062 6563 6175 7365 2073  # data because s
+00022050: 7562 7365 7175 656e 7420 7661 6c75 6573  ubsequent values
+00022060: 2061 7265 2075 7365 640a 2020 2020 2020   are used.      
+00022070: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00022080: 746f 2073 746f 7265 2069 6e64 6976 6964  to store individ
+00022090: 7561 6c73 2720 7068 656e 6f74 7970 6573  uals' phenotypes
+000220a0: 2061 6e64 2066 6974 6e65 7373 0a20 2020   and fitness.   
+000220b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000220c0: 2061 782e 706c 6f74 286c 6f63 735b 6e3a   ax.plot(locs[n:
+000220d0: 6e2b 322c 2030 5d2c 206c 6f63 735b 6e3a  n+2, 0], locs[n:
+000220e0: 6e2b 322c 2031 5d2c 206c 696e 6573 7479  n+2, 1], linesty
+000220f0: 6c65 3d27 736f 6c69 6427 2c0a 2020 2020  le='solid',.    
+00022100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022110: 2020 2020 2020 2020 6d61 726b 6572 3d27          marker='
+00022120: 6f27 2c20 6d61 726b 6572 7369 7a65 3d73  o', markersize=s
+00022130: 697a 652a 2a28 312f 3229 2c20 636f 6c6f  ize**(1/2), colo
+00022140: 723d 636f 6c2c 0a20 2020 2020 2020 2020  r=col,.         
+00022150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022160: 2020 206c 696e 6577 6964 7468 3d6c 696e     linewidth=lin
+00022170: 6577 6964 7468 735b 6e5d 2c20 616c 7068  ewidths[n], alph
+00022180: 613d 616c 7068 6129 0a20 2020 2020 2020  a=alpha).       
+00022190: 2020 2020 2065 6c69 6620 7374 796c 6520       elif style 
+000221a0: 3d3d 2027 7665 6374 6f72 273a 0a20 2020  == 'vector':.   
+000221b0: 2020 2020 2020 2020 2020 2020 2023 2067               # g
+000221c0: 6574 2074 6865 2073 7461 7274 2061 6e64  et the start and
+000221d0: 2065 6e64 206c 6f63 6174 696f 6e73 0a20   end locations. 
+000221e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000221f0: 204e 4f54 4520 6e65 6564 2074 6f20 7461   NOTE need to ta
+00022200: 6b65 206f 6e6c 7920 7468 6520 6669 7273  ke only the firs
+00022210: 7420 3220 7661 6c75 6573 2069 6e20 7468  t 2 values in th
+00022220: 6520 6c6f 6361 7469 6f6e 0a20 2020 2020  e location.     
+00022230: 2020 2020 2020 2020 2020 2023 2064 6174             # dat
+00022240: 6120 6265 6361 7573 6520 7375 6273 6571  a because subseq
+00022250: 7565 6e74 2076 616c 7565 7320 6172 6520  uent values are 
+00022260: 7573 6564 2074 6f20 7374 6f72 6520 696e  used to store in
+00022270: 6469 7669 6475 616c 7327 200a 2020 2020  dividuals' .    
+00022280: 2020 2020 2020 2020 2020 2020 2320 7068              # ph
+00022290: 656e 6f74 7970 6573 2061 6e64 2066 6974  enotypes and fit
+000222a0: 6e65 7373 0a20 2020 2020 2020 2020 2020  ness.           
+000222b0: 2020 2020 2062 6567 5f6c 6f63 203d 205b       beg_loc = [
+000222c0: 2a6c 696e 5f64 6963 745b 6e6f 6465 5d2e  *lin_dict[node].
+000222d0: 7661 6c75 6573 2829 5d5b 2d31 5d5b 315d  values()][-1][1]
+000222e0: 5b3a 325d 0a20 2020 2020 2020 2020 2020  [:2].           
+000222f0: 2020 2020 2065 6e64 5f6c 6f63 203d 205b       end_loc = [
+00022300: 2a6c 696e 5f64 6963 745b 6e6f 6465 5d2e  *lin_dict[node].
+00022310: 7661 6c75 6573 2829 5d5b 305d 5b31 5d5b  values()][0][1][
+00022320: 3a32 5d0a 2020 2020 2020 2020 2020 2020  :2].            
+00022330: 2020 2020 6478 2c20 6479 203d 205b 656e      dx, dy = [en
+00022340: 645f 6c6f 635b 695d 202d 2062 6567 5f6c  d_loc[i] - beg_l
+00022350: 6f63 5b69 5d20 666f 7220 6920 696e 2072  oc[i] for i in r
+00022360: 616e 6765 2832 295d 0a20 2020 2020 2020  ange(2)].       
+00022370: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
+00022380: 7468 6520 7665 6374 6f72 0a20 2020 2020  the vector.     
+00022390: 2020 2020 2020 2020 2020 2023 204e 4f54             # NOT
+000223a0: 453a 2053 484f 554c 4420 4920 4245 2046  E: SHOULD I BE F
+000223b0: 4954 5449 4e47 2041 2052 4547 5245 5353  ITTING A REGRESS
+000223c0: 494f 4e20 4c49 4e45 2054 4f20 5448 4520  ION LINE TO THE 
+000223d0: 5820 414e 4420 590a 2020 2020 2020 2020  X AND Y.        
+000223e0: 2020 2020 2020 2020 2320 4c4f 4341 5449          # LOCATI
+000223f0: 4f4e 532c 2054 4f20 4745 5420 5448 4520  ONS, TO GET THE 
+00022400: 2741 5645 5241 4745 2720 5645 4354 4f52  'AVERAGE' VECTOR
+00022410: 2c20 5241 5448 4552 2054 4841 4e20 4a55  , RATHER THAN JU
+00022420: 5354 0a20 2020 2020 2020 2020 2020 2020  ST.             
+00022430: 2020 2023 2050 4c4f 5454 494e 4720 5448     # PLOTTING TH
+00022440: 4520 5645 4354 4f52 2042 4554 5745 454e  E VECTOR BETWEEN
+00022450: 2054 4845 204f 4c44 4553 5420 414e 4420   THE OLDEST AND 
+00022460: 4355 5252 454e 5420 504f 5349 5449 4f4e  CURRENT POSITION
+00022470: 530a 2020 2020 2020 2020 2020 2020 2020  S.              
+00022480: 2020 2320 2857 4849 4348 2043 4f55 4c44    # (WHICH COULD
+00022490: 2045 4153 494c 5920 4d49 5352 4550 5245   EASILY MISREPRE
+000224a0: 5345 4e54 2054 4845 204f 5645 5241 4c4c  SENT THE OVERALL
+000224b0: 2054 5245 4e44 2042 4543 4155 5345 200a   TREND BECAUSE .
+000224c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000224d0: 2320 4f46 2043 4841 4e43 4520 4154 5950  # OF CHANCE ATYP
+000224e0: 4943 414c 204c 4f43 4154 494f 4e53 2046  ICAL LOCATIONS F
+000224f0: 4f52 2045 4954 4845 5220 4f46 2054 484f  OR EITHER OF THO
+00022500: 5345 2054 574f 2050 4f53 4954 494f 4e53  SE TWO POSITIONS
+00022510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022520: 2061 782e 6172 726f 7728 2a62 6567 5f6c   ax.arrow(*beg_l
+00022530: 6f63 2c20 6478 2c20 6479 2c20 636f 6c6f  oc, dx, dy, colo
+00022540: 723d 7374 6172 745f 636f 6c2c 0a20 2020  r=start_col,.   
+00022550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022560: 2020 2020 2020 7769 6474 683d 302e 3035        width=0.05
+00022570: 2c20 6865 6164 5f77 6964 7468 3d30 2e34  , head_width=0.4
+00022580: 2c20 6c65 6e67 7468 5f69 6e63 6c75 6465  , length_include
+00022590: 735f 6865 6164 3d54 7275 6529 0a20 2020  s_head=True).   
+000225a0: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
+000225b0: 7468 6520 6e6f 6465 7327 2063 7572 7265  the nodes' curre
+000225c0: 6e74 206c 6f63 6174 696f 6e73 2061 6e64  nt locations and
+000225d0: 2074 6865 6972 2062 6972 7468 206c 6f63   their birth loc
+000225e0: 6174 696f 6e73 2c0a 2020 2020 2020 2020  ations,.        
+000225f0: 2020 2020 2320 636f 6e6e 6563 7465 6420      # connected 
+00022600: 6279 2061 2074 6869 6e20 626c 6163 6b20  by a thin black 
+00022610: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
+00022620: 206e 6f64 655f 6375 7272 5f6c 6f63 203d   node_curr_loc =
+00022630: 206e 6f64 655f 6375 7272 5f6c 6f63 735b   node_curr_locs[
+00022640: 695d 0a20 2020 2020 2020 2020 2020 206e  i].            n
+00022650: 6f64 655f 6269 7274 685f 6c6f 6320 3d20  ode_birth_loc = 
+00022660: 5b2a 6c69 6e5f 6469 6374 5b6e 6f64 655d  [*lin_dict[node]
+00022670: 2e76 616c 7565 7328 295d 5b30 5d5b 315d  .values()][0][1]
+00022680: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
+00022690: 2e70 6c6f 7428 5b6e 6f64 655f 6269 7274  .plot([node_birt
+000226a0: 685f 6c6f 635b 305d 2c20 6e6f 6465 5f63  h_loc[0], node_c
+000226b0: 7572 725f 6c6f 635b 305d 5d2c 0a20 2020  urr_loc[0]],.   
 000226c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000226d0: 2063 6f6c 6f72 3d73 7461 7274 5f63 6f6c   color=start_col
-000226e0: 2c20 6c69 6e65 7374 796c 653d 273a 272c  , linestyle=':',
-000226f0: 2061 6c70 6861 3d61 6c70 6861 2c0a 2020   alpha=alpha,.  
-00022700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022710: 2020 206c 696e 6577 6964 7468 3d31 2e32     linewidth=1.2
-00022720: 290a 0a20 2020 2020 2020 2069 6620 6164  )..        if ad
-00022730: 645f 726f 6f74 733a 0a20 2020 2020 2020  d_roots:.       
-00022740: 2020 2020 2073 656c 662e 5f70 6c6f 745f       self._plot_
-00022750: 6c69 6e65 6167 655f 726f 6f74 7328 7463  lineage_roots(tc
-00022760: 2c20 7472 6565 290a 0a0a 2020 2020 2320  , tree)...    # 
-00022770: 706c 6f74 2074 6865 206c 696e 6561 6765  plot the lineage
-00022780: 2066 6f72 2061 2067 6976 656e 206e 6f64   for a given nod
-00022790: 6520 616e 6420 6c6f 6375 730a 2020 2020  e and locus.    
-000227a0: 6465 6620 5f70 6c6f 745f 6c69 6e65 6167  def _plot_lineag
-000227b0: 655f 726f 6f74 7328 7365 6c66 2c20 7463  e_roots(self, tc
-000227c0: 2c20 7472 6565 2c20 616c 7068 613d 302e  , tree, alpha=0.
-000227d0: 382c 2073 697a 653d 3735 293a 0a20 2020  8, size=75):.   
-000227e0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-000227f0: 2e67 656e 5f61 7263 682e 7573 655f 7473  .gen_arch.use_ts
-00022800: 6b69 743a 0a20 2020 2020 2020 2020 2020  kit:.           
-00022810: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00022820: 2828 224c 696e 6561 6765 2072 6f6f 7473  (("Lineage roots
-00022830: 2063 616e 6e6f 7420 6265 2070 6c6f 7474   cannot be plott
-00022840: 6564 2066 6f72 2061 2053 7065 6369 6573  ed for a Species
-00022850: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00022860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022870: 2277 686f 7365 2073 7061 7469 616c 2070  "whose spatial p
-00022880: 6564 6967 7265 6520 6973 206e 6f74 2062  edigree is not b
-00022890: 6569 6e67 2074 7261 636b 6564 2022 0a20  eing tracked ". 
-000228a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228b0: 2020 2020 2020 2020 2020 2020 2262 7920              "by 
-000228c0: 7473 6b69 742e 2229 290a 0a20 2020 2020  tskit."))..     
-000228d0: 2020 2023 2067 6574 2074 6865 206e 6f64     # get the nod
-000228e0: 6573 0a20 2020 2020 2020 2061 6c6c 5f6e  es.        all_n
-000228f0: 6f64 6573 203d 2073 656c 662e 5f67 6574  odes = self._get
-00022900: 5f6e 6f64 6573 2829 0a0a 2020 2020 2020  _nodes()..      
-00022910: 2020 2320 6765 7420 7468 6520 6c69 6e65    # get the line
-00022920: 6167 6520 6469 6374 2066 6f72 2061 6c6c  age dict for all
-00022930: 206e 6f64 6573 0a20 2020 2020 2020 206c   nodes.        l
-00022940: 696e 5f64 6963 7420 3d20 5f67 6574 5f6c  in_dict = _get_l
-00022950: 696e 6561 6765 5f64 6963 7473 5f6f 6e65  ineage_dicts_one
-00022960: 5f74 7265 6528 7463 2c20 7472 6565 2c20  _tree(tc, tree, 
-00022970: 616c 6c5f 6e6f 6465 732c 2073 656c 662e  all_nodes, self.
-00022980: 7429 0a0a 2020 2020 2020 2020 2320 6765  t)..        # ge
-00022990: 7420 7468 6520 726f 6f74 7320 666f 7220  t the roots for 
-000229a0: 616c 6c20 6469 7374 696e 6374 206c 696e  all distinct lin
-000229b0: 6561 6765 7320 6174 2074 6869 7320 6c6f  eages at this lo
-000229c0: 6375 730a 2020 2020 2020 2020 726f 6f74  cus.        root
-000229d0: 5f6e 6f64 6573 203d 206e 702e 756e 6971  _nodes = np.uniq
-000229e0: 7565 285b 5b2a 6c69 6e5f 6469 6374 5b6e  ue([[*lin_dict[n
-000229f0: 5d2e 6b65 7973 2829 5d5b 2d31 5d20 666f  ].keys()][-1] fo
-00022a00: 7220 6e20 696e 2061 6c6c 5f6e 6f64 6573  r n in all_nodes
-00022a10: 5d29 0a0a 2020 2020 2020 2020 2320 6765  ])..        # ge
-00022a20: 7420 6269 7274 6820 6c6f 6361 7469 6f6e  t birth location
-00022a30: 7320 666f 7220 6561 6368 2072 6f6f 7420  s for each root 
-00022a40: 6e6f 6465 0a20 2020 2020 2020 2072 6f6f  node.        roo
-00022a50: 745f 696e 6469 7669 6473 203d 205b 7463  t_individs = [tc
-00022a60: 2e6e 6f64 6573 5b6e 5d2e 696e 6469 7669  .nodes[n].indivi
-00022a70: 6475 616c 2066 6f72 206e 2069 6e20 726f  dual for n in ro
-00022a80: 6f74 5f6e 6f64 6573 5d0a 2020 2020 2020  ot_nodes].      
-00022a90: 2020 726f 6f74 5f6c 6f63 7320 3d20 5b74    root_locs = [t
-00022aa0: 632e 696e 6469 7669 6475 616c 735b 695d  c.individuals[i]
-00022ab0: 2e6c 6f63 6174 696f 6e20 666f 7220 6920  .location for i 
-00022ac0: 696e 2072 6f6f 745f 696e 6469 7669 6473  in root_individs
-00022ad0: 5d0a 0a20 2020 2020 2020 2023 2065 7874  ]..        # ext
-00022ae0: 7261 6374 2061 6e64 2070 6c6f 7420 7468  ract and plot th
-00022af0: 6520 7365 7269 6573 206f 6620 706f 696e  e series of poin
-00022b00: 7473 2066 6f72 2065 6163 6820 6e6f 6465  ts for each node
-00022b10: 0a20 2020 2020 2020 2066 6f72 2078 2c20  .        for x, 
-00022b20: 7920 696e 2072 6f6f 745f 6c6f 6373 3a0a  y in root_locs:.
-00022b30: 2020 2020 2020 2020 2020 2020 2320 706c              # pl
-00022b40: 6f74 2074 6865 2072 6f6f 7420 6e6f 6465  ot the root node
-00022b50: 7327 2062 6972 7468 206c 6f63 6174 696f  s' birth locatio
-00022b60: 6e73 0a20 2020 2020 2020 2020 2020 2070  ns.            p
-00022b70: 6c74 2e73 6361 7474 6572 2878 2c20 792c  lt.scatter(x, y,
-00022b80: 2063 3d27 7768 6974 6527 2c20 733d 7369   c='white', s=si
-00022b90: 7a65 2c20 616c 7068 613d 616c 7068 612c  ze, alpha=alpha,
-00022ba0: 206d 6172 6b65 723d 2773 2729 0a20 2020   marker='s').   
-00022bb0: 2020 2020 2070 6c74 2e73 686f 7728 290a       plt.show().
-00022bc0: 0a0a 2020 2020 2320 6d65 7468 6f64 2066  ..    # method f
-00022bd0: 6f72 2070 6c6f 7474 696e 6720 6120 7370  or plotting a sp
-00022be0: 6563 6965 7327 2070 6f70 756c 6174 696f  ecies' populatio
-00022bf0: 6e20 7079 7261 6d69 640a 2020 2020 6465  n pyramid.    de
-00022c00: 6620 5f70 6c6f 745f 6465 6d6f 6772 6170  f _plot_demograp
-00022c10: 6869 635f 7079 7261 6d69 6428 7365 6c66  hic_pyramid(self
-00022c20: 293a 0a20 2020 2020 2020 2023 6d61 6b65  ):.        #make
-00022c30: 2064 6963 7420 6f66 2066 656d 616c 6520   dict of female 
-00022c40: 616e 6420 6d61 6c65 2063 6f6c 6f72 730a  and male colors.
-00022c50: 2020 2020 2020 2020 636f 6c5f 6469 6374          col_dict
-00022c60: 203d 207b 2d31 3a20 2763 7961 6e27 2c20   = {-1: 'cyan', 
-00022c70: 313a 2027 7069 6e6b 277d 0a20 2020 2020  1: 'pink'}.     
-00022c80: 2020 2023 6372 6561 7465 2061 2066 6967     #create a fig
-00022c90: 7572 650a 2020 2020 2020 2020 6669 6720  ure.        fig 
-00022ca0: 3d20 706c 742e 6669 6775 7265 2829 0a20  = plt.figure(). 
-00022cb0: 2020 2020 2020 2023 7661 7269 6162 6c65         #variable
-00022cc0: 7320 746f 2067 7261 6220 7468 6520 6d61  s to grab the ma
-00022cd0: 7820 636f 756e 740a 2020 2020 2020 2020  x count.        
-00022ce0: 6d61 785f 636f 756e 7420 3d20 300a 2020  max_count = 0.  
-00022cf0: 2020 2020 2020 2366 6f72 2065 6163 6820        #for each 
-00022d00: 7365 780a 2020 2020 2020 2020 666f 7220  sex.        for 
-00022d10: 7365 785f 7661 6c20 696e 205b 2a63 6f6c  sex_val in [*col
-00022d20: 5f64 6963 745d 3a0a 2020 2020 2020 2020  _dict]:.        
-00022d30: 2020 2020 2367 6574 2061 2063 6f75 6e74      #get a count
-00022d40: 6572 0a20 2020 2020 2020 2020 2020 2063  er.            c
-00022d50: 6f75 6e74 7320 3d20 4328 5b69 6e64 2e61  ounts = C([ind.a
-00022d60: 6765 2066 6f72 2069 6e64 2069 6e20 7365  ge for ind in se
-00022d70: 6c66 2e76 616c 7565 7328 0a20 2020 2020  lf.values(.     
-00022d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022da0: 2020 2020 2020 2029 2069 6620 696e 642e         ) if ind.
-00022db0: 7365 7820 3d3d 2069 6e74 2873 6578 5f76  sex == int(sex_v
-00022dc0: 616c 203c 2030 295d 290a 2020 2020 2020  al < 0)]).      
-00022dd0: 2020 2020 2020 2367 7261 6220 7468 6520        #grab the 
-00022de0: 6167 6573 2066 726f 6d20 6974 0a20 2020  ages from it.   
-00022df0: 2020 2020 2020 2020 2061 6765 7320 3d20           ages = 
-00022e00: 5b2a 636f 756e 7473 5d0a 2020 2020 2020  [*counts].      
-00022e10: 2020 2020 2020 2361 6e64 2067 7261 6220        #and grab 
-00022e20: 7468 6520 636f 756e 7473 2066 726f 6d20  the counts from 
-00022e30: 6974 2028 6d75 6c74 6970 6c79 696e 6720  it (multiplying 
-00022e40: 6279 202d 3120 666f 7220 6665 6d61 6c65  by -1 for female
-00022e50: 732c 0a20 2020 2020 2020 2020 2020 2023  s,.            #
-00022e60: 746f 2073 6574 206f 6e65 2073 6578 206f  to set one sex o
-00022e70: 6e20 6569 7468 6572 2073 6964 6520 6f66  n either side of
-00022e80: 2078 3d30 2c20 666f 7220 7468 6520 7079   x=0, for the py
-00022e90: 7261 6d69 6429 0a20 2020 2020 2020 2020  ramid).         
-00022ea0: 2020 2063 6f75 6e74 7320 3d20 5b73 6578     counts = [sex
-00022eb0: 5f76 616c 2a63 6f75 6e74 2066 6f72 2063  _val*count for c
-00022ec0: 6f75 6e74 2069 6e20 636f 756e 7473 2e76  ount in counts.v
-00022ed0: 616c 7565 7328 295d 0a20 2020 2020 2020  alues()].       
-00022ee0: 2020 2020 2023 7570 6461 7465 2074 6865       #update the
-00022ef0: 206d 6178 5f63 6f75 6e74 2076 6172 0a20   max_count var. 
-00022f00: 2020 2020 2020 2020 2020 206d 6178 5f63             max_c
-00022f10: 6f75 6e74 203d 206d 6178 286d 6178 2863  ount = max(max(c
-00022f20: 6f75 6e74 7329 2c20 6d61 785f 636f 756e  ounts), max_coun
-00022f30: 7429 0a20 2020 2020 2020 2020 2020 2023  t).            #
-00022f40: 7468 656e 2063 7265 6174 6520 7468 6520  then create the 
-00022f50: 686f 7269 7a6f 6e74 616c 2062 6172 706c  horizontal barpl
-00022f60: 6f74 0a20 2020 2020 2020 2020 2020 2070  ot.            p
-00022f70: 6c74 2e62 6172 6828 6167 6573 2c20 636f  lt.barh(ages, co
-00022f80: 756e 7473 2c20 636f 6c6f 7220 3d20 636f  unts, color = co
-00022f90: 6c5f 6469 6374 5b73 6578 5f76 616c 5d29  l_dict[sex_val])
-00022fa0: 0a20 2020 2020 2020 2023 7573 6520 6d61  .        #use ma
-00022fb0: 785f 636f 756e 7420 746f 2073 6574 2074  x_count to set t
-00022fc0: 6865 2078 2d6c 696d 6974 7320 616e 6420  he x-limits and 
-00022fd0: 792d 6c69 6d69 7473 0a20 2020 2020 2020  y-limits.       
-00022fe0: 2070 6c74 2e78 6c69 6d28 282d 312a 6d61   plt.xlim((-1*ma
-00022ff0: 785f 636f 756e 742d 322c 206d 6178 5f63  x_count-2, max_c
-00023000: 6f75 6e74 2b32 2929 0a20 2020 2020 2020  ount+2)).       
-00023010: 2023 7365 7420 7468 6520 6178 6973 206c   #set the axis l
-00023020: 6162 656c 730a 2020 2020 2020 2020 706c  abels.        pl
-00023030: 742e 786c 6162 656c 2827 5370 6563 6965  t.xlabel('Specie
-00023040: 7320 2869 6e64 6976 6964 7561 6c73 2927  s (individuals)'
-00023050: 290a 2020 2020 2020 2020 706c 742e 796c  ).        plt.yl
-00023060: 6162 656c 2827 4167 6520 2874 696d 6573  abel('Age (times
-00023070: 7465 7073 2927 290a 2020 2020 2020 2020  teps)').        
-00023080: 2374 6865 6e20 7365 7420 7468 6520 786c  #then set the xl
-00023090: 6162 656c 7320 746f 2070 6f73 6974 6976  abels to positiv
-000230a0: 6520 6e75 6d62 6572 7320 6f6e 2065 6974  e numbers on eit
-000230b0: 6865 7220 7369 6465 0a20 2020 2020 2020  her side.       
-000230c0: 206c 6f63 732c 206c 6162 656c 7320 3d20   locs, labels = 
-000230d0: 706c 742e 7874 6963 6b73 2829 0a20 2020  plt.xticks().   
-000230e0: 2020 2020 2070 6c74 2e78 7469 636b 7328       plt.xticks(
-000230f0: 6c6f 6373 2c20 5b73 7472 2869 6e74 286c  locs, [str(int(l
-00023100: 6f63 2929 2066 6f72 206c 6f63 2069 6e20  oc)) for loc in 
-00023110: 6e70 2e61 6273 286c 6f63 7329 5d29 0a20  np.abs(locs)]). 
-00023120: 2020 2020 2020 2023 6164 6420 7365 7820         #add sex 
-00023130: 7379 6d62 6f6c 7320 6173 2074 6974 6c65  symbols as title
-00023140: 0a20 2020 2020 2020 2070 6c74 2e73 7570  .        plt.sup
-00023150: 7469 746c 6528 275c 7532 3634 3225 735c  title('\u2642%s\
-00023160: 7532 3634 3027 2025 2027 272e 6a6f 696e  u2640' % ''.join
-00023170: 285b 2720 2720 666f 7220 5f20 696e 2072  ([' ' for _ in r
-00023180: 616e 6765 2832 3029 5d29 2c0a 2020 2020  ange(20)]),.    
-00023190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231d0: 7369 7a65 203d 2033 3029 0a20 2020 2020  size = 30).     
-000231e0: 2020 2023 7368 6f77 2069 740a 2020 2020     #show it.    
-000231f0: 2020 2020 706c 742e 7368 6f77 2829 0a0a      plt.show()..
-00023200: 2020 2020 6465 6620 5f70 6c6f 745f 706f      def _plot_po
-00023210: 705f 6772 6f77 7468 2873 656c 662c 2065  p_growth(self, e
-00023220: 7870 6563 7465 643d 5472 7565 2c20 6163  xpected=True, ac
-00023230: 7475 616c 3d54 7275 652c 2065 7870 6563  tual=True, expec
-00023240: 7465 645f 636f 6c6f 723d 2772 6564 272c  ted_color='red',
-00023250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023260: 2020 2020 2020 2020 2061 6374 7561 6c5f           actual_
-00023270: 636f 6c6f 723d 2762 6c75 6527 293a 0a20  color='blue'):. 
-00023280: 2020 2020 2020 2054 203d 2072 616e 6765         T = range
-00023290: 286c 656e 2873 656c 662e 4e74 2929 0a20  (len(self.Nt)). 
-000232a0: 2020 2020 2020 2078 3020 3d20 7365 6c66         x0 = self
-000232b0: 2e4e 745b 305d 202f 2073 656c 662e 4b2e  .Nt[0] / self.K.
-000232c0: 7375 6d28 290a 2020 2020 2020 2020 6966  sum().        if
-000232d0: 2065 7870 6563 7465 643a 0a20 2020 2020   expected:.     
-000232e0: 2020 2020 2020 2070 6c74 2e70 6c6f 7428         plt.plot(
-000232f0: 542c 205b 5f63 616c 635f 6c6f 6769 7374  T, [_calc_logist
-00023300: 6963 5f73 6f6c 6e28 7830 2c20 7365 6c66  ic_soln(x0, self
-00023310: 2e52 2c0a 2020 2020 2020 2020 2020 2020  .R,.            
-00023320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023330: 2020 2020 7429 202a 2073 656c 662e 4b2e      t) * self.K.
-00023340: 7375 6d28 2920 666f 7220 7420 696e 2054  sum() for t in T
-00023350: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00023360: 2020 2020 2020 2020 636f 6c6f 723d 6578          color=ex
-00023370: 7065 6374 6564 5f63 6f6c 6f72 290a 2020  pected_color).  
-00023380: 2020 2020 2020 6966 2061 6374 7561 6c3a        if actual:
-00023390: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
-000233a0: 2e70 6c6f 7428 542c 2073 656c 662e 4e74  .plot(T, self.Nt
-000233b0: 2c20 636f 6c6f 723d 6163 7475 616c 5f63  , color=actual_c
-000233c0: 6f6c 6f72 290a 2020 2020 2020 2020 706c  olor).        pl
-000233d0: 742e 786c 6162 656c 2827 7427 290a 2020  t.xlabel('t').  
-000233e0: 2020 2020 2020 706c 742e 796c 6162 656c        plt.ylabel
-000233f0: 2827 4e28 7429 2729 0a0a 2020 2020 6465  ('N(t)')..    de
-00023400: 6620 5f70 6c6f 745f 6465 6d6f 6772 6170  f _plot_demograp
-00023410: 6869 635f 6368 616e 6765 7328 7365 6c66  hic_changes(self
-00023420: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00023430: 6c66 2e5f 6368 616e 6765 7220 6973 204e  lf._changer is N
-00023440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00023450: 2070 7269 6e74 2828 2253 7065 6369 6573   print(("Species
-00023460: 2e5f 706c 6f74 5f64 656d 6f67 7261 7068  ._plot_demograph
-00023470: 6963 5f63 6861 6e67 6573 2069 7320 6e6f  ic_changes is no
-00023480: 7420 7661 6c69 6420 220a 2020 2020 2020  t valid ".      
-00023490: 2020 2020 2020 2020 2020 2266 6f72 2073            "for s
-000234a0: 7065 6369 6573 2077 6974 6820 6e6f 205f  pecies with no _
-000234b0: 5370 6563 6965 7343 6861 6e67 6572 206f  SpeciesChanger o
-000234c0: 626a 6563 742e 5c6e 2229 290a 2020 2020  bject.\n")).    
-000234d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000234e0: 2020 2020 2020 7365 6c66 2e5f 6368 616e        self._chan
-000234f0: 6765 722e 5f70 6c6f 745f 6465 6d5f 6368  ger._plot_dem_ch
-00023500: 616e 6765 7328 7365 6c66 290a 0a0a 2020  anges(self)...  
-00023510: 2020 6465 6620 5f70 6c6f 745f 6578 616d    def _plot_exam
-00023520: 706c 655f 7265 636f 6d62 696e 616e 745f  ple_recombinant_
-00023530: 6765 6e6f 6d65 2873 656c 6629 3a0a 2020  genome(self):.  
-00023540: 2020 2020 2020 7072 696e 7428 2754 4f44        print('TOD
-00023550: 4f3a 2046 4958 204d 4521 2729 0a20 2020  O: FIX ME!').   
-00023560: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00023570: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00023580: 6765 6e5f 6172 6368 2069 7320 6e6f 7420  gen_arch is not 
-00023590: 4e6f 6e65 2c20 2822 5468 6973 2073 7065  None, ("This spe
-000235a0: 6369 6573 2064 6f65 7320 6e6f 7420 6861  cies does not ha
-000235b0: 7665 2022 0a20 2020 2020 2020 2020 2020  ve ".           
-000235c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235e0: 2022 6765 6e6f 6d65 732c 2073 6f20 6974   "genomes, so it
-000235f0: 2063 616e 6e6f 7420 6265 2075 7365 6420   cannot be used 
-00023600: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00023610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023620: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00023630: 6f20 706c 6f74 2061 6e20 6578 616d 706c  o plot an exampl
-00023640: 6520 7265 636f 6d62 696e 616e 7420 220a  e recombinant ".
+000226d0: 2020 5b6e 6f64 655f 6269 7274 685f 6c6f    [node_birth_lo
+000226e0: 635b 315d 2c20 6e6f 6465 5f63 7572 725f  c[1], node_curr_
+000226f0: 6c6f 635b 315d 5d2c 0a20 2020 2020 2020  loc[1]],.       
+00022700: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00022710: 6c6f 723d 7374 6172 745f 636f 6c2c 206c  lor=start_col, l
+00022720: 696e 6573 7479 6c65 3d27 3a27 2c20 616c  inestyle=':', al
+00022730: 7068 613d 616c 7068 612c 0a20 2020 2020  pha=alpha,.     
+00022740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022750: 6c69 6e65 7769 6474 683d 312e 3229 0a0a  linewidth=1.2)..
+00022760: 2020 2020 2020 2020 6966 2061 6464 5f72          if add_r
+00022770: 6f6f 7473 3a0a 2020 2020 2020 2020 2020  oots:.          
+00022780: 2020 7365 6c66 2e5f 706c 6f74 5f6c 696e    self._plot_lin
+00022790: 6561 6765 5f72 6f6f 7473 2874 632c 2074  eage_roots(tc, t
+000227a0: 7265 6529 0a0a 0a20 2020 2023 2070 6c6f  ree)...    # plo
+000227b0: 7420 7468 6520 6c69 6e65 6167 6520 666f  t the lineage fo
+000227c0: 7220 6120 6769 7665 6e20 6e6f 6465 2061  r a given node a
+000227d0: 6e64 206c 6f63 7573 0a20 2020 2064 6566  nd locus.    def
+000227e0: 205f 706c 6f74 5f6c 696e 6561 6765 5f72   _plot_lineage_r
+000227f0: 6f6f 7473 2873 656c 662c 2074 632c 2074  oots(self, tc, t
+00022800: 7265 652c 2061 6c70 6861 3d30 2e38 2c20  ree, alpha=0.8, 
+00022810: 7369 7a65 3d37 3529 3a0a 2020 2020 2020  size=75):.      
+00022820: 2020 6966 206e 6f74 2073 656c 662e 6765    if not self.ge
+00022830: 6e5f 6172 6368 2e75 7365 5f74 736b 6974  n_arch.use_tskit
+00022840: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00022850: 6973 6520 4578 6365 7074 696f 6e28 2822  ise Exception(("
+00022860: 4c69 6e65 6167 6520 726f 6f74 7320 6361  Lineage roots ca
+00022870: 6e6e 6f74 2062 6520 706c 6f74 7465 6420  nnot be plotted 
+00022880: 666f 7220 6120 5370 6563 6965 7320 220a  for a Species ".
+00022890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228a0: 2020 2020 2020 2020 2020 2020 2022 7768               "wh
+000228b0: 6f73 6520 7370 6174 6961 6c20 7065 6469  ose spatial pedi
+000228c0: 6772 6565 2069 7320 6e6f 7420 6265 696e  gree is not bein
+000228d0: 6720 7472 6163 6b65 6420 220a 2020 2020  g tracked ".    
+000228e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228f0: 2020 2020 2020 2020 2022 6279 2074 736b           "by tsk
+00022900: 6974 2e22 2929 0a0a 2020 2020 2020 2020  it."))..        
+00022910: 2320 6765 7420 7468 6520 6e6f 6465 730a  # get the nodes.
+00022920: 2020 2020 2020 2020 616c 6c5f 6e6f 6465          all_node
+00022930: 7320 3d20 7365 6c66 2e5f 6765 745f 6e6f  s = self._get_no
+00022940: 6465 7328 290a 0a20 2020 2020 2020 2023  des()..        #
+00022950: 2067 6574 2074 6865 206c 696e 6561 6765   get the lineage
+00022960: 2064 6963 7420 666f 7220 616c 6c20 6e6f   dict for all no
+00022970: 6465 730a 2020 2020 2020 2020 6c69 6e5f  des.        lin_
+00022980: 6469 6374 203d 205f 6765 745f 6c69 6e65  dict = _get_line
+00022990: 6167 655f 6469 6374 735f 6f6e 655f 7472  age_dicts_one_tr
+000229a0: 6565 2874 632c 2074 7265 652c 2061 6c6c  ee(tc, tree, all
+000229b0: 5f6e 6f64 6573 2c20 7365 6c66 2e74 290a  _nodes, self.t).
+000229c0: 0a20 2020 2020 2020 2023 2067 6574 2074  .        # get t
+000229d0: 6865 2072 6f6f 7473 2066 6f72 2061 6c6c  he roots for all
+000229e0: 2064 6973 7469 6e63 7420 6c69 6e65 6167   distinct lineag
+000229f0: 6573 2061 7420 7468 6973 206c 6f63 7573  es at this locus
+00022a00: 0a20 2020 2020 2020 2072 6f6f 745f 6e6f  .        root_no
+00022a10: 6465 7320 3d20 6e70 2e75 6e69 7175 6528  des = np.unique(
+00022a20: 5b5b 2a6c 696e 5f64 6963 745b 6e5d 2e6b  [[*lin_dict[n].k
+00022a30: 6579 7328 295d 5b2d 315d 2066 6f72 206e  eys()][-1] for n
+00022a40: 2069 6e20 616c 6c5f 6e6f 6465 735d 290a   in all_nodes]).
+00022a50: 0a20 2020 2020 2020 2023 2067 6574 2062  .        # get b
+00022a60: 6972 7468 206c 6f63 6174 696f 6e73 2066  irth locations f
+00022a70: 6f72 2065 6163 6820 726f 6f74 206e 6f64  or each root nod
+00022a80: 650a 2020 2020 2020 2020 726f 6f74 5f69  e.        root_i
+00022a90: 6e64 6976 6964 7320 3d20 5b74 632e 6e6f  ndivids = [tc.no
+00022aa0: 6465 735b 6e5d 2e69 6e64 6976 6964 7561  des[n].individua
+00022ab0: 6c20 666f 7220 6e20 696e 2072 6f6f 745f  l for n in root_
+00022ac0: 6e6f 6465 735d 0a20 2020 2020 2020 2072  nodes].        r
+00022ad0: 6f6f 745f 6c6f 6373 203d 205b 7463 2e69  oot_locs = [tc.i
+00022ae0: 6e64 6976 6964 7561 6c73 5b69 5d2e 6c6f  ndividuals[i].lo
+00022af0: 6361 7469 6f6e 2066 6f72 2069 2069 6e20  cation for i in 
+00022b00: 726f 6f74 5f69 6e64 6976 6964 735d 0a0a  root_individs]..
+00022b10: 2020 2020 2020 2020 2320 6578 7472 6163          # extrac
+00022b20: 7420 616e 6420 706c 6f74 2074 6865 2073  t and plot the s
+00022b30: 6572 6965 7320 6f66 2070 6f69 6e74 7320  eries of points 
+00022b40: 666f 7220 6561 6368 206e 6f64 650a 2020  for each node.  
+00022b50: 2020 2020 2020 666f 7220 782c 2079 2069        for x, y i
+00022b60: 6e20 726f 6f74 5f6c 6f63 733a 0a20 2020  n root_locs:.   
+00022b70: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
+00022b80: 7468 6520 726f 6f74 206e 6f64 6573 2720  the root nodes' 
+00022b90: 6269 7274 6820 6c6f 6361 7469 6f6e 730a  birth locations.
+00022ba0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+00022bb0: 7363 6174 7465 7228 782c 2079 2c20 633d  scatter(x, y, c=
+00022bc0: 2777 6869 7465 272c 2073 3d73 697a 652c  'white', s=size,
+00022bd0: 2061 6c70 6861 3d61 6c70 6861 2c20 6d61   alpha=alpha, ma
+00022be0: 726b 6572 3d27 7327 290a 2020 2020 2020  rker='s').      
+00022bf0: 2020 706c 742e 7368 6f77 2829 0a0a 0a20    plt.show()... 
+00022c00: 2020 2023 206d 6574 686f 6420 666f 7220     # method for 
+00022c10: 706c 6f74 7469 6e67 2061 2073 7065 6369  plotting a speci
+00022c20: 6573 2720 706f 7075 6c61 7469 6f6e 2070  es' population p
+00022c30: 7972 616d 6964 0a20 2020 2064 6566 205f  yramid.    def _
+00022c40: 706c 6f74 5f64 656d 6f67 7261 7068 6963  plot_demographic
+00022c50: 5f70 7972 616d 6964 2873 656c 6629 3a0a  _pyramid(self):.
+00022c60: 2020 2020 2020 2020 236d 616b 6520 6469          #make di
+00022c70: 6374 206f 6620 6665 6d61 6c65 2061 6e64  ct of female and
+00022c80: 206d 616c 6520 636f 6c6f 7273 0a20 2020   male colors.   
+00022c90: 2020 2020 2063 6f6c 5f64 6963 7420 3d20       col_dict = 
+00022ca0: 7b2d 313a 2027 6379 616e 272c 2031 3a20  {-1: 'cyan', 1: 
+00022cb0: 2770 696e 6b27 7d0a 2020 2020 2020 2020  'pink'}.        
+00022cc0: 2363 7265 6174 6520 6120 6669 6775 7265  #create a figure
+00022cd0: 0a20 2020 2020 2020 2066 6967 203d 2070  .        fig = p
+00022ce0: 6c74 2e66 6967 7572 6528 290a 2020 2020  lt.figure().    
+00022cf0: 2020 2020 2376 6172 6961 626c 6573 2074      #variables t
+00022d00: 6f20 6772 6162 2074 6865 206d 6178 2063  o grab the max c
+00022d10: 6f75 6e74 0a20 2020 2020 2020 206d 6178  ount.        max
+00022d20: 5f63 6f75 6e74 203d 2030 0a20 2020 2020  _count = 0.     
+00022d30: 2020 2023 666f 7220 6561 6368 2073 6578     #for each sex
+00022d40: 0a20 2020 2020 2020 2066 6f72 2073 6578  .        for sex
+00022d50: 5f76 616c 2069 6e20 5b2a 636f 6c5f 6469  _val in [*col_di
+00022d60: 6374 5d3a 0a20 2020 2020 2020 2020 2020  ct]:.           
+00022d70: 2023 6765 7420 6120 636f 756e 7465 720a   #get a counter.
+00022d80: 2020 2020 2020 2020 2020 2020 636f 756e              coun
+00022d90: 7473 203d 2043 285b 696e 642e 6167 6520  ts = C([ind.age 
+00022da0: 666f 7220 696e 6420 696e 2073 656c 662e  for ind in self.
+00022db0: 7661 6c75 6573 280a 2020 2020 2020 2020  values(.        
+00022dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022de0: 2020 2020 2920 6966 2069 6e64 2e73 6578      ) if ind.sex
+00022df0: 203d 3d20 696e 7428 7365 785f 7661 6c20   == int(sex_val 
+00022e00: 3c20 3029 5d29 0a20 2020 2020 2020 2020  < 0)]).         
+00022e10: 2020 2023 6772 6162 2074 6865 2061 6765     #grab the age
+00022e20: 7320 6672 6f6d 2069 740a 2020 2020 2020  s from it.      
+00022e30: 2020 2020 2020 6167 6573 203d 205b 2a63        ages = [*c
+00022e40: 6f75 6e74 735d 0a20 2020 2020 2020 2020  ounts].         
+00022e50: 2020 2023 616e 6420 6772 6162 2074 6865     #and grab the
+00022e60: 2063 6f75 6e74 7320 6672 6f6d 2069 7420   counts from it 
+00022e70: 286d 756c 7469 706c 7969 6e67 2062 7920  (multiplying by 
+00022e80: 2d31 2066 6f72 2066 656d 616c 6573 2c0a  -1 for females,.
+00022e90: 2020 2020 2020 2020 2020 2020 2374 6f20              #to 
+00022ea0: 7365 7420 6f6e 6520 7365 7820 6f6e 2065  set one sex on e
+00022eb0: 6974 6865 7220 7369 6465 206f 6620 783d  ither side of x=
+00022ec0: 302c 2066 6f72 2074 6865 2070 7972 616d  0, for the pyram
+00022ed0: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
+00022ee0: 636f 756e 7473 203d 205b 7365 785f 7661  counts = [sex_va
+00022ef0: 6c2a 636f 756e 7420 666f 7220 636f 756e  l*count for coun
+00022f00: 7420 696e 2063 6f75 6e74 732e 7661 6c75  t in counts.valu
+00022f10: 6573 2829 5d0a 2020 2020 2020 2020 2020  es()].          
+00022f20: 2020 2375 7064 6174 6520 7468 6520 6d61    #update the ma
+00022f30: 785f 636f 756e 7420 7661 720a 2020 2020  x_count var.    
+00022f40: 2020 2020 2020 2020 6d61 785f 636f 756e          max_coun
+00022f50: 7420 3d20 6d61 7828 6d61 7828 636f 756e  t = max(max(coun
+00022f60: 7473 292c 206d 6178 5f63 6f75 6e74 290a  ts), max_count).
+00022f70: 2020 2020 2020 2020 2020 2020 2374 6865              #the
+00022f80: 6e20 6372 6561 7465 2074 6865 2068 6f72  n create the hor
+00022f90: 697a 6f6e 7461 6c20 6261 7270 6c6f 740a  izontal barplot.
+00022fa0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+00022fb0: 6261 7268 2861 6765 732c 2063 6f75 6e74  barh(ages, count
+00022fc0: 732c 2063 6f6c 6f72 203d 2063 6f6c 5f64  s, color = col_d
+00022fd0: 6963 745b 7365 785f 7661 6c5d 290a 2020  ict[sex_val]).  
+00022fe0: 2020 2020 2020 2375 7365 206d 6178 5f63        #use max_c
+00022ff0: 6f75 6e74 2074 6f20 7365 7420 7468 6520  ount to set the 
+00023000: 782d 6c69 6d69 7473 2061 6e64 2079 2d6c  x-limits and y-l
+00023010: 696d 6974 730a 2020 2020 2020 2020 706c  imits.        pl
+00023020: 742e 786c 696d 2828 2d31 2a6d 6178 5f63  t.xlim((-1*max_c
+00023030: 6f75 6e74 2d32 2c20 6d61 785f 636f 756e  ount-2, max_coun
+00023040: 742b 3229 290a 2020 2020 2020 2020 2373  t+2)).        #s
+00023050: 6574 2074 6865 2061 7869 7320 6c61 6265  et the axis labe
+00023060: 6c73 0a20 2020 2020 2020 2070 6c74 2e78  ls.        plt.x
+00023070: 6c61 6265 6c28 2753 7065 6369 6573 2028  label('Species (
+00023080: 696e 6469 7669 6475 616c 7329 2729 0a20  individuals)'). 
+00023090: 2020 2020 2020 2070 6c74 2e79 6c61 6265         plt.ylabe
+000230a0: 6c28 2741 6765 2028 7469 6d65 7374 6570  l('Age (timestep
+000230b0: 7329 2729 0a20 2020 2020 2020 2023 7468  s)').        #th
+000230c0: 656e 2073 6574 2074 6865 2078 6c61 6265  en set the xlabe
+000230d0: 6c73 2074 6f20 706f 7369 7469 7665 206e  ls to positive n
+000230e0: 756d 6265 7273 206f 6e20 6569 7468 6572  umbers on either
+000230f0: 2073 6964 650a 2020 2020 2020 2020 6c6f   side.        lo
+00023100: 6373 2c20 6c61 6265 6c73 203d 2070 6c74  cs, labels = plt
+00023110: 2e78 7469 636b 7328 290a 2020 2020 2020  .xticks().      
+00023120: 2020 706c 742e 7874 6963 6b73 286c 6f63    plt.xticks(loc
+00023130: 732c 205b 7374 7228 696e 7428 6c6f 6329  s, [str(int(loc)
+00023140: 2920 666f 7220 6c6f 6320 696e 206e 702e  ) for loc in np.
+00023150: 6162 7328 6c6f 6373 295d 290a 2020 2020  abs(locs)]).    
+00023160: 2020 2020 2361 6464 2073 6578 2073 796d      #add sex sym
+00023170: 626f 6c73 2061 7320 7469 746c 650a 2020  bols as title.  
+00023180: 2020 2020 2020 706c 742e 7375 7074 6974        plt.suptit
+00023190: 6c65 2827 5c75 3236 3432 2573 5c75 3236  le('\u2642%s\u26
+000231a0: 3430 2720 2520 2727 2e6a 6f69 6e28 5b27  40' % ''.join(['
+000231b0: 2027 2066 6f72 205f 2069 6e20 7261 6e67   ' for _ in rang
+000231c0: 6528 3230 295d 292c 0a20 2020 2020 2020  e(20)]),.       
+000231d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000231e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000231f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023200: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+00023210: 6520 3d20 3330 290a 2020 2020 2020 2020  e = 30).        
+00023220: 2373 686f 7720 6974 0a20 2020 2020 2020  #show it.       
+00023230: 2070 6c74 2e73 686f 7728 290a 0a20 2020   plt.show()..   
+00023240: 2064 6566 205f 706c 6f74 5f70 6f70 5f67   def _plot_pop_g
+00023250: 726f 7774 6828 7365 6c66 2c20 6578 7065  rowth(self, expe
+00023260: 6374 6564 3d54 7275 652c 2061 6374 7561  cted=True, actua
+00023270: 6c3d 5472 7565 2c20 6578 7065 6374 6564  l=True, expected
+00023280: 5f63 6f6c 6f72 3d27 7265 6427 2c0a 2020  _color='red',.  
+00023290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000232a0: 2020 2020 2020 6163 7475 616c 5f63 6f6c        actual_col
+000232b0: 6f72 3d27 626c 7565 2729 3a0a 2020 2020  or='blue'):.    
+000232c0: 2020 2020 5420 3d20 7261 6e67 6528 6c65      T = range(le
+000232d0: 6e28 7365 6c66 2e4e 7429 290a 2020 2020  n(self.Nt)).    
+000232e0: 2020 2020 7830 203d 2073 656c 662e 4e74      x0 = self.Nt
+000232f0: 5b30 5d20 2f20 7365 6c66 2e4b 2e73 756d  [0] / self.K.sum
+00023300: 2829 0a20 2020 2020 2020 2069 6620 6578  ().        if ex
+00023310: 7065 6374 6564 3a0a 2020 2020 2020 2020  pected:.        
+00023320: 2020 2020 706c 742e 706c 6f74 2854 2c20      plt.plot(T, 
+00023330: 5b5f 6361 6c63 5f6c 6f67 6973 7469 635f  [_calc_logistic_
+00023340: 736f 6c6e 2878 302c 2073 656c 662e 522c  soln(x0, self.R,
+00023350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023370: 2074 2920 2a20 7365 6c66 2e4b 2e73 756d   t) * self.K.sum
+00023380: 2829 2066 6f72 2074 2069 6e20 545d 2c0a  () for t in T],.
+00023390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233a0: 2020 2020 2063 6f6c 6f72 3d65 7870 6563       color=expec
+000233b0: 7465 645f 636f 6c6f 7229 0a20 2020 2020  ted_color).     
+000233c0: 2020 2069 6620 6163 7475 616c 3a0a 2020     if actual:.  
+000233d0: 2020 2020 2020 2020 2020 706c 742e 706c            plt.pl
+000233e0: 6f74 2854 2c20 7365 6c66 2e4e 742c 2063  ot(T, self.Nt, c
+000233f0: 6f6c 6f72 3d61 6374 7561 6c5f 636f 6c6f  olor=actual_colo
+00023400: 7229 0a20 2020 2020 2020 2070 6c74 2e78  r).        plt.x
+00023410: 6c61 6265 6c28 2774 2729 0a20 2020 2020  label('t').     
+00023420: 2020 2070 6c74 2e79 6c61 6265 6c28 274e     plt.ylabel('N
+00023430: 2874 2927 290a 0a20 2020 2064 6566 205f  (t)')..    def _
+00023440: 706c 6f74 5f64 656d 6f67 7261 7068 6963  plot_demographic
+00023450: 5f63 6861 6e67 6573 2873 656c 6629 3a0a  _changes(self):.
+00023460: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00023470: 5f63 6861 6e67 6572 2069 7320 4e6f 6e65  _changer is None
+00023480: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00023490: 696e 7428 2822 5370 6563 6965 732e 5f70  int(("Species._p
+000234a0: 6c6f 745f 6465 6d6f 6772 6170 6869 635f  lot_demographic_
+000234b0: 6368 616e 6765 7320 6973 206e 6f74 2076  changes is not v
+000234c0: 616c 6964 2022 0a20 2020 2020 2020 2020  alid ".         
+000234d0: 2020 2020 2020 2022 666f 7220 7370 6563         "for spec
+000234e0: 6965 7320 7769 7468 206e 6f20 5f53 7065  ies with no _Spe
+000234f0: 6369 6573 4368 616e 6765 7220 6f62 6a65  ciesChanger obje
+00023500: 6374 2e5c 6e22 2929 0a20 2020 2020 2020  ct.\n")).       
+00023510: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00023520: 2020 2073 656c 662e 5f63 6861 6e67 6572     self._changer
+00023530: 2e5f 706c 6f74 5f64 656d 5f63 6861 6e67  ._plot_dem_chang
+00023540: 6573 2873 656c 6629 0a0a 0a20 2020 2064  es(self)...    d
+00023550: 6566 205f 706c 6f74 5f65 7861 6d70 6c65  ef _plot_example
+00023560: 5f72 6563 6f6d 6269 6e61 6e74 5f67 656e  _recombinant_gen
+00023570: 6f6d 6528 7365 6c66 293a 0a20 2020 2020  ome(self):.     
+00023580: 2020 2070 7269 6e74 2827 544f 444f 3a20     print('TODO: 
+00023590: 4649 5820 4d45 2127 290a 2020 2020 2020  FIX ME!').      
+000235a0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+000235b0: 2061 7373 6572 7420 7365 6c66 2e67 656e   assert self.gen
+000235c0: 5f61 7263 6820 6973 206e 6f74 204e 6f6e  _arch is not Non
+000235d0: 652c 2028 2254 6869 7320 7370 6563 6965  e, ("This specie
+000235e0: 7320 646f 6573 206e 6f74 2068 6176 6520  s does not have 
+000235f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00023600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023610: 2020 2020 2020 2020 2020 2020 2020 2267                "g
+00023620: 656e 6f6d 6573 2c20 736f 2069 7420 6361  enomes, so it ca
+00023630: 6e6e 6f74 2062 6520 7573 6564 2022 0a20  nnot be used ". 
+00023640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023670: 2020 2020 2020 2020 2020 2020 2267 656e              "gen
-00023680: 6f6d 652e 2229 0a0a 2020 2020 2020 2020  ome.")..        
-00023690: 7265 636f 6d62 5f70 6174 6873 203d 2073  recomb_paths = s
-000236a0: 656c 662e 6765 6e5f 6172 6368 2e5f 7265  elf.gen_arch._re
-000236b0: 636f 6d62 5f70 6174 6873 2e5f 6765 745f  comb_paths._get_
-000236c0: 7061 7468 7328 3229 0a20 2020 2020 2020  paths(2).       
-000236d0: 2069 6478 7320 3d20 2830 2c20 3229 0a20   idxs = (0, 2). 
-000236e0: 2020 2020 2020 206d 6f63 6b5f 7370 7020         mock_spp 
-000236f0: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
-00023700: 2069 6478 2069 6e20 6964 7873 3a0a 2020   idx in idxs:.  
-00023710: 2020 2020 2020 2020 2020 6e65 775f 6765            new_ge
-00023720: 6e6f 6d65 203d 206e 702e 6873 7461 636b  nome = np.hstack
-00023730: 285b 286e 702e 6f6e 6573 2828 7365 6c66  ([(np.ones((self
-00023740: 2e67 656e 5f61 7263 682e 4c2c 0a20 2020  .gen_arch.L,.   
-00023750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023770: 2020 2020 2020 2020 2020 2031 2929 202a             1)) *
-00023780: 206e 2029 202b 2069 6478 2066 6f72 206e   n ) + idx for n
-00023790: 2069 6e20 2831 2c32 295d 290a 2020 2020   in (1,2)]).    
-000237a0: 2020 2020 2020 2020 6d6f 636b 5f73 7070          mock_spp
-000237b0: 5b69 6478 5d20 3d20 496e 6469 7669 6475  [idx] = Individu
-000237c0: 616c 2869 6478 3d69 6478 2c20 783d 302c  al(idx=idx, x=0,
-000237d0: 2079 3d30 2c0a 2020 2020 2020 2020 2020   y=0,.          
-000237e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237f0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-00023800: 5f67 656e 6f6d 653d 6e65 775f 6765 6e6f  _genome=new_geno
-00023810: 6d65 290a 0a20 2020 2020 2020 2072 6563  me)..        rec
-00023820: 6f6d 625f 6765 6e6f 6d65 203d 205f 646f  omb_genome = _do
-00023830: 5f6d 6174 696e 6728 7370 703d 6d6f 636b  _mating(spp=mock
-00023840: 5f73 7070 2c0a 2020 2020 2020 2020 2020  _spp,.          
-00023850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023860: 2020 2020 2020 2020 206d 6174 696e 675f           mating_
-00023870: 7061 6972 733d 5b69 6478 735d 2c0a 2020  pairs=[idxs],.  
-00023880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023660: 2020 2020 2020 2020 2020 2022 746f 2070             "to p
+00023670: 6c6f 7420 616e 2065 7861 6d70 6c65 2072  lot an example r
+00023680: 6563 6f6d 6269 6e61 6e74 2022 0a20 2020  ecombinant ".   
+00023690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000236a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000236b0: 2020 2020 2020 2020 2022 6765 6e6f 6d65           "genome
+000236c0: 2e22 290a 0a20 2020 2020 2020 2072 6563  .")..        rec
+000236d0: 6f6d 625f 7061 7468 7320 3d20 7365 6c66  omb_paths = self
+000236e0: 2e67 656e 5f61 7263 682e 5f72 6563 6f6d  .gen_arch._recom
+000236f0: 625f 7061 7468 732e 5f67 6574 5f70 6174  b_paths._get_pat
+00023700: 6873 2832 290a 2020 2020 2020 2020 6964  hs(2).        id
+00023710: 7873 203d 2028 302c 2032 290a 2020 2020  xs = (0, 2).    
+00023720: 2020 2020 6d6f 636b 5f73 7070 203d 207b      mock_spp = {
+00023730: 7d0a 2020 2020 2020 2020 666f 7220 6964  }.        for id
+00023740: 7820 696e 2069 6478 733a 0a20 2020 2020  x in idxs:.     
+00023750: 2020 2020 2020 206e 6577 5f67 656e 6f6d         new_genom
+00023760: 6520 3d20 6e70 2e68 7374 6163 6b28 5b28  e = np.hstack([(
+00023770: 6e70 2e6f 6e65 7328 2873 656c 662e 6765  np.ones((self.ge
+00023780: 6e5f 6172 6368 2e4c 2c0a 2020 2020 2020  n_arch.L,.      
+00023790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237b0: 2020 2020 2020 2020 3129 2920 2a20 6e20          1)) * n 
+000237c0: 2920 2b20 6964 7820 666f 7220 6e20 696e  ) + idx for n in
+000237d0: 2028 312c 3229 5d29 0a20 2020 2020 2020   (1,2)]).       
+000237e0: 2020 2020 206d 6f63 6b5f 7370 705b 6964       mock_spp[id
+000237f0: 785d 203d 2049 6e64 6976 6964 7561 6c28  x] = Individual(
+00023800: 6964 783d 6964 782c 2078 3d30 2c20 793d  idx=idx, x=0, y=
+00023810: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00023820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023830: 2020 2020 2020 2020 2020 6e65 775f 6765            new_ge
+00023840: 6e6f 6d65 3d6e 6577 5f67 656e 6f6d 6529  nome=new_genome)
+00023850: 0a0a 2020 2020 2020 2020 7265 636f 6d62  ..        recomb
+00023860: 5f67 656e 6f6d 6520 3d20 5f64 6f5f 6d61  _genome = _do_ma
+00023870: 7469 6e67 2873 7070 3d6d 6f63 6b5f 7370  ting(spp=mock_sp
+00023880: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
 00023890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238a0: 206e 5f6f 6666 7370 7269 6e67 3d5b 315d   n_offspring=[1]
-000238b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000238a0: 2020 2020 2020 6d61 7469 6e67 5f70 6169        mating_pai
+000238b0: 7273 3d5b 6964 7873 5d2c 0a20 2020 2020  rs=[idxs],.     
 000238c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238d0: 2020 2020 2072 6563 6f6d 625f 7061 7468       recomb_path
-000238e0: 733d 7265 636f 6d62 5f70 6174 6873 295b  s=recomb_paths)[
-000238f0: 305d 5b30 5d0a 2020 2020 2020 2020 2372  0][0].        #r
-00023900: 6563 6f6d 625f 6765 6e6f 6d65 203d 2072  ecomb_genome = r
-00023910: 6563 6f6d 625f 6765 6e6f 6d65 2b31 0a20  ecomb_genome+1. 
-00023920: 2020 2020 2020 2023 7265 636f 6d62 5f67         #recomb_g
-00023930: 656e 6f6d 655b 3a2c 315d 203d 2072 6563  enome[:,1] = rec
-00023940: 6f6d 625f 6765 6e6f 6d65 5b3a 2c31 5d20  omb_genome[:,1] 
-00023950: 2a20 350a 2020 2020 2020 2020 6669 6720  * 5.        fig 
-00023960: 3d20 706c 742e 6669 6775 7265 2829 0a20  = plt.figure(). 
-00023970: 2020 2020 2020 2061 7820 3d20 6669 672e         ax = fig.
-00023980: 6164 645f 7375 6270 6c6f 7428 3131 3129  add_subplot(111)
-00023990: 0a20 2020 2020 2020 2061 782e 696d 7368  .        ax.imsh
-000239a0: 6f77 286e 702e 7265 7065 6174 2872 6563  ow(np.repeat(rec
-000239b0: 6f6d 625f 6765 6e6f 6d65 2c0a 2020 2020  omb_genome,.    
-000239c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000239d0: 2020 2020 2020 2020 696e 7428 302e 3035          int(0.05
-000239e0: 202a 2073 656c 662e 6765 6e5f 6172 6368   * self.gen_arch
-000239f0: 2e4c 292c 0a20 2020 2020 2020 2020 2020  .L),.           
+000238d0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+000238e0: 6f66 6673 7072 696e 673d 5b31 5d2c 0a20  offspring=[1],. 
+000238f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023910: 2020 7265 636f 6d62 5f70 6174 6873 3d72    recomb_paths=r
+00023920: 6563 6f6d 625f 7061 7468 7329 5b30 5d5b  ecomb_paths)[0][
+00023930: 305d 0a20 2020 2020 2020 2023 7265 636f  0].        #reco
+00023940: 6d62 5f67 656e 6f6d 6520 3d20 7265 636f  mb_genome = reco
+00023950: 6d62 5f67 656e 6f6d 652b 310a 2020 2020  mb_genome+1.    
+00023960: 2020 2020 2372 6563 6f6d 625f 6765 6e6f      #recomb_geno
+00023970: 6d65 5b3a 2c31 5d20 3d20 7265 636f 6d62  me[:,1] = recomb
+00023980: 5f67 656e 6f6d 655b 3a2c 315d 202a 2035  _genome[:,1] * 5
+00023990: 0a20 2020 2020 2020 2066 6967 203d 2070  .        fig = p
+000239a0: 6c74 2e66 6967 7572 6528 290a 2020 2020  lt.figure().    
+000239b0: 2020 2020 6178 203d 2066 6967 2e61 6464      ax = fig.add
+000239c0: 5f73 7562 706c 6f74 2831 3131 290a 2020  _subplot(111).  
+000239d0: 2020 2020 2020 6178 2e69 6d73 686f 7728        ax.imshow(
+000239e0: 6e70 2e72 6570 6561 7428 7265 636f 6d62  np.repeat(recomb
+000239f0: 5f67 656e 6f6d 652c 0a20 2020 2020 2020  _genome,.       
 00023a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023a10: 2061 7869 733d 3129 2c0a 2020 2020 2020   axis=1),.      
-00023a20: 2020 2020 2020 2020 2020 2020 636d 6170              cmap
-00023a30: 3d27 7465 7272 6169 6e27 290a 2020 2020  ='terrain').    
-00023a40: 2020 2020 6178 2e73 6574 5f74 6974 6c65      ax.set_title
-00023a50: 2822 6761 6d65 7465 2030 2020 2020 2067  ("gamete 0     g
-00023a60: 616d 6574 6531 2229 0a20 2020 2020 2020  amete1").       
-00023a70: 2061 782e 7365 745f 7874 6963 6b73 285b   ax.set_xticks([
-00023a80: 5d29 0a20 2020 2020 2020 2061 782e 7365  ]).        ax.se
-00023a90: 745f 796c 6162 656c 2827 6c6f 6375 7327  t_ylabel('locus'
-00023aa0: 290a 2020 2020 2020 2020 706c 742e 7368  ).        plt.sh
-00023ab0: 6f77 2829 0a20 2020 2020 2020 2072 6574  ow().        ret
-00023ac0: 7572 6e28 7265 636f 6d62 5f70 6174 6873  urn(recomb_paths
-00023ad0: 2c20 6d6f 636b 5f73 7070 2c20 7265 636f  , mock_spp, reco
-00023ae0: 6d62 5f67 656e 6f6d 6529 0a0a 0a20 2020  mb_genome)...   
-00023af0: 2064 6566 205f 706c 6f74 5f73 7461 7428   def _plot_stat(
-00023b00: 7365 6c66 2c20 7374 6174 293a 0a20 2020  self, stat):.   
-00023b10: 2020 2020 2069 6620 7365 6c66 2e5f 7374       if self._st
-00023b20: 6174 735f 636f 6c6c 6563 746f 7220 6973  ats_collector is
-00023b30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00023b40: 2020 2070 7269 6e74 2828 2253 7065 6369     print(("Speci
-00023b50: 6573 2e5f 706c 6f74 5f73 7461 7420 6973  es._plot_stat is
-00023b60: 206e 6f74 2076 616c 6964 2022 0a20 2020   not valid ".   
-00023b70: 2020 2020 2020 2020 2020 2020 2022 666f               "fo
-00023b80: 7220 7370 6563 6965 7320 7769 7468 206e  r species with n
-00023b90: 6f20 5f53 7461 7473 436f 6c6c 6563 746f  o _StatsCollecto
-00023ba0: 7220 6f62 6a65 6374 2e5c 6e22 2929 0a0a  r object.\n"))..
-00023bb0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00023bc0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00023bd0: 7374 6174 735f 636f 6c6c 6563 746f 722e  stats_collector.
-00023be0: 5f70 6c6f 745f 7374 6174 2873 7461 742c  _plot_stat(stat,
-00023bf0: 2073 7070 5f6e 616d 6520 3d20 7365 6c66   spp_name = self
-00023c00: 2e6e 616d 6529 0a0a 0a20 2020 2020 2020  .name)...       
-00023c10: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00023c20: 230a 2020 2020 2020 2020 2370 7562 6c69  #.        #publi
-00023c30: 6320 6d65 7468 6f64 7323 0a20 2020 2020  c methods#.     
-00023c40: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-00023c50: 2323 230a 0a20 2020 2064 6566 205f 7772  ###..    def _wr
-00023c60: 6974 655f 7069 636b 6c65 2873 656c 662c  ite_pickle(self,
-00023c70: 2066 696c 656e 616d 6529 3a0a 2020 2020   filename):.    
-00023c80: 2020 2020 696d 706f 7274 2063 5069 636b      import cPick
-00023c90: 6c65 0a20 2020 2020 2020 2077 6974 6820  le.        with 
-00023ca0: 6f70 656e 2866 696c 656e 616d 652c 2027  open(filename, '
-00023cb0: 7762 2729 2061 7320 663a 0a20 2020 2020  wb') as f:.     
-00023cc0: 2020 2020 2020 2063 5069 636b 6c65 2e64         cPickle.d
-00023cd0: 756d 7028 7365 6c66 2c20 6629 0a0a 0a23  ump(self, f)...#
-00023ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023d00: 2323 2323 230a 2320 2d2d 2d2d 2d2d 2d2d  #####.# --------
-00023d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d23 0a23 2046  -----------#.# F
-00023d30: 554e 4354 494f 4e53 202d 2d2d 2d2d 2d2d  UNCTIONS -------
-00023d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023d50: 2d2d 230a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  --#.# ----------
-00023d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023d70: 2d2d 2d2d 2d2d 2d2d 2d23 0a23 2323 2323  ---------#.#####
-00023d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023da0: 230a 0a23 6675 6e63 7469 6f6e 2074 6f20  #..#function to 
-00023db0: 6265 2063 616c 6c65 6420 7768 656e 2061  be called when a
-00023dc0: 2053 7065 6369 6573 2069 7320 696e 6974   Species is init
-00023dd0: 6961 7465 642c 0a23 7768 6963 6820 7573  iated,.#which us
-00023de0: 6573 2074 6865 2070 6172 616d 732e 7370  es the params.sp
-00023df0: 6563 6965 735b 3c73 7070 5f6e 756d 3e5d  ecies[<spp_num>]
-00023e00: 2e69 6e69 742e 5b27 4b5f 3c3e 275d 2070  .init.['K_<>'] p
-00023e10: 6172 616d 6574 6572 7320 0a23 746f 206d  arameters .#to m
-00023e20: 616b 6520 7468 6520 696e 6974 6961 6c20  ake the initial 
-00023e30: 6361 7272 7969 6e67 2d63 6170 6163 6974  carrying-capacit
-00023e40: 7920 7261 7374 6572 2c20 616e 6420 616c  y raster, and al
-00023e50: 736f 0a23 7365 7473 2074 6865 2053 7065  so.#sets the Spe
-00023e60: 6369 6573 2720 4b5f 6c61 7965 7220 616e  cies' K_layer an
-00023e70: 6420 4b5f 6661 6374 6f72 2061 7474 7269  d K_factor attri
-00023e80: 6275 7465 730a 6465 6620 5f6d 616b 655f  butes.def _make_
-00023e90: 4b28 7370 702c 206c 616e 642c 204b 5f6c  K(spp, land, K_l
-00023ea0: 6179 6572 2c20 4b5f 6661 6374 6f72 293a  ayer, K_factor):
-00023eb0: 0a20 2020 2023 6d61 6b65 2073 7572 6520  .    #make sure 
-00023ec0: 7765 2066 696e 6420 6f6e 6c79 2061 2073  we find only a s
-00023ed0: 696e 676c 6520 6c61 7965 7220 7769 7468  ingle layer with
-00023ee0: 2074 6865 206e 616d 6520 7370 6563 6966   the name specif
-00023ef0: 6965 6420 6279 204b 5f6c 6179 6572 0a20  ied by K_layer. 
-00023f00: 2020 204b 5f6c 6179 6572 203d 205b 6c79     K_layer = [ly
-00023f10: 7220 666f 7220 6c79 7220 696e 206c 616e  r for lyr in lan
-00023f20: 642e 7661 6c75 6573 2829 2069 6620 6c79  d.values() if ly
-00023f30: 722e 6e61 6d65 203d 3d20 4b5f 6c61 7965  r.name == K_laye
-00023f40: 725d 0a20 2020 2061 7373 6572 7420 6c65  r].    assert le
-00023f50: 6e28 4b5f 6c61 7965 7229 203d 3d20 312c  n(K_layer) == 1,
-00023f60: 2028 2254 6865 204b 5f6c 6179 6572 2070   ("The K_layer p
-00023f70: 6172 616d 6574 6572 2073 686f 756c 6420  arameter should 
-00023f80: 706f 696e 7420 746f 220a 2020 2020 2020  point to".      
-00023f90: 2020 2261 2073 696e 676c 6520 4c61 7965    "a single Laye
-00023fa0: 722c 2062 7574 2069 6e73 7465 6164 2025  r, but instead %
-00023fb0: 6920 4c61 7965 7273 2077 6572 6520 666f  i Layers were fo
-00023fc0: 756e 642e 2229 2025 206c 656e 284b 5f6c  und.") % len(K_l
-00023fd0: 6179 6572 290a 2020 2020 2367 7261 6220  ayer).    #grab 
-00023fe0: 7468 6520 6964 656e 7469 6669 6564 206c  the identified l
-00023ff0: 6179 6572 0a20 2020 204b 5f6c 6179 6572  ayer.    K_layer
-00024000: 203d 204b 5f6c 6179 6572 5b30 5d0a 2020   = K_layer[0].  
-00024010: 2020 2373 6574 2074 6865 2053 7065 6369    #set the Speci
-00024020: 6573 2720 4b5f 6c61 7965 7220 616e 6420  es' K_layer and 
-00024030: 4b5f 6661 6374 6f72 2061 7474 7269 6275  K_factor attribu
-00024040: 7465 730a 2020 2020 7370 702e 4b5f 6c61  tes.    spp.K_la
-00024050: 7965 7220 3d20 4b5f 6c61 7965 722e 6964  yer = K_layer.id
-00024060: 780a 2020 2020 7370 702e 4b5f 6661 6374  x.    spp.K_fact
-00024070: 6f72 203d 204b 5f66 6163 746f 720a 2020  or = K_factor.  
-00024080: 2020 2361 6464 2074 6869 7320 5370 6563    #add this Spec
-00024090: 6965 7320 746f 2074 6869 7320 4c61 7965  ies to this Laye
-000240a0: 7227 7320 2e5f 6973 5f4b 2061 7474 7269  r's ._is_K attri
-000240b0: 6275 7465 0a20 2020 2023 2877 6869 6368  bute.    #(which
-000240c0: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
-000240d0: 2075 7064 6174 6520 5370 6563 6965 732e   update Species.
-000240e0: 4b20 6966 2074 6869 7320 4c61 7965 7220  K if this Layer 
-000240f0: 756e 6465 7267 6f65 730a 2020 2020 2361  undergoes.    #a
-00024100: 6e79 206b 616e 6473 6361 7065 2063 6861  ny kandscape cha
-00024110: 6e67 6573 290a 2020 2020 4b5f 6c61 7965  nges).    K_laye
-00024120: 722e 5f69 735f 4b2e 6170 7065 6e64 2873  r._is_K.append(s
-00024130: 7070 2e69 6478 290a 2020 2020 236e 6f77  pp.idx).    #now
-00024140: 2063 616c 6375 6c61 7465 2061 6e64 2073   calculate and s
-00024150: 6574 2074 6865 204b 2072 6173 7465 720a  et the K raster.
-00024160: 2020 2020 7370 702e 5f73 6574 5f4b 286c      spp._set_K(l
-00024170: 616e 6429 0a0a 0a64 6566 205f 6d61 6b65  and)...def _make
-00024180: 5f73 7065 6369 6573 286c 616e 642c 206e  _species(land, n
-00024190: 616d 652c 2069 6478 2c20 7370 705f 7061  ame, idx, spp_pa
-000241a0: 7261 6d73 2c20 6275 726e 3d46 616c 7365  rams, burn=False
-000241b0: 2c20 7665 7262 6f73 653d 4661 6c73 6529  , verbose=False)
-000241c0: 3a0a 2020 2020 2367 6574 2073 7070 2773  :.    #get spp's
-000241d0: 2069 6e74 6961 6c69 7a69 6e67 2070 6172   intializing par
-000241e0: 616d 730a 2020 2020 696e 6974 5f70 6172  ams.    init_par
-000241f0: 616d 7320 3d20 6465 6570 636f 7079 2873  ams = deepcopy(s
-00024200: 7070 5f70 6172 616d 732e 696e 6974 290a  pp_params.init).
-00024210: 0a20 2020 2023 2070 7269 6e74 2076 6572  .    # print ver
-00024220: 626f 7365 206f 7574 7075 740a 2020 2020  bose output.    
-00024230: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-00024240: 2020 2020 7072 696e 7428 275c 745c 744d      print('\t\tM
-00024250: 414b 494e 4720 5350 4543 4945 5320 2573  AKING SPECIES %s
-00024260: 2e2e 2e5c 6e27 2025 206e 616d 652c 2066  ...\n' % name, f
-00024270: 6c75 7368 3d54 7275 6529 0a0a 2020 2020  lush=True)..    
-00024280: 2369 6620 7468 6973 2073 7065 6369 6573  #if this species
-00024290: 2073 686f 756c 6420 6861 7665 2067 656e   should have gen
-000242a0: 6f6d 6573 2c20 6372 6561 7465 2074 6865  omes, create the
-000242b0: 2067 656e 6f6d 6963 2061 7263 6869 7465   genomic archite
-000242c0: 6374 7572 650a 2020 2020 6966 2027 6765  cture.    if 'ge
-000242d0: 6e5f 6172 6368 2720 696e 2073 7070 5f70  n_arch' in spp_p
-000242e0: 6172 616d 732e 6b65 7973 2829 3a0a 2020  arams.keys():.  
-000242f0: 2020 2020 2020 2320 7072 696e 7420 7665        # print ve
-00024300: 7262 6f73 6520 6f75 7470 7574 0a20 2020  rbose output.   
-00024310: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
-00024320: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00024330: 6e74 2827 5c74 5c74 5c74 6d61 6b69 6e67  nt('\t\t\tmaking
-00024340: 2067 656e 6f6d 6963 2061 7263 6869 7465   genomic archite
-00024350: 6374 7572 652e 2e2e 5c6e 272c 2066 6c75  cture...\n', flu
-00024360: 7368 3d54 7275 6529 0a20 2020 2020 2020  sh=True).       
-00024370: 2067 5f70 6172 616d 7320 3d20 7370 705f   g_params = spp_
-00024380: 7061 7261 6d73 2e67 656e 5f61 7263 680a  params.gen_arch.
-00024390: 2020 2020 2020 2020 236d 616b 6520 6765          #make ge
-000243a0: 6e6f 6d69 635f 6172 6368 6974 6563 7475  nomic_architectu
-000243b0: 7265 0a20 2020 2020 2020 2067 656e 5f61  re.        gen_a
-000243c0: 7263 6820 3d20 5f6d 616b 655f 6765 6e6f  rch = _make_geno
-000243d0: 6d69 635f 6172 6368 6974 6563 7475 7265  mic_architecture
-000243e0: 2873 7070 5f70 6172 616d 7320 3d20 7370  (spp_params = sp
-000243f0: 705f 7061 7261 6d73 2c0a 2020 2020 2020  p_params,.      
-00024400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024430: 2020 2020 2020 2020 2020 6c61 6e64 203d            land =
-00024440: 206c 616e 6429 0a20 2020 2065 6c73 653a   land).    else:
-00024450: 0a20 2020 2020 2020 2067 656e 5f61 7263  .        gen_arc
-00024460: 6820 3d20 4e6f 6e65 0a0a 2020 2020 2320  h = None..    # 
-00024470: 7072 696e 7420 7665 7262 6f73 6520 6f75  print verbose ou
-00024480: 7470 7574 0a20 2020 2069 6620 7665 7262  tput.    if verb
-00024490: 6f73 653a 0a20 2020 2020 2020 2070 7269  ose:.        pri
-000244a0: 6e74 2827 5c74 5c74 5c74 6d61 6b69 6e67  nt('\t\t\tmaking
-000244b0: 2069 6e64 6976 6964 7561 6c73 2e2e 2e5c   individuals...\
-000244c0: 6e27 2c20 666c 7573 683d 5472 7565 290a  n', flush=True).
-000244d0: 2020 2020 236d 616b 6520 696e 6469 7669      #make indivi
-000244e0: 6473 0a20 2020 204e 203d 2069 6e69 745f  ds.    N = init_
-000244f0: 7061 7261 6d73 2e70 6f70 2827 4e27 290a  params.pop('N').
-00024500: 2020 2020 2363 7265 6174 6520 616e 206f      #create an o
-00024510: 7264 6572 6564 2064 6963 7469 6f6e 6172  rdered dictionar
-00024520: 7920 746f 2068 6f6c 6420 7468 6520 696e  y to hold the in
-00024530: 6469 7669 6475 616c 732c 2061 6e64 2066  dividuals, and f
-00024540: 696c 6c20 6974 2075 700a 2020 2020 696e  ill it up.    in
-00024550: 6473 203d 204f 4428 290a 2020 2020 666f  ds = OD().    fo
-00024560: 7220 696e 645f 6964 7820 696e 2072 616e  r ind_idx in ran
-00024570: 6765 284e 293a 0a20 2020 2020 2020 2023  ge(N):.        #
-00024580: 2075 7365 2069 6e64 6976 6964 7561 6c2e   use individual.
-00024590: 6372 6561 7465 5f69 6e64 6976 6964 7561  create_individua
-000245a0: 6c20 746f 2073 696d 756c 6174 6520 696e  l to simulate in
-000245b0: 6469 7669 6475 616c 730a 2020 2020 2020  dividuals.      
-000245c0: 2020 2361 6e64 2061 6464 2074 6865 6d20    #and add them 
-000245d0: 746f 2074 6865 2073 7065 6369 6573 0a20  to the species. 
-000245e0: 2020 2020 2020 2069 6e64 203d 205f 6d61         ind = _ma
-000245f0: 6b65 5f69 6e64 6976 6964 7561 6c28 6964  ke_individual(id
-00024600: 783d 696e 645f 6964 782c 206f 6666 7370  x=ind_idx, offsp
-00024610: 7269 6e67 3d46 616c 7365 2c0a 2020 2020  ring=False,.    
-00024620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024630: 2020 2020 2020 2020 2020 2064 696d 3d6c             dim=l
-00024640: 616e 642e 6469 6d2c 2067 656e 6f6d 6963  and.dim, genomic
-00024650: 5f61 7263 6869 7465 6374 7572 653d 6765  _architecture=ge
-00024660: 6e5f 6172 6368 2c0a 2020 2020 2020 2020  n_arch,.        
-00024670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024680: 2020 2020 2020 2062 7572 6e3d 6275 726e         burn=burn
-00024690: 290a 2020 2020 2020 2020 696e 6473 5b69  ).        inds[i
-000246a0: 6e64 5f69 6478 5d20 3d20 696e 640a 0a20  nd_idx] = ind.. 
-000246b0: 2020 2023 6372 6561 7465 2074 6865 2073     #create the s
-000246c0: 7065 6369 6573 2066 726f 6d20 7468 6f73  pecies from thos
-000246d0: 6520 696e 6469 7669 6475 616c 730a 2020  e individuals.  
-000246e0: 2020 7370 7020 3d20 5370 6563 6965 7328    spp = Species(
-000246f0: 6e61 6d65 203d 206e 616d 652c 2069 6478  name = name, idx
-00024700: 203d 2069 6478 2c20 696e 6473 203d 2069   = idx, inds = i
-00024710: 6e64 732c 206c 616e 6420 3d20 6c61 6e64  nds, land = land
-00024720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00024730: 2020 2020 2020 2073 7070 5f70 6172 616d         spp_param
-00024740: 7320 3d20 7370 705f 7061 7261 6d73 2c20  s = spp_params, 
-00024750: 6765 6e6f 6d69 635f 6172 6368 6974 6563  genomic_architec
-00024760: 7475 7265 3d67 656e 5f61 7263 6829 0a0a  ture=gen_arch)..
-00024770: 2020 2020 2375 7365 2074 6865 2072 656d      #use the rem
-00024780: 6169 6e69 6e67 2069 6e69 745f 7061 7261  aining init_para
-00024790: 6d73 2074 6f20 7365 7420 7468 6520 6361  ms to set the ca
-000247a0: 7272 7969 6e67 2d63 6170 6163 6974 7920  rrying-capacity 
-000247b0: 7261 7374 6572 2028 4b29 0a20 2020 205f  raster (K).    _
-000247c0: 6d61 6b65 5f4b 2873 7070 2c20 6c61 6e64  make_K(spp, land
-000247d0: 2c20 2a2a 7b6b 3a76 2066 6f72 206b 2c76  , **{k:v for k,v
-000247e0: 2069 6e20 696e 6974 5f70 6172 616d 732e   in init_params.
-000247f0: 6974 656d 7328 2920 6966 206b 2021 3d20  items() if k != 
-00024800: 276d 7370 7269 6d65 277d 290a 2020 2020  'msprime'}).    
-00024810: 2373 6574 2069 6e69 7469 616c 2065 6e76  #set initial env
-00024820: 6972 6f6e 6d65 6e74 2076 616c 7565 730a  ironment values.
-00024830: 2020 2020 7370 702e 5f73 6574 5f65 286c      spp._set_e(l
-00024840: 616e 6429 0a20 2020 2023 7365 7420 696e  and).    #set in
-00024850: 6974 6961 6c20 636f 6f72 6473 2061 6e64  itial coords and
-00024860: 2063 656c 6c73 0a20 2020 2073 7070 2e5f   cells.    spp._
-00024870: 7365 745f 636f 6f72 6473 5f61 6e64 5f63  set_coords_and_c
-00024880: 656c 6c73 2829 0a20 2020 2023 7365 7420  ells().    #set 
-00024890: 7468 6520 6b64 5f74 7265 650a 2020 2020  the kd_tree.    
-000248a0: 7370 702e 5f73 6574 5f6b 645f 7472 6565  spp._set_kd_tree
-000248b0: 2829 0a0a 2020 2020 2373 6574 2070 6865  ()..    #set phe
-000248c0: 6e6f 7479 7065 732c 2069 6620 7468 6520  notypes, if the 
-000248d0: 7370 6563 6965 7320 6861 7320 6765 6e6f  species has geno
-000248e0: 6d65 730a 2020 2020 6966 2073 7070 2e67  mes.    if spp.g
-000248f0: 656e 5f61 7263 6820 6973 206e 6f74 204e  en_arch is not N
-00024900: 6f6e 6520 616e 6420 6e6f 7420 6275 726e  one and not burn
-00024910: 3a0a 2020 2020 2020 2020 5b69 6e64 2e5f  :.        [ind._
-00024920: 7365 745f 7a28 7370 702e 6765 6e5f 6172  set_z(spp.gen_ar
-00024930: 6368 2920 666f 7220 696e 6420 696e 2073  ch) for ind in s
-00024940: 7070 2e76 616c 7565 7328 295d 0a0a 2020  pp.values()]..  
-00024950: 2020 236d 616b 6520 6465 6e73 6974 795f    #make density_
-00024960: 6772 6964 0a20 2020 2073 7070 2e5f 7365  grid.    spp._se
-00024970: 745f 6465 6e73 5f67 7269 6473 286c 616e  t_dens_grids(lan
-00024980: 6429 0a0a 2020 2020 236d 616b 6520 6d6f  d)..    #make mo
-00024990: 7665 6d65 6e74 2073 7572 6661 6365 2c20  vement surface, 
-000249a0: 6966 206e 6565 6465 640a 2020 2020 6966  if needed.    if
-000249b0: 2073 7070 2e5f 6d6f 7665 3a0a 2020 2020   spp._move:.    
-000249c0: 2020 2020 6966 2027 6d6f 7665 5f73 7572      if 'move_sur
-000249d0: 6627 2069 6e20 7370 705f 7061 7261 6d73  f' in spp_params
-000249e0: 2e6d 6f76 656d 656e 742e 6b65 7973 2829  .movement.keys()
-000249f0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00024a00: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00024a10: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00024a20: 2827 5c74 5c74 5c74 6d61 6b69 6e67 206d  ('\t\t\tmaking m
-00024a30: 6f76 656d 656e 7420 7375 7266 6163 652e  ovement surface.
-00024a40: 2e2e 5c6e 270a 2020 2020 2020 2020 2020  ..\n'.          
-00024a50: 2020 2020 2020 2020 2020 2020 2027 5c74               '\t
-00024a60: 5c74 5c74 5c74 5b63 616e 2074 616b 6520  \t\t\t[can take 
-00024a70: 6120 6269 745d 5c6e 2729 2c20 666c 7573  a bit]\n'), flus
-00024a80: 683d 5472 7565 290a 2020 2020 2020 2020  h=True).        
-00024a90: 2020 2020 6d73 5f70 6172 616d 7320 3d20      ms_params = 
-00024aa0: 6465 6570 636f 7079 2873 7070 5f70 6172  deepcopy(spp_par
-00024ab0: 616d 732e 6d6f 7665 6d65 6e74 2e6d 6f76  ams.movement.mov
-00024ac0: 655f 7375 7266 290a 2020 2020 2020 2020  e_surf).        
-00024ad0: 2020 2020 2367 7261 6220 7468 6520 6c79      #grab the ly
-00024ae0: 7220 6e75 6d62 6572 2066 6f72 2074 6865  r number for the
-00024af0: 206c 7972 2074 6861 7420 7468 6520 0a20   lyr that the . 
-00024b00: 2020 2020 2020 2020 2020 2023 6d6f 7665             #move
-00024b10: 6d65 6e74 2073 7572 6661 6365 2069 7320  ment surface is 
-00024b20: 746f 2062 6520 6261 7365 6420 6f6e 0a20  to be based on. 
-00024b30: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
-00024b40: 7375 7266 5f6c 7972 203d 206d 735f 7061  surf_lyr = ms_pa
-00024b50: 7261 6d73 2e70 6f70 2827 6c61 7965 7227  rams.pop('layer'
-00024b60: 290a 2020 2020 2020 2020 2020 2020 6d6f  ).            mo
-00024b70: 7665 5f73 7572 665f 6c79 725f 6e75 6d20  ve_surf_lyr_num 
-00024b80: 3d20 5b6b 2066 6f72 206b 2c76 2069 6e20  = [k for k,v in 
-00024b90: 6c61 6e64 2e69 7465 6d73 280a 2020 2020  land.items(.    
-00024ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024bc0: 2020 2020 2020 2020 2920 6966 2076 2e6e          ) if v.n
-00024bd0: 616d 6520 3d3d 206d 6f76 655f 7375 7266  ame == move_surf
-00024be0: 5f6c 7972 5d0a 2020 2020 2020 2020 2020  _lyr].          
-00024bf0: 2020 6173 7365 7274 206c 656e 286d 6f76    assert len(mov
-00024c00: 655f 7375 7266 5f6c 7972 5f6e 756d 2920  e_surf_lyr_num) 
-00024c10: 3d3d 2031 2c20 2822 4578 7065 6374 6564  == 1, ("Expected
-00024c20: 2074 6f20 6669 6e64 206f 6e6c 7920 6120   to find only a 
-00024c30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00024c40: 2020 2273 696e 676c 6520 4c61 7965 7220    "single Layer 
-00024c50: 7769 7468 2074 6865 206e 616d 6520 7072  with the name pr
-00024c60: 6f76 6964 6564 2066 6f72 2074 6865 2022  ovided for the "
-00024c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024c80: 2022 5f43 6f6e 6475 6374 616e 6365 5375   "_ConductanceSu
-00024c90: 7266 6163 652c 220a 2020 2020 2020 2020  rface,".        
-00024ca0: 2020 2020 2020 2020 2220 6275 7420 696e          " but in
-00024cb0: 7374 6561 6420 666f 756e 6420 2569 2229  stead found %i")
-00024cc0: 2025 206c 656e 286d 6f76 655f 7375 7266   % len(move_surf
-00024cd0: 5f6c 7972 5f6e 756d 290a 2020 2020 2020  _lyr_num).      
-00024ce0: 2020 2020 2020 6d6f 7665 5f73 7572 665f        move_surf_
-00024cf0: 6c79 725f 6e75 6d20 3d20 6d6f 7665 5f73  lyr_num = move_s
-00024d00: 7572 665f 6c79 725f 6e75 6d5b 305d 0a20  urf_lyr_num[0]. 
-00024d10: 2020 2020 2020 2020 2020 2023 6d61 6b65             #make
-00024d20: 2074 6865 206d 6f76 656d 656e 7420 7375   the movement su
-00024d30: 7266 6163 6520 616e 6420 7365 7420 6974  rface and set it
-00024d40: 2061 7320 7468 6520 7370 7027 730a 2020   as the spp's.  
-00024d50: 2020 2020 2020 2020 2020 236d 6f76 655f            #move_
-00024d60: 7375 7266 2061 7474 7269 6275 7465 0a20  surf attribute. 
-00024d70: 2020 2020 2020 2020 2020 2073 7070 2e5f             spp._
-00024d80: 6d6f 7665 5f73 7572 663d 2073 7074 2e5f  move_surf= spt._
-00024d90: 436f 6e64 7563 7461 6e63 6553 7572 6661  ConductanceSurfa
-00024da0: 6365 286c 616e 645b 6d6f 7665 5f73 7572  ce(land[move_sur
-00024db0: 665f 6c79 725f 6e75 6d5d 2c0a 2020 2020  f_lyr_num],.    
-00024dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024df0: 2020 2020 2020 2020 2020 2020 2a2a 6d73              **ms
-00024e00: 5f70 6172 616d 7329 0a20 2020 2023 6d61  _params).    #ma
-00024e10: 6b65 2064 6973 7065 7273 616c 2073 7572  ke dispersal sur
-00024e20: 6661 6365 2c20 6966 206e 6565 6465 640a  face, if needed.
-00024e30: 2020 2020 6966 2027 6469 7370 5f73 7572      if 'disp_sur
-00024e40: 6627 2069 6e20 7370 705f 7061 7261 6d73  f' in spp_params
-00024e50: 2e6d 6f76 656d 656e 742e 6b65 7973 2829  .movement.keys()
-00024e60: 3a0a 2020 2020 2020 2020 2320 7072 696e  :.        # prin
-00024e70: 7420 7665 7262 6f73 6520 6f75 7470 7574  t verbose output
-00024e80: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-00024e90: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
-00024ea0: 2070 7269 6e74 2828 275c 745c 745c 746d   print(('\t\t\tm
-00024eb0: 616b 696e 6720 6469 7370 6572 7361 6c20  aking dispersal 
-00024ec0: 7375 7266 6163 652e 2e2e 5c6e 270a 2020  surface...\n'.  
-00024ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ee0: 2027 5c74 5c74 5c74 5c74 5b63 616e 2074   '\t\t\t\t[can t
-00024ef0: 616b 6520 6120 6269 745d 5c6e 2729 2c20  ake a bit]\n'), 
-00024f00: 666c 7573 683d 5472 7565 290a 2020 2020  flush=True).    
-00024f10: 2020 2020 6473 5f70 6172 616d 7320 3d20      ds_params = 
-00024f20: 6465 6570 636f 7079 2873 7070 5f70 6172  deepcopy(spp_par
-00024f30: 616d 732e 6d6f 7665 6d65 6e74 2e64 6973  ams.movement.dis
-00024f40: 705f 7375 7266 290a 2020 2020 2020 2020  p_surf).        
-00024f50: 2367 7261 6220 7468 6520 6c79 7220 6e75  #grab the lyr nu
-00024f60: 6d62 6572 2066 6f72 2074 6865 206c 7972  mber for the lyr
-00024f70: 2074 6861 7420 7468 6520 0a20 2020 2020   that the .     
-00024f80: 2020 2023 6469 7370 6572 7361 6c20 7375     #dispersal su
-00024f90: 7266 6163 6520 6973 2074 6f20 6265 2062  rface is to be b
-00024fa0: 6173 6564 206f 6e0a 2020 2020 2020 2020  ased on.        
-00024fb0: 6469 7370 5f73 7572 665f 6c79 7220 3d20  disp_surf_lyr = 
-00024fc0: 6473 5f70 6172 616d 732e 706f 7028 276c  ds_params.pop('l
-00024fd0: 6179 6572 2729 0a20 2020 2020 2020 2064  ayer').        d
-00024fe0: 6973 705f 7375 7266 5f6c 7972 5f6e 756d  isp_surf_lyr_num
-00024ff0: 203d 205b 6b20 666f 7220 6b2c 7620 696e   = [k for k,v in
-00025000: 206c 616e 642e 6974 656d 7328 0a20 2020   land.items(.   
-00025010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025030: 2020 2020 2029 2069 6620 762e 6e61 6d65       ) if v.name
-00025040: 203d 3d20 6469 7370 5f73 7572 665f 6c79   == disp_surf_ly
-00025050: 725d 0a20 2020 2020 2020 2061 7373 6572  r].        asser
-00025060: 7420 6c65 6e28 6469 7370 5f73 7572 665f  t len(disp_surf_
-00025070: 6c79 725f 6e75 6d29 203d 3d20 312c 2028  lyr_num) == 1, (
-00025080: 2245 7870 6563 7465 6420 746f 2066 696e  "Expected to fin
-00025090: 6420 6f6e 6c79 2061 2022 0a20 2020 2020  d only a ".     
-000250a0: 2020 2020 2020 2022 7369 6e67 6c65 204c         "single L
-000250b0: 6179 6572 2077 6974 6820 7468 6520 6e61  ayer with the na
-000250c0: 6d65 2070 726f 7669 6465 6420 666f 7220  me provided for 
-000250d0: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
-000250e0: 2020 225f 436f 6e64 7563 7461 6e63 6553    "_ConductanceS
-000250f0: 7572 6661 6365 2c20 220a 2020 2020 2020  urface, ".      
-00025100: 2020 2020 2020 2262 7574 2069 6e73 7465        "but inste
-00025110: 6164 2066 6f75 6e64 2025 6922 2920 2520  ad found %i") % 
-00025120: 6c65 6e28 6469 7370 5f73 7572 665f 6c79  len(disp_surf_ly
-00025130: 725f 6e75 6d29 0a20 2020 2020 2020 2064  r_num).        d
-00025140: 6973 705f 7375 7266 5f6c 7972 5f6e 756d  isp_surf_lyr_num
-00025150: 203d 2064 6973 705f 7375 7266 5f6c 7972   = disp_surf_lyr
-00025160: 5f6e 756d 5b30 5d0a 2020 2020 2020 2020  _num[0].        
-00025170: 236d 616b 6520 7468 6520 6469 7370 6572  #make the disper
-00025180: 7361 6c20 7375 7266 6163 6520 616e 6420  sal surface and 
-00025190: 7365 7420 6974 2061 7320 7468 6520 7370  set it as the sp
-000251a0: 7027 730a 2020 2020 2020 2020 2364 6973  p's.        #dis
-000251b0: 705f 7375 7266 2061 7474 7269 6275 7465  p_surf attribute
-000251c0: 0a20 2020 2020 2020 2073 7070 2e5f 6469  .        spp._di
-000251d0: 7370 5f73 7572 6620 3d20 7370 742e 5f43  sp_surf = spt._C
-000251e0: 6f6e 6475 6374 616e 6365 5375 7266 6163  onductanceSurfac
-000251f0: 6528 6c61 6e64 5b64 6973 705f 7375 7266  e(land[disp_surf
-00025200: 5f6c 7972 5f6e 756d 5d2c 0a20 2020 2020  _lyr_num],.     
-00025210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025240: 2020 2020 2020 2020 2020 202a 2a64 735f             **ds_
-00025250: 7061 7261 6d73 290a 0a20 2020 2023 6966  params)..    #if
-00025260: 2074 6869 7320 7370 6563 6965 7320 6861   this species ha
-00025270: 7320 6368 616e 6765 7320 7061 7261 6d65  s changes parame
-00025280: 7465 7269 7a65 642c 206f 7220 6966 206e  terized, or if n
-00025290: 6f74 2062 7574 2069 7420 6861 730a 2020  ot but it has.  
-000252a0: 2020 2365 6974 6865 7220 6120 4d6f 7665    #either a Move
-000252b0: 6d65 6e74 5375 7266 206f 7220 6120 4469  mentSurf or a Di
-000252c0: 7370 6572 7361 6c53 7572 6620 6261 7365  spersalSurf base
-000252d0: 6420 6f6e 2061 204c 6179 6572 2074 6861  d on a Layer tha
-000252e0: 740a 2020 2020 2377 696c 6c20 756e 6465  t.    #will unde
-000252f0: 7267 6f20 6c61 6e64 7363 6170 6520 6368  rgo landscape ch
-00025300: 616e 6765 2c20 7468 656e 2063 7265 6174  ange, then creat
-00025310: 6520 6120 5f53 7065 6369 6573 4368 616e  e a _SpeciesChan
-00025320: 6765 7220 6f62 6a65 6374 2066 6f72 2069  ger object for i
-00025330: 740a 2020 2020 6966 2028 2763 6861 6e67  t.    if ('chang
-00025340: 6527 2069 6e20 7370 705f 7061 7261 6d73  e' in spp_params
-00025350: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
-00025360: 6f72 2028 7370 702e 5f6d 6f76 655f 7375  or (spp._move_su
-00025370: 7266 2069 7320 6e6f 7420 4e6f 6e65 0a20  rf is not None. 
-00025380: 2020 2020 2020 2061 6e64 206c 616e 642e         and land.
-00025390: 5f63 6861 6e67 6572 2069 7320 6e6f 7420  _changer is not 
-000253a0: 4e6f 6e65 0a20 2020 2020 2020 2061 6e64  None.        and
-000253b0: 2073 7070 2e5f 6d6f 7665 5f73 7572 662e   spp._move_surf.
-000253c0: 6c79 725f 6e75 6d20 696e 206c 616e 642e  lyr_num in land.
-000253d0: 5f63 6861 6e67 6572 2e63 6861 6e67 655f  _changer.change_
-000253e0: 696e 666f 2e6b 6579 7328 2929 0a20 2020  info.keys()).   
-000253f0: 2020 2020 206f 7220 2873 7070 2e5f 6469       or (spp._di
-00025400: 7370 5f73 7572 6620 6973 206e 6f74 204e  sp_surf is not N
-00025410: 6f6e 650a 2020 2020 2020 2020 616e 6420  one.        and 
-00025420: 6c61 6e64 2e5f 6368 616e 6765 7220 6973  land._changer is
-00025430: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-00025440: 2020 616e 6420 7370 702e 5f64 6973 705f    and spp._disp_
-00025450: 7375 7266 2e6c 7972 5f6e 756d 2069 6e20  surf.lyr_num in 
-00025460: 6c61 6e64 2e5f 6368 616e 6765 722e 6368  land._changer.ch
-00025470: 616e 6765 5f69 6e66 6f2e 6b65 7973 2829  ange_info.keys()
-00025480: 2929 3a0a 2020 2020 2020 2020 2320 7072  )):.        # pr
-00025490: 696e 7420 7665 7262 6f73 6520 6f75 7470  int verbose outp
-000254a0: 7574 0a20 2020 2020 2020 2069 6620 7665  ut.        if ve
-000254b0: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-000254c0: 2020 2070 7269 6e74 2828 275c 745c 745c     print(('\t\t\
-000254d0: 7473 6574 7469 6e67 2075 7020 7370 6563  tsetting up spec
-000254e0: 6965 7320 6368 616e 6765 732e 2e2e 5c6e  ies changes...\n
-000254f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00025500: 2020 2020 2027 5c74 5c74 5c74 5c74 5b63       '\t\t\t\t[c
-00025510: 616e 2074 616b 6520 6120 7768 696c 652c  an take a while,
-00025520: 5c6e 5c74 5c74 5c74 5c74 2069 6620 6d6f  \n\t\t\t\t if mo
-00025530: 7665 6d65 6e74 206f 7220 270a 2020 2020  vement or '.    
-00025540: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00025550: 6469 7370 6572 7361 6c5c 6e5c 745c 745c  dispersal\n\t\t\
-00025560: 745c 7420 7375 7266 6163 6573 2077 696c  t\t surfaces wil
-00025570: 6c20 6368 616e 6765 5d5c 6e27 292c 2066  l change]\n'), f
-00025580: 6c75 7368 3d54 7275 6529 0a20 2020 2020  lush=True).     
-00025590: 2020 2023 6772 6162 2074 6865 2063 6861     #grab the cha
-000255a0: 6e67 6520 7061 7261 6d73 2028 6f72 204e  nge params (or N
-000255b0: 6f6e 652c 2069 660a 2020 2020 2020 2020  one, if.        
-000255c0: 6966 2027 6368 616e 6765 2720 696e 2073  if 'change' in s
-000255d0: 7070 5f70 6172 616d 732e 6b65 7973 2829  pp_params.keys()
-000255e0: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-000255f0: 5f70 6172 616d 7320 3d20 7370 705f 7061  _params = spp_pa
-00025600: 7261 6d73 2e63 6861 6e67 650a 2020 2020  rams.change.    
-00025610: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00025620: 2020 2020 2020 6368 5f70 6172 616d 7320        ch_params 
-00025630: 3d20 4e6f 6e65 0a20 2020 2020 2020 2023  = None.        #
-00025640: 6d61 6b65 205f 5370 6563 6965 7343 6861  make _SpeciesCha
-00025650: 6e67 6572 2061 6e64 2073 6574 2069 7420  nger and set it 
-00025660: 746f 2074 6865 2073 7070 2773 2063 6861  to the spp's cha
-00025670: 6e67 6572 2061 7474 7269 6275 7465 0a20  nger attribute. 
-00025680: 2020 2020 2020 2073 7070 2e5f 6368 616e         spp._chan
-00025690: 6765 7220 3d20 5f53 7065 6369 6573 4368  ger = _SpeciesCh
-000256a0: 616e 6765 7228 7370 702c 2063 685f 7061  anger(spp, ch_pa
-000256b0: 7261 6d73 2c20 6c61 6e64 203d 206c 616e  rams, land = lan
-000256c0: 6429 0a0a 2020 2020 7265 7475 726e 2073  d)..    return s
-000256d0: 7070 0a0a 0a23 2066 756e 6374 696f 6e20  pp...# function 
-000256e0: 666f 7220 7265 6164 696e 6720 696e 2061  for reading in a
-000256f0: 2070 6963 6b6c 6564 2073 7070 0a64 6566   pickled spp.def
-00025700: 2072 6561 645f 7069 636b 6c65 645f 7370   read_pickled_sp
-00025710: 7028 6669 6c65 6e61 6d65 293a 0a20 2020  p(filename):.   
-00025720: 2069 6d70 6f72 7420 6350 6963 6b6c 650a   import cPickle.
-00025730: 2020 2020 7769 7468 206f 7065 6e28 6669      with open(fi
-00025740: 6c65 6e61 6d65 2c20 2772 6227 2920 6173  lename, 'rb') as
-00025750: 2066 3a0a 2020 2020 2020 2020 7370 7020   f:.        spp 
-00025760: 3d20 6350 6963 6b6c 652e 6c6f 6164 2866  = cPickle.load(f
-00025770: 290a 2020 2020 7265 7475 726e 2073 7070  ).    return spp
-00025780: 0a0a 0a                                  ...
+00023a10: 2020 2020 2069 6e74 2830 2e30 3520 2a20       int(0.05 * 
+00023a20: 7365 6c66 2e67 656e 5f61 7263 682e 4c29  self.gen_arch.L)
+00023a30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023a40: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00023a50: 6973 3d31 292c 0a20 2020 2020 2020 2020  is=1),.         
+00023a60: 2020 2020 2020 2020 2063 6d61 703d 2774           cmap='t
+00023a70: 6572 7261 696e 2729 0a20 2020 2020 2020  errain').       
+00023a80: 2061 782e 7365 745f 7469 746c 6528 2267   ax.set_title("g
+00023a90: 616d 6574 6520 3020 2020 2020 6761 6d65  amete 0     game
+00023aa0: 7465 3122 290a 2020 2020 2020 2020 6178  te1").        ax
+00023ab0: 2e73 6574 5f78 7469 636b 7328 5b5d 290a  .set_xticks([]).
+00023ac0: 2020 2020 2020 2020 6178 2e73 6574 5f79          ax.set_y
+00023ad0: 6c61 6265 6c28 276c 6f63 7573 2729 0a20  label('locus'). 
+00023ae0: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
+00023af0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00023b00: 2872 6563 6f6d 625f 7061 7468 732c 206d  (recomb_paths, m
+00023b10: 6f63 6b5f 7370 702c 2072 6563 6f6d 625f  ock_spp, recomb_
+00023b20: 6765 6e6f 6d65 290a 0a0a 2020 2020 6465  genome)...    de
+00023b30: 6620 5f70 6c6f 745f 7374 6174 2873 656c  f _plot_stat(sel
+00023b40: 662c 2073 7461 7429 3a0a 2020 2020 2020  f, stat):.      
+00023b50: 2020 6966 2073 656c 662e 5f73 7461 7473    if self._stats
+00023b60: 5f63 6f6c 6c65 6374 6f72 2069 7320 4e6f  _collector is No
+00023b70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00023b80: 7072 696e 7428 2822 5370 6563 6965 732e  print(("Species.
+00023b90: 5f70 6c6f 745f 7374 6174 2069 7320 6e6f  _plot_stat is no
+00023ba0: 7420 7661 6c69 6420 220a 2020 2020 2020  t valid ".      
+00023bb0: 2020 2020 2020 2020 2020 2266 6f72 2073            "for s
+00023bc0: 7065 6369 6573 2077 6974 6820 6e6f 205f  pecies with no _
+00023bd0: 5374 6174 7343 6f6c 6c65 6374 6f72 206f  StatsCollector o
+00023be0: 626a 6563 742e 5c6e 2229 290a 0a20 2020  bject.\n"))..   
+00023bf0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00023c00: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
+00023c10: 7473 5f63 6f6c 6c65 6374 6f72 2e5f 706c  ts_collector._pl
+00023c20: 6f74 5f73 7461 7428 7374 6174 2c20 7370  ot_stat(stat, sp
+00023c30: 705f 6e61 6d65 203d 2073 656c 662e 6e61  p_name = self.na
+00023c40: 6d65 290a 0a0a 2020 2020 2020 2020 2323  me)...        ##
+00023c50: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+00023c60: 2020 2020 2020 2023 7075 626c 6963 206d         #public m
+00023c70: 6574 686f 6473 230a 2020 2020 2020 2020  ethods#.        
+00023c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023c90: 0a0a 2020 2020 6465 6620 5f77 7269 7465  ..    def _write
+00023ca0: 5f70 6963 6b6c 6528 7365 6c66 2c20 6669  _pickle(self, fi
+00023cb0: 6c65 6e61 6d65 293a 0a20 2020 2020 2020  lename):.       
+00023cc0: 2069 6d70 6f72 7420 6350 6963 6b6c 650a   import cPickle.
+00023cd0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00023ce0: 6e28 6669 6c65 6e61 6d65 2c20 2777 6227  n(filename, 'wb'
+00023cf0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+00023d00: 2020 2020 6350 6963 6b6c 652e 6475 6d70      cPickle.dump
+00023d10: 2873 656c 662c 2066 290a 0a0a 2323 2323  (self, f)...####
+00023d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023d40: 2323 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ##.# -----------
+00023d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023d60: 2d2d 2d2d 2d2d 2d2d 230a 2320 4655 4e43  --------#.# FUNC
+00023d70: 5449 4f4e 5320 2d2d 2d2d 2d2d 2d2d 2d2d  TIONS ----------
+00023d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d23  ---------------#
+00023d90: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
+00023da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023db0: 2d2d 2d2d 2d2d 230a 2323 2323 2323 2323  ------#.########
+00023dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023dd0: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
+00023de0: 2366 756e 6374 696f 6e20 746f 2062 6520  #function to be 
+00023df0: 6361 6c6c 6564 2077 6865 6e20 6120 5370  called when a Sp
+00023e00: 6563 6965 7320 6973 2069 6e69 7469 6174  ecies is initiat
+00023e10: 6564 2c0a 2377 6869 6368 2075 7365 7320  ed,.#which uses 
+00023e20: 7468 6520 7061 7261 6d73 2e73 7065 6369  the params.speci
+00023e30: 6573 5b3c 7370 705f 6e75 6d3e 5d2e 696e  es[<spp_num>].in
+00023e40: 6974 2e5b 274b 5f3c 3e27 5d20 7061 7261  it.['K_<>'] para
+00023e50: 6d65 7465 7273 200a 2374 6f20 6d61 6b65  meters .#to make
+00023e60: 2074 6865 2069 6e69 7469 616c 2063 6172   the initial car
+00023e70: 7279 696e 672d 6361 7061 6369 7479 2072  rying-capacity r
+00023e80: 6173 7465 722c 2061 6e64 2061 6c73 6f0a  aster, and also.
+00023e90: 2373 6574 7320 7468 6520 5370 6563 6965  #sets the Specie
+00023ea0: 7327 204b 5f6c 6179 6572 2061 6e64 204b  s' K_layer and K
+00023eb0: 5f66 6163 746f 7220 6174 7472 6962 7574  _factor attribut
+00023ec0: 6573 0a64 6566 205f 6d61 6b65 5f4b 2873  es.def _make_K(s
+00023ed0: 7070 2c20 6c61 6e64 2c20 4b5f 6c61 7965  pp, land, K_laye
+00023ee0: 722c 204b 5f66 6163 746f 7229 3a0a 2020  r, K_factor):.  
+00023ef0: 2020 236d 616b 6520 7375 7265 2077 6520    #make sure we 
+00023f00: 6669 6e64 206f 6e6c 7920 6120 7369 6e67  find only a sing
+00023f10: 6c65 206c 6179 6572 2077 6974 6820 7468  le layer with th
+00023f20: 6520 6e61 6d65 2073 7065 6369 6669 6564  e name specified
+00023f30: 2062 7920 4b5f 6c61 7965 720a 2020 2020   by K_layer.    
+00023f40: 4b5f 6c61 7965 7220 3d20 5b6c 7972 2066  K_layer = [lyr f
+00023f50: 6f72 206c 7972 2069 6e20 6c61 6e64 2e76  or lyr in land.v
+00023f60: 616c 7565 7328 2920 6966 206c 7972 2e6e  alues() if lyr.n
+00023f70: 616d 6520 3d3d 204b 5f6c 6179 6572 5d0a  ame == K_layer].
+00023f80: 2020 2020 6173 7365 7274 206c 656e 284b      assert len(K
+00023f90: 5f6c 6179 6572 2920 3d3d 2031 2c20 2822  _layer) == 1, ("
+00023fa0: 5468 6520 4b5f 6c61 7965 7220 7061 7261  The K_layer para
+00023fb0: 6d65 7465 7220 7368 6f75 6c64 2070 6f69  meter should poi
+00023fc0: 6e74 2074 6f22 0a20 2020 2020 2020 2022  nt to".        "
+00023fd0: 6120 7369 6e67 6c65 204c 6179 6572 2c20  a single Layer, 
+00023fe0: 6275 7420 696e 7374 6561 6420 2569 204c  but instead %i L
+00023ff0: 6179 6572 7320 7765 7265 2066 6f75 6e64  ayers were found
+00024000: 2e22 2920 2520 6c65 6e28 4b5f 6c61 7965  .") % len(K_laye
+00024010: 7229 0a20 2020 2023 6772 6162 2074 6865  r).    #grab the
+00024020: 2069 6465 6e74 6966 6965 6420 6c61 7965   identified laye
+00024030: 720a 2020 2020 4b5f 6c61 7965 7220 3d20  r.    K_layer = 
+00024040: 4b5f 6c61 7965 725b 305d 0a20 2020 2023  K_layer[0].    #
+00024050: 7365 7420 7468 6520 5370 6563 6965 7327  set the Species'
+00024060: 204b 5f6c 6179 6572 2061 6e64 204b 5f66   K_layer and K_f
+00024070: 6163 746f 7220 6174 7472 6962 7574 6573  actor attributes
+00024080: 0a20 2020 2073 7070 2e4b 5f6c 6179 6572  .    spp.K_layer
+00024090: 203d 204b 5f6c 6179 6572 2e69 6478 0a20   = K_layer.idx. 
+000240a0: 2020 2073 7070 2e4b 5f66 6163 746f 7220     spp.K_factor 
+000240b0: 3d20 4b5f 6661 6374 6f72 0a20 2020 2023  = K_factor.    #
+000240c0: 6164 6420 7468 6973 2053 7065 6369 6573  add this Species
+000240d0: 2074 6f20 7468 6973 204c 6179 6572 2773   to this Layer's
+000240e0: 202e 5f69 735f 4b20 6174 7472 6962 7574   ._is_K attribut
+000240f0: 650a 2020 2020 2328 7768 6963 6820 7769  e.    #(which wi
+00024100: 6c6c 2062 6520 7573 6564 2074 6f20 7570  ll be used to up
+00024110: 6461 7465 2053 7065 6369 6573 2e4b 2069  date Species.K i
+00024120: 6620 7468 6973 204c 6179 6572 2075 6e64  f this Layer und
+00024130: 6572 676f 6573 0a20 2020 2023 616e 7920  ergoes.    #any 
+00024140: 6b61 6e64 7363 6170 6520 6368 616e 6765  kandscape change
+00024150: 7329 0a20 2020 204b 5f6c 6179 6572 2e5f  s).    K_layer._
+00024160: 6973 5f4b 2e61 7070 656e 6428 7370 702e  is_K.append(spp.
+00024170: 6964 7829 0a20 2020 2023 6e6f 7720 6361  idx).    #now ca
+00024180: 6c63 756c 6174 6520 616e 6420 7365 7420  lculate and set 
+00024190: 7468 6520 4b20 7261 7374 6572 0a20 2020  the K raster.   
+000241a0: 2073 7070 2e5f 7365 745f 4b28 6c61 6e64   spp._set_K(land
+000241b0: 290a 0a0a 6465 6620 5f6d 616b 655f 7370  )...def _make_sp
+000241c0: 6563 6965 7328 6c61 6e64 2c20 6e61 6d65  ecies(land, name
+000241d0: 2c20 6964 782c 2073 7070 5f70 6172 616d  , idx, spp_param
+000241e0: 732c 2062 7572 6e3d 4661 6c73 652c 2076  s, burn=False, v
+000241f0: 6572 626f 7365 3d46 616c 7365 293a 0a20  erbose=False):. 
+00024200: 2020 2023 6765 7420 7370 7027 7320 696e     #get spp's in
+00024210: 7469 616c 697a 696e 6720 7061 7261 6d73  tializing params
+00024220: 0a20 2020 2069 6e69 745f 7061 7261 6d73  .    init_params
+00024230: 203d 2064 6565 7063 6f70 7928 7370 705f   = deepcopy(spp_
+00024240: 7061 7261 6d73 2e69 6e69 7429 0a0a 2020  params.init)..  
+00024250: 2020 2320 7072 696e 7420 7665 7262 6f73    # print verbos
+00024260: 6520 6f75 7470 7574 0a20 2020 2069 6620  e output.    if 
+00024270: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+00024280: 2070 7269 6e74 2827 5c74 5c74 4d41 4b49   print('\t\tMAKI
+00024290: 4e47 2053 5045 4349 4553 2025 732e 2e2e  NG SPECIES %s...
+000242a0: 5c6e 2720 2520 6e61 6d65 2c20 666c 7573  \n' % name, flus
+000242b0: 683d 5472 7565 290a 0a20 2020 2023 6966  h=True)..    #if
+000242c0: 2074 6869 7320 7370 6563 6965 7320 7368   this species sh
+000242d0: 6f75 6c64 2068 6176 6520 6765 6e6f 6d65  ould have genome
+000242e0: 732c 2063 7265 6174 6520 7468 6520 6765  s, create the ge
+000242f0: 6e6f 6d69 6320 6172 6368 6974 6563 7475  nomic architectu
+00024300: 7265 0a20 2020 2069 6620 2767 656e 5f61  re.    if 'gen_a
+00024310: 7263 6827 2069 6e20 7370 705f 7061 7261  rch' in spp_para
+00024320: 6d73 2e6b 6579 7328 293a 0a20 2020 2020  ms.keys():.     
+00024330: 2020 2023 2070 7269 6e74 2076 6572 626f     # print verbo
+00024340: 7365 206f 7574 7075 740a 2020 2020 2020  se output.      
+00024350: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+00024360: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00024370: 275c 745c 745c 746d 616b 696e 6720 6765  '\t\t\tmaking ge
+00024380: 6e6f 6d69 6320 6172 6368 6974 6563 7475  nomic architectu
+00024390: 7265 2e2e 2e5c 6e27 2c20 666c 7573 683d  re...\n', flush=
+000243a0: 5472 7565 290a 2020 2020 2020 2020 675f  True).        g_
+000243b0: 7061 7261 6d73 203d 2073 7070 5f70 6172  params = spp_par
+000243c0: 616d 732e 6765 6e5f 6172 6368 0a20 2020  ams.gen_arch.   
+000243d0: 2020 2020 2023 6d61 6b65 2067 656e 6f6d       #make genom
+000243e0: 6963 5f61 7263 6869 7465 6374 7572 650a  ic_architecture.
+000243f0: 2020 2020 2020 2020 6765 6e5f 6172 6368          gen_arch
+00024400: 203d 205f 6d61 6b65 5f67 656e 6f6d 6963   = _make_genomic
+00024410: 5f61 7263 6869 7465 6374 7572 6528 7370  _architecture(sp
+00024420: 705f 7061 7261 6d73 203d 2073 7070 5f70  p_params = spp_p
+00024430: 6172 616d 732c 0a20 2020 2020 2020 2020  arams,.         
+00024440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024470: 2020 2020 2020 206c 616e 6420 3d20 6c61         land = la
+00024480: 6e64 290a 2020 2020 656c 7365 3a0a 2020  nd).    else:.  
+00024490: 2020 2020 2020 6765 6e5f 6172 6368 203d        gen_arch =
+000244a0: 204e 6f6e 650a 0a20 2020 2023 2070 7269   None..    # pri
+000244b0: 6e74 2076 6572 626f 7365 206f 7574 7075  nt verbose outpu
+000244c0: 740a 2020 2020 6966 2076 6572 626f 7365  t.    if verbose
+000244d0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+000244e0: 275c 745c 745c 746d 616b 696e 6720 696e  '\t\t\tmaking in
+000244f0: 6469 7669 6475 616c 732e 2e2e 5c6e 272c  dividuals...\n',
+00024500: 2066 6c75 7368 3d54 7275 6529 0a20 2020   flush=True).   
+00024510: 2023 6d61 6b65 2069 6e64 6976 6964 730a   #make individs.
+00024520: 2020 2020 4e20 3d20 696e 6974 5f70 6172      N = init_par
+00024530: 616d 732e 706f 7028 274e 2729 0a20 2020  ams.pop('N').   
+00024540: 2023 6372 6561 7465 2061 6e20 6f72 6465   #create an orde
+00024550: 7265 6420 6469 6374 696f 6e61 7279 2074  red dictionary t
+00024560: 6f20 686f 6c64 2074 6865 2069 6e64 6976  o hold the indiv
+00024570: 6964 7561 6c73 2c20 616e 6420 6669 6c6c  iduals, and fill
+00024580: 2069 7420 7570 0a20 2020 2069 6e64 7320   it up.    inds 
+00024590: 3d20 4f44 2829 0a20 2020 2066 6f72 2069  = OD().    for i
+000245a0: 6e64 5f69 6478 2069 6e20 7261 6e67 6528  nd_idx in range(
+000245b0: 4e29 3a0a 2020 2020 2020 2020 2320 7573  N):.        # us
+000245c0: 6520 696e 6469 7669 6475 616c 2e63 7265  e individual.cre
+000245d0: 6174 655f 696e 6469 7669 6475 616c 2074  ate_individual t
+000245e0: 6f20 7369 6d75 6c61 7465 2069 6e64 6976  o simulate indiv
+000245f0: 6964 7561 6c73 0a20 2020 2020 2020 2023  iduals.        #
+00024600: 616e 6420 6164 6420 7468 656d 2074 6f20  and add them to 
+00024610: 7468 6520 7370 6563 6965 730a 2020 2020  the species.    
+00024620: 2020 2020 696e 6420 3d20 5f6d 616b 655f      ind = _make_
+00024630: 696e 6469 7669 6475 616c 2869 6478 3d69  individual(idx=i
+00024640: 6e64 5f69 6478 2c20 6f66 6673 7072 696e  nd_idx, offsprin
+00024650: 673d 4661 6c73 652c 0a20 2020 2020 2020  g=False,.       
+00024660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024670: 2020 2020 2020 2020 6469 6d3d 6c61 6e64          dim=land
+00024680: 2e64 696d 2c20 6765 6e6f 6d69 635f 6172  .dim, genomic_ar
+00024690: 6368 6974 6563 7475 7265 3d67 656e 5f61  chitecture=gen_a
+000246a0: 7263 682c 0a20 2020 2020 2020 2020 2020  rch,.           
+000246b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246c0: 2020 2020 6275 726e 3d62 7572 6e29 0a20      burn=burn). 
+000246d0: 2020 2020 2020 2069 6e64 735b 696e 645f         inds[ind_
+000246e0: 6964 785d 203d 2069 6e64 0a0a 2020 2020  idx] = ind..    
+000246f0: 2363 7265 6174 6520 7468 6520 7370 6563  #create the spec
+00024700: 6965 7320 6672 6f6d 2074 686f 7365 2069  ies from those i
+00024710: 6e64 6976 6964 7561 6c73 0a20 2020 2073  ndividuals.    s
+00024720: 7070 203d 2053 7065 6369 6573 286e 616d  pp = Species(nam
+00024730: 6520 3d20 6e61 6d65 2c20 6964 7820 3d20  e = name, idx = 
+00024740: 6964 782c 2069 6e64 7320 3d20 696e 6473  idx, inds = inds
+00024750: 2c20 6c61 6e64 203d 206c 616e 642c 0a20  , land = land,. 
+00024760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024770: 2020 2020 7370 705f 7061 7261 6d73 203d      spp_params =
+00024780: 2073 7070 5f70 6172 616d 732c 2067 656e   spp_params, gen
+00024790: 6f6d 6963 5f61 7263 6869 7465 6374 7572  omic_architectur
+000247a0: 653d 6765 6e5f 6172 6368 290a 0a20 2020  e=gen_arch)..   
+000247b0: 2023 7573 6520 7468 6520 7265 6d61 696e   #use the remain
+000247c0: 696e 6720 696e 6974 5f70 6172 616d 7320  ing init_params 
+000247d0: 746f 2073 6574 2074 6865 2063 6172 7279  to set the carry
+000247e0: 696e 672d 6361 7061 6369 7479 2072 6173  ing-capacity ras
+000247f0: 7465 7220 284b 290a 2020 2020 5f6d 616b  ter (K).    _mak
+00024800: 655f 4b28 7370 702c 206c 616e 642c 202a  e_K(spp, land, *
+00024810: 2a7b 6b3a 7620 666f 7220 6b2c 7620 696e  *{k:v for k,v in
+00024820: 2069 6e69 745f 7061 7261 6d73 2e69 7465   init_params.ite
+00024830: 6d73 2829 2069 6620 6b20 213d 2027 6d73  ms() if k != 'ms
+00024840: 7072 696d 6527 7d29 0a20 2020 2023 7365  prime'}).    #se
+00024850: 7420 696e 6974 6961 6c20 656e 7669 726f  t initial enviro
+00024860: 6e6d 656e 7420 7661 6c75 6573 0a20 2020  nment values.   
+00024870: 2073 7070 2e5f 7365 745f 6528 6c61 6e64   spp._set_e(land
+00024880: 290a 2020 2020 2373 6574 2069 6e69 7469  ).    #set initi
+00024890: 616c 2063 6f6f 7264 7320 616e 6420 6365  al coords and ce
+000248a0: 6c6c 730a 2020 2020 7370 702e 5f73 6574  lls.    spp._set
+000248b0: 5f63 6f6f 7264 735f 616e 645f 6365 6c6c  _coords_and_cell
+000248c0: 7328 290a 2020 2020 2373 6574 2074 6865  s().    #set the
+000248d0: 206b 645f 7472 6565 0a20 2020 2073 7070   kd_tree.    spp
+000248e0: 2e5f 7365 745f 6b64 5f74 7265 6528 290a  ._set_kd_tree().
+000248f0: 0a20 2020 2023 7365 7420 7068 656e 6f74  .    #set phenot
+00024900: 7970 6573 2c20 6966 2074 6865 2073 7065  ypes, if the spe
+00024910: 6369 6573 2068 6173 2067 656e 6f6d 6573  cies has genomes
+00024920: 0a20 2020 2069 6620 7370 702e 6765 6e5f  .    if spp.gen_
+00024930: 6172 6368 2069 7320 6e6f 7420 4e6f 6e65  arch is not None
+00024940: 2061 6e64 206e 6f74 2062 7572 6e3a 0a20   and not burn:. 
+00024950: 2020 2020 2020 205b 696e 642e 5f73 6574         [ind._set
+00024960: 5f7a 2873 7070 2e67 656e 5f61 7263 6829  _z(spp.gen_arch)
+00024970: 2066 6f72 2069 6e64 2069 6e20 7370 702e   for ind in spp.
+00024980: 7661 6c75 6573 2829 5d0a 0a20 2020 2023  values()]..    #
+00024990: 6d61 6b65 2064 656e 7369 7479 5f67 7269  make density_gri
+000249a0: 640a 2020 2020 7370 702e 5f73 6574 5f64  d.    spp._set_d
+000249b0: 656e 735f 6772 6964 7328 6c61 6e64 290a  ens_grids(land).
+000249c0: 0a20 2020 2023 6d61 6b65 206d 6f76 656d  .    #make movem
+000249d0: 656e 7420 7375 7266 6163 652c 2069 6620  ent surface, if 
+000249e0: 6e65 6564 6564 0a20 2020 2069 6620 7370  needed.    if sp
+000249f0: 702e 5f6d 6f76 653a 0a20 2020 2020 2020  p._move:.       
+00024a00: 2069 6620 276d 6f76 655f 7375 7266 2720   if 'move_surf' 
+00024a10: 696e 2073 7070 5f70 6172 616d 732e 6d6f  in spp_params.mo
+00024a20: 7665 6d65 6e74 2e6b 6579 7328 293a 0a20  vement.keys():. 
+00024a30: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
+00024a40: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
+00024a50: 2020 2020 2020 2070 7269 6e74 2828 275c         print(('\
+00024a60: 745c 745c 746d 616b 696e 6720 6d6f 7665  t\t\tmaking move
+00024a70: 6d65 6e74 2073 7572 6661 6365 2e2e 2e5c  ment surface...\
+00024a80: 6e27 0a20 2020 2020 2020 2020 2020 2020  n'.             
+00024a90: 2020 2020 2020 2020 2020 275c 745c 745c            '\t\t\
+00024aa0: 745c 745b 6361 6e20 7461 6b65 2061 2062  t\t[can take a b
+00024ab0: 6974 5d5c 6e27 292c 2066 6c75 7368 3d54  it]\n'), flush=T
+00024ac0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00024ad0: 206d 735f 7061 7261 6d73 203d 2064 6565   ms_params = dee
+00024ae0: 7063 6f70 7928 7370 705f 7061 7261 6d73  pcopy(spp_params
+00024af0: 2e6d 6f76 656d 656e 742e 6d6f 7665 5f73  .movement.move_s
+00024b00: 7572 6629 0a20 2020 2020 2020 2020 2020  urf).           
+00024b10: 2023 6772 6162 2074 6865 206c 7972 206e   #grab the lyr n
+00024b20: 756d 6265 7220 666f 7220 7468 6520 6c79  umber for the ly
+00024b30: 7220 7468 6174 2074 6865 200a 2020 2020  r that the .    
+00024b40: 2020 2020 2020 2020 236d 6f76 656d 656e          #movemen
+00024b50: 7420 7375 7266 6163 6520 6973 2074 6f20  t surface is to 
+00024b60: 6265 2062 6173 6564 206f 6e0a 2020 2020  be based on.    
+00024b70: 2020 2020 2020 2020 6d6f 7665 5f73 7572          move_sur
+00024b80: 665f 6c79 7220 3d20 6d73 5f70 6172 616d  f_lyr = ms_param
+00024b90: 732e 706f 7028 276c 6179 6572 2729 0a20  s.pop('layer'). 
+00024ba0: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
+00024bb0: 7375 7266 5f6c 7972 5f6e 756d 203d 205b  surf_lyr_num = [
+00024bc0: 6b20 666f 7220 6b2c 7620 696e 206c 616e  k for k,v in lan
+00024bd0: 642e 6974 656d 7328 0a20 2020 2020 2020  d.items(.       
+00024be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024c00: 2020 2020 2029 2069 6620 762e 6e61 6d65       ) if v.name
+00024c10: 203d 3d20 6d6f 7665 5f73 7572 665f 6c79   == move_surf_ly
+00024c20: 725d 0a20 2020 2020 2020 2020 2020 2061  r].            a
+00024c30: 7373 6572 7420 6c65 6e28 6d6f 7665 5f73  ssert len(move_s
+00024c40: 7572 665f 6c79 725f 6e75 6d29 203d 3d20  urf_lyr_num) == 
+00024c50: 312c 2028 2245 7870 6563 7465 6420 746f  1, ("Expected to
+00024c60: 2066 696e 6420 6f6e 6c79 2061 2022 0a20   find only a ". 
+00024c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00024c80: 7369 6e67 6c65 204c 6179 6572 2077 6974  single Layer wit
+00024c90: 6820 7468 6520 6e61 6d65 2070 726f 7669  h the name provi
+00024ca0: 6465 6420 666f 7220 7468 6520 220a 2020  ded for the ".  
+00024cb0: 2020 2020 2020 2020 2020 2020 2020 225f                "_
+00024cc0: 436f 6e64 7563 7461 6e63 6553 7572 6661  ConductanceSurfa
+00024cd0: 6365 2c22 0a20 2020 2020 2020 2020 2020  ce,".           
+00024ce0: 2020 2020 2022 2062 7574 2069 6e73 7465       " but inste
+00024cf0: 6164 2066 6f75 6e64 2025 6922 2920 2520  ad found %i") % 
+00024d00: 6c65 6e28 6d6f 7665 5f73 7572 665f 6c79  len(move_surf_ly
+00024d10: 725f 6e75 6d29 0a20 2020 2020 2020 2020  r_num).         
+00024d20: 2020 206d 6f76 655f 7375 7266 5f6c 7972     move_surf_lyr
+00024d30: 5f6e 756d 203d 206d 6f76 655f 7375 7266  _num = move_surf
+00024d40: 5f6c 7972 5f6e 756d 5b30 5d0a 2020 2020  _lyr_num[0].    
+00024d50: 2020 2020 2020 2020 236d 616b 6520 7468          #make th
+00024d60: 6520 6d6f 7665 6d65 6e74 2073 7572 6661  e movement surfa
+00024d70: 6365 2061 6e64 2073 6574 2069 7420 6173  ce and set it as
+00024d80: 2074 6865 2073 7070 2773 0a20 2020 2020   the spp's.     
+00024d90: 2020 2020 2020 2023 6d6f 7665 5f73 7572         #move_sur
+00024da0: 6620 6174 7472 6962 7574 650a 2020 2020  f attribute.    
+00024db0: 2020 2020 2020 2020 7370 702e 5f6d 6f76          spp._mov
+00024dc0: 655f 7375 7266 3d20 7370 742e 5f43 6f6e  e_surf= spt._Con
+00024dd0: 6475 6374 616e 6365 5375 7266 6163 6528  ductanceSurface(
+00024de0: 6c61 6e64 5b6d 6f76 655f 7375 7266 5f6c  land[move_surf_l
+00024df0: 7972 5f6e 756d 5d2c 0a20 2020 2020 2020  yr_num],.       
+00024e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e30: 2020 2020 2020 2020 202a 2a6d 735f 7061           **ms_pa
+00024e40: 7261 6d73 290a 2020 2020 236d 616b 6520  rams).    #make 
+00024e50: 6469 7370 6572 7361 6c20 7375 7266 6163  dispersal surfac
+00024e60: 652c 2069 6620 6e65 6564 6564 0a20 2020  e, if needed.   
+00024e70: 2069 6620 2764 6973 705f 7375 7266 2720   if 'disp_surf' 
+00024e80: 696e 2073 7070 5f70 6172 616d 732e 6d6f  in spp_params.mo
+00024e90: 7665 6d65 6e74 2e6b 6579 7328 293a 0a20  vement.keys():. 
+00024ea0: 2020 2020 2020 2023 2070 7269 6e74 2076         # print v
+00024eb0: 6572 626f 7365 206f 7574 7075 740a 2020  erbose output.  
+00024ec0: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00024ed0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00024ee0: 696e 7428 2827 5c74 5c74 5c74 6d61 6b69  int(('\t\t\tmaki
+00024ef0: 6e67 2064 6973 7065 7273 616c 2073 7572  ng dispersal sur
+00024f00: 6661 6365 2e2e 2e5c 6e27 0a20 2020 2020  face...\n'.     
+00024f10: 2020 2020 2020 2020 2020 2020 2020 275c                '\
+00024f20: 745c 745c 745c 745b 6361 6e20 7461 6b65  t\t\t\t[can take
+00024f30: 2061 2062 6974 5d5c 6e27 292c 2066 6c75   a bit]\n'), flu
+00024f40: 7368 3d54 7275 6529 0a20 2020 2020 2020  sh=True).       
+00024f50: 2064 735f 7061 7261 6d73 203d 2064 6565   ds_params = dee
+00024f60: 7063 6f70 7928 7370 705f 7061 7261 6d73  pcopy(spp_params
+00024f70: 2e6d 6f76 656d 656e 742e 6469 7370 5f73  .movement.disp_s
+00024f80: 7572 6629 0a20 2020 2020 2020 2023 6772  urf).        #gr
+00024f90: 6162 2074 6865 206c 7972 206e 756d 6265  ab the lyr numbe
+00024fa0: 7220 666f 7220 7468 6520 6c79 7220 7468  r for the lyr th
+00024fb0: 6174 2074 6865 200a 2020 2020 2020 2020  at the .        
+00024fc0: 2364 6973 7065 7273 616c 2073 7572 6661  #dispersal surfa
+00024fd0: 6365 2069 7320 746f 2062 6520 6261 7365  ce is to be base
+00024fe0: 6420 6f6e 0a20 2020 2020 2020 2064 6973  d on.        dis
+00024ff0: 705f 7375 7266 5f6c 7972 203d 2064 735f  p_surf_lyr = ds_
+00025000: 7061 7261 6d73 2e70 6f70 2827 6c61 7965  params.pop('laye
+00025010: 7227 290a 2020 2020 2020 2020 6469 7370  r').        disp
+00025020: 5f73 7572 665f 6c79 725f 6e75 6d20 3d20  _surf_lyr_num = 
+00025030: 5b6b 2066 6f72 206b 2c76 2069 6e20 6c61  [k for k,v in la
+00025040: 6e64 2e69 7465 6d73 280a 2020 2020 2020  nd.items(.      
+00025050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025070: 2020 2920 6966 2076 2e6e 616d 6520 3d3d    ) if v.name ==
+00025080: 2064 6973 705f 7375 7266 5f6c 7972 5d0a   disp_surf_lyr].
+00025090: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+000250a0: 656e 2864 6973 705f 7375 7266 5f6c 7972  en(disp_surf_lyr
+000250b0: 5f6e 756d 2920 3d3d 2031 2c20 2822 4578  _num) == 1, ("Ex
+000250c0: 7065 6374 6564 2074 6f20 6669 6e64 206f  pected to find o
+000250d0: 6e6c 7920 6120 220a 2020 2020 2020 2020  nly a ".        
+000250e0: 2020 2020 2273 696e 676c 6520 4c61 7965      "single Laye
+000250f0: 7220 7769 7468 2074 6865 206e 616d 6520  r with the name 
+00025100: 7072 6f76 6964 6564 2066 6f72 2074 6865  provided for the
+00025110: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+00025120: 5f43 6f6e 6475 6374 616e 6365 5375 7266  _ConductanceSurf
+00025130: 6163 652c 2022 0a20 2020 2020 2020 2020  ace, ".         
+00025140: 2020 2022 6275 7420 696e 7374 6561 6420     "but instead 
+00025150: 666f 756e 6420 2569 2229 2025 206c 656e  found %i") % len
+00025160: 2864 6973 705f 7375 7266 5f6c 7972 5f6e  (disp_surf_lyr_n
+00025170: 756d 290a 2020 2020 2020 2020 6469 7370  um).        disp
+00025180: 5f73 7572 665f 6c79 725f 6e75 6d20 3d20  _surf_lyr_num = 
+00025190: 6469 7370 5f73 7572 665f 6c79 725f 6e75  disp_surf_lyr_nu
+000251a0: 6d5b 305d 0a20 2020 2020 2020 2023 6d61  m[0].        #ma
+000251b0: 6b65 2074 6865 2064 6973 7065 7273 616c  ke the dispersal
+000251c0: 2073 7572 6661 6365 2061 6e64 2073 6574   surface and set
+000251d0: 2069 7420 6173 2074 6865 2073 7070 2773   it as the spp's
+000251e0: 0a20 2020 2020 2020 2023 6469 7370 5f73  .        #disp_s
+000251f0: 7572 6620 6174 7472 6962 7574 650a 2020  urf attribute.  
+00025200: 2020 2020 2020 7370 702e 5f64 6973 705f        spp._disp_
+00025210: 7375 7266 203d 2073 7074 2e5f 436f 6e64  surf = spt._Cond
+00025220: 7563 7461 6e63 6553 7572 6661 6365 286c  uctanceSurface(l
+00025230: 616e 645b 6469 7370 5f73 7572 665f 6c79  and[disp_surf_ly
+00025240: 725f 6e75 6d5d 2c0a 2020 2020 2020 2020  r_num],.        
+00025250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025280: 2020 2020 2020 2020 2a2a 6473 5f70 6172          **ds_par
+00025290: 616d 7329 0a0a 2020 2020 2369 6620 7468  ams)..    #if th
+000252a0: 6973 2073 7065 6369 6573 2068 6173 2063  is species has c
+000252b0: 6861 6e67 6573 2070 6172 616d 6574 6572  hanges parameter
+000252c0: 697a 6564 2c20 6f72 2069 6620 6e6f 7420  ized, or if not 
+000252d0: 6275 7420 6974 2068 6173 0a20 2020 2023  but it has.    #
+000252e0: 6569 7468 6572 2061 204d 6f76 656d 656e  either a Movemen
+000252f0: 7453 7572 6620 6f72 2061 2044 6973 7065  tSurf or a Dispe
+00025300: 7273 616c 5375 7266 2062 6173 6564 206f  rsalSurf based o
+00025310: 6e20 6120 4c61 7965 7220 7468 6174 0a20  n a Layer that. 
+00025320: 2020 2023 7769 6c6c 2075 6e64 6572 676f     #will undergo
+00025330: 206c 616e 6473 6361 7065 2063 6861 6e67   landscape chang
+00025340: 652c 2074 6865 6e20 6372 6561 7465 2061  e, then create a
+00025350: 205f 5370 6563 6965 7343 6861 6e67 6572   _SpeciesChanger
+00025360: 206f 626a 6563 7420 666f 7220 6974 0a20   object for it. 
+00025370: 2020 2069 6620 2827 6368 616e 6765 2720     if ('change' 
+00025380: 696e 2073 7070 5f70 6172 616d 732e 6b65  in spp_params.ke
+00025390: 7973 2829 0a20 2020 2020 2020 206f 7220  ys().        or 
+000253a0: 2873 7070 2e5f 6d6f 7665 5f73 7572 6620  (spp._move_surf 
+000253b0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+000253c0: 2020 2020 616e 6420 6c61 6e64 2e5f 6368      and land._ch
+000253d0: 616e 6765 7220 6973 206e 6f74 204e 6f6e  anger is not Non
+000253e0: 650a 2020 2020 2020 2020 616e 6420 7370  e.        and sp
+000253f0: 702e 5f6d 6f76 655f 7375 7266 2e6c 7972  p._move_surf.lyr
+00025400: 5f6e 756d 2069 6e20 6c61 6e64 2e5f 6368  _num in land._ch
+00025410: 616e 6765 722e 6368 616e 6765 5f69 6e66  anger.change_inf
+00025420: 6f2e 6b65 7973 2829 290a 2020 2020 2020  o.keys()).      
+00025430: 2020 6f72 2028 7370 702e 5f64 6973 705f    or (spp._disp_
+00025440: 7375 7266 2069 7320 6e6f 7420 4e6f 6e65  surf is not None
+00025450: 0a20 2020 2020 2020 2061 6e64 206c 616e  .        and lan
+00025460: 642e 5f63 6861 6e67 6572 2069 7320 6e6f  d._changer is no
+00025470: 7420 4e6f 6e65 0a20 2020 2020 2020 2061  t None.        a
+00025480: 6e64 2073 7070 2e5f 6469 7370 5f73 7572  nd spp._disp_sur
+00025490: 662e 6c79 725f 6e75 6d20 696e 206c 616e  f.lyr_num in lan
+000254a0: 642e 5f63 6861 6e67 6572 2e63 6861 6e67  d._changer.chang
+000254b0: 655f 696e 666f 2e6b 6579 7328 2929 293a  e_info.keys())):
+000254c0: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
+000254d0: 2076 6572 626f 7365 206f 7574 7075 740a   verbose output.
+000254e0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+000254f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00025500: 7072 696e 7428 2827 5c74 5c74 5c74 7365  print(('\t\t\tse
+00025510: 7474 696e 6720 7570 2073 7065 6369 6573  tting up species
+00025520: 2063 6861 6e67 6573 2e2e 2e5c 6e27 0a20   changes...\n'. 
+00025530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025540: 2020 275c 745c 745c 745c 745b 6361 6e20    '\t\t\t\t[can 
+00025550: 7461 6b65 2061 2077 6869 6c65 2c5c 6e5c  take a while,\n\
+00025560: 745c 745c 745c 7420 6966 206d 6f76 656d  t\t\t\t if movem
+00025570: 656e 7420 6f72 2027 0a20 2020 2020 2020  ent or '.       
+00025580: 2020 2020 2020 2020 2020 2020 2764 6973              'dis
+00025590: 7065 7273 616c 5c6e 5c74 5c74 5c74 5c74  persal\n\t\t\t\t
+000255a0: 2073 7572 6661 6365 7320 7769 6c6c 2063   surfaces will c
+000255b0: 6861 6e67 655d 5c6e 2729 2c20 666c 7573  hange]\n'), flus
+000255c0: 683d 5472 7565 290a 2020 2020 2020 2020  h=True).        
+000255d0: 2367 7261 6220 7468 6520 6368 616e 6765  #grab the change
+000255e0: 2070 6172 616d 7320 286f 7220 4e6f 6e65   params (or None
+000255f0: 2c20 6966 0a20 2020 2020 2020 2069 6620  , if.        if 
+00025600: 2763 6861 6e67 6527 2069 6e20 7370 705f  'change' in spp_
+00025610: 7061 7261 6d73 2e6b 6579 7328 293a 0a20  params.keys():. 
+00025620: 2020 2020 2020 2020 2020 2063 685f 7061             ch_pa
+00025630: 7261 6d73 203d 2073 7070 5f70 6172 616d  rams = spp_param
+00025640: 732e 6368 616e 6765 0a20 2020 2020 2020  s.change.       
+00025650: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00025660: 2020 2063 685f 7061 7261 6d73 203d 204e     ch_params = N
+00025670: 6f6e 650a 2020 2020 2020 2020 236d 616b  one.        #mak
+00025680: 6520 5f53 7065 6369 6573 4368 616e 6765  e _SpeciesChange
+00025690: 7220 616e 6420 7365 7420 6974 2074 6f20  r and set it to 
+000256a0: 7468 6520 7370 7027 7320 6368 616e 6765  the spp's change
+000256b0: 7220 6174 7472 6962 7574 650a 2020 2020  r attribute.    
+000256c0: 2020 2020 7370 702e 5f63 6861 6e67 6572      spp._changer
+000256d0: 203d 205f 5370 6563 6965 7343 6861 6e67   = _SpeciesChang
+000256e0: 6572 2873 7070 2c20 6368 5f70 6172 616d  er(spp, ch_param
+000256f0: 732c 206c 616e 6420 3d20 6c61 6e64 290a  s, land = land).
+00025700: 0a20 2020 2072 6574 7572 6e20 7370 700a  .    return spp.
+00025710: 0a0a 2320 6675 6e63 7469 6f6e 2066 6f72  ..# function for
+00025720: 2072 6561 6469 6e67 2069 6e20 6120 7069   reading in a pi
+00025730: 636b 6c65 6420 7370 700a 6465 6620 7265  ckled spp.def re
+00025740: 6164 5f70 6963 6b6c 6564 5f73 7070 2866  ad_pickled_spp(f
+00025750: 696c 656e 616d 6529 3a0a 2020 2020 696d  ilename):.    im
+00025760: 706f 7274 2063 5069 636b 6c65 0a20 2020  port cPickle.   
+00025770: 2077 6974 6820 6f70 656e 2866 696c 656e   with open(filen
+00025780: 616d 652c 2027 7262 2729 2061 7320 663a  ame, 'rb') as f:
+00025790: 0a20 2020 2020 2020 2073 7070 203d 2063  .        spp = c
+000257a0: 5069 636b 6c65 2e6c 6f61 6428 6629 0a20  Pickle.load(f). 
+000257b0: 2020 2072 6574 7572 6e20 7370 700a 0a0a     return spp...
```

### Comparing `geonomics-1.4.1/geonomics/utils/_str_repr_.py` & `geonomics-1.4.2/geonomics/utils/_str_repr_.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/utils/io.py` & `geonomics-1.4.2/geonomics/utils/io.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/utils/spatial.py` & `geonomics-1.4.2/geonomics/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics/utils/viz.py` & `geonomics-1.4.2/geonomics/utils/viz.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/geonomics.egg-info/PKG-INFO` & `geonomics-1.4.2/geonomics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.4.1.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.4.2.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
+Project-URL: Methods Paper, https://doi.org/10.1093/molbev/msab175
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

### Comparing `geonomics-1.4.1/geonomics.egg-info/SOURCES.txt` & `geonomics-1.4.2/geonomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.1/setup.py` & `geonomics-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,17 +48,16 @@
         'Topic :: Scientific/Engineering :: Bio-Informatics'
     ],
     keywords=('landscape genomics genetics ecology evolution simulation model '
               'environmental model agent-based'),
     project_urls={
         'Documentation': ('https://htmlpreview.github.io/?https://github.com/'
                           'drewhart/geonomics/blob/master/doc/built/doc.html'),
-        # 'Methods Paper': 'PAPER URL HERE!',
+        'Methods Paper': 'https://doi.org/10.1093/molbev/msab175',
         'Source': 'https://github.com/drewhart/geonomics',
-        # 'Tracker': 'BUGTRACKERSITHERE',
     },
 #    install_requires=['numpy', 'matplotlib>=3.0.0', 'pandas>=0.23.4', 'geopandas',
 #                      'scipy>=1.3.1', 'scikit-learn', 'statsmodels>=0.9.0',
 #                      'shapely', 'bitarray', 'rasterio',
 #                      'msprime>=0.7.4', 'tskit>=0.2.3'],
     extras_require={'simulation on neutral landscape models': ['nlmpy'],
                    '3d plots for Yosemite demo': ['pykrige']},
```

