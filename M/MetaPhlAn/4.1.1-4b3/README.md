# Comparing `tmp/MetaPhlAn-4.1.1.tar.gz` & `tmp/MetaPhlAn-4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MetaPhlAn-4.1.1.tar", last modified: Wed May 22 14:20:04 2024, max compression
+gzip compressed data, was "dist/MetaPhlAn-4b3.tar", last modified: Mon Aug 22 13:28:14 2022, max compression
```

## Comparing `MetaPhlAn-4.1.1.tar` & `MetaPhlAn-4b3.tar`

### file list

```diff
@@ -1,128 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/MetaPhlAn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3958 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/
--rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    85308 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/metaphlan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/metaphlan_databases/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/metaphlan_databases/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    35546 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/strainphlan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    18334 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/VallesColomerM_2022_Jan21_thresholds.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/VallesColomerM_2022_Nov19_thresholds.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4080 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/add_metadata_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/calculate_diversity.R
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/consensus_markers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7865 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/create_toy_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/database_controller.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9864 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/external_exec.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2249 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/extract_markers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7115 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/fix_relab_mpa4.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3342 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/merge_metaphlan_tables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4059 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/merge_vsc_tables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1581 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/metaphlan2krona.py
--rw-r--r--   0 runner    (1001) docker     (127)   640680 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJan21_CHOCOPhlAnSGB_202103.nwk
--rw-r--r--   0 runner    (1001) docker     (127)  3641218 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJan21_CHOCOPhlAnSGB_202103_SGB2GTDB.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    78261 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJan21_CHOCOPhlAnSGB_202103_size.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)  1227124 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJun23_CHOCOPhlAnSGB_202307.nwk
--rw-r--r--   0 runner    (1001) docker     (127)  4751735 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJun23_CHOCOPhlAnSGB_202307_SGB2GTDB.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   114962 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJun23_CHOCOPhlAnSGB_202307_size.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)  1227124 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJun23_CHOCOPhlAnSGB_202403.nwk
--rw-r--r--   0 runner    (1001) docker     (127)  4751735 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJun23_CHOCOPhlAnSGB_202403_SGB2GTDB.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   114918 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJun23_CHOCOPhlAnSGB_202403_size.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)  1013460 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vOct22_CHOCOPhlAnSGB_202212.nwk
--rw-r--r--   0 runner    (1001) docker     (127)  4038566 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vOct22_CHOCOPhlAnSGB_202212_SGB2GTDB.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    92432 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/mpa_vOct22_CHOCOPhlAnSGB_202212_size.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (127)   553399 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/oct22_fix_tax.tsv
--rwxr-xr-x   0 runner    (1001) docker     (127)     3039 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/parallelisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/phylophlan_controller.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10040 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/plot_bug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/plot_tree_graphlan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28646 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/pyphlan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5145 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/read_fastx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21152 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/sample2markers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4006 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/sgb_to_gtdb_profile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11834 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/strain_transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/Rfunctions.R
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_d.R
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_outliers.R
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_outliers_IQR.R
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_outliers_IQR.log.R
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_outliers_adjIQR.R
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_outliers_bootliers.R
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold.R
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold_IQR.R
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold_hnorm.R
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold_kernel.R
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold_lkernel.R
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold_lnorm.R
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/find_threshold_loglnorm.R
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/plot_allgenes.R
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/plot_pergene.R
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/plot_perspecies.R
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/R_scripts/plot_threshold.R
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/INDEX
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/Rd.rds
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/data.rds
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/demo.rds
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/features.rds
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/hsearch.rds
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/links.rds
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/nsInfo.rds
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/package.rds
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/Meta/vignette.rds
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/NAMESPACE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/R/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/R/BMS
--rw-r--r--   0 runner    (1001) docker     (127)   260660 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/R/BMS.rdb
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/R/BMS.rdx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/data/
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/data/datafls.rda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/demo/BMS.growth.R
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/doc/bmasmall.bib
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/doc/bms.R
--rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/doc/bms.Rnw
--rw-r--r--   0 runner    (1001) docker     (127)   367343 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/doc/bms.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/doc/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/help/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/help/AnIndex
--rw-r--r--   0 runner    (1001) docker     (127)   173921 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/help/BMS.rdb
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/help/BMS.rdx
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/help/aliases.rds
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/help/paths.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/html/
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/html/00Index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/Rlib/BMS/html/R.css
--rw-r--r--   0 runner    (1001) docker     (127)    18440 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/run_treeshrink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    31110 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/Tree_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57794 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/decompose_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17079 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/filemgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/filter_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12897 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/optimal_filter_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/sequence_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/tree_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/scripts/util_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/treeshrink/treeshrink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3223 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/metaphlan/utils/util_fun.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:20:04.000000 MetaPhlAn-4.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2785 2024-05-22 14:19:54.000000 MetaPhlAn-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-08-22 13:28:13.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 13:28:13.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-08-22 13:28:13.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-08-22 13:28:13.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-22 13:28:13.000000 MetaPhlAn-4b3/MetaPhlAn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4282 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/metaphlan/
+-rw-r--r--   0 runner    (1001) docker     (121)    12326 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    64412 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/metaphlan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/metaphlan/metaphlan_databases/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/metaphlan_databases/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    42509 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/strainphlan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/metaphlan/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)  3641218 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/Jan21_SGB2GTDB.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)     9590 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/VallesColomerM_2022_Nov19_thresholds.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4086 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/add_metadata_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/calculate_unifrac.R
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12264 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/external_exec.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5222 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/extract_markers.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3713 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/merge_metaphlan_tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1581 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/metaphlan2krona.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1721736 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/mpa_v30_CHOCOPhlAn_201901_species_tree.nwk
+-rw-r--r--   0 runner    (1001) docker     (121)   640680 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/mpa_v4beta_Jan21_SGB_tree.nwk
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1923 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/parallelisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10040 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/plot_bug.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6122 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/plot_tree_graphlan.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    28646 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/pyphlan.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4987 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/read_fastx.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13817 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/sample2markers.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3003 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/sgb_to_gtdb_profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11742 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/strain_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3638 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/metaphlan/utils/util_fun.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 13:28:14.000000 MetaPhlAn-4b3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2135 2022-08-22 13:28:06.000000 MetaPhlAn-4b3/setup.py
```

### Comparing `MetaPhlAn-4.1.1/MetaPhlAn.egg-info/PKG-INFO` & `MetaPhlAn-4b3/MetaPhlAn.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 Metadata-Version: 2.1
 Name: MetaPhlAn
