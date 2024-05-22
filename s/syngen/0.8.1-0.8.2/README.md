# Comparing `tmp/syngen-0.8.1.tar.gz` & `tmp/syngen-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.8.1.tar", last modified: Fri May 17 14:26:59 2024, max compression
+gzip compressed data, was "syngen-0.8.2.tar", last modified: Wed May 22 10:36:02 2024, max compression
```

## Comparing `syngen-0.8.1.tar` & `syngen-0.8.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.597661 syngen-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-17 14:25:39.000000 syngen-0.8.1/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 14:25:39.000000 syngen-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 14:25:39.000000 syngen-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26926 2024-05-17 14:26:59.597661 syngen-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-05-17 14:25:39.000000 syngen-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 14:25:39.000000 syngen-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-17 14:26:59.597661 syngen-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.577661 syngen-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/config/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.585661 syngen-0.8.1/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/mlflow_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/mlflow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.589661 syngen-0.8.1/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/ml/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/streamlit_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/streamlit_app/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/streamlit_app/css/
--rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.593661 syngen-0.8.1/src/syngen/streamlit_app/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.597661 syngen-0.8.1/src/syngen/streamlit_app/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/img/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.597661 syngen-0.8.1/src/syngen/streamlit_app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/streamlit_app/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-17 14:25:39.000000 syngen-0.8.1/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:26:59.597661 syngen-0.8.1/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26926 2024-05-17 14:26:59.000000 syngen-0.8.1/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-17 14:26:59.000000 syngen-0.8.1/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:26:59.000000 syngen-0.8.1/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 14:26:59.000000 syngen-0.8.1/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-17 14:26:59.000000 syngen-0.8.1/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 14:26:59.000000 syngen-0.8.1/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-22 10:34:41.000000 syngen-0.8.2/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 10:34:41.000000 syngen-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 10:34:41.000000 syngen-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26933 2024-05-22 10:36:02.741406 syngen-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-22 10:34:41.000000 syngen-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 10:34:41.000000 syngen-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 10:36:02.745406 syngen-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.725406 syngen-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.729406 syngen-0.8.2/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/config/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/mlflow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/mlflow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/img/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26933 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.8.1/LICENSE` & `syngen-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/PKG-INFO` & `syngen-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.1
+Version: 0.8.2
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -212,15 +212,15 @@
 ```bash
 train --source STR --table_name STR --log_level STR
 train --metadata_path STR --log_level STR
 infer --size INT --table_name STR --log_level STR
 infer --metadata_path STR --log_level STR
 ```
 
-where <i>log_level</i> might be one of the following values: <i>DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
+where <i>log_level</i> might be one of the following values: <i>TRACE, DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
 
 
 ### Linked tables generation
 
 To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships
 between tables via metadata, it becomes possible to manage complex relationships across any number of tables.
 You can also specify additional parameters needed for training and inference in the metadata file and in this case,
```

### Comparing `syngen-0.8.1/README.md` & `syngen-0.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 ```bash
 train --source STR --table_name STR --log_level STR
 train --metadata_path STR --log_level STR
 infer --size INT --table_name STR --log_level STR
 infer --metadata_path STR --log_level STR
 ```
 
-where <i>log_level</i> might be one of the following values: <i>DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
+where <i>log_level</i> might be one of the following values: <i>TRACE, DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
 
 
 ### Linked tables generation
 
 To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships
 between tables via metadata, it becomes possible to manage complex relationships across any number of tables.
 You can also specify additional parameters needed for training and inference in the metadata file and in this case,
```

#### html2text {}

```diff
@@ -86,43 +86,43 @@
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
 table. If so, the duplicated arguments from the CLI will be ignored. Note: If
 you want to set the logging level, you can use the parameter log_level in the
 CLI call: ```bash train --source STR --table_name STR --log_level STR train --
 metadata_path STR --log_level STR infer --size INT --table_name STR --log_level
 STR infer --metadata_path STR --log_level STR ``` where log_level might be one
