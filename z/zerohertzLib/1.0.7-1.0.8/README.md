# Comparing `tmp/zerohertzLib-1.0.7.tar.gz` & `tmp/zerohertzLib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.7.tar", last modified: Tue May  7 15:17:43 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.8.tar", last modified: Wed May 22 16:26:47 2024, max compression
```

## Comparing `zerohertzLib-1.0.7.tar` & `zerohertzLib-1.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 15:17:38.000000 zerohertzLib-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-07 15:17:38.000000 zerohertzLib-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-05-07 15:17:38.000000 zerohertzLib-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-05-07 15:17:38.000000 zerohertzLib-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     7698 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     5264 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    44758 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.642015 zerohertzLib-1.0.7/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22463 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17516 2024-05-07 15:17:39.000000 zerohertzLib-1.0.7/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:17:43.634014 zerohertzLib-1.0.7/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-05-07 15:17:43.000000 zerohertzLib-1.0.7/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-05-07 15:17:43.000000 zerohertzLib-1.0.7/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 15:17:43.000000 zerohertzLib-1.0.7/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-07 15:17:43.000000 zerohertzLib-1.0.7/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 15:17:43.000000 zerohertzLib-1.0.7/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.252767 zerohertzLib-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-22 16:26:41.000000 zerohertzLib-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-22 16:26:41.000000 zerohertzLib-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-05-22 16:26:47.252767 zerohertzLib-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-05-22 16:26:41.000000 zerohertzLib-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 16:26:47.252767 zerohertzLib-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4672 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     7698 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.248767 zerohertzLib-1.0.8/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.248767 zerohertzLib-1.0.8/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    44458 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.248767 zerohertzLib-1.0.8/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11652 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.252767 zerohertzLib-1.0.8/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22463 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17516 2024-05-22 16:26:42.000000 zerohertzLib-1.0.8/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:26:47.244767 zerohertzLib-1.0.8/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-05-22 16:26:47.000000 zerohertzLib-1.0.8/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-22 16:26:47.000000 zerohertzLib-1.0.8/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 16:26:47.000000 zerohertzLib-1.0.8/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-22 16:26:47.000000 zerohertzLib-1.0.8/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-22 16:26:47.000000 zerohertzLib-1.0.8/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.7/LICENSE` & `zerohertzLib-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/PKG-INFO` & `zerohertzLib-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.7
+Version: 1.0.8
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -81,9 +80,7 @@
 <p align="center">
     <img src="https://github.com/Zerohertz/Zerohertz/assets/42334717/85c44efa-1440-4962-a6e5-7453b0bdc689" width="600">
 </p>
 
 ```python
 import zerohertzLib as zz
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.7 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.8 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
-Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Author-email: ohg3417@gmail.com License: MIT Classifier: Development Status ::
+5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0 Description-Content-Type: text/markdown Provides-
 Extra: api Provides-Extra: mlops Provides-Extra: quant Provides-Extra: all
 License-File: LICENSE
   [https://github.com/Zerohertz/Zerohertz/assets/42334717/90adcc0f-c6ec-4aca-
```

### Comparing `zerohertzLib-1.0.7/README.md` & `zerohertzLib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/setup.py` & `zerohertzLib-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_algorithm.py` & `zerohertzLib-1.0.8/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_api.py` & `zerohertzLib-1.0.8/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_logging.py` & `zerohertzLib-1.0.8/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_plot.py` & `zerohertzLib-1.0.8/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_quant.py` & `zerohertzLib-1.0.8/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_util.py` & `zerohertzLib-1.0.8/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/test/test_vision.py` & `zerohertzLib-1.0.8/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/__init__.py` & `zerohertzLib-1.0.8/zerohertzLib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.7"
+__version__ = "v1.0.8"
```

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.8/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.8/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/api/github.py` & `zerohertzLib-1.0.8/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.8/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.8/zerohertzLib/api/open_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,22 @@
         .. image:: _static/examples/static/api.OpenAI.client.gif
             :align: center
             :width: 600px
     """
 
     def __init__(self, api_key: str) -> None:
         super().__init__(api_key=api_key)
-        self.model_dict = {"gpt3": "gpt-3.5-turbo", "gpt4": "gpt-4"}
+        self.model_dict = {"gpt3": "gpt-3.5-turbo", "gpt4": "gpt-4", "gpt4o": "gpt-4o"}
         self.model = list(self.model_dict.keys())
 
     def __call__(
         self,
         message: str,
         prompt: Optional[str] = None,
-        model: Optional[str] = "gpt4",
+        model: Optional[str] = "gpt4o",
         stream: Optional[bool] = False,
     ) -> str:
         if prompt is None:
             messages = [{"role": "user", "content": message}]
         else:
             messages = [
                 {"role": "system", "content": prompt},
```

### Comparing `zerohertzLib-1.0.7/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.8/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.8/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.8/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.8/zerohertzLib/mlops/triton.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.8/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.8/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.8/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.8/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.8/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.8/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.8/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.8/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.8/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.8/zerohertzLib/quant/quant.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
+import copy
 import multiprocessing as mp
 import time
 import traceback
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import datetime, timedelta
 from itertools import combinations
