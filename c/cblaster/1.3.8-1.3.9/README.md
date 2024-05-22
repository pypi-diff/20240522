# Comparing `tmp/cblaster-1.3.8.tar.gz` & `tmp/cblaster-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cblaster-1.3.8.tar", last modified: Wed Jun 30 06:33:55 2021, max compression
+gzip compressed data, was "cblaster-1.3.9.tar", last modified: Tue Jul 27 05:27:18 2021, max compression
```

## Comparing `cblaster-1.3.8.tar` & `cblaster-1.3.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:55.809760 cblaster-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-06-30 06:33:37.000000 cblaster-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9200 2021-06-30 06:33:55.809760 cblaster-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7521 2021-06-30 06:33:37.000000 cblaster-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:55.793760 cblaster-1.3.8/cblaster/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21443 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    18919 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     7212 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     7372 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)    16493 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/extract_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)     8362 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     9055 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/genome_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:55.801760 cblaster-1.3.8/cblaster/gui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/citation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/extract_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/gne.py
--rw-r--r--   0 runner    (1001) docker     (121)    13553 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/makedb.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/parts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/plot_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)    12139 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/gui/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/hmm_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     9547 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/intermediate_genes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/local.py
--rw-r--r--   0 runner    (1001) docker     (121)    17872 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    29770 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:55.805760 cblaster-1.3.8/cblaster/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot/cblaster.html
--rw-r--r--   0 runner    (1001) docker     (121)    22091 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot/cblaster.js
--rw-r--r--   0 runner    (1001) docker     (121)   248314 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot/gne.html
--rw-r--r--   0 runner    (1001) docker     (121)     8946 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot/gne.js
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot/index.css
--rw-r--r--   0 runner    (1001) docker     (121)     9799 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6471 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/plot_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)    11961 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2021-06-30 06:33:37.000000 cblaster-1.3.8/cblaster/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:55.797760 cblaster-1.3.8/cblaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9200 2021-06-30 06:33:55.000000 cblaster-1.3.8/cblaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-06-30 06:33:55.000000 cblaster-1.3.8/cblaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-30 06:33:55.000000 cblaster-1.3.8/cblaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-30 06:33:55.000000 cblaster-1.3.8/cblaster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-06-30 06:33:55.000000 cblaster-1.3.8/cblaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-06-30 06:33:55.000000 cblaster-1.3.8/cblaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-30 06:33:55.809760 cblaster-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-06-30 06:33:38.000000 cblaster-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:55.809760 cblaster-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19287 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5692 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     6027 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_genome_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5836 2021-06-30 06:33:38.000000 cblaster-1.3.8/tests/test_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:18.017989 cblaster-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-07-27 05:27:04.000000 cblaster-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     9200 2021-07-27 05:27:18.017989 cblaster-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7521 2021-07-27 05:27:04.000000 cblaster-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:18.013989 cblaster-1.3.9/cblaster/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21443 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18919 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7212 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7372 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16493 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/extract_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8362 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9055 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/genome_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:18.013989 cblaster-1.3.9/cblaster/gui/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/citation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3880 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/extract_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/gne.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13599 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2211 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/makedb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/parts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3521 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/plot_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12398 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/gui/search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6649 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8114 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/hmm_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9547 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/intermediate_genes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17872 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29770 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:18.013989 cblaster-1.3.9/cblaster/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)     2252 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot/cblaster.html
+-rw-r--r--   0 runner    (1001) docker     (121)    22091 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot/cblaster.js
+-rw-r--r--   0 runner    (1001) docker     (121)   248314 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot/gne.html
+-rw-r--r--   0 runner    (1001) docker     (121)     8946 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot/gne.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot/index.css
+-rw-r--r--   0 runner    (1001) docker     (121)     9799 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6471 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/plot_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11961 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2021-07-27 05:27:04.000000 cblaster-1.3.9/cblaster/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:18.013989 cblaster-1.3.9/cblaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9200 2021-07-27 05:27:17.000000 cblaster-1.3.9/cblaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-07-27 05:27:17.000000 cblaster-1.3.9/cblaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-27 05:27:17.000000 cblaster-1.3.9/cblaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-07-27 05:27:17.000000 cblaster-1.3.9/cblaster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-07-27 05:27:17.000000 cblaster-1.3.9/cblaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-07-27 05:27:17.000000 cblaster-1.3.9/cblaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-27 05:27:18.017989 cblaster-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-07-27 05:27:04.000000 cblaster-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:18.017989 cblaster-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19287 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5692 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6027 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_genome_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2844 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5836 2021-07-27 05:27:04.000000 cblaster-1.3.9/tests/test_remote.py
```

### Comparing `cblaster-1.3.8/LICENSE` & `cblaster-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/PKG-INFO` & `cblaster-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cblaster
-Version: 1.3.8
+Version: 1.3.9
 Summary: UNKNOWN
 Home-page: https://github.com/gamcil/cblaster
 Author: Cameron Gilchrist
 License: MIT
 Description: # cblaster
         [![Python package](https://github.com/gamcil/cblaster/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/gamcil/cblaster/actions/workflows/pythonapp.yml)
         [![codecov](https://codecov.io/gh/gamcil/cblaster/branch/master/graph/badge.svg?token=O61R3ORNDT)](https://codecov.io/gh/gamcil/cblaster)
```

### Comparing `cblaster-1.3.8/README.md` & `cblaster-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/classes.py` & `cblaster-1.3.9/cblaster/classes.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/config.py` & `cblaster-1.3.9/cblaster/config.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/context.py` & `cblaster-1.3.9/cblaster/context.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/database.py` & `cblaster-1.3.9/cblaster/database.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/extract.py` & `cblaster-1.3.9/cblaster/extract.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/extract_clusters.py` & `cblaster-1.3.9/cblaster/extract_clusters.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/formatters.py` & `cblaster-1.3.9/cblaster/formatters.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/genome_parsers.py` & `cblaster-1.3.9/cblaster/genome_parsers.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/citation.py` & `cblaster-1.3.9/cblaster/gui/citation.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/config.py` & `cblaster-1.3.9/cblaster/gui/config.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/extract.py` & `cblaster-1.3.9/cblaster/gui/extract.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/extract_clusters.py` & `cblaster-1.3.9/cblaster/gui/extract_clusters.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/gne.py` & `cblaster-1.3.9/cblaster/gui/gne.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/main.py` & `cblaster-1.3.9/cblaster/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Args:
         values (dict): Dictionary of values from PySimpleGUI.
     """
     if values["cblaster_tabs"] == "Search":
         args = dict(
             query_file=values["query_file"],
             query_ids=values["query_ids"],
-            query_profiles=values["query_profiles"],
+            query_profiles=values["query_profiles"].split(";") + values["query_pfams"].split(" "),
             session_file=values["session_file"],
             mode=values["search_mode"],
             gap=values["gap"],
             unique=values["unique"],
             min_hits=values["min_hits"],
             require=values["require"],
             min_identity=values["min_identity"],
```

### Comparing `cblaster-1.3.8/cblaster/gui/makedb.py` & `cblaster-1.3.9/cblaster/gui/makedb.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/parts.py` & `cblaster-1.3.9/cblaster/gui/parts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Common components shared between layouts."""
 
 
 import PySimpleGUI as sg
 
 
-TEXT_WIDTH = 65
+TEXT_WIDTH = 70
 
 
 def SectionLabel(text):
     return sg.Text(text, justification="l", font="Arial 12 bold")
 
 
 def TextLabel(text):
```

### Comparing `cblaster-1.3.8/cblaster/gui/plot_clusters.py` & `cblaster-1.3.9/cblaster/gui/plot_clusters.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/gui/search.py` & `cblaster-1.3.9/cblaster/gui/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,18 @@
         [sg.Text(
             "Specify the search mode and databases to be used in the cblaster "
             "run. In remote mode, the database value should correspond to a BLAST "
             "database hosted by the NCBI. In local mode, the database arguments "
             "should refer to files generated using cblaster makedb. When using any "
             "of the HMM modes, a local copy of the Pfam database will be stored at "
             "the indicated location or extracted from there. The FASTA database "
-            "should refer to the FASTA file generated using cblaster makedb.",
-            size=(TEXT_WIDTH, 6))],
+            "should refer to the FASTA file generated using cblaster makedb.\n"
+            "NOTE: you must set an e-mail using cblaster config before doing "
+            "a search with cblaster.",
+            size=(TEXT_WIDTH, 8))],
         [search_tabgroup]
     ]
 )
 
 input_frame = Frame(
     "Input",
     key="input_frame",
@@ -137,15 +139,20 @@
             "cblaster run can be loaded so that you do not have to repeat a search",
             size=(TEXT_WIDTH, 6),
         )],
         [TextLabel("File"),
          sg.InputText(size=(34, 1), key="query_file"),
          sg.FileBrowse(key="query_file")],
         [TextLabel("Sequence IDs"), sg.InputText(key="query_ids", default_text="e.g. space separated values")],