-of the following values: DEBUG, INFO, WARNING, ERROR, CRITICAL. ### Linked
-tables generation To generate one or more tables, you might provide metadata in
-yaml format. By providing information about the relationships between tables
-via metadata, it becomes possible to manage complex relationships across any
-number of tables. You can also specify additional parameters needed for
-training and inference in the metadata file and in this case, they will be
-ignored in the CLI call. Note: By using metadata file, you can also generate
-tables with absent relationships. In this case, the tables will be generated
-independently. The yaml metadata file should match the following template:
-```yaml global: # Global settings. Optional parameter. In this section you can
-specify training and inference settings which will be set for all tables
-train_settings: # Settings for training process. Optional parameter epochs: 10
-# Number of epochs if different from the default in the command line options.
-Optional parameter drop_null: False # Drop rows with NULL values. Optional
-parameter row_limit: null # Number of rows to train over. A number less than
-the original table length will randomly subset the specified rows number.
-Optional parameter batch_size: 32 # If specified, the training is split into
-batches. This can save the RAM. Optional parameter print_report: False # Turn
-on or turn off generation of the report. Optional parameter infer_settings: #
-Settings for infer process. Optional parameter size: 100 # Size for generated
-data. Optional parameter run_parallel: False # Turn on or turn off parallel
-training process. Optional parameter print_report: False # Turn on or turn off
-generation of the report. Optional parameter batch_size: null # If specified,
-the generation is split into batches. This can save the RAM. Optional parameter
-random_seed: null # If specified, generates a reproducible result. Optional
-parameter get_infer_metrics: False # Whether to fetch metrics for the inference
-process. If the parameter 'print_report' is set to True, the
-'get_infer_metrics' parameter will be ignored and metrics will be fetched
-anyway. Optional parameter CUSTOMER: # Table name. Required parameter
+of the following values: TRACE, DEBUG, INFO, WARNING, ERROR, CRITICAL. ###
+Linked tables generation To generate one or more tables, you might provide
+metadata in yaml format. By providing information about the relationships
+between tables via metadata, it becomes possible to manage complex
+relationships across any number of tables. You can also specify additional
+parameters needed for training and inference in the metadata file and in this
+case, they will be ignored in the CLI call. Note: By using metadata file, you
+can also generate tables with absent relationships. In this case, the tables
+will be generated independently. The yaml metadata file should match the
+following template: ```yaml global: # Global settings. Optional parameter. In
+this section you can specify training and inference settings which will be set
+for all tables train_settings: # Settings for training process. Optional
+parameter epochs: 10 # Number of epochs if different from the default in the
+command line options. Optional parameter drop_null: False # Drop rows with NULL
+values. Optional parameter row_limit: null # Number of rows to train over. A
+number less than the original table length will randomly subset the specified
+rows number. Optional parameter batch_size: 32 # If specified, the training is
+split into batches. This can save the RAM. Optional parameter print_report:
+False # Turn on or turn off generation of the report. Optional parameter
+infer_settings: # Settings for infer process. Optional parameter size: 100 #
+Size for generated data. Optional parameter run_parallel: False # Turn on or
+turn off parallel training process. Optional parameter print_report: False #
+Turn on or turn off generation of the report. Optional parameter batch_size:
+null # If specified, the generation is split into batches. This can save the
+RAM. Optional parameter random_seed: null # If specified, generates a
+reproducible result. Optional parameter get_infer_metrics: False # Whether to
+fetch metrics for the inference process. If the parameter 'print_report' is set
+to True, the 'get_infer_metrics' parameter will be ignored and metrics will be
+fetched anyway. Optional parameter CUSTOMER: # Table name. Required parameter
 train_settings: # Settings for training process. Required parameter source: "./
 files/customer.csv" # The path to the original data. Supported formats include
 local files in CSV, Avro formats. Required parameter epochs: 10 # Number of
 epochs if different from the default in the command line options. Optional
 parameter drop_null: False # Drop rows with NULL values. Optional parameter
 row_limit: null # Number of rows to train over. A number less than the original
 table length will randomly subset the specified rows number. Optional parameter
