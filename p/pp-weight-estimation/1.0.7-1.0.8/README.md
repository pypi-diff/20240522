# Comparing `tmp/pp_weight_estimation-1.0.7.tar.gz` & `tmp/pp_weight_estimation-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.0.7.tar", last modified: Thu May 16 16:36:59 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.0.8.tar", last modified: Wed May 22 13:16:53 2024, max compression
```

## Comparing `pp_weight_estimation-1.0.7.tar` & `pp_weight_estimation-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 16:36:59.250428 pp_weight_estimation-1.0.7/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      245 2024-05-16 16:36:59.250428 pp_weight_estimation-1.0.7/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       56 2024-05-16 12:25:41.000000 pp_weight_estimation-1.0.7/README.md
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 16:36:59.250428 pp_weight_estimation-1.0.7/pp_weight_estimation/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2024-05-16 11:09:18.000000 pp_weight_estimation-1.0.7/pp_weight_estimation/__init__.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      206 2024-05-16 16:36:53.000000 pp_weight_estimation-1.0.7/pp_weight_estimation/version.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 16:36:59.250428 pp_weight_estimation-1.0.7/pp_weight_estimation.egg-info/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      245 2024-05-16 16:36:59.000000 pp_weight_estimation-1.0.7/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      342 2024-05-16 16:36:59.000000 pp_weight_estimation-1.0.7/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-05-16 16:36:59.000000 pp_weight_estimation-1.0.7/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       27 2024-05-16 16:36:59.000000 pp_weight_estimation-1.0.7/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       21 2024-05-16 16:36:59.000000 pp_weight_estimation-1.0.7/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-05-16 11:05:46.000000 pp_weight_estimation-1.0.7/pyproject.toml
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 16:36:59.250428 pp_weight_estimation-1.0.7/scripts/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      318 2024-05-16 16:36:49.000000 pp_weight_estimation-1.0.7/scripts/weight_pred.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-05-16 16:36:59.250428 pp_weight_estimation-1.0.7/setup.cfg
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      884 2024-05-16 16:33:48.000000 pp_weight_estimation-1.0.7/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:16:53.573711 pp_weight_estimation-1.0.8/
+-rw-r--r--   0 malav     (1000) malav     (1000)      245 2024-05-22 13:16:53.573711 pp_weight_estimation-1.0.8/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.8/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:16:53.573711 pp_weight_estimation-1.0.8/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.8/pp_weight_estimation/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      206 2024-05-22 13:16:46.000000 pp_weight_estimation-1.0.8/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:16:53.573711 pp_weight_estimation-1.0.8/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      245 2024-05-22 13:16:53.000000 pp_weight_estimation-1.0.8/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      342 2024-05-22 13:16:53.000000 pp_weight_estimation-1.0.8/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-22 13:16:53.000000 pp_weight_estimation-1.0.8/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-22 13:16:53.000000 pp_weight_estimation-1.0.8/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-22 13:16:53.000000 pp_weight_estimation-1.0.8/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.8/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:16:53.573711 pp_weight_estimation-1.0.8/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      318 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.8/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-22 13:16:53.573711 pp_weight_estimation-1.0.8/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.8/setup.py
```

### Comparing `pp_weight_estimation-1.0.7/setup.py` & `pp_weight_estimation-1.0.8/setup.py`

 * *Files identical despite different names*

