# Comparing `tmp/naluconfigs-13.8.2.tar.gz` & `tmp/naluconfigs-13.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-13.8.2.tar", last modified: Mon Apr 22 05:21:11 2024, max compression
+gzip compressed data, was "naluconfigs-13.8.3.tar", last modified: Wed May 22 20:34:20 2024, max compression
```

## Comparing `naluconfigs-13.8.2.tar` & `naluconfigs-13.8.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.634337 naluconfigs-13.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-22 05:21:11.634337 naluconfigs-13.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 05:21:11.634337 naluconfigs-13.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.618337 naluconfigs-13.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.618337 naluconfigs-13.8.2/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.618337 naluconfigs-13.8.2/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.622337 naluconfigs-13.8.2/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    51581 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15092 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.626337 naluconfigs-13.8.2/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.630337 naluconfigs-13.8.2/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/asocv3s.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (127)    32887 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.634337 naluconfigs-13.8.2/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-22 05:21:11.000000 naluconfigs-13.8.2/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-22 05:21:11.000000 naluconfigs-13.8.2/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:21:11.000000 naluconfigs-13.8.2/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 05:21:11.000000 naluconfigs-13.8.2/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 05:21:11.000000 naluconfigs-13.8.2/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:21:11.634337 naluconfigs-13.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-22 05:20:56.000000 naluconfigs-13.8.2/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.725114 naluconfigs-13.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.729114 naluconfigs-13.8.3/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.725114 naluconfigs-13.8.3/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.733114 naluconfigs-13.8.3/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    51581 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.737114 naluconfigs-13.8.3/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3s.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20010 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32887 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_range_keys.py
```

### Comparing `naluconfigs-13.8.2/PKG-INFO` & `naluconfigs-13.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 13.8.2
+Version: 13.8.3
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-13.8.2/README.md` & `naluconfigs-13.8.3/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/pyproject.toml` & `naluconfigs-13.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/setup.py` & `naluconfigs-13.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/__init__.py` & `naluconfigs-13.8.3/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/_constructors.py` & `naluconfigs-13.8.3/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/aardvarcv4.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/hiper.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/hiper.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 params:
-  channels: 56
+  channels: 4
   name: hiper
   readable_name: HIPER
   resolution: 12
   samples: 64
   windows: 64
 registers:
   analog_registers:
@@ -480,21 +480,21 @@
     enabletestpatt:
       address: 0x88
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    # excludechan:  # TODO: New register, verify address and value
-    #   address: 0x96
-    #   bitposition: 0
-    #   bitwidth: 4
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
+    excludechannelmask:  # TODO: New register, verify address and value
+      address: 0x96
+      bitposition: 0
+      bitwidth: 4
+      description: ''
+      readwrite: rw
+      value: 0
     loadwait:
       address: 0x8B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
```

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/asocv3s.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3s.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 model: hiper
 features:
   adc2mv: false
   dac_sweep: false
-  ext_dac: false
+  ext_dac: true
   pedestals: true
   threshold_scan: false
   tia_dac: false
   timing_calibration: false
   naludaq_rs: false
 params:
+  uart:
+    tx_pause: 0.01
+    bundle: true
   chanmask: 3072
   channels: 56
   chanshift: 10
   chips:
-    0:
+    0..13:
       !include_chip
       from: hiper::params
   num_chips: 14
   installed_chips: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]
   clock_file: Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
   connections:
     - serial
@@ -29,15 +32,15 @@
   default_clock: 100000000.0
   default_divider: 33
   default_trigger_value: 1500
   ext_dac:
     max_mv: 1200
     max_counts: 4095
     channels:
-      0..55: 0
+      0..55: 2730
     side_mapping: # asic channel: dac side (0 = left, 1 = right)
       0..27: 0
       28..55: 1
     chip_mapping: # asic channel: dac chip number
       0..3: 0
       4..7: 1
       8..11: 2
@@ -50,17 +53,17 @@
       36..39: 2
       40..43: 3
       44..47: 4
       48..51: 5
       52..55: 6
     channel_mapping: # asic channel: ext. dac channel
       0, 4, 8, 12, 16, 20, 24, 28, 32, 36, 40, 44, 48, 52: 0
-      1, 5, 9, 13, 17, 21, 25, 29, 33, 37, 41, 45, 49, 53: 1
-      2, 6, 10, 14, 18, 22, 26, 30, 34, 38, 42, 46, 50, 54: 2
-      3, 7, 11, 15, 19, 23, 27, 31, 35, 39, 43, 47, 51, 55: 3
+      1, 5, 9, 13, 17, 21, 25, 29, 33, 37, 41, 45, 49, 53: 6
+      2, 6, 10, 14, 18, 22, 26, 30, 34, 38, 42, 46, 50, 54: 3
+      3, 7, 11, 15, 19, 23, 27, 31, 35, 39, 43, 47, 51, 55: 4
   headers: 3
   numregs: 64
   pedestals_blocks: 16
   peripherals:
     current:
       chan: 0
       addr: 0xD0
@@ -91,23 +94,25 @@
   wbias: 2000
   windmask: 1022
   windows: 64
 registers:
   analog_registers:
     !include_registers
       from: hiper::registers::analog_registers
+      value_count: 14
       override:
         isel:
           value: [3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000, 3000]
   digital_registers:
     !include_registers
       from: hiper::registers::digital_registers
-      override:
-        txspeed:
-          value: 0
+      value_count: 14
+      # override:
+        # txspeed:
+          # value: 0
   control_registers:
     1v2_en:
       address: 0x17
       bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
```

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-13.8.3/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/exceptions.py` & `naluconfigs-13.8.3/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/helpers.py` & `naluconfigs-13.8.3/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs/postprocess.py` & `naluconfigs-13.8.3/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-13.8.3/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 13.8.2
+Version: 13.8.3
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-13.8.2/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-13.8.3/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/tests/test_hex_addr_converter.py` & `naluconfigs-13.8.3/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/tests/test_i2c_registers.py` & `naluconfigs-13.8.3/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/tests/test_multichip.py` & `naluconfigs-13.8.3/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/tests/test_post_processing.py` & `naluconfigs-13.8.3/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.2/tests/test_range_keys.py` & `naluconfigs-13.8.3/tests/test_range_keys.py`

 * *Files identical despite different names*

