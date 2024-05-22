# Comparing `tmp/sn_trackeval-0.2.0.tar.gz` & `tmp/sn_trackeval-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sn_trackeval-0.2.0.tar", last modified: Tue May 21 18:12:51 2024, max compression
+gzip compressed data, was "sn_trackeval-0.2.1.tar", last modified: Wed May 22 08:36:44 2024, max compression
```

## Comparing `sn_trackeval-0.2.0.tar` & `sn_trackeval-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.415256 sn_trackeval-0.2.0/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1072 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/LICENSE
--rw-r--r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    15685 2024-05-21 18:12:51.415256 sn_trackeval-0.2.0/PKG-INFO
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    13561 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/Readme.md
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1140 2024-05-21 18:12:41.000000 sn_trackeval-0.2.0/pyproject.toml
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)       38 2024-05-21 18:12:51.415256 sn_trackeval-0.2.0/setup.cfg
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)       38 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/setup.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.415256 sn_trackeval-0.2.0/sn_trackeval.egg-info/
--rw-r--r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    15685 2024-05-21 18:12:51.000000 sn_trackeval-0.2.0/sn_trackeval.egg-info/PKG-INFO
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1882 2024-05-21 18:12:51.000000 sn_trackeval-0.2.0/sn_trackeval.egg-info/SOURCES.txt
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        1 2024-05-21 18:12:51.000000 sn_trackeval-0.2.0/sn_trackeval.egg-info/dependency_links.txt
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)       90 2024-05-21 18:12:51.000000 sn_trackeval-0.2.0/sn_trackeval.egg-info/requires.txt
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)       10 2024-05-21 18:12:51.000000 sn_trackeval-0.2.0/sn_trackeval.egg-info/top_level.txt
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.399255 sn_trackeval-0.2.0/test/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     7248 2024-05-21 12:57:39.000000 sn_trackeval-0.2.0/test/test_gsr.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.399255 sn_trackeval-0.2.0/tests/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     3495 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/tests/test_all_quick.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     2749 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/tests/test_davis.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     6734 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/tests/test_metrics.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     2725 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/tests/test_mot17.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     2860 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/tests/test_mots.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.399255 sn_trackeval-0.2.0/trackeval/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)      116 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/__init__.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     2323 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/_timing.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.403256 sn_trackeval-0.2.0/trackeval/baselines/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)      110 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/__init__.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    12727 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/baseline_utils.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     3330 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/non_overlap.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     8723 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/pascal_colormap.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     5976 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/stp.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     3111 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/thresholder.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     3417 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/baselines/vizualize.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.411256 sn_trackeval-0.2.0/trackeval/datasets/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)      647 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/__init__.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    17008 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/_base_dataset.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    16583 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/bdd100k.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1848 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.411256 sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/__init__.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    31062 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/burst_base.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    34703 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/burst_ow_base.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1588 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/convert_burst_format_to_tao_format.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    11845 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/format_converter.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     3173 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/burst_ow.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    14161 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/davis.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    24673 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/head_tracking_challenge.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    21536 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/kitti_2d_box.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    22374 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/kitti_mots.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    23964 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/mot_challenge_2d_box.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    23607 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/mots_challenge.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    24951 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/person_path_22.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    28114 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/rob_mots.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1270 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/rob_mots_classmap.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     5817 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/run_rob_mots.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    33917 2024-05-21 14:36:52.000000 sn_trackeval-0.2.0/trackeval/datasets/soccernet_gs.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    29833 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/tao.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    33918 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/tao_ow.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    19620 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/datasets/youtube_vis.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    12740 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/eval.py
-drwxrwxr-x   0 vjoosdeterb  (1001) vjoosdeterb  (1001)        0 2024-05-21 18:12:51.415256 sn_trackeval-0.2.0/trackeval/metrics/
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)      212 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/__init__.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     5025 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/_base_metric.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     9166 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/clear.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     1584 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/count.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    10489 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/hota.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     6205 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/identity.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     5514 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/ideucl.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    13021 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/j_and_f.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)    20841 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/track_map.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     5881 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/metrics/vace.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     8400 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/plotting.py
--rw-rw-r--   0 vjoosdeterb  (1001) vjoosdeterb  (1001)     5806 2024-05-21 09:54:05.000000 sn_trackeval-0.2.0/trackeval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.352300 sn_trackeval-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-22 08:36:44.352300 sn_trackeval-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:36:44.352300 sn_trackeval-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.352300 sn_trackeval-0.2.1/sn_trackeval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-22 08:36:44.000000 sn_trackeval-0.2.1/sn_trackeval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-22 08:36:44.000000 sn_trackeval-0.2.1/sn_trackeval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:36:44.000000 sn_trackeval-0.2.1/sn_trackeval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 08:36:44.000000 sn_trackeval-0.2.1/sn_trackeval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 08:36:44.000000 sn_trackeval-0.2.1/sn_trackeval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.344300 sn_trackeval-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/tests/test_all_quick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/tests/test_davis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/tests/test_mot17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/tests/test_mots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.344300 sn_trackeval-0.2.1/trackeval/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/_timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.344300 sn_trackeval-0.2.1/trackeval/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12727 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/baseline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/non_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/pascal_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/stp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/thresholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/baselines/vizualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.348300 sn_trackeval-0.2.1/trackeval/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17008 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/_base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/bdd100k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.348300 sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31062 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/burst_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34703 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/burst_ow_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/convert_burst_format_to_tao_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11845 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/format_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/burst_ow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/davis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24673 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/head_tracking_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21536 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/kitti_2d_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/kitti_mots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23964 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/mot_challenge_2d_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/mots_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/person_path_22.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/rob_mots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/rob_mots_classmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/run_rob_mots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33917 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/soccernet_gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29833 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/tao.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33918 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/tao_ow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19620 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/datasets/youtube_vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:44.352300 sn_trackeval-0.2.1/trackeval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/_base_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/hota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/ideucl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/j_and_f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/track_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/metrics/vace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-22 08:36:39.000000 sn_trackeval-0.2.1/trackeval/utils.py
```

### Comparing `sn_trackeval-0.2.0/LICENSE` & `sn_trackeval-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/PKG-INFO` & `sn_trackeval-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: sn-trackeval
-Version: 0.2.0
+Version: 0.2.1
 Summary: Code for evaluating object tracking