@@ -216,21 +217,21 @@
         if self.total_cnt < 1:
             return {"position": "NULL"}
         if day != -1 and "-" not in day:
             day = day[:4] + "-" + day[4:6] + "-" + day[6:8]
         possibility = defaultdict(list)
         for key in self.methods:
             possibility[key] = [
-                self.signals[key][day],
-                self.signals[key][day] / self.methods_cnt[key] * 100,
+                self.signals[key].iloc[day],
+                self.signals[key].iloc[day] / self.methods_cnt[key] * 100,
             ]
-        possibility["logic"] = self.signals["logic"][day]
+        possibility["logic"] = self.signals["logic"].iloc[day]
         possibility["total"] = [
-            self.signals["signals"][day],
-            self.signals["signals"][day] / self.total_cnt * 100,
+            self.signals["signals"].iloc[day],
+            self.signals["signals"].iloc[day] / self.total_cnt * 100,
         ]
         if 0 < possibility["logic"]:
             possibility["position"] = "Buy"
         elif 0 > possibility["logic"]:
             possibility["position"] = "Sell"
         elif self.threshold_buy <= possibility["total"][0]:
             possibility["position"] = "Buy"
@@ -384,29 +385,24 @@
 
         Returns:
             ``None``: 현재 계좌에 정보 update
 
         Examples:
             >>> balance_1.merge(balance_2)
         """
-        merged_balance = balance.balance.copy()
+        merged_balance = copy.deepcopy(balance.balance)
         if self.kor != balance.kor:
             exchange = self._exchange()
-            if self.kor:
-                for key, value in balance.items():
-                    merged_balance["stock"][key][1] = value[1] * exchange
-                    merged_balance["stock"][key][2] = value[2] * exchange
-                    merged_balance["stock"][key][-1] = value[-1] * exchange
-                merged_balance["cash"] = balance.balance["cash"] * exchange
-            else:
-                for key, value in balance.items():
-                    merged_balance["stock"][key][1] = value[1] / exchange
-                    merged_balance["stock"][key][2] = value[2] / exchange
-                    merged_balance["stock"][key][-1] = value[-1] / exchange
-                merged_balance["cash"] = balance.balance["cash"] / exchange
+            if not self.kor:
+                exchange = 1 / exchange
+            for key, value in balance.items():
+                merged_balance["stock"][key][1] = value[1] * exchange
+                merged_balance["stock"][key][2] = value[2] * exchange
+                merged_balance["stock"][key][-1] = value[-1] * exchange
+            merged_balance["cash"] = balance.balance["cash"] * exchange
         for key, value in merged_balance["stock"].items():
             if key in self:
                 (
                     _merged_code,
                     _merged_buy_price,
                     _merged_present_price,
                     _merged_cnt,
```

### Comparing `zerohertzLib-1.0.7/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.8/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.8/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/util/data.py` & `zerohertzLib-1.0.8/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/util/json.py` & `zerohertzLib-1.0.8/zerohertzLib/util/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import json
 import os
 from glob import glob
 from typing import Any, Dict, List, Optional, Set, Union
 
+import orjson
 from tqdm import tqdm
 
 
 class Json:
     """JSON 형식 file을 읽고 사용하기 위한 class
 
     객체 생성 시 ``path`` 를 입력하지 않을 시 현재 경로에 존재하는 JSON file을 읽고 ``path`` 를 경로로 입력하면 해당 경로에 존재하는 JSON file을 읽는다.
@@ -92,15 +92,15 @@
     def __init__(self, path: Optional[str] = None) -> None:
         if path is None:
             path = glob("*.json")[0]
         elif not path.endswith(".json"):
             path = glob(f"{path}/*.json")[0]
         self.name = path.replace(os.path.dirname(path), "").replace("/", "")
         with open(path, "r", encoding="utf-8") as file:
-            self.data = json.load(file)
+            self.data = orjson.loads(file.read())
         self.keys = []
         self.map = []
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __getitem__(self, key: Union[int, str]) -> Any:
@@ -354,10 +354,10 @@
                 "정보": [
                     "아무",
                     "거나"
                 ]
             },
         ...
     """
-    with open(f"{path}.json", "w", encoding="utf-8") as file:
-        json.dump(data, file, indent=4, ensure_ascii=False)
+    with open(f"{path}.json", "wb") as file:
+        file.write(orjson.dumps(data, option=orjson.OPT_INDENT_2))
     return os.path.abspath(f"{path}.json")
```

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.8/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.7/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.8/zerohertzLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.7
+Version: 1.0.8
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -81,9 +80,7 @@
 <p align="center">
     <img src="https://github.com/Zerohertz/Zerohertz/assets/42334717/85c44efa-1440-4962-a6e5-7453b0bdc689" width="600">
 </p>
 
 ```python
 import zerohertzLib as zz
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.7 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.8 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
-Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Author-email: ohg3417@gmail.com License: MIT Classifier: Development Status ::
+5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0 Description-Content-Type: text/markdown Provides-
 Extra: api Provides-Extra: mlops Provides-Extra: quant Provides-Extra: all
 License-File: LICENSE
   [https://github.com/Zerohertz/Zerohertz/assets/42334717/90adcc0f-c6ec-4aca-
```

### Comparing `zerohertzLib-1.0.7/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.8/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