-        [TextLabel("HMM profiles"), sg.InputText(key="query_profiles", default_text="e.g. space separated values")],
+        [TextLabel("Pfam domains"),
+         sg.InputText(key="query_pfams",
+         default_text="e.g. space separated values")],
+        [TextLabel("Local profile HMMs"),
+         sg.Input(size=(34, 1), key="query_profiles"),
+         sg.FilesBrowse()],
         [TextLabel("Session file"),
          sg.InputText(size=(34, 1), key="session_file"),
          sg.FileBrowse(key="session_file")],
     ],
 )
 
 clustering_frame = Frame(
@@ -305,15 +312,15 @@
         [sg.Text(
             "This generates a visual representation of the binary table as a"
             " cluster heatmap. If this is not"
             " specified, the plot will be saved in a plot.html in the temporary folder,"
             " at which point the figure can be manipulated and saved as SVG."
             " If a file path is specified, a static HTML file will be generated at"
             " that path.",
-            size=(TEXT_WIDTH, 4)
+            size=(TEXT_WIDTH, 5)
         )],
         [TextLabel("Output file"),
          sg.InputText(key="figure_text", disabled=True, size=(34, 1)),
          sg.FileSaveAs(key="figure_browse", disabled=True)],
     ],
 )
```

### Comparing `cblaster-1.3.8/cblaster/helpers.py` & `cblaster-1.3.9/cblaster/helpers.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/intermediate_genes.py` & `cblaster-1.3.9/cblaster/intermediate_genes.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/local.py` & `cblaster-1.3.9/cblaster/local.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/main.py` & `cblaster-1.3.9/cblaster/main.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/parsers.py` & `cblaster-1.3.9/cblaster/parsers.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot/cblaster.html` & `cblaster-1.3.9/cblaster/plot/cblaster.html`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot/cblaster.js` & `cblaster-1.3.9/cblaster/plot/cblaster.js`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot/d3.min.js` & `cblaster-1.3.9/cblaster/plot/d3.min.js`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot/gne.html` & `cblaster-1.3.9/cblaster/plot/gne.html`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot/gne.js` & `cblaster-1.3.9/cblaster/plot/gne.js`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot/index.css` & `cblaster-1.3.9/cblaster/plot/index.css`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 body {
 	margin: 0;
 	padding: 0;
 	overflow: hidden;
+	font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, "Helvetica Neue", Oxygen, Cantarell, sans-serif;
 }
 
 .tooltip {
 	background-color: hsla(0, 0%, 20%, 0.9);
 	color: white;
 	border-radius: 4px;
 }