-Version: 4.1.1
+Version: 4b3
 Summary: MetaPhlAn is a computational tool for profiling the composition of microbial communities (Bacteria, Archaea and Eukaryotes) from metagenomic shotgun sequencing data (i.e. not 16S) with species-level. With the newly added StrainPhlAn module, it is now possible to perform accurate strain-level microbial profiling.
 Home-page: http://github.com/biobakery/MetaPhlAn/
 Author: Aitor Blanco-Miguez
 Author-email: aitor.blancomiguez@unitn.it
 License: LICENSE.txt
 Description: # MetaPhlAn: Metagenomic Phylogenetic Analysis
         [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/metaphlan/README.html) [![PyPI - Downloads](https://img.shields.io/pypi/dm/metaphlan?label=MetaPhlAn%20on%20PyPi)](https://pypi.org/project/MetaPhlAn/) [![MetaPhlAn on DockerHub](https://img.shields.io/docker/pulls/biobakery/metaphlan?label=MetaPhlAn%20on%20DockerHub)](https://hub.docker.com/r/biobakery/metaphlan) [![Build MetaPhlAn package](https://github.com/biobakery/MetaPhlAn/workflows/Build%20MetaPhlAn%20package/badge.svg?branch=3.0)](https://github.com/biobakery/MetaPhlAn/actions?query=workflow%3A%22Build+MetaPhlAn+package%22)
-        
-        MetaPhlAn is a computational tool for species-level microbial profiling (bacteria, archaea, eukaryotes, and viruses) from metagenomic shotgun sequencing data. 
-        StrainPhlAn (available within MetaPhlAn) allows strain-level microbial population genomics.
-        
+        ## What's new in version 4
+        * Adoption of the species-level genome bins system (SGBs, http://segatalab.cibio.unitn.it/data/Pasolli_et_al.html)
+        * New MetaPhlAn marker genes extracted identified from ~1M microbial genomes
+        * Ability to profile 21,978 known (kSGBs) and 4,992 unknown (uSGBs) microbial species
+        * Better representation of, not only the human gut microbiome but also many other animal and ecological environments
+        * Estimation of metagenome composed by microbes not included in the database with parameter `--unclassified_estimation`
+        * Compatibility with MetaPhlAn 3 databases with parameter `--mpa3`
         -------------
         
-        ### Installation
+        ## Description
+        MetaPhlAn is a computational tool for profiling the composition of microbial communities (Bacteria, Archaea and Eukaryotes) from metagenomic shotgun sequencing data (i.e. not 16S) with species-level. With StrainPhlAn, it is possible to perform accurate strain-level microbial profiling.
+        MetaPhlAn 4 relies on ~5.1M unique clade-specific marker genes identified from ~1M microbial genomes (~236,600 references and 771,500 metagenomic assembled genomes) spanning 26,970 species-level genome bins (SGBs, http://segatalab.cibio.unitn.it/data/Pasolli_et_al.html), 4,992 of them taxonomically unidentified at the species level, allowing:
+        
+        * unambiguous taxonomic assignments;
+        * an accurate estimation of organismal relative abundance;
+        * SGB-level resolution for bacteria, archaea and eukaryotes;
+        * strain identification and tracking
+        * orders of magnitude speedups compared to existing methods.
+        * metagenomic strain-level population genomics
         
-        To install MetaPhlan through conda run:
+        If you use MetaPhlAn, please cite:
         
-        ```
-        $ conda install -c bioconda metaphlan
-        ```
+        **Extending and improving metagenomic taxonomic profiling with uncharacterized species with MetaPhlAn 4.** Aitor Blanco-Miguez, Francesco Beghini, Fabio Cumbo, Lauren J. McIver, Kelsey N. Thompson, Moreno Zolfo, Paolo Manghi, Leonard Dubois, Kun D. Huang, Andrew Maltez Thomas, Gianmarco Piccinno, Elisa Piperni, Michal Punčochář, Mireia Valles-Colomer, Adrian Tett, Francesca Giordano, Richard Davies, Jonathan Wolf, Sarah E. Berry, Tim D. Spector, Eric A. Franzosa, Edoardo Pasolli, Francesco Asnicar, Curtis Huttenhower, Nicola Segata. Preprint (2022)
         
-        For further installation instructions and alternative installation methods check the [MetaPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/MetaPhlAn-4#installation).
+        If you use StrainPhlAn, please cite the MetaPhlAn paper and the following StrainPhlAn paper:
         
-        -------------
+        [**Microbial strain-level population structure and genetic diversity from metagenomes.**](http://genome.cshlp.org/content/27/4/626.full.pdf) *Duy Tin Truong, Adrian Tett, Edoardo Pasolli, Curtis Huttenhower, & Nicola Segata*. Genome Research 27:626-638 (2017)
         
-        ### Citation
-        If you use MetaPhlAn, please cite:
         
-        [**Extending and improving metagenomic taxonomic profiling with uncharacterized species using MetaPhlAn 4.**](https://doi.org/10.1038/s41587-023-01688-w) Aitor Blanco-Miguez, Francesco Beghini, Fabio Cumbo, Lauren J. McIver, Kelsey N. Thompson, Moreno Zolfo, Paolo Manghi, Leonard Dubois, Kun D. Huang, Andrew Maltez Thomas, Gianmarco Piccinno, Elisa Piperni, Michal Punčochář, Mireia Valles-Colomer, Adrian Tett, Francesca Giordano, Richard Davies, Jonathan Wolf, Sarah E. Berry, Tim D. Spector, Eric A. Franzosa, Edoardo Pasolli, Francesco Asnicar, Curtis Huttenhower, Nicola Segata. Nature Biotechnology (2023)
-        
-        If you use StrainPhlAn, please cite the MetaPhlAn paper and the StrainPhlAn paper:
-        
-        [**Microbial strain-level population structure and genetic diversity from metagenomes.**](http://genome.cshlp.org/content/27/4/626.full.pdf) Duy Tin Truong, Adrian Tett, Edoardo Pasolli, Curtis Huttenhower, Nicola Segata. Genome Research (2017)
+        -------------
         
-        If you use the MetaPhlAn viral module, please cite the MetaPhlAn paper and the MetaPhlan viral module paper:
+        ## MetaPhlAn and StrainPhlAn tutorials and resources
         
-        [**Discovering and exploring the hidden diversity of human gut viruses using highly enriched virome samples.**](https://doi.org/10.1101/2024.02.19.580813 ) Moreno Zolfo, Andrea Silverj, Aitor Blanco-Míguez, Paolo Manghi, Omar Rota-Stabelli, Vitor Heidrich, Jordan Jensen, Sagun Maharjan, Eric Franzosa, Cristina Menni, Alessia Visconti, Federica Pinto, Matteo Ciciani, Curtis Huttenhower, Anna Cereseto, Francesco Asnicar, Hiroaki Kitano, Takuji Yamada, Nicola Segata. bioRxiv (2024)
+        In addition to the information on this page, you can refer to the following additional resources.
         
-        -------------
+        * The [MetaPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/MetaPhlAn-4).
         
-        ### Tutorials and resources
+        * The [StrainPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/StrainPhlAn-4).
         
-        * [MetaPhlan webpage](http://segatalab.cibio.unitn.it/tools/metaphlan/index.html)
-        * [MetaPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/MetaPhlAn-4)
-        * [MetaPhlan tutorial](https://github.com/biobakery/biobakery/wiki/metaphlan4)
-        * [MetaPhlan user support](https://forum.biobakery.org/c/microbial-community-profiling/metaphlan/)
-        * [MetaPhlan change log](https://github.com/biobakery/MetaPhlAn/blob/master/CHANGELOG.md)
-        * [StrainPhlAn webpage](http://segatalab.cibio.unitn.it/tools/strainphlan/index.html)
-        * [StrainPhlAn documentation](http://segatalab.cibio.unitn.it/tools/strainphlan/index.html)
-        * [StrainPhlan tutorial](https://github.com/biobakery/biobakery/wiki/strainphlan4)
-        * [StrainPhlan user support](https://forum.biobakery.org/c/microbial-community-profiling/strainphlan/)
+        * Related tools including [PanPhlAn](https://github.com/segatalab/panphlan) (and its [tutorial](https://github.com/segatalab/panphlan/wiki/Home)), [GraPhlAn](https://github.com/segatalab/graphlan) (and it [tutorial](https://github.com/biobakery/biobakery/wiki/graphlan)), [PhyloPhlAn 3](https://github.com/biobakery/phylophlan) (and its [tutorial](https://github.com/biobakery/biobakery/wiki/phylophlan)), [HUMAnN](https://github.com/biobakery/humann/) (and its [tutorial](https://github.com/biobakery/biobakery/wiki/humann2)).
         
-        #
-        MetaPhlAn and StrainPhlAn are part of the bioBakery suite. For further bioBakery tools and tutorials visit the [bioBakery wiki](https://github.com/biobakery/biobakery).
+        * The related [bioBakery workflows](https://github.com/biobakery/biobakery/wiki/biobakery_workflows)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `MetaPhlAn-4.1.1/PKG-INFO` & `MetaPhlAn-4b3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 Metadata-Version: 2.1
 Name: MetaPhlAn
-Version: 4.1.1
+Version: 4b3
 Summary: MetaPhlAn is a computational tool for profiling the composition of microbial communities (Bacteria, Archaea and Eukaryotes) from metagenomic shotgun sequencing data (i.e. not 16S) with species-level. With the newly added StrainPhlAn module, it is now possible to perform accurate strain-level microbial profiling.
 Home-page: http://github.com/biobakery/MetaPhlAn/
 Author: Aitor Blanco-Miguez
 Author-email: aitor.blancomiguez@unitn.it
 License: LICENSE.txt
 Description: # MetaPhlAn: Metagenomic Phylogenetic Analysis
         [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/metaphlan/README.html) [![PyPI - Downloads](https://img.shields.io/pypi/dm/metaphlan?label=MetaPhlAn%20on%20PyPi)](https://pypi.org/project/MetaPhlAn/) [![MetaPhlAn on DockerHub](https://img.shields.io/docker/pulls/biobakery/metaphlan?label=MetaPhlAn%20on%20DockerHub)](https://hub.docker.com/r/biobakery/metaphlan) [![Build MetaPhlAn package](https://github.com/biobakery/MetaPhlAn/workflows/Build%20MetaPhlAn%20package/badge.svg?branch=3.0)](https://github.com/biobakery/MetaPhlAn/actions?query=workflow%3A%22Build+MetaPhlAn+package%22)
-        
-        MetaPhlAn is a computational tool for species-level microbial profiling (bacteria, archaea, eukaryotes, and viruses) from metagenomic shotgun sequencing data. 
-        StrainPhlAn (available within MetaPhlAn) allows strain-level microbial population genomics.
-        
+        ## What's new in version 4
+        * Adoption of the species-level genome bins system (SGBs, http://segatalab.cibio.unitn.it/data/Pasolli_et_al.html)
+        * New MetaPhlAn marker genes extracted identified from ~1M microbial genomes
+        * Ability to profile 21,978 known (kSGBs) and 4,992 unknown (uSGBs) microbial species
+        * Better representation of, not only the human gut microbiome but also many other animal and ecological environments
+        * Estimation of metagenome composed by microbes not included in the database with parameter `--unclassified_estimation`
+        * Compatibility with MetaPhlAn 3 databases with parameter `--mpa3`
         -------------
         
-        ### Installation
+        ## Description
+        MetaPhlAn is a computational tool for profiling the composition of microbial communities (Bacteria, Archaea and Eukaryotes) from metagenomic shotgun sequencing data (i.e. not 16S) with species-level. With StrainPhlAn, it is possible to perform accurate strain-level microbial profiling.
+        MetaPhlAn 4 relies on ~5.1M unique clade-specific marker genes identified from ~1M microbial genomes (~236,600 references and 771,500 metagenomic assembled genomes) spanning 26,970 species-level genome bins (SGBs, http://segatalab.cibio.unitn.it/data/Pasolli_et_al.html), 4,992 of them taxonomically unidentified at the species level, allowing:
+        
+        * unambiguous taxonomic assignments;
+        * an accurate estimation of organismal relative abundance;
+        * SGB-level resolution for bacteria, archaea and eukaryotes;
+        * strain identification and tracking
+        * orders of magnitude speedups compared to existing methods.
+        * metagenomic strain-level population genomics
         
-        To install MetaPhlan through conda run:
+        If you use MetaPhlAn, please cite:
         
-        ```
-        $ conda install -c bioconda metaphlan
-        ```
+        **Extending and improving metagenomic taxonomic profiling with uncharacterized species with MetaPhlAn 4.** Aitor Blanco-Miguez, Francesco Beghini, Fabio Cumbo, Lauren J. McIver, Kelsey N. Thompson, Moreno Zolfo, Paolo Manghi, Leonard Dubois, Kun D. Huang, Andrew Maltez Thomas, Gianmarco Piccinno, Elisa Piperni, Michal Punčochář, Mireia Valles-Colomer, Adrian Tett, Francesca Giordano, Richard Davies, Jonathan Wolf, Sarah E. Berry, Tim D. Spector, Eric A. Franzosa, Edoardo Pasolli, Francesco Asnicar, Curtis Huttenhower, Nicola Segata. Preprint (2022)
         
-        For further installation instructions and alternative installation methods check the [MetaPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/MetaPhlAn-4#installation).
+        If you use StrainPhlAn, please cite the MetaPhlAn paper and the following StrainPhlAn paper:
         
-        -------------
+        [**Microbial strain-level population structure and genetic diversity from metagenomes.**](http://genome.cshlp.org/content/27/4/626.full.pdf) *Duy Tin Truong, Adrian Tett, Edoardo Pasolli, Curtis Huttenhower, & Nicola Segata*. Genome Research 27:626-638 (2017)
         
-        ### Citation
-        If you use MetaPhlAn, please cite:
         
-        [**Extending and improving metagenomic taxonomic profiling with uncharacterized species using MetaPhlAn 4.**](https://doi.org/10.1038/s41587-023-01688-w) Aitor Blanco-Miguez, Francesco Beghini, Fabio Cumbo, Lauren J. McIver, Kelsey N. Thompson, Moreno Zolfo, Paolo Manghi, Leonard Dubois, Kun D. Huang, Andrew Maltez Thomas, Gianmarco Piccinno, Elisa Piperni, Michal Punčochář, Mireia Valles-Colomer, Adrian Tett, Francesca Giordano, Richard Davies, Jonathan Wolf, Sarah E. Berry, Tim D. Spector, Eric A. Franzosa, Edoardo Pasolli, Francesco Asnicar, Curtis Huttenhower, Nicola Segata. Nature Biotechnology (2023)
-        
-        If you use StrainPhlAn, please cite the MetaPhlAn paper and the StrainPhlAn paper:
-        
-        [**Microbial strain-level population structure and genetic diversity from metagenomes.**](http://genome.cshlp.org/content/27/4/626.full.pdf) Duy Tin Truong, Adrian Tett, Edoardo Pasolli, Curtis Huttenhower, Nicola Segata. Genome Research (2017)
+        -------------
         
-        If you use the MetaPhlAn viral module, please cite the MetaPhlAn paper and the MetaPhlan viral module paper:
+        ## MetaPhlAn and StrainPhlAn tutorials and resources
         
-        [**Discovering and exploring the hidden diversity of human gut viruses using highly enriched virome samples.**](https://doi.org/10.1101/2024.02.19.580813 ) Moreno Zolfo, Andrea Silverj, Aitor Blanco-Míguez, Paolo Manghi, Omar Rota-Stabelli, Vitor Heidrich, Jordan Jensen, Sagun Maharjan, Eric Franzosa, Cristina Menni, Alessia Visconti, Federica Pinto, Matteo Ciciani, Curtis Huttenhower, Anna Cereseto, Francesco Asnicar, Hiroaki Kitano, Takuji Yamada, Nicola Segata. bioRxiv (2024)
+        In addition to the information on this page, you can refer to the following additional resources.
         
-        -------------
+        * The [MetaPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/MetaPhlAn-4).
         
-        ### Tutorials and resources
+        * The [StrainPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/StrainPhlAn-4).
         
-        * [MetaPhlan webpage](http://segatalab.cibio.unitn.it/tools/metaphlan/index.html)
-        * [MetaPhlAn documentation](https://github.com/biobakery/MetaPhlAn/wiki/MetaPhlAn-4)
-        * [MetaPhlan tutorial](https://github.com/biobakery/biobakery/wiki/metaphlan4)
-        * [MetaPhlan user support](https://forum.biobakery.org/c/microbial-community-profiling/metaphlan/)
-        * [MetaPhlan change log](https://github.com/biobakery/MetaPhlAn/blob/master/CHANGELOG.md)
-        * [StrainPhlAn webpage](http://segatalab.cibio.unitn.it/tools/strainphlan/index.html)
-        * [StrainPhlAn documentation](http://segatalab.cibio.unitn.it/tools/strainphlan/index.html)
-        * [StrainPhlan tutorial](https://github.com/biobakery/biobakery/wiki/strainphlan4)
-        * [StrainPhlan user support](https://forum.biobakery.org/c/microbial-community-profiling/strainphlan/)
+        * Related tools including [PanPhlAn](https://github.com/segatalab/panphlan) (and its [tutorial](https://github.com/segatalab/panphlan/wiki/Home)), [GraPhlAn](https://github.com/segatalab/graphlan) (and it [tutorial](https://github.com/biobakery/biobakery/wiki/graphlan)), [PhyloPhlAn 3](https://github.com/biobakery/phylophlan) (and its [tutorial](https://github.com/biobakery/biobakery/wiki/phylophlan)), [HUMAnN](https://github.com/biobakery/humann/) (and its [tutorial](https://github.com/biobakery/biobakery/wiki/humann2)).
         
-        #
-        MetaPhlAn and StrainPhlAn are part of the bioBakery suite. For further bioBakery tools and tutorials visit the [bioBakery wiki](https://github.com/biobakery/biobakery).
+        * The related [bioBakery workflows](https://github.com/biobakery/biobakery/wiki/biobakery_workflows)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/__init__.py` & `MetaPhlAn-4b3/metaphlan/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,151 +79,138 @@
             sys.stderr.write("\nDownloading " + url + "\n")
             file, headers = urllib.request.urlretrieve(url, download_file,
                                         reporthook=ReportHook().report)
         except EnvironmentError:
             sys.stderr.write("\nWarning: Unable to download " + url + "\n")
     else:
         sys.stderr.write("\nFile {} already present!\n".format(download_file))
-        
-        
-def download_and_untar(download_file_name, folder, origin):
-        #local path of the tarfile and md5file
+
+def download_unpack_tar(download_file_name, folder, bowtie2_build, nproc, use_zenodo):
+    """
+    Download the url to the file and decompress into the folder
+    """
+
+    # Create the folder if it does not already exist
+    if not os.path.isdir(folder):
+        try:
+            os.makedirs(folder)
+        except EnvironmentError:
+            sys.exit("ERROR: Unable to create folder for database install: " + folder)
+
+    # Check the directory permissions
+    if not os.access(folder, os.W_OK):
+        sys.exit("ERROR: The directory is not writeable: " + folder + ". "
+                 "Please modify the permissions.")
+
+    #local path of the tarfile and md5file
     tar_file = os.path.join(folder, download_file_name + ".tar")
     md5_file = os.path.join(folder, download_file_name + ".md5")
+
     #Download the list of all the files in the FPT    
-    url_tar_file = "{}/{}.tar".format(origin, download_file_name)
-    url_md5_file = "{}/{}.md5".format(origin, download_file_name)
+    url_tar_file = "http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/{}.tar".format(download_file_name)
+    url_md5_file = "http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/{}.md5".format(download_file_name)
+
     # download tar and MD5 checksum
     download(url_tar_file, tar_file)
     download(url_md5_file, md5_file)
+
     md5_md5 = None
     md5_tar = None
+
     if os.path.isfile(md5_file):
         with open(md5_file) as f:
             for row in f:
                 md5_md5 = row.strip().split(' ')[0]
     else:
         sys.stderr.write('File "{}" not found!\n'.format(md5_file))
+
     # compute MD5 of .tar.bz2
     if os.path.isfile(tar_file):
         hash_md5 = hashlib.md5()
 
         with open(tar_file, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
 
         md5_tar = hash_md5.hexdigest()[:32]
     else:
         sys.stderr.write('File "{}" not found!\n'.format(tar_file))
+
     if (md5_tar is None) or (md5_md5 is None):
         sys.exit("MD5 checksums not found, something went wrong!")
+
     # compare checksums
     if md5_tar != md5_md5:
         sys.exit("MD5 checksums do not correspond! If this happens again, you should remove the database files and "
                  "rerun MetaPhlAn so they are re-downloaded")
+
     # untar
     try:
         tarfile_handle = tarfile.open(tar_file)
         tarfile_handle.extractall(path=folder)
         tarfile_handle.close()
-        os.remove(tar_file)
-        os.remove(md5_file)
     except EnvironmentError:
         sys.stderr.write("Warning: Unable to extract {}.\n".format(tar_file))
 
-def download_unpack_tar(download_file_name, folder, bowtie2_build, nproc, use_zenodo):
-    """
-    Download the url to the file and decompress into the folder
-    """
-
-    # Create the folder if it does not already exist
-    if not os.path.isdir(folder):
-        try:
-            os.makedirs(folder)
-        except EnvironmentError:
-            sys.exit("ERROR: Unable to create folder for database install: " + folder)
-
-    # Check the directory permissions
-    if not os.access(folder, os.W_OK):
-        sys.exit("ERROR: The directory is not writeable: " + folder + ". "
-                 "Please modify the permissions.")
-        
-    sys.stderr.write('\n\Downloading and uncompressing indexes\n')
-    download_and_untar("{}_bt2".format(download_file_name), folder, "http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/bowtie2_indexes")
-    sys.stderr.write('\nDownloading and uncompressing additional files\n')
-    download_and_untar(download_file_name, folder, "http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases")
-
     # uncompress sequences
     for bz2_file in iglob(os.path.join(folder, download_file_name + "_*.fna.bz2")):
         fna_file = bz2_file[:-4]
 
         if not os.path.isfile(fna_file):
             sys.stderr.write('\n\nDecompressing {} into {}\n'.format(bz2_file, fna_file))
 
             with open(fna_file, 'wb') as fna_h, \
                 bz2.BZ2File(bz2_file, 'rb') as bz2_h:
                 for data in iter(lambda: bz2_h.read(100 * 1024), b''):
                     fna_h.write(data)
-        os.remove(bz2_file)  
+        os.remove(bz2_file)
+
+    # join fasta files
+    sys.stderr.write('\n\nJoining FASTA databases\n')
+    with open(os.path.join(folder, download_file_name + ".fna"), 'w') as fna_h:
+        for fna_file in iglob(os.path.join(folder, download_file_name + "_*.fna")):
+            with open(fna_file, 'r') as fna_r:
+                for line in fna_r:
+                    fna_h.write(line)
+    fna_file = os.path.join(folder, download_file_name + ".fna")
 
     # build bowtie2 indexes
     if not glob(os.path.join(folder, download_file_name + "*.bt2l")):
-        build_bwt_indexes(folder, download_file_name, bowtie2_build, nproc)
-    else:
+        bt2_base = os.path.join(folder, download_file_name)
+        bt2_cmd = [bowtie2_build, '--quiet']
+
+        if nproc > 1:
+            bt2_build_output = subp.check_output([bowtie2_build, '--usage'], stderr=subp.STDOUT)
+
+            if 'threads' in str(bt2_build_output):
+                bt2_cmd += ['--threads', str(nproc)]
+
+        bt2_cmd += ['-f', fna_file, bt2_base]
+
+        sys.stderr.write('\nBuilding Bowtie2 indexes\n')
+
         try:
-            subp.check_call(['bowtie2-inspect', '-n', os.path.join(folder, download_file_name)], stdout=subp.DEVNULL, stderr=subp.DEVNULL)
+            subp.check_call(bt2_cmd)
         except Exception as e:
-            sys.stderr.write('Downloaded indexes are not compatible with the installed verion of Bowtie2\n')
-            sys.stderr.write('Building indexes from the FASTA files\n')
-            for btw_file in iglob(os.path.join(folder, download_file_name + "*.bt2l")):
-                os.remove(btw_file)
-            build_bwt_indexes(folder, download_file_name, bowtie2_build, nproc)
+            sys.stderr.write("Fatal error running '{}'\nError message: '{}'\n\n".format(' '.join(bt2_cmd), e))
+            sys.exit(1)
 
     try:
         for bt2 in glob(os.path.join(folder, download_file_name + "*.bt2l")):
             os.chmod(bt2, stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IWGRP | stat.S_IROTH)  # change permissions to 664
     except PermissionError as e:
         sys.stderr.write('Cannot change permission for {}. Make sure the files are readable.'.format(os.path.join(folder, download_file_name + "*.bt2l")))
 
     sys.stderr.write('Removing uncompressed databases\n')
-    #os.remove(fna_file)
+    os.remove(fna_file)
 
     # remove all the individual FASTA files but ViralDB
     for fna_file in iglob(os.path.join(folder, download_file_name + "_*.fna")):
         if not fna_file.endswith('_VSG.fna'):
             os.remove(fna_file)
-            
-   
-def build_bwt_indexes(folder, download_file_name, bowtie2_build, nproc):
-    sys.stderr.write('\n\nJoining FASTA databases\n')
-    with open(os.path.join(folder, download_file_name + ".fna"), 'w') as fna_h:
-        for fna_file in iglob(os.path.join(folder, download_file_name + "_*.fna")):
-            with open(fna_file, 'r') as fna_r:
-                for line in fna_r:
-                    fna_h.write(line)
-    fna_file = os.path.join(folder, download_file_name + ".fna")
-    
-    bt2_base = os.path.join(folder, download_file_name)
-    bt2_cmd = [bowtie2_build, '--quiet']
-
-    if nproc > 1:
-        bt2_build_output = subp.check_output([bowtie2_build, '--usage'], stderr=subp.STDOUT)
-
-        if 'threads' in str(bt2_build_output):
-            bt2_cmd += ['--threads', str(nproc)]
-
-    bt2_cmd += ['-f', fna_file, bt2_base]
-
-    sys.stderr.write('\nBuilding Bowtie2 indexes\n')
-
-    try:
-        subp.check_call(bt2_cmd)
-    except Exception as e:
-        sys.stderr.write("Fatal error running '{}'\nError message: '{}'\n\n".format(' '.join(bt2_cmd), e))
-        sys.exit(1)
     
 def download_unpack_zip(url,download_file_name,folder,software_name):
     """
     Download the url to the file and decompress into the folder
     """
     
     # Check for write permission to the target folder
@@ -247,46 +234,43 @@
         
     if not error_during_extract:
         try:
             os.unlink(download_file)
         except EnvironmentError:
             print("WARNING: Unable to remove the temp download: " + download_file)
 
-def resolve_latest_database(bowtie2_db,mpa_latest_url, force=False, offline=False):
-    if not offline and os.path.exists(os.path.join(bowtie2_db,'mpa_latest')):
+def resolve_latest_database(bowtie2_db,mpa_latest_url, force=False):
+    if os.path.exists(os.path.join(bowtie2_db,'mpa_latest')):
         ctime_latest_db = int(os.path.getctime(os.path.join(bowtie2_db,'mpa_latest')))
         if int(time.time()) - ctime_latest_db > 31536000:         #1 year in epoch
             os.rename(os.path.join(bowtie2_db,'mpa_latest'),os.path.join(bowtie2_db,'mpa_previous'))
             download(mpa_latest_url, os.path.join(bowtie2_db,'mpa_latest'), force=True)
 
     if not os.path.exists(os.path.join(bowtie2_db,'mpa_latest') or force):
-        if offline:
-            print("Database cannot be downloaded with the --offline option activated")
-            sys.exit()        
         download(mpa_latest_url, os.path.join(bowtie2_db,'mpa_latest'))
 
     with open(os.path.join(bowtie2_db,'mpa_latest')) as mpa_latest:
         latest_db_version = [line.strip() for line in mpa_latest if not line.startswith('#')]
     
     return ''.join(latest_db_version)
 
-def check_and_install_database(index, bowtie2_db, bowtie2_build, nproc, force_redownload_latest, offline):
+def check_and_install_database(index, bowtie2_db, bowtie2_build, nproc, force_redownload_latest):
     # Create the folder if it does not already exist
     if not os.path.isdir(bowtie2_db):
         try:
             os.makedirs(bowtie2_db)
         except EnvironmentError:
             sys.exit("ERROR: Unable to create folder for database install: " + bowtie2_db)
 
     if index != 'latest' and len(glob(os.path.join(bowtie2_db, "*{}*".format(index)))) >= 6:
         return index
     
     use_zenodo = False
     try:
-        if not offline and urllib.request.urlopen("http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/mpa_latest").getcode() != 200:
+        if urllib.request.urlopen("http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/mpa_latest").getcode() != 200:
             # use_zenodo = True
             pass
     except:
         print('WARNING: It seems that you do not have Internet access.')
         if os.path.exists(os.path.join(bowtie2_db,'mpa_latest')):
             print('WARNING: Cannot connect to the database server. The latest available local database will be used.')
             with open(os.path.join(bowtie2_db,'mpa_latest')) as mpa_latest:
@@ -296,33 +280,32 @@
             You can download the MetaPhlAn database from \n {} 
                   """.format('http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases'))
             sys.exit()
 
     #try downloading from the segatalab website. If fails, use zenodo
     if index == 'latest':
         mpa_latest = 'http://cmprod1.cibio.unitn.it/biobakery4/metaphlan_databases/mpa_latest'
-        index = resolve_latest_database(bowtie2_db, mpa_latest, force_redownload_latest, offline)
+
+        index = resolve_latest_database(bowtie2_db, mpa_latest, force_redownload_latest)
     
-    if not offline and os.path.exists(os.path.join(bowtie2_db,'mpa_previous')):
+    if os.path.exists(os.path.join(bowtie2_db,'mpa_previous')):
         with open(os.path.join(bowtie2_db,'mpa_previous')) as mpa_previous:
             previous_db_version = ''.join([line.strip() for line in mpa_previous if not line.startswith('#')])
     
         if index != previous_db_version:
             choice = ''
             while choice.upper() not in ['Y','N']:
                 choice = input('A newer version of the database ({}) is available. Do you want to download it and replace the current one ({})?\t[Y/N]'.format(index, previous_db_version))
 
             if choice.upper() == 'N':
                 os.rename(os.path.join(bowtie2_db,'mpa_previous'),os.path.join(bowtie2_db,'mpa_latest'))
                 index = previous_db_version
                 
     if len(glob(os.path.join(bowtie2_db, "*{}*".format(index)))) >= 7:
         return index
-    if offline:
-        print("Database cannot be downloaded with the --offline option activated")
-        sys.exit()
+
     # download the tar archive and decompress
     sys.stderr.write("\nDownloading MetaPhlAn database\nPlease note due to "
                      "the size this might take a few minutes\n")
     download_unpack_tar(index, bowtie2_db, bowtie2_build, nproc, use_zenodo)
     sys.stderr.write("\nDownload complete\n")
     return index
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/metaphlan.py` & `MetaPhlAn-4b3/metaphlan/metaphlan.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,44 @@
 #!/usr/bin/env python
 __author__ = ('Aitor Blanco-Miguez (aitor.blancomiguez@unitn.it), '
               'Francesco Beghini (francesco.beghini@unitn.it), '
-              'Moreno Zolfo (moreno.zolfo@unitn.it), '
               'Nicola Segata (nicola.segata@unitn.it), '
               'Duy Tin Truong, '
-              'Francesco Asnicar (f.asnicar@unitn.it), ' 
-              'Claudia Mengoni (claudia.mengoni@unitn.it)')
-__version__ = '4.1.1'
-__date__ = '11 Mar 2024'
+              'Francesco Asnicar (f.asnicar@unitn.it)')
+__version__ = '4.beta.3'
+__date__ = '22 Aug 2022'
 
 import sys
 try:
     from metaphlan import mybytes, plain_read_and_split, plain_read_and_split_line, read_and_split, read_and_split_line, check_and_install_database, remove_prefix
 except ImportError:
-    sys.exit("CRITICAL ERROR: Unable to find the MetaPhlAn python package. Please check your install.")
+    sys.exit("CRITICAL ERROR: Unable to find the MetaPhlAn python package. Please check your install.") 
 
 if float(sys.version_info[0]) < 3.0:
     sys.stderr.write("MetaPhlAn requires Python 3, your current Python version is {}.{}.{}\n"
                     .format(sys.version_info[0], sys.version_info[1], sys.version_info[2]))
     sys.exit(1)
 import os
 import stat
 import re
 import time
-import random
 from collections import defaultdict as defdict
 from distutils.version import LooseVersion
 from glob import glob
 from subprocess import DEVNULL
 import argparse as ap
 import bz2
-import gzip
 import pickle
 import subprocess as subp
 import tempfile as tf
 
-from Bio.Seq import Seq
-from Bio import SeqIO
-from Bio.SeqRecord import SeqRecord
-from collections import Counter
 try:
-    from .utils.parallelisation import execute_pool
-except ImportError:
-    from utils.parallelisation import execute_pool
-try:
-    import pandas as pd
     import numpy as np
-    import pysam
-except Exception as e:
-    sys.stderr.write("Error! python library not detected\n{}\n".format(e))
+except ImportError:
+    sys.stderr.write("Error! numpy python library not detected!!\n")
     sys.exit(1)
 
 #**********************************************************************************************
 #  Modification of Code :                                                                     *
 #  Modified the code so instead of using the current clade IDs, which are numbers, we will    *
 #      use the clade_names                                                                    *
 #      Users reported the biom output is invalid and also the IDs were changing from run to   *
@@ -78,15 +64,15 @@
 DEFAULT_DB_FOLDER= os.environ.get('METAPHLAN_DB_DIR', DEFAULT_DB_FOLDER)
 #Wether to execute a SGB-based analysis
 SGB_ANALYSIS = True
 INDEX = 'latest'
 tax_units = "kpcofgst"
 
 def read_params(args):
-    p = ap.ArgumentParser( description =
+    p = ap.ArgumentParser( description=
             "DESCRIPTION\n"
             " MetaPhlAn version "+__version__+" ("+__date__+"): \n"
             " METAgenomic PHyLogenetic ANalysis for metagenomic taxonomic profiling.\n\n"
             "AUTHORS: "+__author__+"\n\n"
             "COMMON COMMANDS\n\n"
             " We assume here that MetaPhlAn is installed using the several options available (pip, conda, PyPi)\n"
             " Also BowTie2 should be in the system path with execution and read permissions, and Perl should be installed)\n\n"
@@ -298,29 +284,25 @@
          " * clade_profiles: normalized marker counts for clades with at least a non-null marker\n"
          " * marker_ab_table: normalized marker counts (only when > 0.0 and normalized by metagenome size if --nreads is specified)\n"
          " * marker_counts: non-normalized marker counts [use with extreme caution]\n"
          " * marker_pres_table: list of markers present in the sample (threshold at 1.0 if not differently specified with --pres_th\n"
          " * clade_specific_strain_tracker: list of markers present for a specific clade, specified with --clade, and all its subclades\n"
          "[default 'rel_ab']" )
     arg( '--nreads', metavar="NUMBER_OF_READS", type=int, default = None, help =
-         "The total number of reads in the original metagenome. It is mandatory when the --input_type is a SAM file." )
+         "The total number of reads in the original metagenome. It is used only when \n"
+         "-t marker_table is specified for normalizing the length-normalized counts \n"
+         "with the metagenome size as well. No normalization applied if --nreads is not \n"
+         "specified" )
     arg( '--pres_th', metavar="PRESENCE_THRESHOLD", type=int, default = 1.0, help =
          'Threshold for calling a marker present by the -t marker_pres_table option' )
     arg( '--clade', metavar="", default=None, type=str, help =
          "The clade for clade_specific_strain_tracker analysis\n"  )
     arg( '--min_ab', metavar="", default=0.1, type=float, help =
          "The minimum percentage abundance for the clade in the clade_specific_strain_tracker analysis\n"  )
 
-    g = p.add_argument_group('Viral Sequence Clusters Analisys')
-    arg = g.add_argument
-    arg("--profile_vsc", action="store_true",help="Add this parameter to profile Viruses with VSCs approach.")
-    arg("--vsc_out", help="Path to the VSCs breadth-of-coverage output file", default="mp3_viruses.csv")
-    arg("--vsc_breadth", help="Minimum Breadth of Coverage for a Viral Group to be reported.\n"
-        "Default is 0.75 (at least 75 percent breadth to report)", default=0.75,type=float)
-
     g = p.add_argument_group('Output arguments')
     arg = g.add_argument
     arg( '-o', '--output_file',  metavar="output file", type=str, default=None, help =
          "The output file (if not specified as positional argument)\n")
     arg('--sample_id_key',  metavar="name", type=str, default="SampleID",
         help =("Specify the sample ID key for this analysis."
                " Defaults to 'SampleID'."))
@@ -349,32 +331,16 @@
     #* End parameters related to biom file generation            *
     #*************************************************************
 
     g = p.add_argument_group('Other arguments')
     arg = g.add_argument
     arg('--nproc', metavar="N", type=int, default=4,
         help="The number of CPUs to use for parallelizing the mapping [default 4]")
-    arg('--subsampling', type=int, default=None,
-        help="Specify the number of reads to be considered from the input metagenomes [default None]")
-    arg('--subsampling_output', type=str, default=None,
-        help="The output file for the subsampled reads. If --subsampling_paired is specified two files are created with suffixes R1 and R2. If not specified the subsampled reads will not be saved.")
-    arg('--subsampling_paired',  type=int, default=None,
-        help="Specify the number of paired reads to be considered from the input metagenomes [default None]")
-    arg('-1', type=str, default=None, metavar='FORWARD_READS',
-        help="Specify the fastq file with forward reads of the input metagenomes. Reads are assumed to be in the same order in the forward and reverse files! [default None]")
-    arg('-2', type=str, default=None, metavar='REVERSE_READS',
-        help="Specify the fastq file with reverse reads of the input metagenomes. Reads are assumed to be in the same order in the forward and reverse files! [default None]")
-    arg('--mapping_subsampling', action='store_true',
-        help="If used, the subsamping will be done on the mapping results instead of on the reads.")
-    arg('--subsampling_seed', type=str, default='1992',
-        help="Random seed to use in the selection of the subsampled reads. Choose \"random\r for a random behaviour") 
     arg('--install', action='store_true',
         help="Only checks if the MetaPhlAn DB is installed and installs it if not. All other parameters are ignored.")
-    arg('--offline', action='store_true',
-        help="If used, MetaPhlAn will not check for new database updates.")
     arg('--force_download', action='store_true',
         help="Force the re-download of the latest MetaPhlAn database.")
     arg('--read_min_len', type=int, default=70,
         help="Specify the minimum length of the reads to be considered when parsing the input file with "
              "'read_fastx.py' script, default value is 70")
     arg('-v', '--version', action='version',
         version="MetaPhlAn version {} ({})".format(__version__, __date__),
@@ -392,133 +358,16 @@
         mpa_pkl = os.path.join(bowtie2_db, "{}.pkl".format(index))
 
     if glob(os.path.join(bowtie2_db, "{}*.{}".format(index, bt2_ext))):
         bowtie2db = os.path.join(bowtie2_db, "{}".format(index))
 
     return (mpa_pkl, bowtie2db)
 
-
-def set_vsc_parameters(index, bowtie2_db):
-    vsc_fna = os.path.join(bowtie2_db, "{}_VSG.fna".format(index))
-    vsc_vinfo = os.path.join(bowtie2_db, "{}_VINFO.csv".format(index))
-
-    if not os.path.isfile(vsc_fna):
-        sys.stderr.write("Error:\n {} file not found in bowtie2db folder ({}). Re-download MetaPhlAn database.".format("{}_VSG.fna".format(index, bowtie2_db)))
-        sys.exit(1)
-
-    if not os.path.isfile(vsc_vinfo):
-        sys.stderr.write("Error:\n {} file not found in bowtie2db folder ({}). Re-download MetaPhlAn database.".format("{}_VINFO.csv".format(index, bowtie2_db)))
-        sys.exit(1)
-
-    return(vsc_fna, vsc_vinfo)
-
-def vsc_bowtie2(profile_vsc_folder, nproc, file_format="fasta",
-                exe=None,bt2build_exe=None, min_alignment_len=None, read_min_len=0):
-
-    try:
-        subp.check_call([exe if exe else 'bowtie2', "-h"], stdout=DEVNULL)
-        subp.check_call([bt2build_exe if bt2build_exe else 'bowtie2-build', "-h"], stdout=DEVNULL)
-    except Exception as e:
-        sys.stderr.write('OSError: "{}"\nFatal error running BowTie2 and bowtie2-build. Is BowTie2 in the system path?\n'.format(e))
-        sys.exit(1)
-
-    # checking files
-    markerfile= profile_vsc_folder+'/v_mks.fa' 
-    readsfile= profile_vsc_folder+'/v_reads.fq' 
-    vscBamFile= profile_vsc_folder+'/v_align.bam'
-
-    if not os.path.exists(markerfile) or not os.path.exists(readsfile):
-        
-        sys.stderr.write('Error:\nThere was an error in the VSCs file lookup.\n \
-            It may be that there are not enough reads to profile (not enough depth).\n \
-            Passing without reporting any virus.\n')
-        return []
-
-    if os.stat(markerfile).st_size == 0:
-        sys.stderr.write('Warning:\nNo reads aligning to VSC markers in this file.\n')        
-        #return an empty list. MetaPhlAn will continue as normal, without VSCs
-        return []
-
-    #build the db
-
-    bt2build_call = bt2build_exe if bt2build_exe else 'bowtie2-build'
-    dbpath = profile_vsc_folder+'/v_mks'
-    subp.check_call( [bt2build_call, markerfile, dbpath, '-q','--threads', str(nproc)] )
-
-
-    if not all([os.path.exists(".".join([str(dbpath), p]))
-                            for p in ["1.bt2", "2.bt2", "3.bt2", "4.bt2", "rev.1.bt2", "rev.2.bt2"]]):
-        sys.stderr.write('Error:\nThere was an error in running bowtie2-map and not all files were generated. Stopping.\n')
-        sys.exit(1)
-
-    try:
-
-        bt2_call = exe if exe else 'bowtie2'
-        bt2_command = [bt2_call,'--very-sensitive','--quiet','-p',str(nproc),'-x',dbpath,'--no-unal','-U',readsfile]
-        stv_command = ['samtools','view','-bS','-','-@',str(nproc)]
-        sts_command = ['samtools','sort','-','-@',str(nproc),'-o',vscBamFile]
-        sti_command = ['samtools','index',vscBamFile]
-
-        p3 = subp.Popen(sts_command, stdin=subp.PIPE)
-        p2 = subp.Popen(stv_command, stdin=subp.PIPE, stdout=p3.stdin)
-        p1 = subp.Popen(bt2_command, stdout=p2.stdin)
-
-        p1.communicate() 
-        p2.communicate()
-        p3.communicate()
-
-        #index
-        subp.check_call(sti_command)
-
-    except Exception as e:
-        sys.stderr.write('Error: "{}"\nFatal error running BowTie2 for Viruses\n'.format(e))
-        sys.exit(1)
-
-    if not os.path.exists(vscBamFile):
-        sys.stderr.write('Error:\nUnable to create BAM FILE for viruses\n')
-        sys.exit(1)
-
-    try:
-        bamHandle = pysam.AlignmentFile(vscBamFile, "rb")
-    except Exception as e:
-        sys.stderr.write('Error: "{}"\nCheck PySam is correctly working\n'.format(e))
-        sys.exit(1)
-
-    VSC_report=[]
-
-    for c, length in zip(bamHandle.references,bamHandle.lengths):
-        coverage_positions = {}
-
-        for pileupcolumn in bamHandle.pileup(c):
-
-            tCoverage = 0
-            for pileupread in pileupcolumn.pileups:
-
-                if not pileupread.is_del and not pileupread.is_refskip \
-                        and pileupread.alignment.query_qualities[pileupread.query_position] >= 20 \
-                        and pileupread.alignment.query_sequence[pileupread.query_position].upper() in ('A','T','C','G'):
-                        tCoverage +=1
-
-            if tCoverage >= 1:
-                coverage_positions[pileupcolumn.pos] = tCoverage
-        
-        breadth = float(len(coverage_positions.keys()))/float(length)
-        
-        if breadth > 0:
-            cvals=list(coverage_positions.values())
-            VSC_report.append({'M-Group/Cluster':c.split('|')[2].split('-')[0], 'genomeName':c, 'len':length, 'breadth_of_coverage':breadth, 'depth_of_coverage_mean': np.mean(cvals), 'depth_of_coverage_median': np.median(cvals)})
-
-    if bamHandle:
-        bamHandle.close()
-
-    return VSC_report
-
-
 def run_bowtie2(fna_in, outfmt6_out, bowtie2_db, preset, nproc, min_mapq_val, file_format="fasta",
-                exe=None, samout=None, min_alignment_len=None, read_min_len=0, profile_vsc_folder=False):
+                exe=None, samout=None, min_alignment_len=None, read_min_len=0):
     # checking read_fastx.py
     read_fastx = "read_fastx.py"
 
     try:
         subp.check_call([read_fastx, "-h"], stdout=DEVNULL, stderr=DEVNULL)
     except Exception as e:
         try:
@@ -552,19 +401,14 @@
 
         if file_format == "fasta":
             bowtie2_cmd += ["-f"]
 
         p = subp.Popen(bowtie2_cmd, stdout=subp.PIPE, stdin=readin.stdout)
         readin.stdout.close()
         lmybytes, outf = (mybytes, bz2.BZ2File(outfmt6_out, "w")) if outfmt6_out.endswith(".bz2") else (str, open(outfmt6_out, "w"))
-
-        if profile_vsc_folder:
-            CREAD=[]
-            list_of_viral_markers = open(profile_vsc_folder+'/viralmk.txt','w')
-
         try:
             if samout:
                 if samout[-4:] == '.bz2':
                     sam_file = bz2.BZ2File(samout, 'w')
                 else:
                     sam_file = open(samout, 'wb')
         except IOError as e:
@@ -577,36 +421,16 @@
             o = read_and_split_line(line)
             if not o[0].startswith('@'):
                 if not o[2].endswith('*'):
                     if (hex(int(o[1]) & 0x100) == '0x0'): #no secondary
                         if mapq_filter(o[2], int(o[4]), min_mapq_val) :  # filter low mapq reads
                             if ((min_alignment_len is None) or
                                     (max([int(x.strip('M')) for x in re.findall(r'(\d*M)', o[5]) if x]) >= min_alignment_len)):
-                                                                # Profile viral markers in a different way
-                                if profile_vsc_folder and o[2].startswith('VDB|'):
-
-                                    mCluster = o[2]
-                                    mGroup = o[2].split('|')[2].split('-')[0]
-
-                                    list_of_viral_markers.write(mGroup+'\t'+mCluster+'\n')
-
-                                    if (hex(int(o[1]) & 0x10) == '0x0'): #front read
-                                        rr=SeqRecord(Seq(o[9]),letter_annotations={'phred_quality':[ord(_)-33 for _ in o[10][::-1]]}, id=o[0])
-                                    else:
-                                        rr=SeqRecord(Seq(o[9]).reverse_complement(),letter_annotations={'phred_quality':[ord(_)-33 for _ in o[10][::-1]]}, id=o[0])
-
-                                    CREAD.append(rr)
-
-                                # normal route for non-viral markers
                                 outf.write(lmybytes("\t".join([ o[0], o[2].split('/')[0] ]) + "\n"))
 
-        if profile_vsc_folder and os.path.isdir(profile_vsc_folder):
-            SeqIO.write(CREAD,profile_vsc_folder+'/v_reads.fq','fastq')
-            list_of_viral_markers.close()
-
         if samout:  
             sam_file.close()
 
         p.communicate()
         read_fastx_stderr = readin.stderr.readlines()
         nreads = None
         avg_read_length = None
@@ -692,17 +516,17 @@
             cl = cl.father
         return "|".join(fullname[1:])
 
     def get_normalized_counts( self ):
         return [(m,float(n)*1000.0/(np.absolute(self.markers2lens[m] - self.avg_read_length) +1) )
                     for m,n in self.markers2nreads.items()]
 
-    def compute_mapped_reads( self ):    
+    def compute_mapped_reads( self ):        
         tax_level = 't__' if SGB_ANALYSIS else 's__'
-        if self.nreads != 0 or self.name.startswith(tax_level):
+        if self.name.startswith(tax_level):
             return self.nreads
         for c in self.children.values():
             self.nreads += c.compute_mapped_reads()
         return self.nreads
         
     def compute_abundance( self ):
         if self.abundance is not None: return self.abundance
@@ -967,45 +791,37 @@
                         continue
                     clade2abundance[(clade_label, tax_id)] = abundance
         
         for tax_label, clade in clade2abundance_n.items():
             tot_reads += clade.compute_mapped_reads()
 
         for clade_label, clade in self.all_clades.items():
-            if SGB_ANALYSIS or clade.name[:3] != 't__':
+            if clade.name[:3] != 't__':
                 nreads = clade.nreads
                 clade_label = clade.get_full_name()
                 tax_id = clade.get_full_taxids()
                 clade2est_nreads[(clade_label, tax_id)] = nreads
 
         ret_d = dict([( tax, float(abundance) / tot_ab if tot_ab else 0.0) for tax, abundance in clade2abundance.items()])
 
         ret_r = dict([( tax, (abundance, clade2est_nreads[tax] )) for tax, abundance in clade2abundance.items() if tax in clade2est_nreads])
 
         if tax_lev:
-            ret_d[("UNCLASSIFIED", '-1')] = 1.0 - sum(ret_d.values())
+            ret_d[("UNCLASSIFIED", '-1')] = 1.0 - sum(ret_d.values())  
         return ret_d, ret_r, tot_reads
 
 def mapq_filter(marker_name, mapq_value, min_mapq_val):
-    ##if 'GeneID:' in marker_name:
-    if 'GeneID:' in marker_name or 'VDB' in marker_name:
+    if 'GeneID:' in marker_name:
         return True
     else:
         if mapq_value > min_mapq_val:
             return True
     return False
 
-
-def separate_reads2markers(reads2markers):
-    if not SGB_ANALYSIS:
-        return reads2markers, {}
-    else:
-        return {r: m for r, m in reads2markers.items() if ('SGB' in m or 'EUK' in m) and not 'VDB' in m}, {r: m for r, m in reads2markers.items() if 'VDB' in m and not ('SGB' in m or 'EUK' in m)}
-
-def map2bbh(mapping_f, min_mapq_val, input_type='bowtie2out', min_alignment_len=None, nreads=None, mapping_subsampling=False, subsampling=None, subsampling_seed='1992', remove_input=False):
+def map2bbh(mapping_f, min_mapq_val, input_type='bowtie2out', min_alignment_len=None):
     if not mapping_f:
         ras, ras_line, inpf = plain_read_and_split, plain_read_and_split_line, sys.stdin
     else:
         if mapping_f.endswith(".bz2"):
             ras, ras_line, inpf = read_and_split, read_and_split_line, bz2.BZ2File(mapping_f, "r")
         else:
             ras, ras_line, inpf = plain_read_and_split, plain_read_and_split_line, open(mapping_f)
@@ -1019,48 +835,25 @@
             if r.startswith('#') and 'nreads' in r:
                 n_metagenome_reads = int(c)
             if r.startswith('#') and 'avg_read_length' in r:
                 avg_read_length = float(c)
             else:
                 reads2markers[r] = c
     elif input_type == 'sam':
-        n_metagenome_reads = nreads 
         for line in inpf:
             o = ras_line(line)
             if ((o[0][0] != '@') and #no header
                 (o[2][-1] != '*') and # no unmapped reads
                 (hex(int(o[1]) & 0x100) == '0x0') and #no secondary
                 mapq_filter(o[2], int(o[4]), min_mapq_val) and # filter low mapq reads
                 ( (min_alignment_len is None) or ( max(int(x.strip('M')) for x in re.findall(r'(\d*M)', o[5]) if x) >= min_alignment_len ) )
             ):
                     reads2markers[o[0]] = o[2].split('/')[0]
     inpf.close()
-    
-    if subsampling is not None and mapping_subsampling:
-        if subsampling >= n_metagenome_reads:
-            sys.stderr.write("WARNING: The specified subsampling ({}) is equal or higher than the original number of reads ({}). Subsampling will be skipped.\n".format(subsampling, n_metagenome_reads))
-        else:
-            reads2markers =  dict(sorted(reads2markers.items()))
-            if subsampling_seed.lower() != 'random':
-                random.seed(int(subsampling_seed))
-            reads2filtmarkers = {}
-            sgb_reads2markers, viral_reads2markers = separate_reads2markers(reads2markers)            
-            n_sgb_mapped_reads = int((len(sgb_reads2markers) * subsampling) / n_metagenome_reads)
-            reads2filtmarkers = { r:sgb_reads2markers[r] for r in random.sample(list(sgb_reads2markers.keys()), n_sgb_mapped_reads) }     
-            if SGB_ANALYSIS:       
-                n_viral_mapped_reads = int((len(viral_reads2markers) * subsampling) / n_metagenome_reads)
-                reads2filtmarkers.update({ r:viral_reads2markers[r] for r in random.sample(list(viral_reads2markers.keys()), n_viral_mapped_reads) })            
-            reads2markers = reads2filtmarkers
-            sgb_reads2markers.clear()
-            viral_reads2markers.clear()
-            n_metagenome_reads = subsampling
-    elif subsampling is None and n_metagenome_reads < 10000:
-        sys.stderr.write("WARNING: The number of reads in the sample ({}) is below the recommended minimum of 10,000 reads.\n".format(n_metagenome_reads))
-        
-    markers2reads = defdict(set)   
+    markers2reads = defdict(set)
     for r, m in reads2markers.items():
         markers2reads[m].add(r)
 
     return (markers2reads, n_metagenome_reads, avg_read_length)
 
 def maybe_generate_biom_file(tree, pars, abundance_predictions):
     json_key = "MetaPhlAn"
@@ -1143,204 +936,32 @@
 
         with open(pars['biom'], 'w') as outfile:
             biom_table.to_json( json_key,
                                 direct_io = outfile )
 
     return True
 
-def _make_gen_fastq(reader):
-    b = reader(1024 * 1024) 
-    while (b):
-        yield b
-        b = reader(1024 * 1024)
-
-def rawpycount(filename):
-    f = bz2.BZ2File(filename, 'rb') if filename.endswith(".bz2") else gzip.open(filename, 'rb') if filename.endswith('.gz') else open(filename, 'rb')
-    f_gen = _make_gen_fastq(f.read)
-    n_metagenome_reads = sum( buf.count(b'\n') for buf in f_gen)
-    f.close()
-    return n_metagenome_reads
-
-def subsample_file(inp, paired, subsampling, out, sample):         
-    length, read_num = 0, -1
-    counter=0
-    out_l = out
-    for inp_f in inp.split(','):
-        if paired:
-            length, read_num = 0, -1  
-            out=out_l[counter]
-            counter+=1
-        line = 1
-        reader = bz2.open(inp_f, 'rt') if inp_f.endswith(".bz2") else gzip.open(inp_f, 'rt') if inp_f.endswith('.gz') else open(inp_f, 'r')
-        while (line and length < subsampling):
-            line = reader.readline()
-            read_num += 1
-            if read_num in sample:
-                length += 1
-                out.write(line)       
-                for _ in range(3):
-                    out.write(reader.readline())
-            else:
-                for _ in range(3):
-                    reader.readline()
-        reader.close()
-    out.close()
-    
-def subsample_reads(inp, subsampling, subsampling_seed, subsampling_output, tmp_dir, paired):
-
-    n_metagenome_reads = execute_pool(((rawpycount, inp_f) for inp_f in inp.split(',')), 2)
-    n_metagenome_reads = [int(n/4) for n in n_metagenome_reads]
-
-    if paired:
-        subsampling //= 2
-        if n_metagenome_reads[0] != n_metagenome_reads[1]:
-            sys.stderr.write("Error: The specified reads file are not the same length! Make sure the forward and reverse reads are files are not damaged and reads are in the same order. Exiting ...\n\n") 
-            sys.exit(1)
-        n_metagenome_reads = n_metagenome_reads[0]
-    else:
-        n_metagenome_reads = sum(n_metagenome_reads)
-
-    if subsampling >= n_metagenome_reads:
-        sys.stderr.write("WARNING: The specified subsampling ({}) is equal or higher than the original number of reads ({}). Subsampling will be skipped.\n".format(subsampling, sum(n_metagenome_reads))) 
-        return inp, None
-
-    if subsampling_seed.lower() != 'random':
-        random.seed(int(subsampling_seed))
-        
-    sample = set(random.sample(range(n_metagenome_reads), subsampling))
-    
-    if subsampling_output is None:
-        if paired:
-            subsampling_output = list()
-            out=list()
-            for _ in inp.split(','):
-                out_f = tf.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False)
-                out.append(out_f)
-                subsampling_output.append(out_f.name)
-        else:
-            out = tf.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False)
-            subsampling_output=out.name
-    else:
-        if paired:
-            r, ext = os.path.splitext(subsampling_output)
-
-            subsampling_output = list()
-            out = list()
-
-            subsampling_output.append('.'.join([r, 'R1'+ext]))
-            subsampling_output.append('.'.join([r, 'R2'+ext]))
-
-            for s in subsampling_output:
-                out.append(bz2.open(s, 'wt') if s.endswith(".bz2") else gzip.open(s, 'wt') if s.endswith('.gz') else open(s, 'w'))
-        else:
-            out = bz2.open(subsampling_output, 'wt') if subsampling_output.endswith(".bz2") else gzip.open(subsampling_output, 'wt') if subsampling_output.endswith('.gz') else open(subsampling_output, 'w')
-            
-    subsample_file(inp, paired, subsampling, out, sample)
-
-    if isinstance(subsampling_output, list):
-        subsampling_output = ','.join(subsampling_output)
-        
-    return subsampling_output, subsampling
-
 def main():
     ranks2code = { 'k' : 'superkingdom', 'p' : 'phylum', 'c':'class',
                    'o' : 'order', 'f' : 'family', 'g' : 'genus', 's' : 'species'}
     pars = read_params(sys.argv)
 
     #Set SGB- / species- analysis
     global SGB_ANALYSIS
     SGB_ANALYSIS = not pars['mpa3']
 
     ESTIMATE_UNK = pars['unclassified_estimation']
 
-    if pars['subsampling'] and pars['subsampling_paired']:
-        sys.stderr.write("Error: You specified both --subsampling and --subsampling_paired. Choose only one of the two options. Exiting...")
-        sys.exit(1)
-
-    if pars['subsampling']:
-        sys.stderr.write("WARNING: If you use --subsampling the reads will be subsampled NOT taking into account paired information. Use --subsampling_paired if you have paired ends reads.\n".format(pars['subsampling']))
-    
-    if pars['mapping_subsampling'] and pars['subsampling'] is None:
-        sys.stderr.write("Error: The --mapping_subsampling parameter should be used together with the --subsampling parameter. Exiting...\n\n")
-        sys.exit(1)
-
-    if pars['subsampling_paired']:
-        subsampling_paired=True
-        pars['subsampling']=pars['subsampling_paired']
-    else:
-        subsampling_paired=False
-
-    if subsampling_paired and (pars['1'] is None or pars['2'] is None):
-        sys.stderr.write("Error: If you specify --subsampling_paired you have to provide forward and reverse reads as -1 and -2 respectively. Reads are assumed to be in the same order in the two files.\n Exiting...\n\n".format(pars['subsampling']))
-        sys.exit(1)
-    
-    if pars['subsampling'] is not None and pars['subsampling'] < 10000:
-        sys.stderr.write("WARNING: The specified subsampling ({}) is below the recommended minimum of 10,000 reads.\n".format(pars['subsampling']))
-    
-    if not (pars['subsampling_seed'].lower() == 'random' or pars['subsampling_seed'].isdigit()):
-        sys.stderr.write("Error: The --subsampling_seed parameter is not accepted. It should contain an integer number or \"random\". Exiting...\n\n")
-        sys.exit(1)
-        
-    if not pars['mapping_subsampling'] and pars['subsampling'] is not None:
-        if pars['input_type'] != 'fastq':
-            sys.stderr.write("Error: The reads' subsampling procedure requires fastq input! Exiting...\n\n")
-            sys.exit(1)
-        elif (not pars['inp']) and (not subsampling_paired):
-            sys.stderr.write("Error: Input reads for the subsampling must be provided as parameter. Stdin input is not allowed! Exiting...\n\n")
-            sys.exit(1)
-        
-        if subsampling_paired:
-            if not os.path.exists(pars['2']) or not os.path.exists(pars['1']):
-                sys.stderr.write("Error: Files passed with -1 ({}) or -2 ({}) not found. Exiting...\n\n".format(pars['1'],pars['2']))
-                sys.exit(1)
-
-            if pars['inp']:
-                sys.stderr.write("WARNING: since --subsampling_paired has been specified, reads are taken from -1 ({}) and -2 ({}), not from -inp.\n".format(pars['1'],pars['2']))
-            pars['inp'] = pars['1']+','+pars['2']
-
-        pars['inp'], pars['subsampling'] = subsample_reads(pars['inp'], pars['subsampling'], pars['subsampling_seed'], pars['subsampling_output'], pars['tmp_dir'], paired=subsampling_paired)
-        
     # check if the database is installed, if not then install
-    pars['index'] = check_and_install_database(pars['index'], pars['bowtie2db'], pars['bowtie2_build'], pars['nproc'], pars['force_download'], pars['offline'])
+    pars['index'] = check_and_install_database(pars['index'], pars['bowtie2db'], pars['bowtie2_build'], pars['nproc'], pars['force_download'])
 
     if pars['install']:
         sys.stderr.write('The database is installed\n')
         return
 
-    #if we are to profile viral clusters:
-
-    if pars['profile_vsc']:
-        #TODO: comply to other input types
-        if pars['input_type'] != 'fastq':
-            sys.stderr.write("The Viral Sequence Clusters mode requires fastq input!\n")
-            sys.exit(1)
-        
-        if not pars['vsc_out']:
-            sys.stderr.write("The Viral Sequence Clusters mode requires to specify an output file with the --vsc_out parameter\n")
-            sys.exit(1)
-
-        tmpvirdir=tf.TemporaryDirectory(dir=pars['tmp_dir'])
-        viralTempFolder=tmpvirdir.name
-        
-        # Uncomment to preserve tmp dir
-        #tmpvirdir=tf.mkdtemp(dir=pars['tmp_dir'])
-        #viralTempFolder=tmpvirdir
-        #print("VF: ",viralTempFolder)
-
-        vsc_fna, vsc_vinfo = set_vsc_parameters(pars['index'], pars['bowtie2db'])
-
-        # implies SGBs (uses the same database with SGBs, so this is needed to avoid
-        # the need to specify --sgb when using --profile_vscs)
-        SGB_ANALYSIS = True
-
-
-    else:
-        viralTempFolder = None
-
-
     # set correct map_pkl and bowtie2db variables
     pars['mpa_pkl'], pars['bowtie2db'] = set_mapping_arguments(pars['index'], pars['bowtie2db'])
 
     if (pars['bt2_ps'] in ["sensitive-local", "very-sensitive-local"]) and (pars['min_alignment_len'] is None):
             pars['min_alignment_len'] = 100
             sys.stderr.write('Warning! bt2_ps is set to local mode, and min_alignment_len is None, I automatically '
                              'set min_alignment_len to 100! If you do not like, rerun the command and set '
@@ -1408,92 +1029,42 @@
                              .format(pars['bowtie2db']))
             sys.exit(1)
 
         if bow:
             run_bowtie2(pars['inp'], pars['bowtie2out'], pars['bowtie2db'],
                                 pars['bt2_ps'], pars['nproc'], file_format=pars['input_type'],
                                 exe=pars['bowtie2_exe'], samout=pars['samout'],
-
-                                min_alignment_len=pars['min_alignment_len'], read_min_len=pars['read_min_len'], min_mapq_val=pars['min_mapq_val'],profile_vsc_folder=viralTempFolder)
-            if pars['subsampling_output'] is None and not pars['mapping_subsampling'] and pars['subsampling'] is not None:
-                for inp_f in pars['inp'].split(','):
-                    os.remove(inp_f)
+                                min_alignment_len=pars['min_alignment_len'], read_min_len=pars['read_min_len'], min_mapq_val=pars['min_mapq_val'])
             pars['input_type'] = 'bowtie2out'
         pars['inp'] = pars['bowtie2out'] # !!!
     with bz2.BZ2File( pars['mpa_pkl'], 'r' ) as a:
         mpa_pkl = pickle.load( a )
 
     REPORT_MERGED = mpa_pkl.get('merged_taxon',False)
     tree = TaxTree( mpa_pkl, ignore_markers )
     tree.set_min_cu_len( pars['min_cu_len'] )
 
-    if pars['input_type'] == 'sam' and not pars['nreads']:
-        sys.stderr.write(
-                "Please provide the size of the metagenome using the "
-                "--nreads parameter when running MetaPhlAn using SAM files as input"
-                "\nExiting...\n\n" )
-        sys.exit(1)
-
-    markers2reads, n_metagenome_reads, avg_read_length = map2bbh(pars['inp'], pars['min_mapq_val'], pars['input_type'], pars['min_alignment_len'], pars['nreads'], pars['mapping_subsampling'], pars['subsampling'], pars['subsampling_seed'])
-
-    if pars['profile_vsc']:
-        
-        try:
-            VSCs_markers = SeqIO.index(vsc_fna, "fasta")
-        except Exception as e:
-            sys.stderr.write('Error: "{}"\nCould not access to {}.\n'.format(e,vsc_fna))
-            sys.exit(1)
-
-        with open(viralTempFolder+'/viralmk.txt') as viral_markers_to_remap:
-
-            allViralMarkers = {}
-            for vmarker in viral_markers_to_remap:
-                group,marker = vmarker.strip().split()
-                if group not in allViralMarkers:
-                    allViralMarkers[group] = [marker]
-                else:
-                    allViralMarkers[group].append(marker)
-
-            selectedMakrers=[]
-            for grp,v in allViralMarkers.items():
-
-                cv=Counter(v)
-                if (len(cv) > 1):
-                    normalized_occurrencies=sorted([(mk,mk_occurrencies,len(VSCs_markers[mk].seq)) for (mk,mk_occurrencies) in cv.items()],key=lambda x: x[1]/x[2],reverse=True)
-                    topMarker= VSCs_markers[normalized_occurrencies[0][0]] #name of the viralGenome
-                else:
-                    topMarker=VSCs_markers[v[0]] # the only hitted viralGenome is the winning one
-
-                selectedMakrers.append(topMarker)
-
-
-            SeqIO.write( selectedMakrers,viralTempFolder+'/v_mks.fa','fasta' )
-
-            VSC_report = vsc_bowtie2(viralTempFolder, pars['nproc'], file_format=pars['input_type'],
-                        exe=pars['bowtie2_exe'], bt2build_exe=pars['bowtie2_build']) 
-
-
-            if not VSC_report == []:
-                with open(pars['vsc_out'],'w') as outf:
-
-                    outf.write('#{}\n'.format(pars['index']))
-                    outf.write('#{}\n'.format(' '.join(sys.argv)))
-                    outf.write('#SampleID\t{}\n'.format(pars['sample_id']))
-                    vsc_out_df = pd.DataFrame.from_dict(VSC_report).query('breadth_of_coverage >= {}'.format(pars['vsc_breadth']))
-                    vsc_info_df = pd.read_table(vsc_vinfo, sep='\t')
-                    vsc_out_df = vsc_out_df.merge(vsc_info_df, on='M-Group/Cluster').sort_values(by='breadth_of_coverage', ascending=False).set_index('M-Group/Cluster')
-
-                    vsc_out_df.to_csv(outf,sep='\t',na_rep='-')
-
+    markers2reads, n_metagenome_reads, avg_read_length = map2bbh(pars['inp'], pars['min_mapq_val'], pars['input_type'], pars['min_alignment_len'])
 
     tree.set_stat( pars['stat'], pars['stat_q'], pars['perc_nonzero'], avg_read_length, pars['avoid_disqm'])
 
     if no_map:
         os.remove( pars['inp'] )
 
+    if not n_metagenome_reads and pars['nreads']:
+        n_metagenome_reads = pars['nreads']
+    
+    if ESTIMATE_UNK and pars['input_type'] == 'sam':
+        if not n_metagenome_reads and not pars['nreads']:
+            sys.stderr.write(
+                    "Please provide the size of the metagenome using the "
+                    "--nreads parameter when running MetaPhlAn using SAM files as input"
+                    "\nExiting...\n\n" )
+            sys.exit(1)
+
     map_out = []
     for marker,reads in sorted(markers2reads.items(), key=lambda pars: pars[0]):
         if marker not in tree.markers2lens:
             continue
         tax_seq, ids_seq = tree.add_reads( marker, len(reads),
                                   add_viruses = pars['add_viruses'],
                                   ignore_eukaryotes = pars['ignore_eukaryotes'],
@@ -1512,18 +1083,14 @@
     MPA2_OUTPUT = pars['legacy_output']
     CAMI_OUTPUT = pars['CAMI_format_output']
 
     with out_stream as outf:
         if not MPA2_OUTPUT:
             outf.write('#{}\n'.format(pars['index']))
             outf.write('#{}\n'.format(' '.join(sys.argv)))
-            outf.write('#{} reads processed\n'.format(n_metagenome_reads))
-        
-        if pars['t'] == 'rel_ab_w_read_stats':
-            outf.write('#Average read length {}\n'.format(avg_read_length))           
 
         if not CAMI_OUTPUT:
             outf.write('#' + '\t'.join((pars["sample_id_key"], pars["sample_id"])) + '\n')
 
         if ESTIMATE_UNK:
             mapped_reads = 0
             cl2pr = tree.clade_profiles( pars['tax_lev']+"__" if pars['tax_lev'] != 'a' else None  )
@@ -1558,15 +1125,15 @@
             outpred = [(taxstr, taxid,round(relab*100.0,5)) for (taxstr, taxid), relab in cl2ab.items() if relab > 0.0]
             has_repr = False
             
             if outpred:
                 if CAMI_OUTPUT:
                     for clade, taxid, relab in sorted(  outpred, reverse=True,
                                         key=lambda x:x[2]+(100.0*(8-(x[0].count("|"))))):
-                        if taxid and clade.split('|')[-1][0] != 't':
+                        if taxid:
                             rank = ranks2code[clade.split('|')[-1][0]]
                             leaf_taxid = taxid.split('|')[-1]
                             taxpathsh = '|'.join([remove_prefix(name) if '_unclassified' not in name else '' for name in clade.split('|')])
                             outf.write( '\t'.join( [ leaf_taxid, rank, taxid, taxpathsh, str(relab*fraction_mapped_reads) ] ) + '\n' )
                 else:
                     if ESTIMATE_UNK:
                         outf.write( "\t".join( [    "UNCLASSIFIED",
@@ -1609,26 +1176,26 @@
                         pars['tax_lev']+"__" if pars['tax_lev'] != 'a' else None )
 
             unmapped_reads = max(n_metagenome_reads - tot_nreads, 0)
 
             outpred = [(taxstr, taxid,round(relab*100.0*fraction_mapped_reads,5)) for (taxstr, taxid),relab in cl2ab.items() if relab > 0.0]
 
             if outpred:
-                outf.write( "#estimated_reads_mapped_to_known_clades:{}\n".format(round(tot_nreads)) )
+                outf.write( "#estimated_reads_mapped_to_known_clades:{}\n".format(tot_nreads) )
                 outf.write( "\t".join( [    "#clade_name",
                                             "clade_taxid",
                                             "relative_abundance",
                                             "coverage",
                                             "estimated_number_of_reads_from_the_clade" ]) +"\n" )
                 if ESTIMATE_UNK:
                     outf.write( "\t".join( [    "UNCLASSIFIED",
                                                 "-1",
                                                 str(round((1-fraction_mapped_reads)*100,5)),
                                                 "-",
-                                                str(round(unmapped_reads)) ]) + "\n" )
+                                                str(unmapped_reads) ]) + "\n" )
                                                 
                 for taxstr, taxid, relab in sorted(  outpred, reverse=True,
                                     key=lambda x:x[2]+(100.0*(8-(x[0].count("|"))))):
                     outf.write( "\t".join( [    taxstr,
                                                 taxid,
                                                 str(relab),
                                                 str(round(rr[(taxstr, taxid)][0],5)) if (taxstr, taxid) in rr else '-',          #coverage
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/VallesColomerM_2022_Nov19_thresholds.tsv` & `MetaPhlAn-4b3/metaphlan/utils/VallesColomerM_2022_Nov19_thresholds.tsv`

 * *Files identical despite different names*

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/add_metadata_tree.py` & `MetaPhlAn-4b3/metaphlan/utils/add_metadata_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 __author__ = ('Duy Tin Truong (duytin.truong@unitn.it), '
               'Aitor Blanco Miguez (aitor.blancomiguez@unitn.it)')
-__version__ = '4.1.0'
-__date__ = '23 Aug 2023'
+__version__ = '4.beta.3'
+__date__    = '22 Aug 2022'
 
 import argparse as ap
 import pandas
 import dendropy
 import numpy
 
 def read_params():
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/external_exec.py` & `MetaPhlAn-4b3/metaphlan/utils/external_exec.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,197 +1,309 @@
 __author__ = ('Aitor Blanco Miguez (aitor.blancomiguez@unitn.it), '
               'Duy Tin Truong (duytin.truong@unitn.it), '
               'Francesco Asnicar (f.asnicar@unitn.it), '
               'Moreno Zolfo (moreno.zolfo@unitn.it), '
               'Francesco Beghini (francesco.beghini@unitn.it)')
-__version__ = '4.1.1'
-__date__ = '11 Mar 2024'
+__version__ = '4.beta.3'
+__date__ = '22 Aug 2022'
 
-
-import os
-import re
-import shlex
-import shutil
-import tempfile
+import os, sys, re, shutil, tempfile
 import subprocess as sb
 try:
     from .util_fun import info, error
 except ImportError:
     from util_fun import info, error
 
+"""
+Executes a command
 
+:param cmd: the command to execute
+"""
 def execute(cmd):
-    """Runs a command line executable
-
-    Args:
-        cmd (dict): the dict with the command line information
-    """
     inp_f = None
-    out_f = sb.PIPE
+    out_f = sb.DEVNULL
+
     if cmd['stdin']:
         inp_f = open(cmd['stdin'], 'r')
     if cmd['stdout']:
         out_f = open(cmd['stdout'], 'w')
+
     exec_res = sb.run(cmd['command_line'], stdin=inp_f, stdout=out_f)
     if exec_res.returncode == 1:
-        error("An error was ocurred executing a external tool, exiting...", exit=True)
-        print(exec_res.stdout)
-        print('===')
-        print(exec_res.stderr)
+        error("An error was ocurred executing a external tool, exiting...", 
+            init_new_line=True, exit=True) 
+
     if cmd['stdin']:
         inp_f.close()
     if cmd['stdout']:
         out_f.close()
 
 
-def build_bowtie2_db(input_fasta, output_database):
+"""
+Creates the BLASTn database to align the reference genomes
+
+:param output_dir: the output directory
+:param reference: the FASTA with the reference
+:returns: the created BLASTn database
+"""
+def create_blastn_db(output_dir, reference):
+    reference_name = os.path.splitext(os.path.basename(reference))[0]    
     params = {
-        "program_name": "bowtie2-build",
-        "params": "--large-index {} {}".format(input_fasta, output_database),
-        "command_line": "#program_name# #params#"
+        "program_name" : "makeblastdb",
+        "params" : "-parse_seqids -dbtype nucl",
+        "input" : "-in",
+        "output" : "-out",
+        "command_line" : "#program_name# #params# #input# #output#"
     }
-    execute(compose_command(params, input_file=input_fasta, output_file=output_database))
+    execute(compose_command(params, input_file=reference, output_file=output_dir+reference_name))
+    return output_dir+reference_name
 
 
-def generate_phylophlan_config_file(output_dir, configuration):
-    """Generates the PhyloPhlan configuration file"""
-    conf_file = os.path.join(output_dir, "phylophlan.cfg")
+"""
+Executes BLASTn
+
+:param output_dir: the output directory
+:param clade_markers: the FASTA with the markers
+:param blastn_db: the BLASTn database
+:param nprocs: the number of thread to use
+:returns: the BLASTn output file
+"""
+def execute_blastn(output_dir, clade_markers, blastn_db, nprocs=1):
+    db_name = os.path.splitext(os.path.basename(blastn_db))[0]
     params = {
-        "program_name": "phylophlan_write_config_file",
-        "params": "-d n --db_dna makeblastdb --map_dna {} --msa {} --tree1 {}".format(configuration['map'], configuration['aligner'], configuration['tree1']),
-        "output": "-o",
-        "command_line": "#program_name# #output# #params#"
+        "program_name" : "blastn",
+        "params" : "-outfmt \"6 qseqid sseqid qlen qstart qend sstart send\" -evalue 1e-10 -max_target_seqs 1",
+        "input" : "-query",
+        "database": "-db",
+        "output" : "-out",
+        "threads" : "-num_threads",
+        "command_line" : "#program_name# #params# #threads# #database# #input# #output#"
     }
-    execute(compose_command(params, output_file=conf_file))
-    return conf_file
+    execute(compose_command(params, input_file=clade_markers, database=blastn_db, 
+        output_file=output_dir+db_name+".blastn", nproc=nprocs))
+    return output_dir+db_name+".blastn"
 
 
-def execute_treeshrink(input_tree, output_dir, tmp=None, centroid=False, q_value=0.05, m_value='all-genes'):
-    """Executes TreeShrink"""
-    advanced_string = ''
-    if tmp is not None:
-        advanced_string += '-p {} '.format(tmp)
-    if centroid:
-        advanced_string += '-c '
-    if not os.path.exists('{}/treeshrink'.format(output_dir)):
-        os.mkdir('{}/treeshrink'.format(output_dir))
+"""
+Creates the PhyloPhlAn database
+
+:param output_dir: the output directory
+:param clade: the clade
+"""
+def create_phylophlan_db(output_dir, clade):
+    markers = output_dir+clade
     params = {
-        "program_name": "treeshrink.py",
-        "params": "{}-q {} -m {} -f".format(advanced_string, q_value, m_value),
-        "input": "-t",
-        "output_path": '-o',
-        "output": "-O",
-        "command_line": "#program_name# #input# #output_path# #output# #params#"
+        "program_name" :"phylophlan_setup_database",
+        "params" : "-d "+clade+" -e fna -t n --overwrite",
+        "input" : "-i",
+        "command_line" : "#program_name# #input# #params#"
     }
-    execute(compose_command(params=params, input_file=input_tree, output_path='{}/treeshrink'.format(
-        output_dir), output_file=input_tree.split('/')[-1].replace('.StrainPhlAn4.tre', '.TreeShrink')))
+    execute(compose_command(params, input_file=markers))
+    #os.rename(output_dir+clade+".fna", markers+"/"+clade+".fna")
+
 
+"""
+Generates the PhyloPhlan configuration file
 
-def compress_bz2(input_file):
-    """Compress BZ2 files"""
+:param output_dir: the output directory
+:returns: the generated configuration file
+"""
+def generate_phylophlan_config_file(output_dir, configuration):
+    conf_file = output_dir+"phylophlan.cfg"
     params = {
-        "program_name": "bzip2",
-        "params": "{}".format(input_file),
-        "command_line": "#program_name# #params#"
+        "program_name" : "phylophlan_write_config_file",
+        "params" : "-d n --db_dna makeblastdb --map_dna "+configuration['map']+
+            " --msa "+configuration['aligner']+" --trim "+configuration['trim']+
+            " --tree1 "+configuration['tree1'], #+
+            # configuration['tree2'],
+        "output" : "-o",
+        "command_line" : "#program_name# #output# #params#"
     }
-    execute(compose_command(params, input_file=input_file))
-    
+    execute(compose_command(params, output_file=conf_file))
+    return conf_file
+
+
+"""
+Executes PhyloPhlAn
+
+:param samples_markers_dir: the temporal samples markers directory
+:param conf_file: the PhyloPhlAn configuration file
+:param min_entries: the minimun number of entries to consider a good marker 
+:param tmp_dir: the temporal output directory
+:param output_dir: the output_directory
+:param clade: the clade
+:param phylogeny_conf: the precision of the phylogenetic analysis
+:param mutation_rates: whether get  the mutation rates for the markers
+:param nproc: the number of threads to run phylophlan
+"""
+def execute_phylophlan(samples_markers_dir, conf_file, min_entries, min_markers, tmp_dir, output_dir, 
+    clade, phylogeny_conf, mutation_rates, nprocs):
+    accuracy = " --"+phylogeny_conf
 
-def decompress_bz2(input_file, output_dir):
-    """Decompresses BZ2 files"""
-    n, _ = os.path.splitext(os.path.basename(input_file))
+    if mutation_rates:
+        accuracy = accuracy + " --mutation_rates"
     params = {
-        "program_name": "bzip2",
-        "input": "-cdk",
-        "command_line": "#program_name# #input# > #output#"
+        "program_name" : "phylophlan",
+        "params" : "-d "+clade[:30]+" --data_folder "+tmp_dir+
+            " --databases_folder "+tmp_dir+" -t n -f "+conf_file+
+            " --diversity low"+accuracy+" --genome_extension fna"+
+            " --force_nucleotides --min_num_entries "+str(min_entries)+
+            " --min_num_markers "+str(min_markers),
+        "input" : "-i",
+        "output_path" : "--output_folder",
+        "output" : "-o",
+        "threads" : "--nproc",
+        "command_line" : "#program_name# #input# #output# #output_path# #params# #threads#"
     }
-    decompressed_file = os.path.join(output_dir, n)
-    execute(compose_command(params, input_file=input_file,
-            output_file=decompressed_file))
+    execute(compose_command(params=params, input_file=samples_markers_dir, output_path=output_dir,
+        output_file=".", nproc=nprocs))
+        
+
+#ToDo: Parametrize this function: default output_dir, remove the compressed file...
+"""
+Decompressed BZ2 files
+
+:param input: the input BZ2 file to decompress
+:param output_dir: the output directory
+:returns: the decompressed file
+"""
+def decompress_bz2(input, output_dir):
+    n, _ = os.path.splitext(os.path.basename(input))
+    params = {
+        "program_name" : "bzip2",
+        "input" : "-cdk",
+        "command_line" : "#program_name# #input# > #output#"
+    }      
+    decompressed_file = output_dir + n 
+    execute(compose_command(params, input_file=input, output_file=decompressed_file))
     if decompressed_file.endswith('_sam'):
         os.rename(decompressed_file, decompressed_file[:-4] + '.sam')
         decompressed_file = decompressed_file[:-4] + '.sam'
     return decompressed_file
 
 
-def samtools_sam_to_bam(input_file, output_dir):
-    """Converts SAM files to sorted BAM files using samtools"""
-    n, _ = os.path.splitext(os.path.basename(input_file))
-    params = {
-        "program_name": "samtools",
-        "params": "view",
-        "input": "-Sb",
-        "command_line": "#program_name# #params# #input# > #output#"
-    }
-    execute(compose_command(params, input_file=input_file,
-            output_file=os.path.join(output_dir, "{}.bam".format(n))))
-    return os.path.join(output_dir, "{}.bam".format(n))
+"""
+Converts SAM files to sorted BAM files using samtools
 
-
-def samtools_sort_bam_v1(input_file, output_dir):
-    """Sort BAM files using samtools"""
-    n, _ = os.path.splitext(os.path.basename(input_file))
+:param input: the input SAM file
+:param output_dir: the output directory
+:returns: the sorted BAM file
+"""
+def samtools_sam_to_bam(input, output_dir):
+    n, _ = os.path.splitext(os.path.basename(input))   
     params = {
-        "program_name": "samtools",
-        "params": "sort",
-        "output": "-o",
-        "command_line": "#program_name# #params# #input# #output#"
-    }
-    execute(compose_command(params, input_file=input_file,
-            output_file=os.path.join(output_dir, "{}.sorted.bam".format(n))))
-    shutil.move(os.path.join(output_dir, "{}.sorted.bam".format(n)),
-                os.path.join(output_dir, "{}.bam".format(n)))
-    return os.path.join(output_dir, "{}.bam".format(n))
-
-
+        "program_name" : "samtools",
+        "params" : "view",
+        "input" : "-Sb",
+        "command_line" : "#program_name# #params# #input# > #output#"
+    }       
+    execute(compose_command(params, input_file=input, output_file=output_dir+n+".bam"))
+    return output_dir+n+".bam"
+
+
+"""
+Sort BAM files using samtools
+
+:param input: the input BAM file
+:param output_dir: the output directory
+:returns: the sorted BAM file
+"""
+def samtools_sort_bam_v0(input, output_dir):
+    n, _ = os.path.splitext(os.path.basename(input))
+    params = {
+        "program_name" : "samtools",
+        "params" : "sort",
+        "command_line" : "#program_name# #params# #input# #output#"
+    }        
+    execute(compose_command(params, input_file=input, output_file=output_dir+n+".sorted"))
+    return output_dir+n+".sorted.bam"
+
+
+"""
+Sort BAM files using samtools
+
+:param input: the input BAM file
+:param output_dir: the output directory
+:returns: the sorted BAM file
+"""
+def samtools_sort_bam_v1(input, output_dir):
+    n, _ = os.path.splitext(os.path.basename(input))  
+    params = {
+        "program_name" : "samtools",
+        "params" : "sort",
+        "output" : "-o",
+        "command_line" : "#program_name# #params# #input# #output#"
+    }      
+    execute(compose_command(params, input_file=input, output_file=output_dir+n+".sorted.bam"))
+    shutil.move(output_dir+n+".sorted.bam", output_dir+n+".bam")
+    return output_dir+n+".bam"
+
+
+"""
+Generates a FASTA file with the markers form a MetaPhlAn database
+
+:param database: the MetaPhlan markers database
+:param output_dir: the output directory
+"""
 def generate_markers_fasta(database, output_dir):
-    """Generates a FASTA file with the markers form a MetaPhlAn database"""
-    file_out, db_markers_faa = tempfile.mkstemp(
-        dir=output_dir, prefix="db_markers_temp_", suffix=".fna")
+    
+    file_out, db_markers_faa = tempfile.mkstemp(dir=output_dir,prefix="db_markers_temp_",suffix=".fna")
     os.close(file_out)
     bowtie_database, _ = os.path.splitext(database)
     params = {
-        "program_name": "bowtie2-inspect",
-        "command_line": "#program_name# #input# > #output#"
+        "program_name" : "bowtie2-inspect",
+        "command_line" : "#program_name# #input# > #output#"
     }
-    execute(compose_command(params, input_file=bowtie_database,
-            output_file=db_markers_faa))
+    execute(compose_command(params, input_file=bowtie_database, output_file=db_markers_faa))
     return db_markers_faa
 
 
+"""
+Compose a command for further executions
+
+:param params: the params of the command
+:param check: [default=False] check if program is available
+:param input_file: [optional] the input file
+:param database: [optional] the database
+:param output_path: [optional] the output path
+:param output_file: [optional] the output file
+:param nproc: [default=1] the number of procs to use
+"""
 def compose_command(params, check=False, input_file=None, database=None, output_path=None, output_file=None, nproc=1):
-    """Compose a command for further executions. Copied from the PhyloPhlAn 3 code"""
+    program_name = None
     stdin = None
     stdout = None
     environment = os.environ.copy()
     r_output_path = None
     r_output_file = None
     command_line = params['command_line']
-    program_name = params['program_name']
-    command_line = command_line.replace('#program_name#', program_name)
+
+    if 'program_name' in list(params):
+        command_line = command_line.replace('#program_name#', params['program_name'])
+        program_name = params['program_name']
+    else:
+        error('Error: something wrong... '+program_name+' not found!', exit=True)
 
     if check:
         command_line = program_name
 
         if 'version' in list(params):
             command_line = '{} {}'.format(program_name, params['version'])
     else:
         if 'params' in list(params):
             command_line = command_line.replace('#params#', params['params'])
 
         if 'threads' in list(params):
-            command_line = command_line.replace(
-                '#threads#', '{} {}'.format(params['threads'], nproc))
+            command_line = command_line.replace('#threads#', '{} {}'.format(params['threads'], nproc))
 
         if output_path:
             r_output_path = output_path
 
             if 'output_path' in list(params):
-                command_line = command_line.replace(
-                    '#output_path#', '{} {}'.format(params['output_path'], output_path))
+                command_line = command_line.replace('#output_path#', '{} {}'.format(params['output_path'], output_path))
             else:
                 output_file = os.path.join(output_path, output_file)
 
         if input_file:
             inp = input_file
 
             if 'input' in list(params):
@@ -201,16 +313,15 @@
                 command_line = command_line.replace('<', '')
                 command_line = command_line.replace('#input#', '')
                 stdin = inp
             else:
                 command_line = command_line.replace('#input#', inp)
 
         if database and ('database' in list(params)):
-            command_line = command_line.replace(
-                '#database#', '{} {}'.format(params['database'], database))
+            command_line = command_line.replace('#database#', '{} {}'.format(params['database'], database))
 
         if output_file:
             out = output_file
             r_output_file = output_file
 
             if 'output' in list(params):
                 out = '{} {}'.format(params['output'], output_file)
@@ -224,50 +335,15 @@
 
         if 'environment' in list(params):
             new_environment = dict([(var.strip(), val.strip())
                                     for var, val in [a.strip().split('=') for a in params['environment'].split(',')]])
             environment.update(new_environment)
 
     # find string sourrunded with " and make them as one string
-    # TODO: we should use shlex.split for this or drop this ugly function altogether (Michal)
     quotes = [j for j, e in enumerate(command_line) if e == '"']
 
     for s, e in zip(quotes[0::2], quotes[1::2]):
-        command_line = command_line.replace(
-            command_line[s + 1:e], command_line[s + 1:e].replace(' ', '#'))
+        command_line = command_line.replace(command_line[s + 1:e], command_line[s + 1:e].replace(' ', '#'))
 
     return {'command_line': [str(a).replace('#', ' ') for a in re.sub(' +', ' ', command_line.replace('"', '')).split(' ') if a],
             'stdin': stdin, 'stdout': stdout, 'env': environment, 'output_path': r_output_path, 'output_file': r_output_file}
 
-
-def run_command(cmd, shell=False, **kwargs):
-    """
-    Runs a command and checks for exit code
-
-    Args:
-        cmd (str): A command to run
-        shell (bool): Whether to invoke shell
-        **kwargs: additional arguments passed to subprocess.run function
-
-    Returns:
-
-    """
-    if not shell:
-        cmd_s = shlex.split(cmd)
-    else:
-        cmd_s = cmd
-
-    r = sb.run(cmd_s, shell=shell, capture_output=True, **kwargs)
-
-    if r.returncode != 0:
-        stdout = r.stdout
-        stderr = r.stderr
-        if isinstance(stdout, bytes):
-            stdout = stdout.decode()
-        if isinstance(stderr, bytes):
-            stderr = stderr.decode()
-        error(f'Execution failed for command {cmd}', exit=False)
-        error(f'stdout:\n{stdout}', exit=False)
-        error(f'stderr:\n{stderr}', exit=False)
-        error('Exiting', exit=True)
-
-    return r
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/merge_metaphlan_tables.py` & `MetaPhlAn-4b3/metaphlan/utils/merge_metaphlan_tables.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 #!/usr/bin/env python3
 
-
 import argparse
 import os
 import sys
+import re
 import pandas as pd
 from itertools import takewhile
 
-
-def merge(aaastrIn, ostm, gtdb):
+def merge( aaastrIn, ostm ):
     """
     Outputs the table join of the given pre-split string collection.
 
     :param  aaastrIn:   One or more split lines from which data are read.
     :type   aaastrIn:   collection of collections of string collections
+    :param  iCol:       Data column in which IDs are matched (zero-indexed).
+    :type   iCol:       int
     :param  ostm:       Output stream to which matched rows are written.
     :type   ostm:       output stream
     """
 
     listmpaVersion = set()
-    profiles_list = []
-    merged_tables = None
+    merged_tables = pd.DataFrame()
 
     for f in aaastrIn:
-        headers = [x.strip() for x in takewhile(lambda x: x.startswith('#'), open(f))]
-        listmpaVersion.add(headers[0])
-        names = headers[-1].split('#')[1].strip().split('\t')
-
+        with open(f) as fin:
+            headers = [x.strip() for x in takewhile(lambda x: x.startswith('#'), fin)]
+        if len(headers) == 1:
+            names = ['clade_name', 'relative_abundance']
+            index_col = 0
+        if len(headers) >= 4:
+            names = headers[-1].split('#')[1].strip().split('\t')
+            index_col = [0,1]
+
+        mpaVersion = list(filter(re.compile('#mpa_v[0-9]{2,}_CHOCOPhlAn\w*/{0,3}_[0-9]{0,}').match, headers))
+        if len(mpaVersion):
+            listmpaVersion.add(mpaVersion[0])
+        else:
+            print('merge_metaphlan_tables found tables without a header including the database version. Exiting.\n')
+            return
         if len(listmpaVersion) > 1:
-            print('merge_metaphlan_tables: profiles from differrent versions of MetaPhlAn, please profile your '
-                  'samples using the same MetaPhlAn version.\n')
+            print('merge_metaphlan_tables found tables made with different versions of the MetaPhlAn database.\nPlease re-run MetaPhlAn with the same database.\n')
             return
-            
-        iIn = pd.read_csv(f, sep='\t', skiprows=len(headers), names=names, usecols=[0,2] if not gtdb else range(2), index_col=0)
-        profiles_list.append(pd.Series(data=iIn['relative_abundance'], index=iIn.index,
-                                       name=os.path.splitext(os.path.basename(f))[0].replace('_profile', '')))
-
-    merged_tables = pd.concat([merged_tables, pd.concat(profiles_list, axis=1).fillna(0)], axis=1).fillna(0)
-    ostm.write(list(listmpaVersion)[0]+'\n')
-    merged_tables.to_csv(ostm, sep='\t')
-
-
-argp = argparse.ArgumentParser(prog="merge_metaphlan_tables.py",
-                               description="Performs a table join on one or more metaphlan output files.")
-argp.add_argument("aistms", metavar="input.txt", nargs="*", help="One or more tab-delimited text tables to join")
-argp.add_argument("-l", help="Name of file containing the paths to the files to combine")
-argp.add_argument('-o', metavar="output.txt", help="Name of output file in which joined tables are saved")
-argp.add_argument('--overwrite', default=False, action='store_true', help="Overwrite output file if exists")
-argp.add_argument('--gtdb_profiles', action='store_true', default=False, help=("To specify when running the script with GTDB-based profiles"))
-
-argp.usage = (argp.format_usage() + "\nPlease make sure to supply file paths to the files to combine.\n\n" +
-              "If combining 3 files (Table1.txt, Table2.txt, and Table3.txt) the call should be:\n" +
-              "   ./merge_metaphlan_tables.py Table1.txt Table2.txt Table3.txt > output.txt\n\n" +
-              "A wildcard to indicate all .txt files that start with Table can be used as follows:\n" +
-              "    ./merge_metaphlan_tables.py Table*.txt > output.txt")
+        
+        iIn = pd.read_csv(f, 
+                          sep='\t',
+                          skiprows=len(headers),
+                          names = names,
+                          usecols=range(3),
+                        ).fillna('')
+        iIn = iIn.set_index(iIn.columns[index_col].to_list())
+        if merged_tables.empty:
+            merged_tables = iIn.iloc[:,0].rename(os.path.splitext(os.path.basename(f))[0]).to_frame()
+        else:
+            merged_tables = pd.merge(iIn.iloc[:,0].rename(os.path.splitext(os.path.basename(f))[0]).to_frame(),
+                                    merged_tables,
+                                    how='outer', 
+                                    left_index=True, 
+                                    right_index=True
+                                    )
+    if listmpaVersion:
+        ostm.write(list(listmpaVersion)[0]+'\n')
+    merged_tables.fillna('0').reset_index().to_csv(ostm, index=False, sep = '\t')
+
+argp = argparse.ArgumentParser( prog = "merge_metaphlan_tables.py",
+    description = """Performs a table join on one or more metaphlan output files.""")
+argp.add_argument( "aistms",    metavar = "input.txt", nargs = "+",
+    help = "One or more tab-delimited text tables to join" )
+argp.add_argument( '-o',    metavar = "output.txt", nargs = 1,
+    help = "Name of output file in which joined tables are saved" )
 
+__doc__ = "::\n\n\t" + argp.format_help( ).replace( "\n", "\n\t" )
 
-def main( ):
-    args = argp.parse_args()
+argp.usage = argp.format_usage()[7:]+"\n\n\tPlease make sure to supply file paths to the files to combine. If combining 3 files (Table1.txt, Table2.txt, and Table3.txt) the call should be:\n\n\t\tpython merge_metaphlan_tables.py Table1.txt Table2.txt Table3.txt > output.txt\n\n\tA wildcard to indicate all .txt files that start with Table can be used as follows:\n\n\t\tpython merge_metaphlan_tables.py Table*.txt > output.txt"
 
-    if args.l:
-        args.aistms = [x.strip().split()[0] for x in open(args.l)]
-
-    if not args.aistms:
-        print('merge_metaphlan_tables: no inputs to merge!')
-        return
-
-    if args.o and os.path.exists(args.o) and not args.overwrite:
-        print('merge_metaphlan_tables: output file "{}" exists, specify the --overwrite param to ovrewrite it!'.format(args.o))
-        return
-
-    merge(args.aistms, open(args.o, 'w') if args.o else sys.stdout, args.gtdb_profiles)
 
+def main( ):
+    args = argp.parse_args( )
+    if args.o is None:
+        merge(args.aistms, sys.stdout)
+    else:
+        with open(args.o[0], 'w') as fout:
+            merge(args.aistms, fout)
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/metaphlan2krona.py` & `MetaPhlAn-4b3/metaphlan/utils/metaphlan2krona.py`

 * *Files identical despite different names*

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJan21_CHOCOPhlAnSGB_202103.nwk` & `MetaPhlAn-4b3/metaphlan/utils/mpa_v4beta_Jan21_SGB_tree.nwk`

 * *Files identical despite different names*

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/mpa_vJan21_CHOCOPhlAnSGB_202103_SGB2GTDB.tsv` & `MetaPhlAn-4b3/metaphlan/utils/Jan21_SGB2GTDB.tsv`

 * *Files identical despite different names*

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/parallelisation.py` & `MetaPhlAn-4b3/metaphlan/utils/parallelisation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,61 @@
 __author__ = ('Aitor Blanco Miguez (aitor.blancomiguez@unitn.it), '
               'Duy Tin Truong (duytin.truong@unitn.it), '
               'Francesco Asnicar (f.asnicar@unitn.it), '
               'Moreno Zolfo (moreno.zolfo@unitn.it), '
               'Francesco Beghini (francesco.beghini@unitn.it)')
-__version__ = '4.1.1'
-__date__ = '11 Mar 2024'
-
-
-from typing import Iterable
-import itertools as it
+__version__ = '4.beta.3'
+__date__ = '22 Aug 2022'
 
 try:
     from .util_fun import error
 except ImportError:
     from util_fun import error
 from multiprocessing import Event, Pool
 
 CHUNKSIZE = 1
 
-
-def init_terminating(terminating_):
-    """Places terminating in the global namespace of the worker subprocesses. 
-    This allows the worker function to access `terminating` even though it is not passed as an argument to the function.
-
-
-    Args:
-        terminating_ (Event): the initialized terminating event
-    """
+"""
+Places terminating in the global namespace of the worker subprocesses.
+This allows the worker function to access `terminating` even though it is
+not passed as an argument to the function.
+
+:param terminating_: the local terminating variable
+"""
+def init_terminating(terminating_):    
     global terminating
     terminating = terminating_
 
 
-def parallel_execution(arguments):
-    """
-    Executes each parallelized call of a function
-
-    Args:
-        arguments (Tuple[Callable, *Any]): tuple with the function and its arguments
+"""
+Executes each parallelised call of a function
 
-    Returns:
-        function: the call to the function
-    """
+:param arguments: the name of the function and the arguments
+:returns: the result of the parallelised execution
+"""
+def parallel_execution(arguments):
     function, *args = arguments
     if not terminating.is_set():
         try:
             return function(*args)
         except Exception as e:
             terminating.set()
-            raise e
+            raise
     else:
         terminating.set()
 
 
-def iterator_shorter_than(i, ln):
-    try:
-        for _ in range(ln):
-            next(i)
-    except StopIteration:
-        return True
-    return False
-
-
-def execute_pool_iter(args, nprocs, ordered):
-    try:
-        terminating = Event()
-        with Pool(initializer=init_terminating, initargs=(terminating,), processes=nprocs) as pool:
-            if ordered:
-                f = pool.imap
-            else:
-                f = pool.imap_unordered
-
-            for r in f(parallel_execution, args, chunksize=CHUNKSIZE):
-                yield r
-    except Exception as e:
-        error('Parallel execution fails: {}'.format(e), exit=False)
-        raise e
-
-
-def execute_pool(args, nprocs, return_generator=False, ordered=False):
-    """
-    Creates a pool for a parallelized function and returns the results of each execution as a list
-
-    Args:
-        args (Iterable[tuple]): tuple with the function and its arguments
-        nprocs (int): number of procs to use
-        return_generator (bool): Whether to return a non-blocking generator instead of list
-        ordered (bool): Whether the returning results should be in the same order as the input arguments
-
-    Returns:
-        list: the list with the results of the parallel executions
-    """
-    args, args_tmp = it.tee(args)  # duplicate the iterator not to consume it
-    if nprocs == 1 or iterator_shorter_than(args_tmp, 2):  # no need to initialize pool
-        gen = (function(*a) for function, *a in args)
-    else:
-        gen = execute_pool_iter(args, nprocs, ordered)
-        
-    if return_generator:
-        return gen
-    else:
-        return list(gen)
+"""
+Creates a pool for a parallelised function and returns the results of each execution
+as a list
+
+:param args: the name of the function and the arguments
+:param nprocs: the number of threads to use in the pool
+:returns: the result of the parallelised funtion
+"""
+def execute_pool(args, nprocs):
+    terminating = Event()
+    with Pool(initializer=init_terminating, initargs=(terminating,), processes=nprocs) as pool:
+        try:
+            return [_ for _ in pool.imap_unordered(parallel_execution, args, chunksize=CHUNKSIZE)] 
+        except Exception as e:
+            error('Parallel execution fails: '+str(e), init_new_line=True, exit=True)
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/plot_bug.py` & `MetaPhlAn-4b3/metaphlan/utils/plot_bug.py`

 * *Files identical despite different names*

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/plot_tree_graphlan.py` & `MetaPhlAn-4b3/metaphlan/utils/plot_tree_graphlan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env python
 __author__ = ('Duy Tin Truong (duytin.truong@unitn.it), '
               'Aitor Blanco Miguez (aitor.blancomiguez@unitn.it)')
-__version__ = '4.1.1'
-__date__ = '11 Mar 2024'
+__version__ = '4.beta.3'
+__date__    = '22 Aug 2022'
 
 import argparse as ap
 import dendropy
 from io import StringIO
 import re
-import random
 from collections import defaultdict
 import matplotlib.colors as colors
 import subprocess
 
-def for_shuffle():
-  return 0.1
 
 def read_params():
     p = ap.ArgumentParser()
     p.add_argument('-t', '--ifn_tree',
                    required=True,
                    default=None,
                    type=str,
@@ -105,18 +102,15 @@
                 md = substrs[0].replace(args.colorized_metadata + '-', '')
                 metadatas.add(md)
                 node2metadata[nodestr] = md
         else:
             count += 1
             node.taxon = dendropy.Taxon(label='node_%d'%count)
     metadatas = sorted(list(metadatas))
-    color_names = list(colors.TABLEAU_COLORS.keys())
-    color_names_plus = list(colors.CSS4_COLORS.keys())
-    random.shuffle(color_names_plus, for_shuffle)
-    color_names += color_names_plus
+    color_names = list(colors.cnames.keys())
     metadata2color = {}
     for i, md in enumerate(metadatas):
         metadata2color[md] = color_names[i % len(color_names)]
 
     if not args.ofn_prefix:
         args.ofn_prefix = args.ifn_tree
     ofn_tree = args.ofn_prefix + '.graphlantree'
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/pyphlan.py` & `MetaPhlAn-4b3/metaphlan/utils/pyphlan.py`

 * *Files identical despite different names*

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/read_fastx.py` & `MetaPhlAn-4b3/metaphlan/utils/read_fastx.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,23 +110,18 @@
         else:
             discarded = discarded + 1
     # else:
     #     for idx, l in enumerate(fd,1):
     #         avg_read_length = len(l) + avg_read_length
     #         _ = sys.stdout.write(ignore_spaces(l))
 
-    if not idx:
-        sys.stderr.write('Error: no reads found.\n')
-        sys.exit(1)
-
     nreads = idx - discarded
 
     if not nreads:
-        sys.stderr.write('Error: no reads longer than {} bp found.\n'.format(min_len))
-        sys.exit(1)
+        nreads, avg_read_length = 0, 0
 
     return (nreads, avg_read_length)
 
 
 def read_and_write_raw(fd, opened=False, min_len=None, prefix_id=""):
     if opened:  # fd is stdin
         nreads, avg_read_length = read_and_write_raw_int(fd, min_len=min_len, prefix_id=prefix_id)
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/sgb_to_gtdb_profile.py` & `MetaPhlAn-4b3/metaphlan/utils/sgb_to_gtdb_profile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,79 @@
-#!/usr/bin/env python
-__author__ = 'Aitor Blanco (aitor.blancomiguez@unitn.it'
-__version__ = '4.1.1'
-__date__ = '11 Mar 2024'
-
-import os
-import time
+import os, time, sys
 import argparse as ap
+
 try:
-    from .util_fun import info, error
-    from .database_controller import MetaphlanDatabaseController
+    from .util_fun import openw, info, error
 except ImportError:
-    from util_fun import info, error
-    from database_controller import MetaphlanDatabaseController
+    from util_fun import openw, info, error
 
+GTDB_ASSIGNMENT_FILE = os.path.join(os.path.dirname(os.path.abspath(__file__)), "Jan21_SGB2GTDB.tsv")
 
 def read_params():
-    """ Reads and parses the command line arguments of the script
-
-    Returns:
-        namespace: The populated namespace with the command line arguments
-    """
-    p = ap.ArgumentParser(
-        description="", formatter_class=ap.ArgumentDefaultsHelpFormatter)
-    p.add_argument('-i', '--input', type=str,
-                   default=None, help="The input profile")
-    p.add_argument('-d', '--database', type=str, default='latest',
-                   help="The path to the MetaPhlAn PKL database")
-    p.add_argument('-o', '--output', type=str,
-                   default=None, help="The output profile")
+    p = ap.ArgumentParser(description="", formatter_class=ap.ArgumentDefaultsHelpFormatter)
+    p.add_argument('-i', '--input', type=str, default=None,
+                   help="The input profile")
+    p.add_argument('-o', '--output', type=str, default=None,
+                   help="The output profile")
+    
     return p.parse_args()
 
-
 def check_params(args):
-    """Checks the mandatory command line arguments of the script
-
-    Args:
-        args (namespace): the arguments to check
-    """
     if not args.input:
-        error('-i (or --input) must be specified', exit=True)
+        error('-i (or --input) must be specified', exit=True, 
+            init_new_line=True)
     if not args.output:
-        error('-o (or --output) must be specified', exit=True)
-
+        error('-o (or --output) must be specified', exit=True, 
+            init_new_line=True)
 
-def get_gtdb_profile(mpa_profile, gtdb_profile, database):
-    """Creates the GDTB profile from a MPA one
-
-    Args:
-        mpa_profile (str): the path to the input MPA profile
-        gtdb_profile (str): the path to the output GTDB profile
-    """
-    tax_levels = ['d', 'p', 'c', 'o', 'f', 'g', 's']
+def get_gtdb_profile(mpa_profile, gtdb_profile):
+    tax_levels = ['d','p','c','o','f','g','s']
     sgb2gtdb = dict()
-    with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "{}_SGB2GTDB.tsv".format(database)), 'r') as read_file:
+    with open(GTDB_ASSIGNMENT_FILE, 'r') as read_file:
         for line in read_file:
             line = line.strip().split('\t')
             sgb2gtdb[line[0]] = line[1]
+
     with open(gtdb_profile, 'w') as wf:
         with open(mpa_profile, 'r') as rf:
             unclassified = 0
-            abundances = {x: dict() for x in tax_levels}
+            abundances = {x:dict() for x in tax_levels}
             for line in rf:
                 if line.startswith('#mpa_'):
                     wf.write(line)
                     wf.write('#clade_name\trelative_abundance\n')
                 elif line.startswith('UNCLASSIFIED'):
                     unclassified = float(line.strip().split('\t')[2])
                     wf.write('UNCLASSIFIED\t{}\n'.format(unclassified))
                 elif 't__SGB' in line:
                     line = line.strip().split('\t')
                     gtdb_tax = sgb2gtdb[line[0].split('|')[-1][3:]]
-                    if gtdb_tax not in abundances['s']:
+                    if gtdb_tax not in abundances:
                         abundances['s'][gtdb_tax] = 0
                     abundances['s'][gtdb_tax] += float(line[2])
         tax_levels.reverse()
         for tax_level in tax_levels[:-1]:
             for tax in abundances[tax_level]:
                 new_tax = tax.replace(';{}'.format(tax.split(';')[-1]), '')
                 new_level = tax_levels[tax_levels.index(tax_level)+1]
                 if new_tax not in abundances[new_level]:
                     abundances[new_level][new_tax] = 0
-                abundances[new_level][new_tax] += abundances[tax_level][tax]        
+                abundances[new_level][new_tax] += abundances[tax_level][tax]
         tax_levels.reverse()
-        total4level = {x:sum([y for x,y in abundances[x].items()]) for x in tax_levels}
         for tax_level in tax_levels:
             for tax in abundances[tax_level]:
-                wf.write('{}\t{}\n'.format(tax, abundances[tax_level][tax] * 100 / total4level[tax_level]))
-
+                wf.write('{}\t{}\n'.format(tax, abundances[tax_level][tax]))
 
 def main():
     t0 = time.time()
     args = read_params()
     info("Start execution")
     check_params(args)
-    database_controller = MetaphlanDatabaseController(args.database)
-    get_gtdb_profile(args.input, args.output, database_controller.get_database_name())
-    exec_time = time.time() - t0
-    info("Finish execution ({} seconds)".format(round(exec_time, 2)))
 
+    get_gtdb_profile(args.input, args.output)
 
+    exec_time = time.time() - t0
+    info("Finish execution ("+str(round(exec_time, 2))+" seconds)\n", 
+        init_new_line=True)
+	
 if __name__ == "__main__":
-    main()
+	main()
```

### Comparing `MetaPhlAn-4.1.1/metaphlan/utils/strain_transmission.py` & `MetaPhlAn-4b3/metaphlan/utils/strain_transmission.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,324 +1,326 @@
-#!/usr/bin/env python
 __author__ = ('Aitor Blanco (aitor.blancomiguez@unitn.it), '
-              'Mireia Valles-Colomer (mireia.vallescolomer@unitn.it)')
-__version__ = '4.1.1'
-__date__ = '11 Mar 2024'
+             'Mireia Valles-Colomer (mireia.vallescolomer@unitn.it)')
+__version__ = '4.beta.3'
+__date__ = '22 Aug 2022'
 
-
-import os
-import time
+import os, time, sys
 import argparse as ap
+
 try:
-    from .util_fun import info, error
+    from .util_fun import openw, info, error
     from .pyphlan import PpaTree, dist_matrix
 except ImportError:
-    from util_fun import info, error
+    from util_fun import openw, info, error
     from pyphlan import PpaTree, dist_matrix
 
 
 DISTRIBUTION_THRESHOLD = 0.03
 metaphlan_script_install_folder = os.path.dirname(os.path.abspath(__file__))
 DEFAULT_UTILS_FOLDER = os.path.join(metaphlan_script_install_folder)
-PRECOMPUTED_FILE = os.path.join(
-    DEFAULT_UTILS_FOLDER, 'VallesColomerM_2022_Jan21_thresholds.tsv')
+DEFAULT_UTILS_FOLDER = os.environ.get('METAPHLAN_DB_DIR', DEFAULT_UTILS_FOLDER)
+PRECOMPUTED_FILE = os.path.join(DEFAULT_UTILS_FOLDER, 'VallesColomerM_2022_Nov19_thresholds.tsv')
 
 
-def read_params():
-    """ Reads and parses the command line arguments of the script
+"""
+Reads and parses the command line arguments of the script.
 
-    Returns:
-        namespace: The populated namespace with the command line arguments
-    """
-    p = ap.ArgumentParser(
-        description="", formatter_class=ap.ArgumentDefaultsHelpFormatter)
+:returns: the parsed arguments
+"""
+def read_params():
+    p = ap.ArgumentParser(description="", formatter_class=ap.ArgumentDefaultsHelpFormatter)
     p.add_argument('-t', '--tree', type=str, default=None,
                    help="The input tree file")
     p.add_argument('-m', '--metadata', type=str, default=None,
                    help="The input metadata")
     p.add_argument('-o', '--output_dir', type=str, default=None,
                    help="The output directory")
     p.add_argument('--sgb_id', type=str, default=None,
                    help="[Optional] If specified, it will use the precomputed transmisison threshold for the specific SGB from the VallesColomerM_2022 study")
     p.add_argument('--threshold', type=float, default=DISTRIBUTION_THRESHOLD,
                    help="[Optional] A custom distribution threshold value")
     p.add_argument('--precomputed_thresholds_file', type=str, default=PRECOMPUTED_FILE,
                    help="[Optional] The file containing the pre-computed thresholds")
     p.add_argument('--save_dist', action='store_true',
                    help="[Optional] Save the PhyPhlAn pairwise distances file")
+    
     return p.parse_args()
 
 
-def check_params(args):
-    """Checks the mandatory command line arguments of the script
+"""
+Checks the mandatory command line arguments of the script.
 
-    Args:
-        args (namespace): the arguments to check
-    """
+"""
+def check_params(args):
     if not args.tree and not args.dist:
-        error('-t (or --tree) must be specified', exit=True)
+        error('-t (or --tree) must be specified', exit=True, 
+            init_new_line=True)
     if not args.output_dir:
-        error('-o (or --output_dir) must be specified', exit=True)
+        error('-o (or --output_dir) must be specified', exit=True, 
+            init_new_line=True)
     elif not os.path.exists(args.output_dir):
-        error('The directory {} does not exist'.format(
-            args.output_dir), exit=True)
+        error('The directory {} does not exist'.format(args.output_dir), exit=True, 
+            init_new_line=True)
     if not args.metadata:
-        error('-m (or --metadata) must be specified', exit=True)
+        error('-m (or --metadata) must be specified', exit=True, 
+            init_new_line=True)
 
 
-def tree_pairwisedist(tree, normalise, matrix, output):
-    """Calls the main function on the tree_pairwisedist.py Script of the Pyphlan tool
+"""
+Calls the main function on the tree_pairwisedist.py Script of the Pyphlan tool
 
-    Args:
-        tree (str): the path to the input tree
-        normalise (bool): whether to normalize the distances
-        matrix (bool): whether the output is a matrix
-        output (str): the path to the output distances file
-    """
+:param tree: the input Newick tree
+:normalise: whether normalise the distances with respect to the total branch length
+:matrix: whether report the results as a matrix
+:output: the output distances file
+"""
+def tree_pairwisedist(tree, normalise, matrix, output):
     ppatree = PpaTree(tree)
-    dists = dist_matrix(ppatree.tree)
+
+    dists = dist_matrix(ppatree.tree) 
     tbl = ppatree.tree.total_branch_length() if normalise else 1.0
-    with open(output, 'w') as out:
+
+    with openw(output) as out:
         if matrix:
             keys = sorted(dists.keys())
-            out.write("\t".join(["ID"]+keys) + "\n")
+            out.write( "\t".join(["ID"]+keys) +"\n" )
             for k1 in keys:
-                out.write("\t".join([k1]+[str(dists[k1][k2]/tbl)
-                          for k2 in keys]) + "\n")
+                out.write( "\t".join([k1]+[str(dists[k1][k2]/tbl) for k2 in keys]) +"\n" )
         else:
-            for k1, v1 in dists.items():
-                for k2, v2 in v1.items():
+            for k1,v1 in dists.items():
+                for k2,v2 in v1.items():
                     if k1 < k2:
-                        out.write("\t".join([k1, k2, str(v2/tbl)]) + "\n")
-
+                        out.write( "\t".join([k1,k2,str(v2/tbl)]) +"\n" )
 
-def get_metadata_info(metadata):
-    """Gets all the information about the families from the metadata
 
-    Args:
-        metadata (str): the path to the metadata file
+"""
+Gets all the information about the families from the metadata
 
-    Returns:
-        (dict, dict): a tuple with the info about relations and the samples
-    """
+:param metadata: the metadata
+:returns: the tree about the samples in the metadata and
+    the samples to metadata dictionary
+"""
+def get_metadata_info(metadata):
     info = dict()
     samples = dict()
     with open(metadata, 'r') as metadata_file:
         metadata_file.readline()
         for line in metadata_file:
             line = line.strip().split("\t")
+
             relation = line[2]
             subject = line[1]
             timepoint = line[3]
             sample = line[0]
+
+            
             if relation not in info:
                 info[relation] = dict()
             if subject not in info[relation]:
                 info[relation][subject] = dict()
             if timepoint not in info[relation][subject]:
                 info[relation][subject][timepoint] = sample
+
             samples[sample] = [relation, subject, timepoint]
-    return info, samples
 
+    return info, samples
 
-def parse_distances(distances_path):
-    """Parses the pairwise distances from the generated distances file
 
-    Args:
-        distances_path (str): the path to the distance matrix
+""""
+Parses the pairwise distances from the generated distances file
 
-    Returns:
-        list: a list with the distances
-    """
+:param distances_path: the pairwise distances file
+:returns: the pairwise distances as a list
+"""
+def parse_distances(distances_path):
     distances = list()
     with open(distances_path, 'r') as distances_file:
         for line in distances_file:
             line = line.strip().split("\t")
             distances.append({"1": line[0], "2": line[1], "dist": line[2]})
     return distances
 
 
-def get_nodes(distances):
-    """Gets the nodes of the tree
-
-    Args:
-        distances (list): a list with the distances between nodes
+"""
+Gets the nodes of the tree
 
-    Returns:
-        set: the list nodes in the tree
-    """
+:param distances: the pairwise distances from the tree
+:returns: the nodes of the tree as a set
+"""
+def get_nodes(distances):
     nodes = set()
     for line in distances:
         nodes.add(line["1"])
         nodes.add(line["2"])
     return nodes
 
 
-def get_training_nodes(nodes, metadata):
-    """Gets the training nodes from the metadata
+"""
+Gets the training nodes from the metadata
 
-    Args:
-        nodes (set): the list of the nodes in the tree
-        metadata (str): the metadata file
-
-    Returns:
-        (dict, dict): a tuplw with the training nodes and the metadata of the samples
-    """
+:param nodes: the tree nodes
+:param metadata: the metadata file
+:returns: the training nodes as a list and the samples to metadata dictionary
+"""
+def get_training_nodes(nodes, metadata):
     metadata_info, metadata_samples = get_metadata_info(metadata)
     training_nodes = dict()
+
     for relation in metadata_info:
         for subject in metadata_info[relation]:
             for timepoint in metadata_info[relation][subject]:
                 sample = metadata_info[relation][subject][timepoint]
                 training_nodes[sample] = metadata_samples[sample]
                 break
+
     for node in nodes:
         if node not in metadata_samples:
-            training_nodes[node] = list()
+            training_nodes[node]=list()
+
     return training_nodes, metadata_samples
 
 
-def get_training_distances(training_nodes, pairwise_distances):
-    """Gets the distances between the training nodes
+"""
+Gets the distances between the training nodes
 
-    Args:
-        training_nodes (list): the ditionary of the training nodes
-        pairwise_distances (list): the list of the pairwise distances
-
-    Returns:
-        list: the list of training distances
-    """
+:param training_nodes: the training nodes
+:param pairwise_distances: a list with the pairwise distances
+:param transmission_type: the type of transmission events to report
+:returns: the training distances as a list
+"""
+def get_training_distances(training_nodes, pairwise_distances):
     training_distances = list()
     for pair in pairwise_distances:
         if pair["1"] in training_nodes and pair["2"] in training_nodes:
             if not training_nodes[pair['1']] or not training_nodes[pair['2']]:
                 training_distances.append(pair)
             elif not training_nodes[pair['1']][0] == training_nodes[pair['2']][0]:
                 training_distances.append(pair)
+
     return training_distances
 
 
-def get_threshold(training_distances, distr_threshold):
-    """Gets the threshold defining strain transmission
+"""
+Gets the threshold defining strain transmission
 
-    Args:
-        training_distances (list): the list of training distances
-        distr_threshold (float): the distribution threshold
-
-    Returns:
-        float: the inferred threshold
-    """
+:param training_distances: the distances between the training nodes
+:param distr_threshold: the distribution threshold
+:returns: the strain transmission threshold
+"""
+def get_threshold(training_distances, distr_threshold):
     distances = list()
     for distance in training_distances:
         distances.append(float(distance['dist']))
     distances.sort()
     return distances[int(len(distances)*distr_threshold)]
 
-
+    
+"""
+Gets the transmission events using a calculated threshold
+
+:param pairwise_distances: the pairwise distances
+:param metadata_samples: the sample to metadata dictionary
+:param threshold: the calculated threshold
+:returns: the transmission events as a list
+"""
 def get_transmission_events(pairwise_distances, metadata_samples, threshold):
-    """Gets the transmission events using a calculated threshold
-
-    Args:
-        pairwise_distances (list): the list of the pairwise distances
-        metadata_samples (dict): the dictionary with the samples metadata
-        threshold (float): the infered threshold
-
-    Returns:
-        list: the list with the transmission events
-    """
     transmission_events = list()
     for pair in pairwise_distances:
         if pair['1'] in metadata_samples and pair['2'] in metadata_samples:
             if not metadata_samples[pair['1']][1] == metadata_samples[pair['2']][1] and float(pair['dist']) <= threshold:
-                if metadata_samples[pair['1']][0] == metadata_samples[pair['2']][0]:
+                if metadata_samples[pair['1']][0] == metadata_samples[pair['2']][0]:   
                     transmission_events.append(pair)
+
     return transmission_events
 
 
-def write_transmission_events(transmission_events, threshold, output_dir):
-    """Writes the detected transmission events to file
+"""
+Writes the detected transmission events to file
 
-    Args:
-        transmission_events (list): the list with the transmission events
-        threshold (float): the infered threshold
-        output_dir (str): the output directory
-    """
+:param transmission_events: the detected transmission events
+:param threshold: the calculated threshold
+:param output_dir: the output directory to store the results
+:param metadata_samples: the sample to metadata dictionary
+"""
+def write_transmission_events(transmission_events, threshold, output_dir, metadata_samples):
     with open(os.path.join(output_dir, "transmission_events.info"), 'w') as report:
-        report.write(
-            "Selected strain-transmission threshold: {}\n".format(threshold))
-        report.write("Number of transmission events: {}\n\n".format(
-            len(transmission_events)))
+        report.write("Selected strain-transmission threshold: "+str(threshold)+"\n")
+        report.write("Number of transmission events: "+str(len(transmission_events))+"\n\n")
         for event in transmission_events:
-            report.write(event['1']+" <-> "+event['2']+"\n")
+            report.write(event['1']+" <-> "+event['2']+"\n") 
 
+"""
+Gets the precomputed threshold from VallesColomerM_2022 study
 
+:param sgb_id: the SGB id
+:returns: the transmission threshold
+"""
 def get_precomputed_threshold(sgb_id, precomputed_thresholds_file):
-    """Gets the precomputed threshold from VallesColomerM_2022 study
-
-    Args:
-        sgb_id (str): the SGB id
-        precomputed_thresholds_file (str): the path to the precomputed thresholds
-
-    Returns:
-        float: the precomputed threshold
-    """
     sgb2thres = dict()
     with open(precomputed_thresholds_file, 'r') as rf:
         rf.readline()
         for line in rf:
             line = line.strip().split('\t')
             sgb2thres[line[0]] = line[1]
     if sgb_id not in sgb2thres:
-        error('The SGB specified "{}" has not been precomputed'.format(
-            sgb_id), exit=True)
+        error('The SGB specified "{}" has not been precomputed'.format(sgb_id), exit=True, init_new_line=True)
     else:
         return float(sgb2thres[sgb_id])
 
+"""
+Identifies transmission events in phylogenetic trees
 
+:param tree: the input Newick tree
+:param metadata: the metadata file
+:param distr_threshold: the distribution threshold
+:param sgb_id: the SGB id
+:param precomputed_thresholds_file: the file containing the precomputed thresholds
+:param save_dist: whether to save the pairwise distances file
+:param output_dir: the output directory to store the results
+"""
 def strain_transmission(tree, metadata, distr_threshold, sgb_id, precomputed_thresholds_file, save_dist, output_dir):
-    """Identifies transmission events in phylogenetic trees
-
-    Args:
-        tree (str): The path to the tree
-        metadata (str): The path to the metadata file
-        distr_threshold (float): the distribution threshold
-        sgb_id (str): the SGB id
-        precomputed_thresholds_file (str): the path to the precomputed thresholds
-        save_dist (bool): whether to save the distance matrix
-        output_dir (str): the output directory
-    """
     normalise = True
     matrix = False
-    distances_file = "{}.dist".format(tree)
-    tree_pairwisedist(tree, normalise, matrix,
-                      os.path.join(output_dir, distances_file))
-    pairwise_distances = parse_distances(
-        os.path.join(output_dir, distances_file))
+    distances_file = tree+".dist"
+    tree_pairwisedist(tree, normalise, matrix, os.path.join(output_dir, distances_file))
+    pairwise_distances = parse_distances(os.path.join(output_dir, distances_file)) 
     if not save_dist:
         os.remove(os.path.join(output_dir, distances_file))
+
     nodes = get_nodes(pairwise_distances)
-    training_nodes, metadata_samples = get_training_nodes(nodes, metadata)
-    training_distances = get_training_distances(
-        training_nodes, pairwise_distances)
+    training_nodes, metadata_samples = get_training_nodes(nodes, metadata)    
+    training_distances = get_training_distances(training_nodes, pairwise_distances)
     if sgb_id is None:
         threshold = get_threshold(training_distances, distr_threshold)
     else:
-        threshold = get_threshold(training_distances, get_precomputed_threshold(
-            sgb_id, precomputed_thresholds_file))
-    transmission_events = get_transmission_events(
-        pairwise_distances, metadata_samples, threshold)
-    write_transmission_events(transmission_events, threshold, output_dir)
+        threshold = get_threshold(training_distances, get_precomputed_threshold(sgb_id, precomputed_thresholds_file))
 
+    transmission_events = get_transmission_events(pairwise_distances, metadata_samples, threshold)
+    write_transmission_events(transmission_events, threshold, output_dir, metadata_samples)
 
+
+"""
+Main call
+
+:param tree: the input Newick tree
+:param metadata: the metadata file
+:param threshold: the distribution threshold
+:param sgb_id: the SGB id
+:param precomputed_thresholds_file: the file containing the precomputed thresholds
+:param save_dist: whether to save the pairwise distances file
+:param output_dir: the output directory to store the results
+"""
 def main():
     t0 = time.time()
     args = read_params()
     info("Start execution")
     check_params(args)
-    strain_transmission(args.tree, args.metadata, args.threshold, args.sgb_id,
-                        args.precomputed_thresholds_file, args.save_dist, args.output_dir)
-    exec_time = time.time() - t0
-    info("Finish execution ({} seconds)".format(round(exec_time, 2)))
 
+    strain_transmission(args.tree, args.metadata, args.threshold, args.sgb_id, args.precomputed_thresholds_file, args.save_dist, args.output_dir)
 
+    exec_time = time.time() - t0
+    info("Finish execution ("+str(round(exec_time, 2))+" seconds)\n", 
+        init_new_line=True)
+	
 if __name__ == "__main__":
-    main()
+	main()
+
```

### Comparing `MetaPhlAn-4.1.1/setup.py` & `MetaPhlAn-4b3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,55 +2,43 @@
 from setuptools.command.install import install
 from io import open
 import sys, shutil, os, zipfile, tarfile, subprocess, tempfile, re, time
 from urllib.request import urlretrieve
 
 from metaphlan import download_unpack_zip
 
-
-install_requires = ['numpy', 'h5py', 'biom-format', 'biopython', 'pandas', 'scipy', 'hclust2', 'requests', 'dendropy', 'pysam', 'phylophlan'],
+install_requires = ['numpy', 'h5py', 'biom-format', 'biopython', 'pandas', 'scipy', 'requests', 'dendropy', 'pysam', 'cmseq', 'phylophlan'],
 
 if sys.version_info[0] < 3:
     sys.stdout.write('MetaPhlAn requires Python 3 or higher. Please update you Python installation')
 
 setuptools.setup(
     name='MetaPhlAn',
-    version='4.1.1',
+    version='4.beta.3',
     author='Aitor Blanco-Miguez',
     author_email='aitor.blancomiguez@unitn.it',
     url='http://github.com/biobakery/MetaPhlAn/',
     license='LICENSE.txt',
     packages=setuptools.find_packages(),
     package_data = { 'metaphlan' : [
         'metaphlan_databases/*.txt',
         'utils/*',
-        'utils/treeshrink/*',
-        'utils/treeshrink/scripts/*',
-        'utils/treeshrink/R_scripts/*',
-        'utils/treeshrink/Rlib/BMS/*',
-        'utils/treeshrink/Rlib/BMS/*/*',
-    ] },    
+    ]},
     entry_points={
         'console_scripts': [
             'metaphlan = metaphlan.metaphlan:main',
             'strainphlan = metaphlan.strainphlan:main',
             'add_metadata_tree.py = metaphlan.utils.add_metadata_tree:main',
             'extract_markers.py = metaphlan.utils.extract_markers:main',
             'merge_metaphlan_tables.py  = metaphlan.utils.merge_metaphlan_tables:main',
-            'merge_vsc_tables.py  = metaphlan.utils.merge_vsc_tables:main',
             'plot_tree_graphlan.py = metaphlan.utils.plot_tree_graphlan:main',
             'read_fastx.py = metaphlan.utils.read_fastx:main',
             'sample2markers.py = metaphlan.utils.sample2markers:main',
             'strain_transmission.py = metaphlan.utils.strain_transmission:main',
             'sgb_to_gtdb_profile.py = metaphlan.utils.sgb_to_gtdb_profile:main',
-            'metaphlan2krona.py = metaphlan.utils.metaphlan2krona:main',
-            'run_treeshrink.py = metaphlan.utils.treeshrink.run_treeshrink:main',
-            'treeshrink.py = metaphlan.utils.treeshrink.treeshrink:main',
-            'create_toy_database.py = metaphlan.utils.create_toy_database:main',
-            'fix_relab_mpa4.py = metaphlan.utils.fix_relab_mpa4:main',
         ]
     },
     description='MetaPhlAn is a computational tool for profiling the composition of microbial communities (Bacteria, Archaea and Eukaryotes) from metagenomic shotgun sequencing data (i.e. not 16S) with species-level. With the newly added StrainPhlAn module, it is now possible to perform accurate strain-level microbial profiling.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=install_requires
 )
```