```

### Comparing `syngen-0.8.1/setup.cfg` & `syngen-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/infer.py` & `syngen-0.8.2/src/syngen/infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     type=click.BOOL,
     help="Whether to print quality report. Might require significant time "
     "for big generated tables (>1000 rows). If absent, it's defaulted to False",
 )
 @click.option(
     "--log_level",
     default="INFO",
-    type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
+    type=click.Choice(["TRACE", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
     help="Set the logging level which will be used in the process. "
          "If absent, it's defaulted to 'INFO'",
 )
 def launch_infer(
     metadata_path: Optional[str],
     size: Optional[int],
     table_name: Optional[str],
```

### Comparing `syngen-0.8.1/src/syngen/ml/config/configurations.py` & `syngen-0.8.2/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/config/validation.py` & `syngen-0.8.2/src/syngen/ml/config/validation.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/context/context.py` & `syngen-0.8.2/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/convertor/convertor.py` & `syngen-0.8.2/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.8.2/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/handlers/handlers.py` & `syngen-0.8.2/src/syngen/ml/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg` & `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/accuracy_test/src/main.css` & `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/main.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/metrics/utils.py` & `syngen-0.8.2/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/mlflow_tracker/mlflow_tracker.py` & `syngen-0.8.2/src/syngen/ml/mlflow_tracker/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/reporters/reporters.py` & `syngen-0.8.2/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/strategies/strategies.py` & `syngen-0.8.2/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/utils/__init__.py` & `syngen-0.8.2/src/syngen/ml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/utils/utils.py` & `syngen-0.8.2/src/syngen/ml/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,17 +391,15 @@
     Redirect logs to the console
     """
     sys.stderr.write(record)
 
 
 def setup_logger():
     """
-    Set up logger with the specified level.
-    Log the messages with level 'INFO' and above to the log file,
-    redirect the messages to stderr with the level set in the environment variable "LOGURU_LEVEL".
+    Set up loggers with the specified level
     """
     logger.remove()
     logger.add(console_sink, colorize=True, level=os.getenv("LOGURU_LEVEL"))
     logger.add(file_sink, level=os.getenv("LOGURU_LEVEL"))
 
 
 def check_if_logs_available():
```

### Comparing `syngen-0.8.1/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.8.2/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/vae/models/dataset.py` & `syngen-0.8.2/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/vae/models/features.py` & `syngen-0.8.2/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/vae/models/model.py` & `syngen-0.8.2/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.8.2/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.8.2/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/ml/worker/worker.py` & `syngen-0.8.2/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/css/style.css` & `syngen-0.8.2/src/syngen/streamlit_app/css/style.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/handlers/handlers.py` & `syngen-0.8.2/src/syngen/streamlit_app/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/img/favicon.svg` & `syngen-0.8.2/src/syngen/streamlit_app/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/img/logo.svg` & `syngen-0.8.2/src/syngen/streamlit_app/img/logo.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/run.py` & `syngen-0.8.2/src/syngen/streamlit_app/run.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/start.py` & `syngen-0.8.2/src/syngen/streamlit_app/start.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/streamlit_app/utils/utils.py` & `syngen-0.8.2/src/syngen/streamlit_app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen/train.py` & `syngen-0.8.2/src/syngen/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     type=click.BOOL,
     help="Whether to print quality report. Might require significant time "
     "for big generated tables (>1000 rows). If absent, it's defaulted to False",
 )
 @click.option(
     "--log_level",
     default="INFO",
-    type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
+    type=click.Choice(["TRACE", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
     help="Set the logging level which will be used in the process. "
          "If absent, it's defaulted to 'INFO'",
 )
 @click.option(
     "--batch_size",
     default=32,
     type=click.IntRange(1),
```

### Comparing `syngen-0.8.1/src/syngen.egg-info/PKG-INFO` & `syngen-0.8.2/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.1
+Version: 0.8.2
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -212,15 +212,15 @@
 ```bash
 train --source STR --table_name STR --log_level STR
 train --metadata_path STR --log_level STR
 infer --size INT --table_name STR --log_level STR
 infer --metadata_path STR --log_level STR
 ```
 
-where <i>log_level</i> might be one of the following values: <i>DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
+where <i>log_level</i> might be one of the following values: <i>TRACE, DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
 
 
 ### Linked tables generation
 
 To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships
 between tables via metadata, it becomes possible to manage complex relationships across any number of tables.
 You can also specify additional parameters needed for training and inference in the metadata file and in this case,
```

### Comparing `syngen-0.8.1/src/syngen.egg-info/SOURCES.txt` & `syngen-0.8.2/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngen-0.8.1/src/syngen.egg-info/requires.txt` & `syngen-0.8.2/src/syngen.egg-info/requires.txt`

 * *Files identical despite different names*