-Author: Arne Hoffhues
-Author-email: Vladimir Somers <somers.vladimir@gmail.com>, Jonathon Luiten <jonoluiten@gmail.com>, Victor Joos <victorjoosdtb@gmail.com>
+Author-email: Vladimir Somers <somers.vladimir@gmail.com>, Jonathon Luiten <jonoluiten@gmail.com>, Arne Hoffhues <no-email@example.com>, Victor Joos <victorjoosdtb@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Jonathon Luiten
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `sn_trackeval-0.2.0/Readme.md` & `sn_trackeval-0.2.1/Readme.md`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/pyproject.toml` & `sn_trackeval-0.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "sn-trackeval"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name = "Vladimir Somers", email = "somers.vladimir@gmail.com"},
     {name = "Jonathon Luiten", email = "jonoluiten@gmail.com"},
-    {name = "Arne Hoffhues"},
+    {name = "Arne Hoffhues", email = "no-email@example.com"},
     {name = "Victor Joos", email = "victorjoosdtb@gmail.com"},
 ]
 description = "Code for evaluating object tracking"
 readme = "Readme.md"
 urls = {homepage = "https://github.com/SoccerNet/sn-trackeval"}
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `sn_trackeval-0.2.0/sn_trackeval.egg-info/PKG-INFO` & `sn_trackeval-0.2.1/sn_trackeval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: sn-trackeval
-Version: 0.2.0
+Version: 0.2.1
 Summary: Code for evaluating object tracking
-Author: Arne Hoffhues
-Author-email: Vladimir Somers <somers.vladimir@gmail.com>, Jonathon Luiten <jonoluiten@gmail.com>, Victor Joos <victorjoosdtb@gmail.com>
+Author-email: Vladimir Somers <somers.vladimir@gmail.com>, Jonathon Luiten <jonoluiten@gmail.com>, Arne Hoffhues <no-email@example.com>, Victor Joos <victorjoosdtb@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Jonathon Luiten
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `sn_trackeval-0.2.0/sn_trackeval.egg-info/SOURCES.txt` & `sn_trackeval-0.2.1/sn_trackeval.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.py
 sn_trackeval.egg-info/PKG-INFO
 sn_trackeval.egg-info/SOURCES.txt
 sn_trackeval.egg-info/dependency_links.txt
 sn_trackeval.egg-info/requires.txt
 sn_trackeval.egg-info/top_level.txt
-test/test_gsr.py
 tests/test_all_quick.py
 tests/test_davis.py
 tests/test_metrics.py
 tests/test_mot17.py
 tests/test_mots.py
 trackeval/__init__.py
 trackeval/_timing.py