@@ -92,28 +93,27 @@
 	flex-direction: column;
 	top: 1em;
 	right: 1em;
 	width: 300px;
 	max-height: 95vh;
 	border: 1px solid black;
 	background-color: white;
+	font-size: 0.9rem;
 }
 
 #div-summary {
 	display: block;
 	padding: 6px;
 	margin-bottom: 6px;
 	overflow-y: auto;
 }
 
 #div-summary p {
 	margin: 0;
 	margin-bottom: 4px;
-	font-size: 10pt;
-	font-family: sans-serif;
 }
 
 #div-summary pre {
 	white-space: normal;
 }
 
 #div-summary button {
```

### Comparing `cblaster-1.3.8/cblaster/plot.py` & `cblaster-1.3.9/cblaster/plot.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/plot_clusters.py` & `cblaster-1.3.9/cblaster/plot_clusters.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/remote.py` & `cblaster-1.3.9/cblaster/remote.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster/sql.py` & `cblaster-1.3.9/cblaster/sql.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/cblaster.egg-info/PKG-INFO` & `cblaster-1.3.9/cblaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cblaster
-Version: 1.3.8
+Version: 1.3.9
 Summary: UNKNOWN
 Home-page: https://github.com/gamcil/cblaster
 Author: Cameron Gilchrist
 License: MIT
 Description: # cblaster
         [![Python package](https://github.com/gamcil/cblaster/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/gamcil/cblaster/actions/workflows/pythonapp.yml)
         [![codecov](https://codecov.io/gh/gamcil/cblaster/branch/master/graph/badge.svg?token=O61R3ORNDT)](https://codecov.io/gh/gamcil/cblaster)
```

### Comparing `cblaster-1.3.8/cblaster.egg-info/SOURCES.txt` & `cblaster-1.3.9/cblaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/setup.py` & `cblaster-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_classes.py` & `cblaster-1.3.9/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_context.py` & `cblaster-1.3.9/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_database.py` & `cblaster-1.3.9/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_genome_parsers.py` & `cblaster-1.3.9/tests/test_genome_parsers.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_helpers.py` & `cblaster-1.3.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_local.py` & `cblaster-1.3.9/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_parsers.py` & `cblaster-1.3.9/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `cblaster-1.3.8/tests/test_remote.py` & `cblaster-1.3.9/tests/test_remote.py`

 * *Files identical despite different names*

