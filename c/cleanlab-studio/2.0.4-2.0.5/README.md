# Comparing `tmp/cleanlab_studio-2.0.4.tar.gz` & `tmp/cleanlab_studio-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab_studio-2.0.4.tar", last modified: Mon May  6 20:36:48 2024, max compression
+gzip compressed data, was "cleanlab_studio-2.0.5.tar", last modified: Wed May 22 16:42:39 2024, max compression
```

## Comparing `cleanlab_studio-2.0.4.tar` & `cleanlab_studio-2.0.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.270947 cleanlab_studio-2.0.4/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.274947 cleanlab_studio-2.0.4/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.274947 cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.274947 cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.274947 cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.278947 cleanlab_studio-2.0.4/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.278947 cleanlab_studio-2.0.4/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.278947 cleanlab_studio-2.0.4/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.278947 cleanlab_studio-2.0.4/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24287 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.278947 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/cleanlab_studio/internal/tlm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/tlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/tlm/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/tlm/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    30336 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/cleanlab_studio/utils/data_enrichment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/utils/data_enrichment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/utils/data_enrichment/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/utils/data_enrichment/enrichment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-06 20:36:48.000000 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-06 20:36:48.000000 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:36:48.000000 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 20:36:48.000000 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 20:36:48.000000 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 20:36:48.000000 cleanlab_studio-2.0.4/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:36:48.282947 cleanlab_studio-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-06 20:36:38.000000 cleanlab_studio-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.277073 cleanlab_studio-2.0.5/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.277073 cleanlab_studio-2.0.5/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.277073 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24527 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/enrichment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30336 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/setup.py
```

### Comparing `cleanlab_studio-2.0.4/LICENSE` & `cleanlab_studio-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/PKG-INFO` & `cleanlab_studio-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.4
+Version: 2.0.5
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
@@ -41,15 +41,15 @@
 Requires-Dist: jsonstreams>=0.6.0
 Requires-Dist: semver<3.0.0,>=2.13.0
 Requires-Dist: Pillow>=9.2.0
 Requires-Dist: typing_extensions>=4.2.0
 Requires-Dist: openpyxl!=3.1.0,>=3.0.0
 Requires-Dist: validators>=0.20.0
 
-# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI]
+# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI] [![py\_versions](https://img.shields.io/badge/python-3.8%2B-blue)](https://pypi.org/pypi/cleanlab-studio/)
 
 Command line and Python library interface to [Cleanlab Studio](https://cleanlab.ai/studio/). Analyze datasets and produce *cleansets* (cleaned datasets) with Cleanlab Studio in a single line of code!
 
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [Advanced Usage](#advanced-usage)
 - [Documentation/Tutorials](https://help.cleanlab.ai/)
@@ -65,14 +65,15 @@
 
 If you already have the client installed and wish to upgrade to the latest version, run:
 
 ```bash
 pip install --upgrade cleanlab-studio
 ```
 
+
 ## Quickstart
 
 ### Python API -- run Cleanlab Studio from Python or Jupyter Notebook
 
 ```python
 from cleanlab_studio import Studio
```

### Comparing `cleanlab_studio-2.0.4/README.md` & `cleanlab_studio-2.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI]
+# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI] [![py\_versions](https://img.shields.io/badge/python-3.8%2B-blue)](https://pypi.org/pypi/cleanlab-studio/)
 
 Command line and Python library interface to [Cleanlab Studio](https://cleanlab.ai/studio/). Analyze datasets and produce *cleansets* (cleaned datasets) with Cleanlab Studio in a single line of code!
 
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [Advanced Usage](#advanced-usage)
 - [Documentation/Tutorials](https://help.cleanlab.ai/)
@@ -18,14 +18,15 @@
 
 If you already have the client installed and wish to upgrade to the latest version, run:
 
 ```bash
 pip install --upgrade cleanlab-studio
 ```
 
+
 ## Quickstart
 
 ### Python API -- run Cleanlab Studio from Python or Jupyter Notebook
 
 ```python
 from cleanlab_studio import Studio
```

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/api_service.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/dataset.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/download.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/click_helpers.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/dataset/upload.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/login/login.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/main.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/types.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/cli/util.py` & `cleanlab_studio-2.0.5/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/errors.py` & `cleanlab_studio-2.0.5/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/api/api.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,14 +457,20 @@
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     status: JSONDict = res.json()
     return status
 
 
+def delete_dataset(api_key: str, dataset_id: str) -> None:
+    check_uuid_well_formed(dataset_id, "dataset ID")
+    res = requests.delete(dataset_base_url + f"/{dataset_id}", headers=_construct_headers(api_key))
+    handle_api_error(res)
+
+
 def delete_project(api_key: str, project_id: str) -> None:
     check_uuid_well_formed(project_id, "project ID")
     res = requests.delete(project_base_url + f"/{project_id}", headers=_construct_headers(api_key))
     handle_api_error(res)
 
 
 def poll_progress(
```

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/clean_helpers.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/constants.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/settings.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/tlm/concurrency.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/concurrency.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/tlm/validation.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/upload_helpers.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/internal/util.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/studio/inference.py` & `cleanlab_studio-2.0.5/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/studio/studio.py` & `cleanlab_studio-2.0.5/cleanlab_studio/studio/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,27 @@
 
         return upload_helpers.upload_dataset(
             self._api_key,
             ds,
             schema_overrides=schema_overrides,
         )
 
+    def delete_dataset(
+        self,
+        dataset_id: str,
+    ) -> None:
+        """Deletes a dataset from Cleanlab Studio.
+
+        If the dataset is used in projects, the projects will be deleted as well.
+        """
+        api.delete_dataset(
+            self._api_key,
+            dataset_id,
+        )
+
     def download_cleanlab_columns(
         self,
         cleanset_id: str,
         include_cleanlab_columns: bool = True,
         include_project_details: bool = False,
         to_spark: bool = False,
     ) -> Any:
@@ -202,15 +215,15 @@
             modality: Modality of project (i.e. text, tabular, image).
             task_type: Type of ML task to perform. Select a supervised task type (i.e. "multi-class", "multi-label", "regression") if your dataset
                 has a label column you would like to predict values for or detect erroneous values in. Select "unsupervised" if your dataset has
                 no specific label column. See the [Projects Guide](/guide/concepts/projects/#machine-learning-task--dataset-type) for more
                 information on task types.
             model_type: Type of model to train (i.e. "fast", "regular"). See the [Projects Guide](/guide/concepts/projects/#model-type) for more information on model types.
             label_column: Name of column in dataset containing labels (if not supplied, we'll make our best guess). For "unsupervised" tasks, this should be `None`.
-            feature_columns: List of columns to use as features when training tabular modality project (if not supplied and modality is "tabular" we'll use all valid feature columns).
+            feature_columns: List of columns to use as features for a tabular project. By default all columns are used as feature columns. This parameter is particularly useful if your dataset has a column containing unique IDs and you want to exclude that column from the feature columns.
             text_column: Name of column containing the text to train text modality project on (if not supplied and modality is "text" we'll make our best guess).
 
         Returns:
             ID of created project.
         """
         dataset_details = api.get_dataset_details(self._api_key, dataset_id, task_type)
```

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/studio/trustworthy_language_model.py` & `cleanlab_studio-2.0.5/cleanlab_studio/studio/trustworthy_language_model.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/utils/data_enrichment/enrich.py` & `cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/enrich.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import Any, List, Optional, Tuple, Union
 import pandas as pd
-from cleanlab_studio.utils.data_enrichment.enrichment_utils import (
+from cleanlab_studio.internal.enrichment_utils import (
     extract_df_subset,
     get_compiled_regex_list,
     get_prompt_outputs,
     get_regex_match,
     get_return_values_match,
     get_optimized_prompt,
 )
```

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/utils/data_enrichment/enrichment_utils.py` & `cleanlab_studio-2.0.5/cleanlab_studio/internal/enrichment_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cleanlab_studio.errors import ValidationError
 from cleanlab_studio.studio.studio import Studio
 from cleanlab_studio.studio.trustworthy_language_model import TLMResponse
 
 
 def get_prompt_outputs(
     studio: Studio, prompt: str, data: pd.DataFrame, **kwargs: Any
-) -> List[TLMResponse | None]:
+) -> List[Optional[TLMResponse]]:
     """Returns the outputs of the prompt for each row in the dataframe."""
     tlm = studio.TLM(**kwargs)
     formatted_prompts = data.apply(lambda x: prompt.format(**x), axis=1).to_list()
     outputs = tlm.try_prompt(formatted_prompts)
     return outputs
 
 
@@ -51,15 +51,15 @@
         raise ValidationError(
             "Passed in regex can only be type one of: str, re.Pattern, or list of re.Pattern."
         )
 
 
 def get_regex_match(
     response: str, regex_list: List[re.Pattern[str]], disable_warnings: bool
-) -> Union[str, None]:
+) -> Optional[str]:
     """Extract the first match from the response using the provided regex patterns. Return first match if multiple exist.
     Note: This function assumes the regex patterns each specify exactly 1 group that is the match group using ``'(<group>)'``."""
     for regex_pattern in regex_list:
         pattern_match = regex_pattern.match(response)
         if pattern_match:
             return pattern_match.group(1)
     if not disable_warnings:
```

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio/utils/synthetic.py` & `cleanlab_studio-2.0.5/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab_studio-2.0.5/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.4
+Version: 2.0.5
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
@@ -41,15 +41,15 @@
 Requires-Dist: jsonstreams>=0.6.0
 Requires-Dist: semver<3.0.0,>=2.13.0
 Requires-Dist: Pillow>=9.2.0
 Requires-Dist: typing_extensions>=4.2.0
 Requires-Dist: openpyxl!=3.1.0,>=3.0.0
 Requires-Dist: validators>=0.20.0
 
-# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI]
+# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI] [![py\_versions](https://img.shields.io/badge/python-3.8%2B-blue)](https://pypi.org/pypi/cleanlab-studio/)
 
 Command line and Python library interface to [Cleanlab Studio](https://cleanlab.ai/studio/). Analyze datasets and produce *cleansets* (cleaned datasets) with Cleanlab Studio in a single line of code!
 
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [Advanced Usage](#advanced-usage)
 - [Documentation/Tutorials](https://help.cleanlab.ai/)
@@ -65,14 +65,15 @@
 
 If you already have the client installed and wish to upgrade to the latest version, run:
 
 ```bash
 pip install --upgrade cleanlab-studio
 ```
 
+
 ## Quickstart
 
 ### Python API -- run Cleanlab Studio from Python or Jupyter Notebook
 
 ```python
 from cleanlab_studio import Studio
```

### Comparing `cleanlab_studio-2.0.4/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab_studio-2.0.5/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 cleanlab_studio/cli/decorators/auth_config.py
 cleanlab_studio/cli/decorators/previous_state.py
 cleanlab_studio/cli/login/__init__.py
 cleanlab_studio/cli/login/login.py
 cleanlab_studio/internal/__init__.py
 cleanlab_studio/internal/clean_helpers.py
 cleanlab_studio/internal/constants.py
+cleanlab_studio/internal/enrichment_utils.py
 cleanlab_studio/internal/settings.py
 cleanlab_studio/internal/types.py
 cleanlab_studio/internal/upload_helpers.py
 cleanlab_studio/internal/util.py
 cleanlab_studio/internal/api/__init__.py
 cleanlab_studio/internal/api/api.py
 cleanlab_studio/internal/api/api_helper.py
@@ -58,9 +59,8 @@
 cleanlab_studio/studio/__init__.py
 cleanlab_studio/studio/inference.py
 cleanlab_studio/studio/studio.py
 cleanlab_studio/studio/trustworthy_language_model.py
 cleanlab_studio/utils/__init__.py
 cleanlab_studio/utils/synthetic.py
 cleanlab_studio/utils/data_enrichment/__init__.py
-cleanlab_studio/utils/data_enrichment/enrich.py
-cleanlab_studio/utils/data_enrichment/enrichment_utils.py
+cleanlab_studio/utils/data_enrichment/enrich.py
```

### Comparing `cleanlab_studio-2.0.4/setup.py` & `cleanlab_studio-2.0.5/setup.py`

 * *Files identical despite different names*