```

### Comparing `sn_trackeval-0.2.0/tests/test_all_quick.py` & `sn_trackeval-0.2.1/tests/test_all_quick.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/tests/test_davis.py` & `sn_trackeval-0.2.1/tests/test_davis.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/tests/test_metrics.py` & `sn_trackeval-0.2.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/tests/test_mot17.py` & `sn_trackeval-0.2.1/tests/test_mot17.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/tests/test_mots.py` & `sn_trackeval-0.2.1/tests/test_mots.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/_timing.py` & `sn_trackeval-0.2.1/trackeval/_timing.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/baselines/baseline_utils.py` & `sn_trackeval-0.2.1/trackeval/baselines/baseline_utils.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/baselines/non_overlap.py` & `sn_trackeval-0.2.1/trackeval/baselines/non_overlap.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/baselines/pascal_colormap.py` & `sn_trackeval-0.2.1/trackeval/baselines/pascal_colormap.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/baselines/stp.py` & `sn_trackeval-0.2.1/trackeval/baselines/stp.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/baselines/thresholder.py` & `sn_trackeval-0.2.1/trackeval/baselines/thresholder.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/baselines/vizualize.py` & `sn_trackeval-0.2.1/trackeval/baselines/vizualize.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/__init__.py` & `sn_trackeval-0.2.1/trackeval/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/_base_dataset.py` & `sn_trackeval-0.2.1/trackeval/datasets/_base_dataset.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/bdd100k.py` & `sn_trackeval-0.2.1/trackeval/datasets/bdd100k.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/burst.py` & `sn_trackeval-0.2.1/trackeval/datasets/burst.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/burst_base.py` & `sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/burst_base.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/burst_ow_base.py` & `sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/burst_ow_base.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/convert_burst_format_to_tao_format.py` & `sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/convert_burst_format_to_tao_format.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/burst_helpers/format_converter.py` & `sn_trackeval-0.2.1/trackeval/datasets/burst_helpers/format_converter.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/burst_ow.py` & `sn_trackeval-0.2.1/trackeval/datasets/burst_ow.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/davis.py` & `sn_trackeval-0.2.1/trackeval/datasets/davis.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/head_tracking_challenge.py` & `sn_trackeval-0.2.1/trackeval/datasets/head_tracking_challenge.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/kitti_2d_box.py` & `sn_trackeval-0.2.1/trackeval/datasets/kitti_2d_box.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/kitti_mots.py` & `sn_trackeval-0.2.1/trackeval/datasets/kitti_mots.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/mot_challenge_2d_box.py` & `sn_trackeval-0.2.1/trackeval/datasets/mot_challenge_2d_box.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/mots_challenge.py` & `sn_trackeval-0.2.1/trackeval/datasets/mots_challenge.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/person_path_22.py` & `sn_trackeval-0.2.1/trackeval/datasets/person_path_22.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/rob_mots.py` & `sn_trackeval-0.2.1/trackeval/datasets/rob_mots.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/rob_mots_classmap.py` & `sn_trackeval-0.2.1/trackeval/datasets/rob_mots_classmap.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/run_rob_mots.py` & `sn_trackeval-0.2.1/trackeval/datasets/run_rob_mots.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/soccernet_gs.py` & `sn_trackeval-0.2.1/trackeval/datasets/soccernet_gs.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/tao.py` & `sn_trackeval-0.2.1/trackeval/datasets/tao.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/tao_ow.py` & `sn_trackeval-0.2.1/trackeval/datasets/tao_ow.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/datasets/youtube_vis.py` & `sn_trackeval-0.2.1/trackeval/datasets/youtube_vis.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/eval.py` & `sn_trackeval-0.2.1/trackeval/eval.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/_base_metric.py` & `sn_trackeval-0.2.1/trackeval/metrics/_base_metric.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/clear.py` & `sn_trackeval-0.2.1/trackeval/metrics/clear.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/count.py` & `sn_trackeval-0.2.1/trackeval/metrics/count.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/hota.py` & `sn_trackeval-0.2.1/trackeval/metrics/hota.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/identity.py` & `sn_trackeval-0.2.1/trackeval/metrics/identity.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/ideucl.py` & `sn_trackeval-0.2.1/trackeval/metrics/ideucl.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/j_and_f.py` & `sn_trackeval-0.2.1/trackeval/metrics/j_and_f.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/track_map.py` & `sn_trackeval-0.2.1/trackeval/metrics/track_map.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/metrics/vace.py` & `sn_trackeval-0.2.1/trackeval/metrics/vace.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/plotting.py` & `sn_trackeval-0.2.1/trackeval/plotting.py`

 * *Files identical despite different names*

### Comparing `sn_trackeval-0.2.0/trackeval/utils.py` & `sn_trackeval-0.2.1/trackeval/utils.py`

 * *Files identical despite different names*

