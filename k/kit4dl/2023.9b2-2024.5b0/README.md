# Comparing `tmp/kit4dl-2023.9b2.tar.gz` & `tmp/kit4dl-2024.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kit4dl-2023.9b2.tar", last modified: Fri Sep 22 12:13:27 2023, max compression
+gzip compressed data, was "kit4dl-2024.5b0.tar", last modified: Mon May 20 09:39:17 2024, max compression
```

## Comparing `kit4dl-2023.9b2.tar` & `kit4dl-2024.5b0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.155733 kit4dl-2023.9b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    31622 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29440 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.143732 kit4dl-2023.9b2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/examples/cnn_mnist_classification/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/examples/cnn_mnist_classification/conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/examples/cnn_s3dis_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/examples/cnn_s3dis_segmentation/conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.143732 kit4dl-2023.9b2/kit4dl/cli/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl/cli/_templates/project/
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/_templates/project/conf.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/_templates/project/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/_templates/project/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/kit4dl_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/kit4dl/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18227 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/confmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31622 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 12:13:27.155733 kit4dl-2023.9b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/cli/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/dummy_module2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22823 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_confmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/resources/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/resources/test_file.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33014 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.322361 kit4dl-2024.5b0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/examples/cnn_mnist_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/examples/cnn_mnist_classification/conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/examples/cnn_s3dis_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/examples/cnn_s3dis_segmentation/conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/kit4dl/
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/kit4dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.322361 kit4dl-2024.5b0/kit4dl/cli/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/kit4dl/cli/_templates/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/_templates/project/conf.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/_templates/project/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/_templates/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/kit4dl_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/kit4dl/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/confmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/kit4dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33014 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/cli/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/dummy_module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/tests/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_confmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/resources/test_file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/utils.py
```

### Comparing `kit4dl-2023.9b2/LICENSE` & `kit4dl-2024.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/PKG-INFO` & `kit4dl-2024.5b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kit4dl
-Version: 2023.9b2
+Version: 2024.5b0
 Summary: Kit4DL - A quick way to start with machine and deep learning
 Author: Jakub Walczak, Marco Mancini, Mirko Stojiljkovic, Shahbaz Alvi
 License: MIT License
         
         Copyright (c) 2023 opengeokube
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,19 +40,19 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lightning<=2.1.0.rc0
-Requires-Dist: torch<2.1.0,>=1.11.0
-Requires-Dist: torchmetrics<1.1.0,>=0.7.0
+Requires-Dist: lightning>=2.2.4
+Requires-Dist: torch>=2.1.0
+Requires-Dist: torchmetrics>=1.1.0
 Requires-Dist: numpy<=1.25.3,>=1.17.2
-Requires-Dist: pydantic<2.2.0,>=2.0.0
+Requires-Dist: pydantic>2.4.0
 Requires-Dist: scikit-learn
 Requires-Dist: colormath
 Requires-Dist: tqdm<4.67.0,>=4.57.0
 Requires-Dist: typing-extensions<4.8.0,>=4.0.0; python_version <= "3.11"
 Requires-Dist: Jinja2<3.2.0
 Requires-Dist: typer[all]
 Requires-Dist: toml; python_version < "3.11"
@@ -89,39 +89,43 @@
 1. Jakub Walczak <a href="https://orcid.org/0000-0002-5632-9484"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Marco Macini <a href="https://orcid.org/0000-0002-9150-943X"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Mirko Stojiljkovic <a href="https://orcid.org/0000-0003-2256-1645"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Shahbaz Alvi <a href="https://orcid.org/0000-0001-5779-8568"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 
 ## 📜 Cite Us
 ```bibtex
-@SOFTWARE{kit4dl,
-  author = {Walczak, Jakub and
-            Mancini, Marco and
-            Stojiljković, Mirko and
-            Alvi, Shahbaz},
-  title = {Kit4DL},
-  month = sep,
-  year = 2023,
-  note = {{Available in GitHub: https://github.com/opengeokube/kit4dl}},
-  publisher = {Zenodo},
-  version = {2023.9b1},
-  doi = {10.5281/zenodo.8328176},
-  url = {https://doi.org/10.5281/zenodo.8328176}
+@ARTICLE{kit4dl,
+    author = {Jakub Walczak and Marco Mancini and Shahbaz Alvi},
+    title = {Kit4DL: Towards fast prototyping and experimentation in machine learning and deep learning},
+    journal = {SoftwareX},
+    volume = {26},
+    pages = {101707},
+    year = {2024},
+    issn = {2352-7110},
+    doi = {https://doi.org/10.1016/j.softx.2024.101707},
+    url = {https://www.sciencedirect.com/science/article/pii/S2352711024000785},
+    keywords = {Deep learning, Machine learning, Prototyping, Python framework},
 }
 ```
+## 📖 Documentation
+Read the official [Documentation](https://opengeokube.github.io/kit4dl/index.html) to learn Kit4DL!
+
 ## 🚧 Roadmap
 
 > **Warning**: Kit4DL is currently in its alpha stage. All recommendations are welcomed.
 
 - [ ] add handling sklearn-like models
 - [ ] add functionality to serve the model
 - [x] enable custom metrics
 - [x] enable using callbacks (also custom ones)
 - [ ] write more unit tests
+- [ ] enable overwritting parameters with command line
 
+## 🙏 Acknowledgement
+This work has received fundings from the Polish National Centre for Research and Development under the LIDER XI program [grant number 0092/L-11/2019, "Semantic analysis of 3D point clouds"] and from the European Union’s Horizon 2020 Research and Innovation programme [SILVANUS Project - grant agreement number 101037247].
 
 ## 🎬 Quickstart
 
 ### Getting started
 
 #### Installation
 ```bash
@@ -201,14 +205,15 @@
 1. [Configuring optimizer](#configuring-optimizer)
 1. [Configuring criterion](#configuring-criterion)
 1. [Configuring metrics](#configuring-metrics)
 1. [Configuring checkpoint](#configuring-checkpoint)
 1. [Defining `target`](#defining-target)
 1. [Substitutable symbols](#substitutable-symbols)
 1. [Context constants](#context-constants)
+1. [Sensitive data obfuscating](#sensitive-data-obfuscating)
 
 #### Configuring base setup
 Most of the training/validation procedure is managed by a configuration file in the TOML format (recommended name is `conf.toml`).
 Each aspect is covered by separate sections. The general one is called `[base]`.
 It has the following properties:
 
 |   **Property** 	|  **Type**        |                                                   **Details**                                          	|
@@ -272,15 +277,15 @@
 In the `configure` method, the architecture of the network should be defined. 
 In `run_step` method, it turn, the logic for single forward pass should be implemented.
 
 ##### ✍️ Example
 ```python
 import torch
 from torch import nn
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 class SimpleCNN(Kit4DLAbstractModule):
     def configure(self, input_dims, output_dims) -> None:
         self.l1 = nn.Sequential(
             nn.Conv2d(
                 input_dims, 16, kernel_size=3, padding="same", bias=True
             ),
@@ -312,15 +317,15 @@
 
 If a forward pass for your model differs for the training, validation, test, or prediction stages, you can define separate methods for them:
 
 ##### ✍️ Example
 ```python
 import torch
 from torch import nn
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 class SimpleCNN(Kit4DLAbstractModule):
     ...
     def run_val_step(self, batch, batch_idx) -> tuple[torch.Tensor, torch.Tensor]:
         pass
 
     def run_test_step(self, batch, batch_idx) -> tuple[torch.Tensor, torch.Tensor]:
@@ -331,27 +336,27 @@
 ```
 
 > **Note**: If you need more customization of the process, you can always override the existing methods according to your needs.
 
 #### Defining datamodule
 Similarily to the model, datamodule instance is fully defined by the Python class and its configuration.
 The datamodule need to be a subclass of the `Kit4DLAbstractDataModule` abstract class from the `kit4dl` package.
-The class has to implement, at least, `prepare_trainvaldataset` (if preparing is the same for the train and validation splits) or `prepare_traindataset` and `prepare_valdataset` (if preparing data differs). Besides those, you can define `prepare_testdataset` and `prepare_predictdataset`, for test and prediction, respectively.
+The class has to implement, at least, `prepare_trainvaldatasets` (if preparing is the same for the train and validation splits) or `prepare_traindatasets` and `prepare_valdatasets` (if preparing data differs). Besides those, you can define `prepare_testdataset` and `prepare_predictdataset`, for test and prediction, respectively.
 
 ##### ✍️ Example
 ```python
 from torch.utils.data import Dataset, random_split
 from torchvision import transforms
 from torchvision.datasets import MNIST
 
-from kit4dl import Kit4DLAbstractDataModule
+from kit4dl.dataset import Kit4DLAbstractDataModule
 
 
 class MNISTCustomDatamodule(Kit4DLAbstractDataModule):
-    def prepare_trainvaldataset(
+    def prepare_trainvaldatasets(
         self, root_dir: str
     ) -> tuple[Dataset, Dataset]:
         dset = MNIST(
             root=root_dir,
             train=True,
             download=True,
             transform=transforms.ToTensor(),
@@ -436,16 +441,16 @@
 batch_size = 150
 shuffle = false
 num_workers = 4
 ```
 
 In the root `[dataset]` you should define `target` property being a path to the subclass of the `Kit4DLAbstractDataModule` module (see [Defining `target`](#defining-target)).
 Then, you need to define either `[dataset.trainval]` section or two separate sections: `[dataset.train]`, `[dataset.validation]`. There are also optional sections: `[dataset.test]` and `[dataset.predict]`.
-In `[dataset.trainval]` you pass values for parameters of the `prepare_trainvaldataset` method.
-Respectively, in the `[dataset.train]` you pass values for the parameters of the `prepare_traindataset` method, in `[dataset.validation]` — `prepare_valdataset`, `[dataset.test]` — `prepare_testdataset`, `[dataset.predict]` — `prepare_predictdataset`.
+In `[dataset.trainval]` you pass values for parameters of the `prepare_trainvaldatasets` method.
+Respectively, in the `[dataset.train]` you pass values for the parameters of the `prepare_traindatasets` method, in `[dataset.validation]` — `prepare_valdatasets`, `[dataset.test]` — `prepare_testdataset`, `[dataset.predict]` — `prepare_predictdataset`.
 
 Besides dataset configuration, you need to specify data loader arguments as indicated in the PyTorch docs [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader).
 
 > **Warning**: You **cannot** specify loader arguments for in the `[dataset.trainval.loader]`. Loaders should be defined for each split separately.
 
 
 #### Configuring training
@@ -476,15 +481,15 @@
 ```python
 import os
 from typing import Any
 
 import lightning.pytorch as pl
 import torchmetrics as tm
 
-from kit4dl import Kit4DLCallback, StepOutput
+from kit4dl import Kit4DLCallback
 
 
 class SaveConfusionMatrixCallback(Kit4DLCallback):
     _cm: tm.ConfusionMatrix
     _num_classes: int
     _task: str
     _save_dir: str
@@ -503,20 +508,20 @@
             task=self._task, num_classes=self._num_classes
         )
 
     def on_validation_batch_end(
         self,
         trainer: pl.Trainer,
         pl_module: pl.LightningModule,
-        outputs: StepOutput,
+        outputs: dict,
         batch: Any,
         batch_idx: int,
         dataloader_idx: int = 0,
     ) -> None:
-        self._cm.update(outputs.predictions, outputs.labels)
+        self._cm.update(outputs['pred'], outputs['true'])
 
     def on_validation_epoch_end(
         self, trainer: pl.Trainer, pl_module: pl.LightningModule
     ) -> None:
         """Called when the val epoch ends."""
         fig, _ = self._cm.plot()
         target_file = os.path.join(
@@ -699,7 +704,22 @@
 |   **Symbol** 	|            **Meaning of the symbol**                                   	|          **Example**                  |
 |-------------	|-----------------------------------------------------------------------	| -----------------------------------	|
 | `PROJECT_DIR`	| the home directory of the TOML configuration file (project directory) 	| `context.PROJECT_DIR`                 |
 | `LOG_LEVEL`	| logging level as defined in the configuration TOML file                	| `context.LOG_LEVEL`                   |
 | `LOG_FORMAT`	| logging message format as defined in the configuration TOML file      	| `context.LOG_FORMAT`                  |
 |  `VERSION`	| the current version of the package                                      	| `context.VERSION`                     |
 
+#### Sensitive data obfuscating
+It might happen, some sensitive data are stored in the configuration file. 
+We should prevent those data from being logged as hyperparameters. This is the reason why
+Kit4DL supports sensitive data obfuscating. By default, all values whose keys contain `key` string
+will be obfuscated with `***`. Both, sensitive data key and obfuscating value can be customized by
+a user, by setting environmental variables accordingly. To obfuscate all
+values containig `url` (e.g.`api-url`, `url-2`, etc.) with `^^^`, just use
+the following code.
+
+##### ✍️ Example
+```python
+import os
+os.environ["KIT4DL_KEY_TO_OBFUSCATE"] = "url"
+os.environ["KIT4DL_OBFUSCATING_VALUE"] = "^^^"
+```
```

### Comparing `kit4dl-2023.9b2/README.md` & `kit4dl-2024.5b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,39 +30,43 @@
 1. Jakub Walczak <a href="https://orcid.org/0000-0002-5632-9484"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Marco Macini <a href="https://orcid.org/0000-0002-9150-943X"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Mirko Stojiljkovic <a href="https://orcid.org/0000-0003-2256-1645"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Shahbaz Alvi <a href="https://orcid.org/0000-0001-5779-8568"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 
 ## 📜 Cite Us
 ```bibtex
-@SOFTWARE{kit4dl,
-  author = {Walczak, Jakub and
-            Mancini, Marco and
-            Stojiljković, Mirko and
-            Alvi, Shahbaz},
-  title = {Kit4DL},
-  month = sep,
-  year = 2023,
-  note = {{Available in GitHub: https://github.com/opengeokube/kit4dl}},
-  publisher = {Zenodo},
-  version = {2023.9b1},
-  doi = {10.5281/zenodo.8328176},
-  url = {https://doi.org/10.5281/zenodo.8328176}
+@ARTICLE{kit4dl,
+    author = {Jakub Walczak and Marco Mancini and Shahbaz Alvi},
+    title = {Kit4DL: Towards fast prototyping and experimentation in machine learning and deep learning},
+    journal = {SoftwareX},
+    volume = {26},
+    pages = {101707},
+    year = {2024},
+    issn = {2352-7110},
+    doi = {https://doi.org/10.1016/j.softx.2024.101707},
+    url = {https://www.sciencedirect.com/science/article/pii/S2352711024000785},
+    keywords = {Deep learning, Machine learning, Prototyping, Python framework},
 }
 ```
+## 📖 Documentation
+Read the official [Documentation](https://opengeokube.github.io/kit4dl/index.html) to learn Kit4DL!
+
 ## 🚧 Roadmap
 
 > **Warning**: Kit4DL is currently in its alpha stage. All recommendations are welcomed.
 
 - [ ] add handling sklearn-like models
 - [ ] add functionality to serve the model
 - [x] enable custom metrics
 - [x] enable using callbacks (also custom ones)
 - [ ] write more unit tests
+- [ ] enable overwritting parameters with command line
 
+## 🙏 Acknowledgement
+This work has received fundings from the Polish National Centre for Research and Development under the LIDER XI program [grant number 0092/L-11/2019, "Semantic analysis of 3D point clouds"] and from the European Union’s Horizon 2020 Research and Innovation programme [SILVANUS Project - grant agreement number 101037247].
 
 ## 🎬 Quickstart
 
 ### Getting started
 
 #### Installation
 ```bash
@@ -142,14 +146,15 @@
 1. [Configuring optimizer](#configuring-optimizer)
 1. [Configuring criterion](#configuring-criterion)
 1. [Configuring metrics](#configuring-metrics)
 1. [Configuring checkpoint](#configuring-checkpoint)
 1. [Defining `target`](#defining-target)
 1. [Substitutable symbols](#substitutable-symbols)
 1. [Context constants](#context-constants)
+1. [Sensitive data obfuscating](#sensitive-data-obfuscating)
 
 #### Configuring base setup
 Most of the training/validation procedure is managed by a configuration file in the TOML format (recommended name is `conf.toml`).
 Each aspect is covered by separate sections. The general one is called `[base]`.
 It has the following properties:
 
 |   **Property** 	|  **Type**        |                                                   **Details**                                          	|
@@ -213,15 +218,15 @@
 In the `configure` method, the architecture of the network should be defined. 
 In `run_step` method, it turn, the logic for single forward pass should be implemented.
 
 ##### ✍️ Example
 ```python
 import torch
 from torch import nn
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 class SimpleCNN(Kit4DLAbstractModule):
     def configure(self, input_dims, output_dims) -> None:
         self.l1 = nn.Sequential(
             nn.Conv2d(
                 input_dims, 16, kernel_size=3, padding="same", bias=True
             ),
@@ -253,15 +258,15 @@
 
 If a forward pass for your model differs for the training, validation, test, or prediction stages, you can define separate methods for them:
 
 ##### ✍️ Example
 ```python
 import torch
 from torch import nn
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 class SimpleCNN(Kit4DLAbstractModule):
     ...
     def run_val_step(self, batch, batch_idx) -> tuple[torch.Tensor, torch.Tensor]:
         pass
 
     def run_test_step(self, batch, batch_idx) -> tuple[torch.Tensor, torch.Tensor]:
@@ -272,27 +277,27 @@
 ```
 
 > **Note**: If you need more customization of the process, you can always override the existing methods according to your needs.
 
 #### Defining datamodule
 Similarily to the model, datamodule instance is fully defined by the Python class and its configuration.
 The datamodule need to be a subclass of the `Kit4DLAbstractDataModule` abstract class from the `kit4dl` package.
-The class has to implement, at least, `prepare_trainvaldataset` (if preparing is the same for the train and validation splits) or `prepare_traindataset` and `prepare_valdataset` (if preparing data differs). Besides those, you can define `prepare_testdataset` and `prepare_predictdataset`, for test and prediction, respectively.
+The class has to implement, at least, `prepare_trainvaldatasets` (if preparing is the same for the train and validation splits) or `prepare_traindatasets` and `prepare_valdatasets` (if preparing data differs). Besides those, you can define `prepare_testdataset` and `prepare_predictdataset`, for test and prediction, respectively.
 
 ##### ✍️ Example
 ```python
 from torch.utils.data import Dataset, random_split
 from torchvision import transforms
 from torchvision.datasets import MNIST
 
-from kit4dl import Kit4DLAbstractDataModule
+from kit4dl.dataset import Kit4DLAbstractDataModule
 
 
 class MNISTCustomDatamodule(Kit4DLAbstractDataModule):
-    def prepare_trainvaldataset(
+    def prepare_trainvaldatasets(
         self, root_dir: str
     ) -> tuple[Dataset, Dataset]:
         dset = MNIST(
             root=root_dir,
             train=True,
             download=True,
             transform=transforms.ToTensor(),
@@ -377,16 +382,16 @@
 batch_size = 150
 shuffle = false
 num_workers = 4
 ```
 
 In the root `[dataset]` you should define `target` property being a path to the subclass of the `Kit4DLAbstractDataModule` module (see [Defining `target`](#defining-target)).
 Then, you need to define either `[dataset.trainval]` section or two separate sections: `[dataset.train]`, `[dataset.validation]`. There are also optional sections: `[dataset.test]` and `[dataset.predict]`.
-In `[dataset.trainval]` you pass values for parameters of the `prepare_trainvaldataset` method.
-Respectively, in the `[dataset.train]` you pass values for the parameters of the `prepare_traindataset` method, in `[dataset.validation]` — `prepare_valdataset`, `[dataset.test]` — `prepare_testdataset`, `[dataset.predict]` — `prepare_predictdataset`.
+In `[dataset.trainval]` you pass values for parameters of the `prepare_trainvaldatasets` method.
+Respectively, in the `[dataset.train]` you pass values for the parameters of the `prepare_traindatasets` method, in `[dataset.validation]` — `prepare_valdatasets`, `[dataset.test]` — `prepare_testdataset`, `[dataset.predict]` — `prepare_predictdataset`.
 
 Besides dataset configuration, you need to specify data loader arguments as indicated in the PyTorch docs [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader).
 
 > **Warning**: You **cannot** specify loader arguments for in the `[dataset.trainval.loader]`. Loaders should be defined for each split separately.
 
 
 #### Configuring training
@@ -417,15 +422,15 @@
 ```python
 import os
 from typing import Any
 
 import lightning.pytorch as pl
 import torchmetrics as tm
 
-from kit4dl import Kit4DLCallback, StepOutput
+from kit4dl import Kit4DLCallback
 
 
 class SaveConfusionMatrixCallback(Kit4DLCallback):
     _cm: tm.ConfusionMatrix
     _num_classes: int
     _task: str
     _save_dir: str
@@ -444,20 +449,20 @@
             task=self._task, num_classes=self._num_classes
         )
 
     def on_validation_batch_end(
         self,
         trainer: pl.Trainer,
         pl_module: pl.LightningModule,
-        outputs: StepOutput,
+        outputs: dict,
         batch: Any,
         batch_idx: int,
         dataloader_idx: int = 0,
     ) -> None:
-        self._cm.update(outputs.predictions, outputs.labels)
+        self._cm.update(outputs['pred'], outputs['true'])
 
     def on_validation_epoch_end(
         self, trainer: pl.Trainer, pl_module: pl.LightningModule
     ) -> None:
         """Called when the val epoch ends."""
         fig, _ = self._cm.plot()
         target_file = os.path.join(
@@ -640,7 +645,22 @@
 |   **Symbol** 	|            **Meaning of the symbol**                                   	|          **Example**                  |
 |-------------	|-----------------------------------------------------------------------	| -----------------------------------	|
 | `PROJECT_DIR`	| the home directory of the TOML configuration file (project directory) 	| `context.PROJECT_DIR`                 |
 | `LOG_LEVEL`	| logging level as defined in the configuration TOML file                	| `context.LOG_LEVEL`                   |
 | `LOG_FORMAT`	| logging message format as defined in the configuration TOML file      	| `context.LOG_FORMAT`                  |
 |  `VERSION`	| the current version of the package                                      	| `context.VERSION`                     |
 
+#### Sensitive data obfuscating
+It might happen, some sensitive data are stored in the configuration file. 
+We should prevent those data from being logged as hyperparameters. This is the reason why
+Kit4DL supports sensitive data obfuscating. By default, all values whose keys contain `key` string
+will be obfuscated with `***`. Both, sensitive data key and obfuscating value can be customized by
+a user, by setting environmental variables accordingly. To obfuscate all
+values containig `url` (e.g.`api-url`, `url-2`, etc.) with `^^^`, just use
+the following code.
+
+##### ✍️ Example
+```python
+import os
+os.environ["KIT4DL_KEY_TO_OBFUSCATE"] = "url"
+os.environ["KIT4DL_OBFUSCATING_VALUE"] = "^^^"
+```
```

#### html2text {}

```diff
@@ -18,77 +18,86 @@
 zenodo.8328176.svg)](https://doi.org/10.5281/zenodo.8328176) [![Conda Version]
 (https://img.shields.io/conda/vn/conda-forge/kit4dl.svg)](https://anaconda.org/
 conda-forge/kit4dl) [![Conda Downloads](https://img.shields.io/conda/dn/conda-
  forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl) [![PyPI version]
     (https://badge.fury.io/py/kit4dl.svg)](https://badge.fury.io/py/kit4dl)
 ## ðï¸ Authors OpenGeokube Developers: 1. Jakub Walczak _[_O_R_C_I_D_ _l_o_g_o_]1.
 Marco Macini _[_O_R_C_I_D_ _l_o_g_o_]1. Mirko Stojiljkovic _[_O_R_C_I_D_ _l_o_g_o_]1. Shahbaz Alvi
-_[_O_R_C_I_D_ _l_o_g_o_]## ð Cite Us ```bibtex @SOFTWARE{kit4dl, author = {Walczak,
-Jakub and Mancini, Marco and StojiljkoviÄ, Mirko and Alvi, Shahbaz}, title =
-{Kit4DL}, month = sep, year = 2023, note = {{Available in GitHub: https://
-github.com/opengeokube/kit4dl}}, publisher = {Zenodo}, version = {2023.9b1},
-doi = {10.5281/zenodo.8328176}, url = {https://doi.org/10.5281/zenodo.8328176}
-} ``` ## ð§ Roadmap > **Warning**: Kit4DL is currently in its alpha stage.
-All recommendations are welcomed. - [ ] add handling sklearn-like models - [ ]
-add functionality to serve the model - [x] enable custom metrics - [x] enable
-using callbacks (also custom ones) - [ ] write more unit tests ## ð¬
-Quickstart ### Getting started #### Installation ```bash pip install kit4dl ```
-or ```bash conda install -c conda-forge kit4dl ``` For contributing: Download
-and install the `make` tool unless it is already available in your system.
-```text git clone https://github.com/opengeokube/kit4dl cd kit4dl conda env
-create -f dev-env.yaml pip install -e . ``` #### Preparing simple project To
-start the new project in the current working directory, just run the following
-command: ```bash kit4dl init --name=my-new-project ``` It will create a
-directory with the name `my-new-project` where you'll find sample files.
-Implement necessery methods for datamodule (`dataset.py`) and network
-(`model.py`). Then, adjust `conf.toml` according to your needs. That's all ð
-#### Running the training To run the training just type the following command:
-```bash kit4dl train ``` > **Note**: If you want to run also test for best
-saved weight, use flag `--test` If the `conf.toml` file is present in your
-current working directory, the training will start. If you need to specify the
-path to the configuration file, use `--conf` argument: ```bash kit4dl train --
-conf=/path/to/your/conf.toml ``` #### Serving the model The packuge does not
-yet support model serving. ## ðª Playground At first, install `kit4dl`
-package as indicated in the Section [Installation](#installation). ####
-Handwritten digit recognition Just navigate to the directory `/examples/
-cnn_mnist_classification` and run ```bash kit4dl train ``` #### Point cloud
-instance segmentation Just navigate to the directory `/examples/
-cnn_s3dis_segmentation` and run ```bash kit4dl train ``` ## ð¡ Instruction 1.
-[Configuring base setup](#configuring-base-setup) 1. [Configuring logging]
-(#configuring-logging) 1. [Defining model](#defining-model) 1. [Defining
-datamodule](#defining-datamodule) 1. [Configuring training](#configuring-
-training) 1. [Configuring optimizer](#configuring-optimizer) 1. [Configuring
-criterion](#configuring-criterion) 1. [Configuring metrics](#configuring-
-metrics) 1. [Configuring checkpoint](#configuring-checkpoint) 1. [Defining
-`target`](#defining-target) 1. [Substitutable symbols](#substitutable-symbols)
-1. [Context constants](#context-constants) #### Configuring base setup Most of
-the training/validation procedure is managed by a configuration file in the
-TOML format (recommended name is `conf.toml`). Each aspect is covered by
-separate sections. The general one is called `[base]`. It has the following
-properties: | **Property** | **Type** | **Details** | |--------------- |-------
----------- | ------------------------------------------------------------------
-------------------------------------- | | `seed` | `int` | seed of the random
-numbers generators for `NumPy` and `PyTorch` | | `cuda_id` | `int` or `None` |
-ID of the cuda device (if available) or `None` for `CPU` | |`experiment_name`*
-| `str` | name of the experiment | > **Note**: Arguments marked with `*` are
-obligatory! > **Warning**: Remember to install the version of `pytorch-cuda`
-package compliant to your CUDA Toolkit version. ##### âï¸ Example ```toml
-[base] seed = 0 cuda_id = 1 experiment_name = "point_clout_segmentation" ```
-#### Configuring logging Logging section is optional but it provides you with
-some extra flexibility regarding the logging. All configuration related to
-logging is included in the `[logging]` section of the configuration file. You
-can define following properties: | **Property** | **Type** | **Details** | |---
------------- |----------------- | ---------------------------------------------
----------------------------------------------------------- | | `type` | `str` |
-type of metric logger (one of the value: `"comet"`, `"csv"`, `"mlflow"`,
-`"neptune"`, `"tensorboard"`, `"wandb"` - metric loggers supported by PyTorch
-Lightning [https://lightning.ai/docs/pytorch/stable/
-api_references.html#loggers](https://lightning.ai/docs/pytorch/stable/
-api_references.html#loggers). **DEFAULT:** `csv`) | | `level` | `str` | Python-
-supported logging levels (i.e. `"DEBUG"`, `"INFO"`, `"WARN"`, `"ERROR"`,
+_[_O_R_C_I_D_ _l_o_g_o_]## ð Cite Us ```bibtex @ARTICLE{kit4dl, author = {Jakub Walczak
+and Marco Mancini and Shahbaz Alvi}, title = {Kit4DL: Towards fast prototyping
+and experimentation in machine learning and deep learning}, journal =
+{SoftwareX}, volume = {26}, pages = {101707}, year = {2024}, issn = {2352-
+7110}, doi = {https://doi.org/10.1016/j.softx.2024.101707}, url = {https://
+www.sciencedirect.com/science/article/pii/S2352711024000785}, keywords = {Deep
+learning, Machine learning, Prototyping, Python framework}, } ``` ## ð
+Documentation Read the official [Documentation](https://opengeokube.github.io/
+kit4dl/index.html) to learn Kit4DL! ## ð§ Roadmap > **Warning**: Kit4DL is
+currently in its alpha stage. All recommendations are welcomed. - [ ] add
+handling sklearn-like models - [ ] add functionality to serve the model - [x]
+enable custom metrics - [x] enable using callbacks (also custom ones) - [ ]
+write more unit tests - [ ] enable overwritting parameters with command line ##
+ð Acknowledgement This work has received fundings from the Polish National
+Centre for Research and Development under the LIDER XI program [grant number
+0092/L-11/2019, "Semantic analysis of 3D point clouds"] and from the European
+Unionâs Horizon 2020 Research and Innovation programme [SILVANUS Project -
+grant agreement number 101037247]. ## ð¬ Quickstart ### Getting started ####
+Installation ```bash pip install kit4dl ``` or ```bash conda install -c conda-
+forge kit4dl ``` For contributing: Download and install the `make` tool unless
+it is already available in your system. ```text git clone https://github.com/
+opengeokube/kit4dl cd kit4dl conda env create -f dev-env.yaml pip install -e .
+``` #### Preparing simple project To start the new project in the current
+working directory, just run the following command: ```bash kit4dl init --
+name=my-new-project ``` It will create a directory with the name `my-new-
+project` where you'll find sample files. Implement necessery methods for
+datamodule (`dataset.py`) and network (`model.py`). Then, adjust `conf.toml`
+according to your needs. That's all ð #### Running the training To run the
+training just type the following command: ```bash kit4dl train ``` > **Note**:
+If you want to run also test for best saved weight, use flag `--test` If the
+`conf.toml` file is present in your current working directory, the training
+will start. If you need to specify the path to the configuration file, use `--
+conf` argument: ```bash kit4dl train --conf=/path/to/your/conf.toml ``` ####
+Serving the model The packuge does not yet support model serving. ## ðª
+Playground At first, install `kit4dl` package as indicated in the Section
+[Installation](#installation). #### Handwritten digit recognition Just navigate
+to the directory `/examples/cnn_mnist_classification` and run ```bash kit4dl
+train ``` #### Point cloud instance segmentation Just navigate to the directory
+`/examples/cnn_s3dis_segmentation` and run ```bash kit4dl train ``` ## ð¡
+Instruction 1. [Configuring base setup](#configuring-base-setup) 1.
+[Configuring logging](#configuring-logging) 1. [Defining model](#defining-
+model) 1. [Defining datamodule](#defining-datamodule) 1. [Configuring training]
+(#configuring-training) 1. [Configuring optimizer](#configuring-optimizer) 1.
+[Configuring criterion](#configuring-criterion) 1. [Configuring metrics]
+(#configuring-metrics) 1. [Configuring checkpoint](#configuring-checkpoint) 1.
+[Defining `target`](#defining-target) 1. [Substitutable symbols]
+(#substitutable-symbols) 1. [Context constants](#context-constants) 1.
+[Sensitive data obfuscating](#sensitive-data-obfuscating) #### Configuring base
+setup Most of the training/validation procedure is managed by a configuration
+file in the TOML format (recommended name is `conf.toml`). Each aspect is
+covered by separate sections. The general one is called `[base]`. It has the
+following properties: | **Property** | **Type** | **Details** | |--------------
+- |----------------- | --------------------------------------------------------
+----------------------------------------------- | | `seed` | `int` | seed of
+the random numbers generators for `NumPy` and `PyTorch` | | `cuda_id` | `int`
+or `None` | ID of the cuda device (if available) or `None` for `CPU` |
+|`experiment_name`* | `str` | name of the experiment | > **Note**: Arguments
+marked with `*` are obligatory! > **Warning**: Remember to install the version
+of `pytorch-cuda` package compliant to your CUDA Toolkit version. ##### âï¸
+Example ```toml [base] seed = 0 cuda_id = 1 experiment_name =
+"point_clout_segmentation" ``` #### Configuring logging Logging section is
+optional but it provides you with some extra flexibility regarding the logging.
+All configuration related to logging is included in the `[logging]` section of
+the configuration file. You can define following properties: | **Property** |
+**Type** | **Details** | |--------------- |----------------- | ----------------
+-------------------------------------------------------------------------------
+-------- | | `type` | `str` | type of metric logger (one of the value:
+`"comet"`, `"csv"`, `"mlflow"`, `"neptune"`, `"tensorboard"`, `"wandb"` -
+metric loggers supported by PyTorch Lightning [https://lightning.ai/docs/
+pytorch/stable/api_references.html#loggers](https://lightning.ai/docs/pytorch/
+stable/api_references.html#loggers). **DEFAULT:** `csv`) | | `level` | `str` |
+Python-supported logging levels (i.e. `"DEBUG"`, `"INFO"`, `"WARN"`, `"ERROR"`,
 `"CRITICAL"`) **DEFAULT:** `INFO` | |`format` | `str` | logging message format
 as defined for the Python `logging` package (see [https://docs.python.org/3/
 library/logging.html#logging.LogRecord](https://docs.python.org/3/library/
 logging.html#logging.LogRecord)) | > **Warning**: Logger `level` and `format`
 are related to the Python `logging` Loggers you can use in your model and
 datamodule classes with approperiate methods `self.debure`, `self.info`, etc.
 In `type`, in turn, you just specify the metric logger as used in PyTorch
@@ -110,52 +119,53 @@
 `.py` file. 1. The configuration in the `[model]` section of the configuration
 file. The file with the model definition should contain a subclass of
 `Kit4DLAbstractModule` abstract class of the `kit4dl` package. The subclass
 should implement, at least, abstract methods `configure` and `run_step`. In the
 `configure` method, the architecture of the network should be defined. In
 `run_step` method, it turn, the logic for single forward pass should be
 implemented. ##### âï¸ Example ```python import torch from torch import nn
-from kit4dl import Kit4DLAbstractModule class SimpleCNN(Kit4DLAbstractModule):
-def configure(self, input_dims, output_dims) -> None: self.l1 = nn.Sequential
-( nn.Conv2d( input_dims, 16, kernel_size=3, padding="same", bias=True ),
-nn.ReLU(), ) def run_step(self, batch, batch_idx) -> tuple[torch.Tensor, ...]:
-x, label = batch logits = self.l1(x) preds = logits.argmax(dim=-1) return
-label, logits, preds ``` > **Note**: `run_step` method should return a tuple of
-2 (ground-truth, scores) or 3 (ground-truth, scores, loss) tensors. > **Note**:
-`batch` argument can be unpacked depending on how you define your dataset for
-datamodule (see [Defining datamodule](#defining-datamodule)) In the
-configuration file, in the dedicated `[model]` section, at least `target`
-property should be set. The extra arguments are treated as the arguments for
-the `configure` method. > **Note**: Arguments' values of the `configure` method
-(i.e. `input_dims` and `output_dims`) are taken from the configuration files.
-Those names can be arbitrary. ##### âï¸ Example ```toml [model] target = "./
-model.py::SimpleCNN" input_dims = 1 output_dims = 10 ``` > **Note**: `target`
-is a required parameter that **must** be set. It contains a path to the class
-(a subclass of `Kit4DLAbstractModule`). To learn how `target` could be defined,
-see Section [Defining `target`](#defining-target). If a forward pass for your
-model differs for the training, validation, test, or prediction stages, you can
-define separate methods for them: ##### âï¸ Example ```python import torch
-from torch import nn from kit4dl import Kit4DLAbstractModule class SimpleCNN
+from kit4dl.nn.base import Kit4DLAbstractModule class SimpleCNN
+(Kit4DLAbstractModule): def configure(self, input_dims, output_dims) -> None:
+self.l1 = nn.Sequential( nn.Conv2d( input_dims, 16, kernel_size=3,
+padding="same", bias=True ), nn.ReLU(), ) def run_step(self, batch, batch_idx)
+-> tuple[torch.Tensor, ...]: x, label = batch logits = self.l1(x) preds =
+logits.argmax(dim=-1) return label, logits, preds ``` > **Note**: `run_step`
+method should return a tuple of 2 (ground-truth, scores) or 3 (ground-truth,
+scores, loss) tensors. > **Note**: `batch` argument can be unpacked depending
+on how you define your dataset for datamodule (see [Defining datamodule]
+(#defining-datamodule)) In the configuration file, in the dedicated `[model]`
+section, at least `target` property should be set. The extra arguments are
+treated as the arguments for the `configure` method. > **Note**: Arguments'
+values of the `configure` method (i.e. `input_dims` and `output_dims`) are
+taken from the configuration files. Those names can be arbitrary. ##### âï¸
+Example ```toml [model] target = "./model.py::SimpleCNN" input_dims = 1
+output_dims = 10 ``` > **Note**: `target` is a required parameter that **must**
+be set. It contains a path to the class (a subclass of `Kit4DLAbstractModule`).
+To learn how `target` could be defined, see Section [Defining `target`]
+(#defining-target). If a forward pass for your model differs for the training,
+validation, test, or prediction stages, you can define separate methods for
+them: ##### âï¸ Example ```python import torch from torch import nn from
+kit4dl.nn.base import Kit4DLAbstractModule class SimpleCNN
 (Kit4DLAbstractModule): ... def run_val_step(self, batch, batch_idx) -> tuple
 [torch.Tensor, torch.Tensor]: pass def run_test_step(self, batch, batch_idx) -
 > tuple[torch.Tensor, torch.Tensor]: pass def run_predict_step(self, batch,
 batch_idx) -> torch.Tensor: pass ``` > **Note**: If you need more customization
 of the process, you can always override the existing methods according to your
 needs. #### Defining datamodule Similarily to the model, datamodule instance is
 fully defined by the Python class and its configuration. The datamodule need to
 be a subclass of the `Kit4DLAbstractDataModule` abstract class from the
 `kit4dl` package. The class has to implement, at least,
-`prepare_trainvaldataset` (if preparing is the same for the train and
-validation splits) or `prepare_traindataset` and `prepare_valdataset` (if
+`prepare_trainvaldatasets` (if preparing is the same for the train and
+validation splits) or `prepare_traindatasets` and `prepare_valdatasets` (if
 preparing data differs). Besides those, you can define `prepare_testdataset`
 and `prepare_predictdataset`, for test and prediction, respectively. #####
 âï¸ Example ```python from torch.utils.data import Dataset, random_split
 from torchvision import transforms from torchvision.datasets import MNIST from
-kit4dl import Kit4DLAbstractDataModule class MNISTCustomDatamodule
-(Kit4DLAbstractDataModule): def prepare_trainvaldataset( self, root_dir: str )
+kit4dl.dataset import Kit4DLAbstractDataModule class MNISTCustomDatamodule
+(Kit4DLAbstractDataModule): def prepare_trainvaldatasets( self, root_dir: str )
 -> tuple[Dataset, Dataset]: dset = MNIST( root=root_dir, train=True,
 download=True, transform=transforms.ToTensor(), ) train_dset, val_dset =
 random_split(dset, [0.8, 0.2]) return (train_dset, val_dset) def
 prepare_testdataset(self, root_dir: str) -> Dataset: return MNIST
 ( root=root_dir, train=False, download=True, transform=transforms.ToTensor(), )
 ``` If you need to acquire data or do some other processing, implement
 `prepare_data` method. In that method you can use extra attributes you defined
@@ -184,17 +194,17 @@
 [dataset.validation.loader] batch_size = 150 shuffle = false num_workers = 4
 ``` In the root `[dataset]` you should define `target` property being a path to
 the subclass of the `Kit4DLAbstractDataModule` module (see [Defining `target`]
 (#defining-target)). Then, you need to define either `[dataset.trainval]`
 section or two separate sections: `[dataset.train]`, `[dataset.validation]`.
 There are also optional sections: `[dataset.test]` and `[dataset.predict]`. In
 `[dataset.trainval]` you pass values for parameters of the
-`prepare_trainvaldataset` method. Respectively, in the `[dataset.train]` you
-pass values for the parameters of the `prepare_traindataset` method, in `
-[dataset.validation]` â `prepare_valdataset`, `[dataset.test]` â
+`prepare_trainvaldatasets` method. Respectively, in the `[dataset.train]` you
+pass values for the parameters of the `prepare_traindatasets` method, in `
+[dataset.validation]` â `prepare_valdatasets`, `[dataset.test]` â
 `prepare_testdataset`, `[dataset.predict]` â `prepare_predictdataset`.
 Besides dataset configuration, you need to specify data loader arguments as
 indicated in the PyTorch docs [torch.utils.data.DataLoader](https://
 pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader). > **Warning**:
 You **cannot** specify loader arguments for in the `[dataset.trainval.loader]`.
 Loaders should be defined for each split separately. #### Configuring training
 Training-related arguments should be defined in the `[training]` section of the
@@ -213,28 +223,28 @@
 [ {target = "./callbacks.py::SaveConfusionMatrixCallback", task="multiclass",
 num_classes=10, save_dir="{{ PROJECT_DIR }}/cm}, {target =
 "lightning.pytorch.callbacks::DeviceStatsMonitor"} ] ``` Where the 1st callback
 is user-defined and the other - PyTorch-Loghtning built-in. For the custom
 callback we need to provide a class (here: located in the `callbacks.py` file
 in the project directory, the class is named `SaveConfusionMatrixCallback`).
 ```python import os from typing import Any import lightning.pytorch as pl
-import torchmetrics as tm from kit4dl import Kit4DLCallback, StepOutput class
+import torchmetrics as tm from kit4dl import Kit4DLCallback class
 SaveConfusionMatrixCallback(Kit4DLCallback): _cm: tm.ConfusionMatrix
 _num_classes: int _task: str _save_dir: str def __init__(self, task: str,
 num_classes: int, save_dir: str) -> None: super().__init__() self._num_classes
 = num_classes self._save_dir = save_dir self._task = task os.makedirs
 (self._save_dir, exist_ok=True) def on_validation_epoch_start( self, trainer:
 pl.Trainer, pl_module: pl.LightningModule ) -> None: self._cm =
 tm.ConfusionMatrix( task=self._task, num_classes=self._num_classes ) def
 on_validation_batch_end( self, trainer: pl.Trainer, pl_module:
-pl.LightningModule, outputs: StepOutput, batch: Any, batch_idx: int,
-dataloader_idx: int = 0, ) -> None: self._cm.update(outputs.predictions,
-outputs.labels) def on_validation_epoch_end( self, trainer: pl.Trainer,
-pl_module: pl.LightningModule ) -> None: """Called when the val epoch ends."""
-fig, _ = self._cm.plot() target_file = os.path.join( self._save_dir,
+pl.LightningModule, outputs: dict, batch: Any, batch_idx: int, dataloader_idx:
+int = 0, ) -> None: self._cm.update(outputs['pred'], outputs['true']) def
+on_validation_epoch_end( self, trainer: pl.Trainer, pl_module:
+pl.LightningModule ) -> None: """Called when the val epoch ends.""" fig, _ =
+self._cm.plot() target_file = os.path.join( self._save_dir,
 f"confusion_matrix_for_epoch_{pl_module.current_epoch}", ) fig.savefig
 (target_file) ``` Besides those listed in the table above, you can specify
 PyTorch Lightning-related `Trainer` arguments, like: 1.
 `accumulate_grad_batches` 1. `gradient_clip_val` 1. `gradient_clip_algorithm`
 1. ... ##### âï¸ Example ```toml [training] epochs = 10 epoch_schedulers =
 [ {target = "torch.optim.lr_scheduler::CosineAnnealingLR", T_max = 100} ]
 accumulate_grad_batches = 2 ``` #### Configuring optimizer Optimizer
@@ -338,8 +348,17 @@
 following: | **Symbol** | **Meaning of the symbol** | **Example** | |----------
 --- |----------------------------------------------------------------------- |
 ----------------------------------- | | `PROJECT_DIR` | the home directory of
 the TOML configuration file (project directory) | `context.PROJECT_DIR` | |
 `LOG_LEVEL` | logging level as defined in the configuration TOML file |
 `context.LOG_LEVEL` | | `LOG_FORMAT` | logging message format as defined in the
 configuration TOML file | `context.LOG_FORMAT` | | `VERSION` | the current
-version of the package | `context.VERSION` |
+version of the package | `context.VERSION` | #### Sensitive data obfuscating It
+might happen, some sensitive data are stored in the configuration file. We
+should prevent those data from being logged as hyperparameters. This is the
+reason why Kit4DL supports sensitive data obfuscating. By default, all values
+whose keys contain `key` string will be obfuscated with `***`. Both, sensitive
+data key and obfuscating value can be customized by a user, by setting
+environmental variables accordingly. To obfuscate all values containig `url`
+(e.g.`api-url`, `url-2`, etc.) with `^^^`, just use the following code. #####
+âï¸ Example ```python import os os.environ["KIT4DL_KEY_TO_OBFUSCATE"] =
+"url" os.environ["KIT4DL_OBFUSCATING_VALUE"] = "^^^" ```
```

### Comparing `kit4dl-2023.9b2/examples/cnn_mnist_classification/conf.toml` & `kit4dl-2024.5b0/examples/cnn_mnist_classification/conf.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,90 +10,91 @@
 00000090: 616d 6529 7320 2d20 2528 6d65 7373 6167  ame)s - %(messag
 000000a0: 6529 7322 0d0a 0d0a 5b6d 6f64 656c 5d0d  e)s"....[model].
 000000b0: 0a23 2057 6520 6361 6e20 7573 6520 7265  .# We can use re
 000000c0: 6c61 7469 7665 2070 6174 6820 2877 2e72  lative path (w.r
 000000d0: 2e74 2e20 7468 6520 636f 6e66 2e74 6f6d  .t. the conf.tom
 000000e0: 6c20 6669 6c65 2920 746f 2074 6865 202e  l file) to the .
 000000f0: 7079 2066 696c 650d 0a74 6172 6765 7420  py file..target 
-00000100: 3d20 222e 2f6d 6f64 656c 2e70 793a 3a53  = "./model.py::S
-00000110: 696d 706c 6543 4e4e 2220 0d0a 696e 7075  impleCNN" ..inpu
-00000120: 745f 6469 6d73 203d 2031 0d0a 6c61 7965  t_dims = 1..laye
-00000130: 7273 203d 2034 0d0a 6472 6f70 6f75 7420  rs = 4..dropout 
-00000140: 3d20 302e 350d 0a6f 7574 7075 745f 6469  = 0.5..output_di
-00000150: 6d73 203d 2031 300d 0a0d 0a5b 7472 6169  ms = 10....[trai
-00000160: 6e69 6e67 5d0d 0a65 706f 6368 7320 3d20  ning]..epochs = 
-00000170: 3130 0d0a 6570 6f63 685f 7363 6865 6475  10..epoch_schedu
-00000180: 6c65 7273 203d 205b 0d0a 2020 2020 7b74  lers = [..    {t
-00000190: 6172 6765 7420 3d20 2274 6f72 6368 2e6f  arget = "torch.o
-000001a0: 7074 696d 2e6c 725f 7363 6865 6475 6c65  ptim.lr_schedule
-000001b0: 723a 3a43 6f73 696e 6541 6e6e 6561 6c69  r::CosineAnneali
-000001c0: 6e67 4c52 222c 2054 5f6d 6178 203d 2031  ngLR", T_max = 1
-000001d0: 3030 7d0d 0a5d 0d0a 6361 6c6c 6261 636b  00}..]..callback
-000001e0: 7320 3d20 5b0d 0a20 2020 207b 7461 7267  s = [..    {targ
-000001f0: 6574 203d 2022 2e2f 6361 6c6c 6261 636b  et = "./callback
-00000200: 732e 7079 3a3a 5361 7665 436f 6e66 7573  s.py::SaveConfus
-00000210: 696f 6e4d 6174 7269 7843 616c 6c62 6163  ionMatrixCallbac
-00000220: 6b22 2c20 2074 6173 6b3d 226d 756c 7469  k",  task="multi
-00000230: 636c 6173 7322 2c20 6e75 6d5f 636c 6173  class", num_clas
-00000240: 7365 7320 3d20 3130 2c20 7361 7665 5f64  ses = 10, save_d
-00000250: 6972 203d 2022 7b7b 2050 524f 4a45 4354  ir = "{{ PROJECT
-00000260: 5f44 4952 207d 7d2f 636d 227d 2c0d 0a20  _DIR }}/cm"},.. 
-00000270: 2020 207b 7461 7267 6574 203d 2022 6c69     {target = "li
-00000280: 6768 746e 696e 672e 7079 746f 7263 682e  ghtning.pytorch.
-00000290: 6361 6c6c 6261 636b 733a 3a44 6576 6963  callbacks::Devic
-000002a0: 6553 7461 7473 4d6f 6e69 746f 7222 7d0d  eStatsMonitor"}.
-000002b0: 0a5d 0d0a 0d0a 5b74 7261 696e 696e 672e  .]....[training.
-000002c0: 6368 6563 6b70 6f69 6e74 5d0d 0a70 6174  checkpoint]..pat
-000002d0: 6820 3d20 2263 6863 6b70 7422 0d0a 6d6f  h = "chckpt"..mo
-000002e0: 6e69 746f 7220 3d20 7b22 6d65 7472 6963  nitor = {"metric
-000002f0: 2220 3d20 224d 7950 7265 6369 7369 6f6e  " = "MyPrecision
-00000300: 222c 2022 7374 6167 6522 203d 2022 7661  ", "stage" = "va
-00000310: 6c22 7d0d 0a66 696c 656e 616d 6520 3d20  l"}..filename = 
-00000320: 227b 6570 6f63 687d 5f7b 7661 6c5f 6d79  "{epoch}_{val_my
-00000330: 7072 6563 6973 696f 6e3a 2e32 667d 5f63  precision:.2f}_c
-00000340: 6e6e 220d 0a6d 6f64 6520 3d20 226d 6178  nn"..mode = "max
-00000350: 220d 0a73 6176 655f 746f 705f 6b20 3d20  "..save_top_k = 
-00000360: 310d 0a0d 0a5b 7472 6169 6e69 6e67 2e6f  1....[training.o
-00000370: 7074 696d 697a 6572 5d0d 0a74 6172 6765  ptimizer]..targe
-00000380: 7420 3d20 2274 6f72 6368 2e6f 7074 696d  t = "torch.optim
-00000390: 3a3a 4164 616d 220d 0a6c 7220 3d20 302e  ::Adam"..lr = 0.
-000003a0: 3030 310d 0a77 6569 6768 745f 6465 6361  001..weight_deca
-000003b0: 7920 3d20 302e 3031 0d0a 0d0a 5b74 7261  y = 0.01....[tra
-000003c0: 696e 696e 672e 6372 6974 6572 696f 6e5d  ining.criterion]
-000003d0: 0d0a 7461 7267 6574 203d 2022 746f 7263  ..target = "torc
-000003e0: 682e 6e6e 3a3a 4372 6f73 7345 6e74 726f  h.nn::CrossEntro
-000003f0: 7079 4c6f 7373 220d 0a77 6569 6768 7420  pyLoss"..weight 
-00000400: 3d20 5b30 2e31 2c20 302e 312c 2030 2e31  = [0.1, 0.1, 0.1
-00000410: 2c20 302e 312c 2030 2e31 2c20 302e 312c  , 0.1, 0.1, 0.1,
-00000420: 2030 2e31 2c20 302e 312c 2030 2e31 2c20   0.1, 0.1, 0.1, 
-00000430: 302e 315d 0d0a 0d0a 5b76 616c 6964 6174  0.1]....[validat
-00000440: 696f 6e5d 0d0a 7275 6e5f 6576 6572 795f  ion]..run_every_
-00000450: 6570 6f63 6820 3d20 310d 0a0d 0a5b 6461  epoch = 1....[da
-00000460: 7461 7365 745d 0d0a 7461 7267 6574 203d  taset]..target =
-00000470: 2022 2e2f 6461 7461 6d6f 6475 6c65 2e70   "./datamodule.p
-00000480: 793a 3a4d 4e49 5354 4375 7374 6f6d 4461  y::MNISTCustomDa
-00000490: 7461 6d6f 6475 6c65 220d 0a0d 0a5b 6461  tamodule"....[da
-000004a0: 7461 7365 742e 7472 6169 6e76 616c 5d0d  taset.trainval].
-000004b0: 0a72 6f6f 745f 6469 7220 3d20 222e 2f6d  .root_dir = "./m
-000004c0: 6e69 7374 220d 0a0d 0a5b 6461 7461 7365  nist"....[datase
-000004d0: 742e 7472 6169 6e2e 6c6f 6164 6572 5d0d  t.train.loader].
-000004e0: 0a62 6174 6368 5f73 697a 6520 3d20 3135  .batch_size = 15
-000004f0: 300d 0a73 6875 6666 6c65 203d 2074 7275  0..shuffle = tru
-00000500: 650d 0a6e 756d 5f77 6f72 6b65 7273 203d  e..num_workers =
-00000510: 2034 0d0a 0d0a 5b64 6174 6173 6574 2e76   4....[dataset.v
-00000520: 616c 6964 6174 696f 6e2e 6c6f 6164 6572  alidation.loader
-00000530: 5d0d 0a62 6174 6368 5f73 697a 6520 3d20  ]..batch_size = 
-00000540: 3135 300d 0a73 6875 6666 6c65 203d 2066  150..shuffle = f
-00000550: 616c 7365 0d0a 6e75 6d5f 776f 726b 6572  alse..num_worker
-00000560: 7320 3d20 340d 0a0d 0a5b 6d65 7472 6963  s = 4....[metric
-00000570: 735d 0d0a 4d79 5072 6563 6973 696f 6e20  s]..MyPrecision 
-00000580: 3d20 7b74 6172 6765 7420 3d20 2274 6f72  = {target = "tor
-00000590: 6368 6d65 7472 6963 733a 3a50 7265 6369  chmetrics::Preci
-000005a0: 7369 6f6e 222c 2074 6173 6b20 3d20 226d  sion", task = "m
-000005b0: 756c 7469 636c 6173 7322 2c20 6e75 6d5f  ulticlass", num_
-000005c0: 636c 6173 7365 733d 3130 7d0d 0a46 4265  classes=10}..FBe
-000005d0: 7461 5363 6f72 6520 3d20 7b74 6172 6765  taScore = {targe
-000005e0: 7420 3d20 2274 6f72 6368 6d65 7472 6963  t = "torchmetric
-000005f0: 733a 3a46 4265 7461 5363 6f72 6522 2c20  s::FBetaScore", 
-00000600: 7461 736b 203d 2022 6d75 6c74 6963 6c61  task = "multicla
-00000610: 7373 222c 206e 756d 5f63 6c61 7373 6573  ss", num_classes
-00000620: 3d31 302c 2062 6574 6120 3d20 302e 317d  =10, beta = 0.1}
+00000100: 3d20 226d 6f64 656c 3a3a 5369 6d70 6c65  = "model::Simple
+00000110: 434e 4e22 200d 0a69 6e70 7574 5f64 696d  CNN" ..input_dim
+00000120: 7320 3d20 310d 0a6c 6179 6572 7320 3d20  s = 1..layers = 
+00000130: 340d 0a64 726f 706f 7574 203d 2030 2e35  4..dropout = 0.5
+00000140: 0d0a 6f75 7470 7574 5f64 696d 7320 3d20  ..output_dims = 
+00000150: 3130 0d0a 0d0a 5b74 7261 696e 696e 675d  10....[training]
+00000160: 0d0a 6570 6f63 6873 203d 2031 0d0a 6570  ..epochs = 1..ep
+00000170: 6f63 685f 7363 6865 6475 6c65 7273 203d  och_schedulers =
+00000180: 205b 0d0a 2020 2020 7b74 6172 6765 7420   [..    {target 
+00000190: 3d20 2274 6f72 6368 2e6f 7074 696d 2e6c  = "torch.optim.l
+000001a0: 725f 7363 6865 6475 6c65 723a 3a43 6f73  r_scheduler::Cos
+000001b0: 696e 6541 6e6e 6561 6c69 6e67 4c52 222c  ineAnnealingLR",
+000001c0: 2054 5f6d 6178 203d 2031 3030 7d0d 0a5d   T_max = 100}..]
+000001d0: 0d0a 6361 6c6c 6261 636b 7320 3d20 5b0d  ..callbacks = [.
+000001e0: 0a20 2020 207b 7461 7267 6574 203d 2022  .    {target = "
+000001f0: 6361 6c6c 6261 636b 733a 3a53 6176 6543  callbacks::SaveC
+00000200: 6f6e 6675 7369 6f6e 4d61 7472 6978 4361  onfusionMatrixCa
+00000210: 6c6c 6261 636b 222c 2020 7461 736b 3d22  llback",  task="
+00000220: 6d75 6c74 6963 6c61 7373 222c 206e 756d  multiclass", num
+00000230: 5f63 6c61 7373 6573 203d 2031 302c 2073  _classes = 10, s
+00000240: 6176 655f 6469 7220 3d20 227b 7b20 5052  ave_dir = "{{ PR
+00000250: 4f4a 4543 545f 4449 5220 7d7d 2f63 6d22  OJECT_DIR }}/cm"
+00000260: 7d2c 0d0a 2020 2020 7b74 6172 6765 7420  },..    {target 
+00000270: 3d20 226c 6967 6874 6e69 6e67 2e70 7974  = "lightning.pyt
+00000280: 6f72 6368 2e63 616c 6c62 6163 6b73 3a3a  orch.callbacks::
+00000290: 4465 7669 6365 5374 6174 734d 6f6e 6974  DeviceStatsMonit
+000002a0: 6f72 227d 0d0a 5d0d 0a0d 0a23 205b 7472  or"}..]....# [tr
+000002b0: 6169 6e69 6e67 2e63 6865 636b 706f 696e  aining.checkpoin
+000002c0: 745d 0d0a 2320 7061 7468 203d 2022 6368  t]..# path = "ch
+000002d0: 636b 7074 220d 0a23 206d 6f6e 6974 6f72  ckpt"..# monitor
+000002e0: 203d 207b 226d 6574 7269 6322 203d 2022   = {"metric" = "
+000002f0: 4d79 5072 6563 6973 696f 6e22 2c20 2273  MyPrecision", "s
+00000300: 7461 6765 2220 3d20 2276 616c 227d 0d0a  tage" = "val"}..
+00000310: 2320 6669 6c65 6e61 6d65 203d 2022 7b65  # filename = "{e
+00000320: 706f 6368 7d5f 7b76 616c 5f6d 7970 7265  poch}_{val_mypre
+00000330: 6369 7369 6f6e 3a2e 3266 7d5f 636e 6e22  cision:.2f}_cnn"
+00000340: 0d0a 2320 6d6f 6465 203d 2022 6d61 7822  ..# mode = "max"
+00000350: 0d0a 2320 7361 7665 5f74 6f70 5f6b 203d  ..# save_top_k =
+00000360: 2031 0d0a 0d0a 5b74 7261 696e 696e 672e   1....[training.
+00000370: 6f70 7469 6d69 7a65 725d 0d0a 7461 7267  optimizer]..targ
+00000380: 6574 203d 2022 746f 7263 682e 6f70 7469  et = "torch.opti
+00000390: 6d3a 3a41 6461 6d22 0d0a 6c72 203d 2030  m::Adam"..lr = 0
+000003a0: 2e30 3031 0d0a 7765 6967 6874 5f64 6563  .001..weight_dec
+000003b0: 6179 203d 2030 2e30 310d 0a0d 0a5b 7472  ay = 0.01....[tr
+000003c0: 6169 6e69 6e67 2e63 7269 7465 7269 6f6e  aining.criterion
+000003d0: 5d0d 0a74 6172 6765 7420 3d20 2274 6f72  ]..target = "tor
+000003e0: 6368 2e6e 6e3a 3a43 726f 7373 456e 7472  ch.nn::CrossEntr
+000003f0: 6f70 794c 6f73 7322 0d0a 7765 6967 6874  opyLoss"..weight
+00000400: 203d 205b 302e 312c 2030 2e31 2c20 302e   = [0.1, 0.1, 0.
+00000410: 312c 2030 2e31 2c20 302e 312c 2030 2e31  1, 0.1, 0.1, 0.1
+00000420: 2c20 302e 312c 2030 2e31 2c20 302e 312c  , 0.1, 0.1, 0.1,
+00000430: 2030 2e31 5d0d 0a0d 0a5b 7661 6c69 6461   0.1]....[valida
+00000440: 7469 6f6e 5d0d 0a72 756e 5f65 7665 7279  tion]..run_every
+00000450: 5f65 706f 6368 203d 2031 0d0a 0d0a 5b64  _epoch = 1....[d
+00000460: 6174 6173 6574 5d0d 0a74 6172 6765 7420  ataset]..target 
+00000470: 3d20 222e 2f64 6174 616d 6f64 756c 652e  = "./datamodule.
+00000480: 7079 3a3a 4d4e 4953 5443 7573 746f 6d44  py::MNISTCustomD
+00000490: 6174 616d 6f64 756c 6522 0d0a 0d0a 5b64  atamodule"....[d
+000004a0: 6174 6173 6574 2e74 7261 696e 7661 6c5d  ataset.trainval]
+000004b0: 0d0a 726f 6f74 5f64 6972 203d 2022 2e2f  ..root_dir = "./
+000004c0: 6d6e 6973 7422 0d0a 0d0a 5b64 6174 6173  mnist"....[datas
+000004d0: 6574 2e74 7261 696e 2e6c 6f61 6465 725d  et.train.loader]
+000004e0: 0d0a 6261 7463 685f 7369 7a65 203d 2031  ..batch_size = 1
+000004f0: 3530 0d0a 7368 7566 666c 6520 3d20 7472  50..shuffle = tr
+00000500: 7565 0d0a 6e75 6d5f 776f 726b 6572 7320  ue..num_workers 
+00000510: 3d20 340d 0a0d 0a5b 6461 7461 7365 742e  = 4....[dataset.
+00000520: 7661 6c69 6461 7469 6f6e 2e6c 6f61 6465  validation.loade
+00000530: 725d 0d0a 6261 7463 685f 7369 7a65 203d  r]..batch_size =
+00000540: 2031 3530 0d0a 7368 7566 666c 6520 3d20   150..shuffle = 
+00000550: 6661 6c73 650d 0a6e 756d 5f77 6f72 6b65  false..num_worke
+00000560: 7273 203d 2034 0d0a 0d0a 5b6d 6574 7269  rs = 4....[metri
+00000570: 6373 5d0d 0a4d 7950 7265 6369 7369 6f6e  cs]..MyPrecision
+00000580: 203d 207b 7461 7267 6574 203d 2022 746f   = {target = "to
+00000590: 7263 686d 6574 7269 6373 3a3a 5072 6563  rchmetrics::Prec
+000005a0: 6973 696f 6e22 2c20 7461 736b 203d 2022  ision", task = "
+000005b0: 6d75 6c74 6963 6c61 7373 222c 206e 756d  multiclass", num
+000005c0: 5f63 6c61 7373 6573 3d31 307d 0d0a 4642  _classes=10}..FB
+000005d0: 6574 6153 636f 7265 203d 207b 7461 7267  etaScore = {targ
+000005e0: 6574 203d 2022 746f 7263 686d 6574 7269  et = "torchmetri
+000005f0: 6373 3a3a 4642 6574 6153 636f 7265 222c  cs::FBetaScore",
+00000600: 2074 6173 6b20 3d20 226d 756c 7469 636c   task = "multicl
+00000610: 6173 7322 2c20 6e75 6d5f 636c 6173 7365  ass", num_classe
+00000620: 733d 3130 2c20 6265 7461 203d 2030 2e31  s=10, beta = 0.1
+00000630: 7d                                       }
```

### Comparing `kit4dl-2023.9b2/examples/cnn_s3dis_segmentation/conf.toml` & `kit4dl-2024.5b0/examples/cnn_s3dis_segmentation/conf.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/kit4dl/cli/_templates/project/conf.toml` & `kit4dl-2024.5b0/kit4dl/cli/_templates/project/conf.toml`

 * *Files 2% similar despite different names*

```diff
@@ -173,65 +173,65 @@
 00000ac0: 6e64 205b 6461 7461 7365 742e 7661 6c69  nd [dataset.vali
 00000ad0: 6461 7469 6f6e 5d0d 0a5b 6461 7461 7365  dation]..[datase
 00000ae0: 742e 7472 6169 6e5d 0d0a 2320 6865 7265  t.train]..# here
 00000af0: 2079 6f75 2063 616e 2064 6566 696e 6520   you can define 
 00000b00: 6172 6775 6d65 6e74 7320 7461 6b65 6e20  arguments taken 
 00000b10: 6279 2074 6865 206d 6574 686f 6420 6070  by the method `p
 00000b20: 7265 7061 7265 5f74 7261 696e 6461 7461  repare_traindata
-00000b30: 7365 7460 0d0a 726f 6f74 5f64 6972 203d  set`..root_dir =
-00000b40: 2022 6d79 5f74 7261 696e 5f66 696c 652e   "my_train_file.
-00000b50: 7478 7422 0d0a 0d0a 5b64 6174 6173 6574  txt"....[dataset
-00000b60: 2e76 616c 6964 6174 696f 6e5d 0d0a 2320  .validation]..# 
-00000b70: 6865 7265 2079 6f75 2063 616e 2064 6566  here you can def
-00000b80: 696e 6520 6172 6775 6d65 6e74 7320 7461  ine arguments ta
-00000b90: 6b65 6e20 6279 2074 6865 206d 6574 686f  ken by the metho
-00000ba0: 6420 6070 7265 7061 7265 5f76 616c 6461  d `prepare_valda
-00000bb0: 7461 7365 7460 0d0a 726f 6f74 5f64 6972  taset`..root_dir
-00000bc0: 203d 2022 6d79 5f76 616c 5f66 696c 652e   = "my_val_file.
-00000bd0: 7478 7422 0d0a 0d0a 5b64 6174 6173 6574  txt"....[dataset
-00000be0: 2e74 7261 696e 2e6c 6f61 6465 725d 0d0a  .train.loader]..
-00000bf0: 2320 6865 7265 2079 6f75 2064 6566 696e  # here you defin
-00000c00: 6520 6172 6775 6d65 6e74 7320 6f66 2064  e arguments of d
-00000c10: 6174 6120 6c6f 6164 6572 2066 6f72 2074  ata loader for t
-00000c20: 7261 696e 2064 6174 6173 6574 0d0a 6261  rain dataset..ba
-00000c30: 7463 685f 7369 7a65 203d 2031 300d 0a73  tch_size = 10..s
-00000c40: 6875 6666 6c65 203d 2074 7275 650d 0a6e  huffle = true..n
-00000c50: 756d 5f77 6f72 6b65 7273 203d 2034 0d0a  um_workers = 4..
-00000c60: 0d0a 5b64 6174 6173 6574 2e76 616c 6964  ..[dataset.valid
-00000c70: 6174 696f 6e2e 6c6f 6164 6572 5d0d 0a23  ation.loader]..#
-00000c80: 2068 6572 6520 796f 7520 6465 6669 6e65   here you define
-00000c90: 2061 7267 756d 656e 7473 206f 6620 6461   arguments of da
-00000ca0: 7461 206c 6f61 6465 7220 666f 7220 7661  ta loader for va
-00000cb0: 6c69 6461 7469 6f6e 2064 6174 6173 6574  lidation dataset
-00000cc0: 0d0a 6261 7463 685f 7369 7a65 203d 2031  ..batch_size = 1
-00000cd0: 300d 0a73 6875 6666 6c65 203d 2066 616c  0..shuffle = fal
-00000ce0: 7365 0d0a 6e75 6d5f 776f 726b 6572 7320  se..num_workers 
-00000cf0: 3d20 340d 0a0d 0a23 2077 6520 6361 6e20  = 4....# we can 
-00000d00: 6465 6669 6e65 2061 6c73 6f20 6172 6775  define also argu
-00000d10: 6d65 6e74 7320 666f 7220 7465 7374 2064  ments for test d
-00000d20: 6174 6120 6c6f 6164 6572 0d0a 2320 5b64  ata loader..# [d
-00000d30: 6174 6173 6574 2e74 6573 742e 6c6f 6164  ataset.test.load
-00000d40: 6572 5d0d 0a23 2062 6174 6368 5f73 697a  er]..# batch_siz
-00000d50: 6520 3d20 3130 0d0a 2320 7368 7566 666c  e = 10..# shuffl
-00000d60: 6520 3d20 6661 6c73 650d 0a23 206e 756d  e = false..# num
-00000d70: 5f77 6f72 6b65 7273 203d 2034 0d0a 0d0a  _workers = 4....
-00000d80: 5b6d 6574 7269 6373 5d0d 0a23 2068 6572  [metrics]..# her
-00000d90: 6520 796f 7520 6465 6669 6e65 206d 6574  e you define met
-00000da0: 7269 6373 2079 6f75 2077 616e 7420 746f  rics you want to
-00000db0: 206c 6f67 0d0a 2320 796f 7520 6361 6e20   log..# you can 
-00000dc0: 7573 6520 6375 7374 6f6d 206d 6574 7269  use custom metri
-00000dd0: 6373 2028 6e65 6564 2074 6f20 6265 2073  cs (need to be s
-00000de0: 7562 636c 6173 7365 7320 6f66 2074 6f72  ubclasses of tor
-00000df0: 6368 6d65 7472 6963 732e 4d65 7472 6963  chmetrics.Metric
-00000e00: 290d 0a4d 7953 636f 7265 203d 207b 7461  )..MyScore = {ta
-00000e10: 7267 6574 203d 2022 746f 7263 686d 6574  rget = "torchmet
-00000e20: 7269 6373 3a3a 5072 6563 6973 696f 6e22  rics::Precision"
-00000e30: 2c20 7461 736b 203d 2022 6d75 6c74 6963  , task = "multic
-00000e40: 6c61 7373 222c 206e 756d 5f63 6c61 7373  lass", num_class
-00000e50: 6573 203d 2031 307d 0d0a 4d79 5365 636f  es = 10}..MySeco
-00000e60: 6e64 5363 6f72 6520 3d20 7b74 6172 6765  ndScore = {targe
-00000e70: 7420 3d20 2274 6f72 6368 6d65 7472 6963  t = "torchmetric
-00000e80: 733a 3a46 4265 7461 5363 6f72 6522 2c20  s::FBetaScore", 
-00000e90: 7461 736b 203d 2022 6d75 6c74 6963 6c61  task = "multicla
-00000ea0: 7373 222c 206e 756d 5f63 6c61 7373 6573  ss", num_classes
-00000eb0: 203d 2031 302c 2062 6574 6120 3d20 302e   = 10, beta = 0.
-00000ec0: 317d                                     1}
+00000b30: 7365 7473 600d 0a72 6f6f 745f 6469 7220  sets`..root_dir 
+00000b40: 3d20 226d 795f 7472 6169 6e5f 6669 6c65  = "my_train_file
+00000b50: 2e74 7874 220d 0a0d 0a5b 6461 7461 7365  .txt"....[datase
+00000b60: 742e 7661 6c69 6461 7469 6f6e 5d0d 0a23  t.validation]..#
+00000b70: 2068 6572 6520 796f 7520 6361 6e20 6465   here you can de
+00000b80: 6669 6e65 2061 7267 756d 656e 7473 2074  fine arguments t
+00000b90: 616b 656e 2062 7920 7468 6520 6d65 7468  aken by the meth
+00000ba0: 6f64 2060 7072 6570 6172 655f 7661 6c64  od `prepare_vald
+00000bb0: 6174 6173 6574 7360 0d0a 726f 6f74 5f64  atasets`..root_d
+00000bc0: 6972 203d 2022 6d79 5f76 616c 5f66 696c  ir = "my_val_fil
+00000bd0: 652e 7478 7422 0d0a 0d0a 5b64 6174 6173  e.txt"....[datas
+00000be0: 6574 2e74 7261 696e 2e6c 6f61 6465 725d  et.train.loader]
+00000bf0: 0d0a 2320 6865 7265 2079 6f75 2064 6566  ..# here you def
+00000c00: 696e 6520 6172 6775 6d65 6e74 7320 6f66  ine arguments of
+00000c10: 2064 6174 6120 6c6f 6164 6572 2066 6f72   data loader for
+00000c20: 2074 7261 696e 2064 6174 6173 6574 0d0a   train dataset..
+00000c30: 6261 7463 685f 7369 7a65 203d 2031 300d  batch_size = 10.
+00000c40: 0a73 6875 6666 6c65 203d 2074 7275 650d  .shuffle = true.
+00000c50: 0a6e 756d 5f77 6f72 6b65 7273 203d 2034  .num_workers = 4
+00000c60: 0d0a 0d0a 5b64 6174 6173 6574 2e76 616c  ....[dataset.val
+00000c70: 6964 6174 696f 6e2e 6c6f 6164 6572 5d0d  idation.loader].
+00000c80: 0a23 2068 6572 6520 796f 7520 6465 6669  .# here you defi
+00000c90: 6e65 2061 7267 756d 656e 7473 206f 6620  ne arguments of 
+00000ca0: 6461 7461 206c 6f61 6465 7220 666f 7220  data loader for 
+00000cb0: 7661 6c69 6461 7469 6f6e 2064 6174 6173  validation datas
+00000cc0: 6574 0d0a 6261 7463 685f 7369 7a65 203d  et..batch_size =
+00000cd0: 2031 300d 0a73 6875 6666 6c65 203d 2066   10..shuffle = f
+00000ce0: 616c 7365 0d0a 6e75 6d5f 776f 726b 6572  alse..num_worker
+00000cf0: 7320 3d20 340d 0a0d 0a23 2077 6520 6361  s = 4....# we ca
+00000d00: 6e20 6465 6669 6e65 2061 6c73 6f20 6172  n define also ar
+00000d10: 6775 6d65 6e74 7320 666f 7220 7465 7374  guments for test
+00000d20: 2064 6174 6120 6c6f 6164 6572 0d0a 2320   data loader..# 
+00000d30: 5b64 6174 6173 6574 2e74 6573 742e 6c6f  [dataset.test.lo
+00000d40: 6164 6572 5d0d 0a23 2062 6174 6368 5f73  ader]..# batch_s
+00000d50: 697a 6520 3d20 3130 0d0a 2320 7368 7566  ize = 10..# shuf
+00000d60: 666c 6520 3d20 6661 6c73 650d 0a23 206e  fle = false..# n
+00000d70: 756d 5f77 6f72 6b65 7273 203d 2034 0d0a  um_workers = 4..
+00000d80: 0d0a 5b6d 6574 7269 6373 5d0d 0a23 2068  ..[metrics]..# h
+00000d90: 6572 6520 796f 7520 6465 6669 6e65 206d  ere you define m
+00000da0: 6574 7269 6373 2079 6f75 2077 616e 7420  etrics you want 
+00000db0: 746f 206c 6f67 0d0a 2320 796f 7520 6361  to log..# you ca
+00000dc0: 6e20 7573 6520 6375 7374 6f6d 206d 6574  n use custom met
+00000dd0: 7269 6373 2028 6e65 6564 2074 6f20 6265  rics (need to be
+00000de0: 2073 7562 636c 6173 7365 7320 6f66 2074   subclasses of t
+00000df0: 6f72 6368 6d65 7472 6963 732e 4d65 7472  orchmetrics.Metr
+00000e00: 6963 290d 0a4d 7953 636f 7265 203d 207b  ic)..MyScore = {
+00000e10: 7461 7267 6574 203d 2022 746f 7263 686d  target = "torchm
+00000e20: 6574 7269 6373 3a3a 5072 6563 6973 696f  etrics::Precisio
+00000e30: 6e22 2c20 7461 736b 203d 2022 6d75 6c74  n", task = "mult
+00000e40: 6963 6c61 7373 222c 206e 756d 5f63 6c61  iclass", num_cla
+00000e50: 7373 6573 203d 2031 307d 0d0a 4d79 5365  sses = 10}..MySe
+00000e60: 636f 6e64 5363 6f72 6520 3d20 7b74 6172  condScore = {tar
+00000e70: 6765 7420 3d20 2274 6f72 6368 6d65 7472  get = "torchmetr
+00000e80: 6963 733a 3a46 4265 7461 5363 6f72 6522  ics::FBetaScore"
+00000e90: 2c20 7461 736b 203d 2022 6d75 6c74 6963  , task = "multic
+00000ea0: 6c61 7373 222c 206e 756d 5f63 6c61 7373  lass", num_class
+00000eb0: 6573 203d 2031 302c 2062 6574 6120 3d20  es = 10, beta = 
+00000ec0: 302e 317d                                0.1}
```

### Comparing `kit4dl-2023.9b2/kit4dl/cli/_templates/project/datamodule.py` & `kit4dl-2024.5b0/kit4dl/cli/_templates/project/datamodule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Docstring of the module containing my data module."""
-from typing import Any
+
+from typing import Any, Generator
 
 from torch.utils.data import Dataset
 
-from kit4dl import Kit4DLAbstractDataModule
+from kit4dl.nn.dataset import Kit4DLAbstractDataModule
 
 
 class MyCustomDatamodule(Kit4DLAbstractDataModule):
     """My datamodule docstring."""
 
-    def prepare_traindataset(self, *args: Any, **kwargs: Any) -> Dataset:
+    def prepare_traindatasets(self, *args: Any, **kwargs: Any) -> Dataset:
         """Prepare train dataset."""
         raise NotImplementedError
 
-    def prepare_valdataset(self, *args: Any, **kwargs: Any) -> Dataset:
+    def prepare_valdatasets(self, *args: Any, **kwargs: Any) -> Dataset:
         """Prepare validation dataset."""
         raise NotImplementedError
 
-    def prepare_trainvaldataset(
+    def prepare_trainvaldatasets(
         self, *args: Any, **kwargs: Any
-    ) -> tuple[Dataset, Dataset]:
+    ) -> Generator[tuple[Dataset, Dataset], None, None]:
         """Prepare train and validation dataset."""
         # NOTE: If you have single logic for train/val split,
-        # implement this method and remove `prepare_traindataset`
-        # and `prepare_valdataset`
+        # implement this method and remove `prepare_traindatasets`
+        # and `prepare_valdatasets`
         raise NotImplementedError
 
     def prepare_testdataset(self, *args: Any, **kwargs: Any) -> Dataset:
         """Prepare test dataset."""
         raise NotImplementedError
 
     def prepare_predictdataset(self, *args: Any, **kwargs: Any) -> Dataset:
```

### Comparing `kit4dl-2023.9b2/kit4dl/cli/_templates/project/model.py` & `kit4dl-2024.5b0/kit4dl/cli/_templates/project/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Docstring of the module containing my neural network module."""
+
 from typing import Any
 
 import torch
 
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 
 class MyNewNetwork(Kit4DLAbstractModule):
     """My network module."""
 
     def configure(self, *args: Any, **kwargs: Any) -> None:
         """Configure the architecture."""
```

### Comparing `kit4dl-2023.9b2/kit4dl/cli/app.py` & `kit4dl-2024.5b0/kit4dl/cli/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,68 @@
 """Module with CLI for Kit4DL."""
+
 import importlib.resources
 import logging
 import os
 import shutil
-import sys
+from typing import Optional
 
-try:
-    import tomllib as toml
-except ModuleNotFoundError:
-    import toml  # type: ignore[no-redef]
 
 import typer
 from typing_extensions import Annotated
 
-from kit4dl import _version, context
-from kit4dl.formatting import escape_os_sep, substitute_symbols
-from kit4dl.nn.confmodels import Conf
+from kit4dl import (
+    _version,
+    setup_env_and_get_conf,
+    get_default_conf_path,
+    configure_logger,
+)
 from kit4dl.nn.trainer import Trainer
 
 # ##############################
 #         CREATE CLI
 # ##############################
 _app = typer.Typer(name="Kit4DL")
 
 # ##############################
 #       CONFIGURE LOGGER
 # ##############################
 _CLI_LOG_LEVEL = "INFO"
 _CLI_LOG_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
 
-
-def _configure_logger(logger: logging.Logger):
-    logger.setLevel(_CLI_LOG_LEVEL)
-    formatter = logging.Formatter(_CLI_LOG_FORMAT)
-    handler = logging.StreamHandler(sys.stdout)
-    logger.addHandler(handler)
-    for hdl in log.handlers:
-        hdl.setFormatter(formatter)
-        hdl.setLevel(_CLI_LOG_LEVEL)  # type: ignore[arg-type]
-
-
 log = logging.getLogger("Kit4DL.CLI")
-_configure_logger(log)
+configure_logger(log, _CLI_LOG_LEVEL, _CLI_LOG_FORMAT)
 
 
 # ##############################
 #         UTILS METHODS
 # ##############################
-def update_context_from_static() -> None:
-    """Update context from static attributes."""
-    context.VERSION = _version.__version__
-
-
-def update_context_from_runtime(
-    prj_dir: str | None = None,
-) -> None:
-    """Update context properties from the runtime variables."""
-    context.PROJECT_DIR = prj_dir
-
-
-def update_context_from_conf(conf: Conf | None = None) -> None:
-    """Update context from the configuration file."""
-    if not conf:
-        return
-    context.LOG_LEVEL = conf.logging.level
-    context.LOG_FORMAT = conf.logging.format_
-
-
-def _get_conf_from_file(conf_path: str, root_dir: str | None = None):
-    assert conf_path and conf_path.endswith(
-        ".toml"
-    ), "`conf_path` needs to be TOML file!"
-    text_load = substitute_symbols(conf_path, **context.get_dict())
-    text_load_escaped = escape_os_sep(text_load)
-    return Conf(root_dir=root_dir, **toml.loads(text_load_escaped))  # type: ignore[arg-type]
-
-
-def _get_default_conf_path() -> str:
-    return os.path.join(os.getcwd(), "conf.toml")
-
-
 def _remove_redundant_items(path):
     shutil.rmtree(os.path.join(path, "__pycache__"), ignore_errors=True)
 
 
+def parse_overwriting_options(
+    ctx: typer.Context, value: str | None
+) -> dict[str, str]:
+    """Parse extra arguments for the `overwrite` option."""
+    assert ctx
+    custom_dict: dict = {}
+    if not value:
+        return custom_dict
+    for kv_pair in value.split(","):
+        try:
+            key, value = kv_pair.split("=")
+        except ValueError as err:
+            raise typer.BadParameter(
+                f"Invalid key-value pair: {kv_pair}"
+            ) from err
+        custom_dict[key] = value
+    return custom_dict
+
+
 def _is_test_allowed(trainer: Trainer) -> bool:
     return trainer.is_finished
 
 
 # ##############################
 #      COMMANDS DEFINITIONS
 # ##############################
@@ -101,18 +76,19 @@
 
     Parameters
     ----------
     name : str, optional
         The optional name of the project.
         If skipped, the deafult `new_kit4dl_project` will be used
     """
+    _template_pkg = "kit4dl.cli._templates"
     log.info("Kit4DL Creating a new skeleton for the project: << %s >>", name)
     assert not os.path.exists(name), f"The project `{name}` already exists!"
-    with importlib.resources.path(
-        "kit4dl.cli._templates", "project"
+    with importlib.resources.as_file(
+        importlib.resources.files(_template_pkg).joinpath("project")
     ) as empty_proj_path:
         shutil.copytree(empty_proj_path, name)
     _remove_redundant_items(name)
 
 
 @_app.command()
 def resume(
@@ -127,51 +103,74 @@
     checkpoint : str
         Path to a checkpoint file
     """
     raise NotImplementedError
 
 
 @_app.command()
+def test(
+    conf: Annotated[
+        str, typer.Option(help="Path to the configuration TOML file")
+    ] = get_default_conf_path(),
+):
+    """Test using the configuration file.
+
+    Parameters
+    ----------
+    conf : str, optional
+        Path to the configuration TOML file.
+        If skipped, the program will search for the `conf.toml` file
+        in the current working directory.
+    """
+    conf_ = setup_env_and_get_conf(conf_path=conf)
+    log.info("Attempt to run testing...")
+    assert (
+        conf_.training.checkpoint_path
+    ), "`checkpoint_path` is not defined, i need to load model state."
+    trainer = Trainer(conf=conf_).prepare()
+    log.info("Running testing \U00002728")
+    trainer.test()
+    log.info("Testing finished \U00002728")
+
+
+@_app.command()
 def train(
     conf: Annotated[
         str, typer.Option(help="Path to the configuration TOML file")
-    ] = _get_default_conf_path(),
-    test: Annotated[
-        bool, typer.Option(help="If perform testing using best weights")
-    ] = True,
+    ] = get_default_conf_path(),
+    skiptest: Annotated[
+        bool,
+        typer.Option(help="If testing (using best weights) should be skipped"),
+    ] = False,
+    overwrite: Annotated[
+        Optional[str],
+        typer.Option(
+            ...,
+            callback=parse_overwriting_options,
+            help="Comma-separated key-value pairs (KEY=VALUE)",
+        ),
+    ] = None,
 ) -> None:
     """Train using the configuration file.
 
     Parameters
     ----------
     conf : str, optional
         Path to the configuration TOML file.
         If skipped, the program will search for the `conf.toml` file
         in the current working directory.
     test
     """
     log.info("Attempt to run training...")
-    root_dir = os.path.dirname(conf)
-    if not os.path.exists(conf):
-        raise RuntimeError(
-            f"the conf file: {conf} does not exist. ensure the default"
-            " configuration file exist or specify --conf argument to a valid"
-            " configuration file."
-        )
-    prj_dir = os.path.join(os.getcwd(), root_dir)
-    sys.path.append(prj_dir)
-    update_context_from_static()
-    update_context_from_runtime(prj_dir=prj_dir)
-    conf_ = _get_conf_from_file(conf, root_dir=root_dir)
-    update_context_from_conf(conf=conf_)
+    conf_ = setup_env_and_get_conf(conf_path=conf, overwrite=overwrite)  # type: ignore[arg-type]
     log.info("Running trainer \U0001f3ac")
     trainer = Trainer(conf=conf_).prepare()
     trainer.fit()
     log.info("Training finished \U00002728")
-    if test:
+    if not skiptest:
         if not _is_test_allowed(trainer):
             return
         log.info("Running testing \U00002728")
         trainer.test()
         log.info("Testing finished \U00002728")
```

### Comparing `kit4dl-2023.9b2/kit4dl/context.py` & `kit4dl-2024.5b0/kit4dl/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Module with session-related attributes."""
+
 import sys
 from typing import Any
 
 
 class _ImmutableAttribute:
     _value: Any = None
     _default: Any = None
+    _set: bool = False
 
     def __init__(self, default: Any) -> None:
         self._default = default
 
     def __get__(self, obj, objtype=None) -> Any:
         return self._value if self._value else self._default
 
     def __set__(self, obj, value: Any) -> None:
-        if self._value is not None:
+        if self._set:
             raise RuntimeError("Session properties can be set only once!")
         self._value = value
+        self._set = True
 
 
 # NOTE: below definitions will not be used, they are required
 # just for suntax suggestions and to avoid mypy [attr-defined] error
 PROJECT_DIR: Any
 LOG_LEVEL: Any
 LOG_FORMAT: Any
```

### Comparing `kit4dl-2023.9b2/kit4dl/dataset.py` & `kit4dl-2024.5b0/kit4dl/nn/dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 """A module with the Kit4DL abstract dataset definition."""
-import logging
+
+from __future__ import annotations
+
+import os
 from abc import ABC
-from typing import Any, Callable
+from types import GeneratorType
+from typing import Any, Callable, TYPE_CHECKING, Generator
 
 import lightning.pytorch as pl
 from torch.utils.data import DataLoader, Dataset
 
 from kit4dl import context
 from kit4dl.mixins import LoggerMixin
-from kit4dl.nn.confmodels import DatasetConf
+
+if TYPE_CHECKING:
+    from kit4dl.nn.confmodels import DatasetConf
 
 
 class Kit4DLAbstractDataModule(ABC, pl.LightningDataModule, LoggerMixin):
     """The class with the logic for dataset management.
 
     The class provides a user with a simple interface:
     `prepare_data` is a method for downloading and preprocessing datasets
-    `prepare_traindataset` is a method returning `torch.Dataset` for train
+    `prepare_traindatasets` is a method returning `torch.Dataset` for train
         data
-    `prepare_valdataset` is a method returning `torch.Dataset` for validation
+    `prepare_valdatasets` is a method returning `torch.Dataset` for validation
         data
-    `prepare_trainvaldataset` is a method returning a tuple of two
+    `prepare_trainvaldatasets` is a method returning a tuple of two
         `torch.Dataset`s for train and validation data
-        (if this method is provided, `prepare_traindataset` and
-        `prepare_valdataset` shouldn't be implemented)
+        (if this method is provided, `prepare_traindatasets` and
+        `prepare_valdatasets` shouldn't be implemented)
     `prepare_testdataset` is a method returning `torch.Dataset` for test data
     `prepare_predictdataset` is a method returning `torch.Dataset` for data
         for prediction
     """
 
     def __init__(self, conf: DatasetConf):
         super().__init__()
         self.conf = conf
+        self.trainval_dataset_generator: (
+            Generator[tuple[Dataset, Dataset], None, None] | None
+        ) = None
         self.train_dataset: Dataset | None = None
         self.val_dataset: Dataset | None = None
         self.test_dataset: Dataset | None = None
         self.predict_dataset: Dataset | None = None
+        self._split_suffix = os.environ.get(
+            "KIT4DL_SPLIT_PREFIX", "(split={:02d})"
+        )
         self._configure_logger()
         for extra_arg_key, extra_arg_value in self.conf.arguments.items():
             self.debug(
                 "setting extra user-defined argument: %s:%s",
                 extra_arg_key,
                 extra_arg_value,
             )
             setattr(self, extra_arg_key, extra_arg_value)
 
     def _configure_logger(self) -> None:
-        self._logger = logging.getLogger("kit4dl.dataset")
-        self._logger.setLevel(context.LOG_LEVEL)
-        if context.LOG_FORMAT:
-            formatter = logging.Formatter(context.LOG_FORMAT)
-            for handler in self._logger.handlers:
-                handler.setFormatter(formatter)
-        for handler in self._logger.handlers:
-            handler.setLevel(context.LOG_LEVEL)  # type: ignore[arg-type]
+        super().configure_logger(
+            name="kit4dl.Dataset",
+            level=context.LOG_LEVEL,
+            logformat=context.LOG_FORMAT,
+        )
 
     def prepare_data(self):
         """Prepare dataset for train/validation/test/predict splits.
 
         Examples
         --------
         ```python
@@ -77,22 +86,22 @@
         *args: Any
             List of positional arguments to setup the dataset
         **kwargs : Any
             List of named arguments required to setup the dataset
 
         Returns
         -------
-        train_datasets : Dataset
+        train_dataset : Dataset
             A training dataset
 
         Examples
         --------
         ```python
         ...
-        def prepare_traindataset(self, root_dir: str) -> Dataset:
+        def prepare_traindatasets(self, root_dir: str) -> Dataset:
             train_dset = MyDataset(root_dir=root_dir)
             return train_dset
         ```
         """
         raise NotImplementedError
 
     def prepare_valdataset(self, *args: Any, **kwargs: Any) -> Dataset:
@@ -103,50 +112,51 @@
         *args: Any
             List of positional arguments to setup the dataset
         **kwargs : Any
             List of named arguments required to setup the dataset
 
         Returns
         -------
-        val_datasets : Dataset
+        val_dataset : Dataset
             A validation dataset
 
         Examples
         --------
         ```python
         ...
-        def prepare_valdataset(self, root_dir: str) -> Dataset:
+        def prepare_valdatasets(self, root_dir: str) -> Dataset:
             val_dset = MyDataset(root_dir=root_dir)
             return val_dset
         ```
         """
         raise NotImplementedError
 
-    def prepare_trainvaldataset(
+    def prepare_trainvaldatasets(
         self, *args: Any, **kwargs: Any
-    ) -> tuple[Dataset, Dataset]:
+    ) -> Generator[tuple[Dataset, Dataset], None, None]:
         """Prepare dataset for training and validation.
 
         Parameters
         ----------
         *args: Any
             List of positional arguments to setup the dataset
         **kwargs : Any
             List of named arguments required to setup the dataset
 
         Returns
         -------
-        trainval_datasets : tuple of Dataset
-            Tuple consisting of train and validation dataset
+        trainval_dataset_generators : tuple of two Datasets and a string
+            Tuple consisting of train and validation dataset, and a suffix
+            for the split
 
         Examples
         --------
         ```python
         ...
-        def prepare_trainvaldataset(self, root_dir: str) -> tuple[Dataset, Dataset]:
+        def prepare_trainvaldatasets(self, root_dir: str) -> tuple[Dataset, Dataset]:
             dset = MyDataset(root_dir=root_dir)
             train_dset, val_dset = random_split(dset, [500, 50])
             return train_dset, val_dset
         ```
         """
         raise NotImplementedError
 
@@ -203,52 +213,78 @@
     def _handle_fit_stage(self) -> None:
         if self.conf.trainval:
             assert self.conf.trainval, (
                 "configuration for train-validation phases is not defined. did"
                 " you forget to define `[dataset.trainval]` section in the"
                 " configuration file?"
             )
-            self.train_dataset, self.val_dataset = (
-                self.prepare_trainvaldataset(**self.conf.trainval.arguments)
+            self.trainval_dataset_generator = self.prepare_trainvaldatasets(
+                **self.conf.trainval.arguments
             )
+            if not isinstance(self.trainval_dataset_generator, GeneratorType):
+                raise ValueError(
+                    "The method `prepare_trainvaldatasets` should "
+                    "be a generator (did you forget to use "
+                    "`yield` keyword)"
+                )
         else:
             assert self.conf.train, (
                 "configuration for train phase is not defined. did you forget"
                 " to define `[dataset.train]` section in the configuration"
                 " file?"
             )
             assert self.conf.validation, (
                 "configuration for validation phase is not defined. did you"
                 " forget to define `[dataset.validation]` section in the"
                 " configuration file?"
             )
             self.train_dataset = self.prepare_traindataset(
                 **self.conf.train.arguments
             )
+            if not isinstance(self.train_dataset, Dataset):
+                raise ValueError(
+                    "The method `prepare_traindataset` should return a pytorch"
+                    " Dataset. Did you forget to return a Dataset"
+                )
             self.val_dataset = self.prepare_valdataset(
                 **self.conf.validation.arguments
             )
+            if not isinstance(self.val_dataset, Dataset):
+                raise ValueError(
+                    "The method `prepare_valdataset` should return a pytorch"
+                    " Dataset. Did you forget to return a Dataset"
+                )
 
     def _handle_test_stage(self) -> None:
         assert self.conf.test, (
             "configuration for test phase is not defined. did you forget to"
             " define `[dataset.test]` section in the configuration file?"
         )
         self.test_dataset = self.prepare_testdataset(
             **self.conf.test.arguments
         )
+        if not isinstance(self.test_dataset, Dataset):
+            raise ValueError(
+                "The method `prepare_testdataset` should "
+                "return a pytorch Dataset. Did you forget to return a Dataset"
+            )
 
     def _handle_predict_stage(self) -> None:
         assert self.conf.predict, (
             "`test_config` is not defined. did you forget to define"
             " `[dataset.predict]` section in the configuration file?"
         )
         self.predict_dataset = self.prepare_predictdataset(
             **self.conf.predict.arguments
         )
+        if not isinstance(self.predict_dataset, Dataset):
+            raise ValueError(
+                "The method `predict_dataset` should "
+                "return a pytorch Dataset. Did you forget to return a Dataset"
+            )
 
     def setup(self, stage: str) -> None:
         """Set up data depending on the stage.
 
         The method should not be overriden unless necessary.
 
         Parameters
@@ -280,71 +316,113 @@
         """Get test specific collate function."""
         return self.get_collate_fn()
 
     def get_predict_collate_fn(self) -> Callable | None:
         """Get predict specific collate function."""
         return self.get_collate_fn()
 
-    def train_dataloader(self) -> DataLoader:
+    def trainval_dataloaders(
+        self,
+    ) -> Generator[tuple[DataLoader, DataLoader, str], None, None]:
+        """Prepare loader for train and validation data."""
+        if self.conf.trainval:
+            assert self.trainval_dataset_generator is not None, (
+                "did you forget to return `torch.utils.data.Dataset`instance"
+                " from the `prepare_trainvaldatasets` method?"
+            )
+            assert self.conf.train is not None, (
+                "[dataset.train.loader] section is is missing in the"
+                " configuration file."
+            )
+            assert self.conf.validation is not None, (
+                "[dataset.validation.loader] section is is missing in the"
+                " configuration file."
+            )
+            assert (
+                self.conf.train.loader is not None
+                and self.conf.validation.loader is not None
+            ), (
+                "did you forget to define [dataset.train.loader] and"
+                "[dataset.validation.loader] sections in the configuration "
+                "file?"
+            )
+            for i, (tr_dataset, val_dataset) in enumerate(
+                self.trainval_dataset_generator
+            ):
+                yield DataLoader(
+                    tr_dataset,
+                    **self.conf.train.loader,
+                    collate_fn=self.get_train_collate_fn(),
+                ), DataLoader(
+                    val_dataset,
+                    **self.conf.validation.loader,
+                    collate_fn=self.get_val_collate_fn(),
+                ), self._split_suffix.format(
+                    i + 1
+                )
+        elif self.conf.train and self.conf.validation:
+            yield self._train_dataloader(), self._val_dataloader(), ""
+
+    def _train_dataloader(self) -> DataLoader:
         """Prepare loader for train data."""
         assert self.conf.train, (
             "train configuration is not defined. did you forget"
             " [dataset.train] section in the configuration file?"
         )
         assert self.train_dataset is not None, (
-            "did you forget to return `torch.utils.data.Dataset`instance from"
-            " the `prepare_traindataset` method?"
+            "did you forget to return `torch.utils.data.Dataset` instance"
+            " from the `prepare_traindataset` method?"
         )
         return DataLoader(
             self.train_dataset,
             **self.conf.train.loader,
             collate_fn=self.get_train_collate_fn(),
         )
 
-    def val_dataloader(self) -> DataLoader:
+    def _val_dataloader(self) -> DataLoader:
         """Prepare loader for validation data."""
         assert self.conf.validation, (
             "validation configuration is not defined. did you forget"
             " [dataset.validation] section in the configuration file?"
         )
         assert self.val_dataset is not None, (
-            "did you forget to return `torch.utils.data.Dataset`instance from"
-            " the `prepare_valdataset` method?"
+            "did you forget to return `torch.utils.data.Dataset` instance"
+            " from the `prepare_valdataset` method?"
         )
         return DataLoader(
             self.val_dataset,
             **self.conf.validation.loader,
             collate_fn=self.get_val_collate_fn(),
         )
 
     def test_dataloader(self) -> DataLoader:
         """Prepare loader for test data."""
         assert self.conf.test, (
             "test configuration is not defined. did you forget"
             " [dataset.test] section in the configuration file?"
         )
         assert self.test_dataset is not None, (
-            "did you forget to return `torch.utils.data.Dataset`instance from"
-            " the `prepare_testdataset` method?"
+            "did you forget to return `torch.utils.data.Dataset` instance"
+            " from the `prepare_testdataset` method?"
         )
         return DataLoader(
             self.test_dataset,
             **self.conf.test.loader,
             collate_fn=self.get_test_collate_fn(),
         )
 
     def predict_dataloader(self) -> DataLoader:
         """Prepare loader for prediction data."""
         assert self.conf.predict, (
             "validation configuration is not defined. did you forget"
             " [dataset.predict] section in the configuration file?"
         )
         assert self.predict_dataset is not None, (
-            "did you forget to return `torch.utils.data.Dataset`instance from"
-            " the `prepare_predictdataset` method?"
+            "did you forget to return `torch.utils.data.Dataset` instance"
+            " from the `prepare_predictdataset` method?"
         )
         return DataLoader(
             self.predict_dataset,
             **self.conf.predict.loader,
             collate_fn=self.get_predict_collate_fn(),
         )
```

### Comparing `kit4dl-2023.9b2/kit4dl/formatting.py` & `kit4dl-2024.5b0/kit4dl/formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration formatting utils."""
+
 import os
 
 from jinja2 import (
     Environment,
     FileSystemLoader,
     StrictUndefined,
     UndefinedError,
```

### Comparing `kit4dl-2023.9b2/kit4dl/io.py` & `kit4dl-2024.5b0/kit4dl/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """A module with input-output operations."""
+
 import importlib
 import os
 import sys
 from typing import Any
 
 from kit4dl.kit4dl_types import FullyQualifiedName
 
 _TARGET_SPLIT = "::"
 _MODULE_SEP = ".py::"
 PROJECT_DIR = "PROJECT_DIR"
 
 
+def assert_valid_class(class_, classinfo):
+    """Assert a `class_` is a subclass of `classinfo`."""
+    assert issubclass(class_, classinfo), (
+        f"the passed class: {class_} is expected to be a subclass of"
+        f" {classinfo} but it's not"
+    )
+
+
 def _does_path_contain_module_file(target: str | FullyQualifiedName):
     return target.strip().endswith(".py") or _MODULE_SEP in target
 
 
 def split_target(target: str | FullyQualifiedName) -> tuple[str, str]:
     """Split target name or fully qualified name by `::` to get the path and the attribute.
```

### Comparing `kit4dl-2023.9b2/kit4dl/metric.py` & `kit4dl-2024.5b0/kit4dl/metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """A module with metric logic."""
+
 import numpy as np
 import torchmetrics as tm
 
 
 class MetricStore:
     """Class being a store for different metrics.
 
     It manages resetting,updating, and computing the metrics result.
     """
 
     __slots__ = ("_metrics",)
 
     def __init__(self, metrics: dict[str, tm.Metric]) -> None:
-        self._metrics = metrics
+        self._metrics = {
+            key: metric.clone() for key, metric in metrics.items()
+        }
 
     def reset(self) -> "MetricStore":
         """Reset metrics to the init state."""
         for met in self._metrics.values():
             met.reset()
         return self
```

### Comparing `kit4dl-2023.9b2/kit4dl/nn/confmodels.py` & `kit4dl-2024.5b0/kit4dl/nn/confmodels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """A module with configuration classes."""
+
+__all__ = ("Conf",)
 import os
 import warnings
 from functools import partial as func_partial
 from inspect import signature
+from types import FunctionType
 from typing import Any, Callable, Literal
 
 import lightning.pytorch.loggers as pl_logs
 import torch
 import torchmetrics as tm
 from pydantic import (
     AfterValidator,
@@ -18,15 +21,16 @@
 )
 from pydantic.fields import FieldInfo
 from typing_extensions import Annotated
 
 import kit4dl.io as io_
 from kit4dl import Kit4DLCallback
 from kit4dl import utils as ut
-from kit4dl.kit4dl_types import FullyQualifiedName
+from kit4dl.mixins import ObfuscateKeyMixing
+from kit4dl.kit4dl_types import FullyQualifiedName, LoggerLevel
 from kit4dl.nn.validators import (
     validate_callback,
     validate_class_exists,
     validate_cuda_device_exists,
     validate_lr_scheduler,
     validate_metric,
 )
@@ -78,32 +82,40 @@
         )
     return class_(**obj_conf_copy)
 
 
 # ################################
 #           ABSTRACT
 # ################################
-class _AbstractClassWithArgumentsConf(BaseModel):
-    model_config = ConfigDict(extra="allow", frozen=True)
+class _AbstractKit4dlConf(
+    BaseModel, ObfuscateKeyMixing, validate_assignment=True
+):
+    pass
+
+
+class _AbstractClassWithArgumentsConf(_AbstractKit4dlConf):
+    model_config = ConfigDict(extra="allow", frozen=False)
     target: Target
     arguments: dict[str, Any] = Field(default_factory=dict)
 
     @model_validator(mode="before")
     def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
+        if "arguments" in values:
+            return values
         field_args, extra_args = split_extra_arguments(
             values, cls.model_fields, consider_alias=False
         )
         field_args["arguments"] = extra_args
         return field_args
 
 
 # ################################
 #  Basic experiment configuration
 # ################################
-class BaseConf(BaseModel):
+class BaseConf(_AbstractKit4dlConf):
     """Base configuration model for the experiment."""
 
     seed: int = Field(default=0, ge=0)
     cuda_id: CudaDevice = None
     experiment_name: str
 
     @property
@@ -127,27 +139,14 @@
 
 # ################################
 #  Neural network model configuration
 # ################################
 class ModelConf(_AbstractClassWithArgumentsConf):
     """Model configuration class."""
 
-    @field_validator("target")
-    def _check_if_target_has_expected_parent_class(cls, value):
-        from kit4dl.nn.base import (  # pylint: disable=import-outside-toplevel
-            Kit4DLAbstractModule,
-        )
-
-        target_class = io_.import_and_get_attr_from_fully_qualified_name(value)
-        assert issubclass(target_class, Kit4DLAbstractModule), (
-            f"target class must be a subclass of `{Kit4DLAbstractModule}`"
-            " class!"
-        )
-        return value
-
     @property
     def model_class(self) -> type:
         """Get Python class of the model defined in the configuration."""
         target_class = io_.import_and_get_attr_from_fully_qualified_name(
             self.target
         )
         return target_class
@@ -182,15 +181,15 @@
             **self.arguments,  # pylint: disable=not-a-mapping
         )
 
 
 # ################################
 #       Checkpoint configuration
 # ################################
-class CheckpointConf(BaseModel):
+class CheckpointConf(_AbstractKit4dlConf):
     """Checkpoint configuration class."""
 
     path: str
     monitor: dict[str, str]
     filename: str
     mode: Literal["min", "max"] = "max"
     save_top_k: int = Field(1, ge=1)
@@ -222,68 +221,85 @@
             [self.monitor["stage"].lower(), self.monitor["metric"].lower()]
         )
 
 
 # ################################
 #     Criterion configuration
 # ################################
-class CriterionConf(BaseModel):
+class CriterionConf(_AbstractKit4dlConf):
     """Criterion configuration class."""
 
     target: Target
-    weight: list[float] | None = None
+    arguments: dict[str, Any] = Field(default_factory=dict)
+
+    @model_validator(mode="before")
+    def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
+        field_args, extra_args = split_extra_arguments(
+            values, cls.model_fields, consider_alias=False
+        )
+        field_args["arguments"] = extra_args
+        return field_args
 
     @field_validator("target")
     def _check_if_target_has_expected_parent_class(cls, value):
-        target_class = io_.import_and_get_attr_from_fully_qualified_name(value)
-        assert issubclass(target_class, torch.nn.Module), (
-            "target class of the criterion must be a subclass of"
-            f" `{torch.nn.Module}` class!"
+        target = io_.import_and_get_attr_from_fully_qualified_name(value)
+        assert isinstance(target, FunctionType) or issubclass(
+            target, torch.nn.Module
+        ), (
+            "target class of the criterion must be a function or a subclass of"
+            " torch.nn.Module class!"
         )
         return value
 
     @model_validator(mode="after")
-    def _match_weight(cls, values):
-        if values.weight:
-            criterion_class = (
-                io_.import_and_get_attr_from_fully_qualified_name(
-                    values.target
-                )
-            )
-            assert "weight" in signature(criterion_class).parameters, (
-                "`weight` parameter is not defined for the criterion"
-                f" `{criterion_class}`"
+    def _match_arguments(cls, values):
+        criterion = io_.import_and_get_attr_from_fully_qualified_name(
+            values.target
+        )
+        for param_name in values.arguments.keys():
+            assert param_name in signature(criterion).parameters, (
+                f"`{param_name}` parameter is not defined for the criterion"
+                f" `{criterion}`"
             )
         return values
 
     @property
-    def criterion(self) -> torch.nn.Module:
+    def criterion(self) -> torch.nn.Module | Callable:
         """Get the torch.nn.Module with the criterion function."""
-        target_class = io_.import_and_get_attr_from_fully_qualified_name(
-            self.target
-        )
-        if self.weight is not None:
-            weight_tensor = torch.FloatTensor(self.weight)
-            return target_class(weight=weight_tensor)
-        return target_class()
+        target = io_.import_and_get_attr_from_fully_qualified_name(self.target)
+        if isinstance(target, FunctionType):
+            return func_partial(
+                target,
+                **self.arguments,  # pylint: disable=not-a-mapping
+            )
+        if issubclass(target, torch.nn.Module):
+            if weight := self.arguments.pop("weight", None):
+                weight_tensor = torch.FloatTensor(weight)
+                return target(
+                    weight=weight_tensor,
+                    **self.arguments,  # pylint: disable=not-a-mapping
+                )
+            return target()
+        raise TypeError
 
 
 # ################################
 #     Training configuration
 # ################################
-class TrainingConf(BaseModel):
+class TrainingConf(_AbstractKit4dlConf):
     """Training procedure configuration class."""
 
     epochs: int = Field(gt=0)
     epoch_schedulers: list[SchedulerDict] = Field(default_factory=list)
     checkpoint: CheckpointConf | None = None
     callbacks: list[CallbackDict] = Field(default_factory=list)
     optimizer: OptimizerConf
-    criterion: CriterionConf
+    criterion: CriterionConf | None = None
     arguments: dict[str, Any]
+    checkpoint_path: str | None = None
 
     @model_validator(mode="before")
     def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
         field_args, extra_args = split_extra_arguments(
             values, cls.model_fields, consider_alias=False
         )
         field_args["arguments"] = extra_args
@@ -308,24 +324,24 @@
             schedulers.append(create_obj_from_conf(sch, partial=True))
         return schedulers
 
 
 # ################################
 #     Validation configuration
 # ################################
-class ValidationConf(BaseModel):
+class ValidationConf(_AbstractKit4dlConf):
     """Validation procedure configuration class."""
 
     run_every_epoch: int = Field(gt=0)
 
 
 # ################################
 #     Split dataset configuration
 # ################################
-class SplitDatasetConf(BaseModel):
+class SplitDatasetConf(_AbstractKit4dlConf):
     """Configuration class with dataset split arguments."""
 
     loader: dict[str, Any] = Field(default_factory=dict)
     arguments: dict[str, Any]
 
     @model_validator(mode="before")
     def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
@@ -335,15 +351,15 @@
         field_args["arguments"] = extra_args
         return field_args
 
 
 # ################################
 #     Dataset configuration
 # ################################
-class DatasetConf(BaseModel):
+class DatasetConf(_AbstractKit4dlConf):
     """Dataset configuration class."""
 
     target: Target
     train: SplitDatasetConf | None = None
     validation: SplitDatasetConf | None = None
     trainval: SplitDatasetConf | None = None
     test: SplitDatasetConf | None = None
@@ -354,27 +370,14 @@
     def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
         field_args, extra_args = split_extra_arguments(
             values, cls.model_fields, consider_alias=False
         )
         field_args["arguments"] = extra_args
         return field_args
 
-    @field_validator("target")
-    def _check_if_target_has_expected_parent_class(cls, value: str):
-        from kit4dl.dataset import (  # pylint: disable=import-outside-toplevel
-            Kit4DLAbstractDataModule,
-        )
-
-        target_class = io_.import_and_get_attr_from_fully_qualified_name(value)
-        assert issubclass(target_class, Kit4DLAbstractDataModule), (
-            "target class of the dataset module must be a subclass of"
-            f" `{Kit4DLAbstractDataModule}` class!"
-        )
-        return value
-
     @property
     def datamodule_class(self) -> type:
         """Get Python class of the data module."""
         target_class = io_.import_and_get_attr_from_fully_qualified_name(
             self.target
         )
         return target_class
@@ -389,24 +392,22 @@
     "mlflow": "MLFlowLogger",
     "neptune": "NeptuneLogger",
     "tensorboard": "TensorBoardLogger",
     "wandb": "WandbLogger",
 }
 
 
-class LoggingConf(BaseModel):
+class LoggingConf(_AbstractKit4dlConf):
     """Logging configuration class."""
 
     model_config = ConfigDict(extra="allow", populate_by_name=True)
     type_: Literal[
         "comet", "csv", "mlflow", "neptune", "tensorboard", "wandb"
     ] = Field("csv", alias="type")
-    level: Literal["DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"] | None = (
-        "INFO"
-    )
+    level: LoggerLevel | None = "INFO"
     format_: str | None = Field("%(asctime)s - %(message)s", alias="format")
     arguments: dict[str, Any] = Field(default_factory=dict)
 
     @model_validator(mode="before")
     def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
         field_args, extra_args = split_extra_arguments(
             values, cls.model_fields, consider_alias=True
@@ -418,25 +419,25 @@
     def _match_log_level(cls, item):
         return item.upper()
 
     def maybe_update_experiment_name(self, experiment_name: str) -> None:
         """Update experiment name for the chosen metric logger."""
         ltype = self.metric_logger_type
         if issubclass(ltype, (pl_logs.CometLogger, pl_logs.MLFlowLogger)):
-            self.arguments.setdefault("experiment_name", experiment_name)
+            self.arguments.update({"experiment_name": experiment_name})
         elif issubclass(
             ltype,
             (
                 pl_logs.CSVLogger,
                 pl_logs.NeptuneLogger,
                 pl_logs.TensorBoardLogger,
                 pl_logs.WandbLogger,
             ),
         ):
-            self.arguments.setdefault("name", experiment_name)
+            self.arguments.update({"name": experiment_name})
         else:
             raise TypeError(
                 f"logger of type `{self.metric_logger_type}` is undefined!"
             )
         if issubclass(ltype, pl_logs.CSVLogger):
             self.arguments.setdefault("save_dir", "./csv_logs")
 
@@ -445,15 +446,15 @@
         """Get type of the selected logger."""
         return getattr(pl_logs, _LOGGERS_NICKNAMES[self.type_])
 
 
 # ################################
 #     Complete configuration
 # ################################
-class Conf(BaseModel):
+class Conf(_AbstractKit4dlConf):
     """Conf class being the reflection of the configuration TOML file."""
 
     base: BaseConf
     logging: LoggingConf = Field(default_factory=LoggingConf)  # type: ignore[arg-type]
     model: ModelConf
     metrics: dict[str, MetricDict] = Field(default_factory=dict)
     training: TrainingConf
@@ -461,14 +462,19 @@
     dataset: DatasetConf
 
     def __init__(self, root_dir: str | None = None, **kwargs):
         if root_dir:
             kwargs = Conf.override_with_abs_target(root_dir, kwargs)
         super().__init__(**kwargs)
 
+    @property
+    def experiment_name(self) -> str:
+        """Get the experiment name."""
+        return self.base.experiment_name
+
     @model_validator(mode="after")
     def _update_experiment_name_if_undefined(cls, value):
         if not value.base:
             return value
         if value.logging:
             value.logging.maybe_update_experiment_name(
                 value.base.experiment_name
@@ -476,14 +482,16 @@
         return value
 
     @model_validator(mode="after")
     def _check_metric_in_checkpoint_is_defined(cls, value):
         if not value.training.checkpoint:
             return value
         monitored_metric_name = value.training.checkpoint.monitor["metric"]
+        if monitored_metric_name == "loss":
+            return value
         assert monitored_metric_name in value.metrics.keys(), (
             f"metric `{monitored_metric_name}` is not defined. did you forget"
             f" to define `{monitored_metric_name}` in [metrics]?"
         )
         return value
 
     @property
```

### Comparing `kit4dl-2023.9b2/kit4dl/nn/trainer.py` & `kit4dl-2024.5b0/kit4dl/nn/trainer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,214 @@
 """A module with neural network train task definition."""
-import logging
-from typing import Any
 
+import os
+
+import torch
 import lightning.pytorch as pl
 from lightning.pytorch import callbacks as pl_callbacks
 from lightning.pytorch import loggers as pl_log
 
-from kit4dl.dataset import Kit4DLAbstractDataModule
+from kit4dl.nn.dataset import Kit4DLAbstractDataModule
 from kit4dl.mixins import LoggerMixin
-from kit4dl.nn.base import Kit4DLAbstractModule
-from kit4dl.nn.callbacks import MetricCallback, ModelCheckpoint
+from kit4dl.nn.base import Kit4DLModuleWrapper
+from kit4dl.nn.callbacks import MetricCallback
 from kit4dl.nn.confmodels import Conf
 from kit4dl.utils import set_seed
+from kit4dl import io as io_
 
 
 class Trainer(LoggerMixin):
     """Class managing the training procedure."""
 
-    _model: Kit4DLAbstractModule
-    _datamodule: Kit4DLAbstractDataModule
-    _pl_trainer: pl.Trainer
     _conf: Conf
-    _metric_logger: Any
+    _device: torch.device
+    _metric_logger: pl_log.Logger
+    model_wrap: Kit4DLModuleWrapper
+    _datamodule: Kit4DLAbstractDataModule
+    pl_trainer: pl.Trainer
 
     def __init__(self, conf: Conf) -> None:
-        self._logger = logging.getLogger("lightning.pytorch")
         self._conf = conf
+        self._configure_logger()
         self._device = self._conf.base.device
         self._metric_logger = self._new_metric_logger()
         set_seed(self._conf.base.seed)
 
+    def prepapre_new(self, *, experiment_name: str | None = None) -> "Trainer":
+        """Copy and prepare the trainer.
+
+        Parameters
+        ----------
+        experiment_name : str, optional
+            Name of the experiment to be used in the new trainer. If not
+            provided, the name is copied from the current trainer.
+        """
+        _conf = self._conf
+        if experiment_name:
+            _conf = self._conf.copy()
+            _conf.base.experiment_name = experiment_name
+            _conf.logging.maybe_update_experiment_name(experiment_name)
+        return type(self)(_conf).prepare()
+
+    def _configure_logger(self) -> None:
+        super().configure_logger(
+            name="lightning.pytorch",
+            level=self._conf.logging.level,
+            logformat=self._conf.logging.format_,
+        )
+
     @property
     def is_finished(self) -> bool:
         """Check if training routing finished."""
-        return self._pl_trainer.state.finished
+        return self.pl_trainer.state.finished
 
     def prepare(self) -> "Trainer":
         """Prepare trainer by configuring the model and data modules."""
-        self._model = self._configure_model()
-        self._pl_trainer = self._configure_trainer()
+        self.model_wrap = self._wrap_model()
+        self.pl_trainer = self._configure_trainer()
         self._datamodule = self._configure_datamodule()
         self._log_hparams()
         return self
 
     def _log_hparams(self) -> None:
-        self._metric_logger.log_hyperparams(self._conf.dict())
+        self._metric_logger.log_hyperparams(self._conf.obfuscated_dict())
         self._metric_logger.log_hyperparams(
             {
                 "trainable_parameters": sum(
                     p.numel()
-                    for p in self._model.parameters()
+                    for p in self.model_wrap.model.parameters()
                     if p.requires_grad
                 )
             }
         )
 
-    def load_checkpoint(self, path: str) -> "Trainer":
-        """Load model weights from the checkpoint."""
-        self._model = type(self._model).load_from_checkpoint(path)
-        return self
-
     def fit(self) -> "Trainer":
         """Fit the trainer making use of `lightning.pytorch.Trainer`."""
-        assert self._pl_trainer, (
+        assert self.pl_trainer, (
             "trainer is not configured. did you forget to call `prepare()`"
             " method first?"
         )
-        self._pl_trainer.fit(self._model, datamodule=self._datamodule)
+        self._datamodule.setup("fit")
+        new_trainer = self
+        i = 0
+        for i, (tr_dataloader, val_dataloader, suff) in enumerate(
+            self._datamodule.trainval_dataloaders()
+        ):
+            self._logger.info("Starting training for split %d...", i + 1)
+            new_trainer.pl_trainer.fit(
+                new_trainer.model_wrap.model,
+                train_dataloaders=tr_dataloader,
+                val_dataloaders=val_dataloader,
+            )
+            new_trainer = new_trainer.prepapre_new(
+                experiment_name=self._conf.experiment_name + suff
+            )
+        self._logger.info("Training finished! %d splits processed", i + 1)
         return self
 
     def test(self) -> "Trainer":
         """Test the model."""
-        assert self._pl_trainer, (
+        assert self.pl_trainer, (
             "trainer is not configured. did you forget to call `prepare()`"
             " method first?"
         )
-        self._pl_trainer.test(
-            self._model, datamodule=self._datamodule, ckpt_path="best"
-        )
+        ckpt_path = None
+        for callback in self.pl_trainer.checkpoint_callbacks:
+            if isinstance(callback, pl_callbacks.ModelCheckpoint):
+                self.debug(
+                    "best checkpoint taken from callback %s",
+                    callback.best_model_path,
+                )
+                ckpt_path = callback.best_model_path
+                break
+        if self._conf.training.checkpoint_path:
+            assert os.path.exists(self._conf.training.checkpoint_path), (
+                "the defined checkpoint:"
+                f" {self._conf.training.checkpoint_path} does not exist!"
+            )
+            self.info(
+                "user-defined checkpoint %s will be used for testing",
+                self._conf.training.checkpoint_path,
+            )
+            ckpt_path = self._conf.training.checkpoint_path
+        if ckpt_path:
+            model = self.model_wrap.load_checkpoint(ckpt_path)
+        self._datamodule.setup("test")
+        for i, test_dataloader in enumerate(
+            self._datamodule.test_dataloader()
+        ):
+            self._logger.info("Starting testing for split %d...", i + 1)
+            self.pl_trainer.test(model, dataloaders=test_dataloader)
         return self
 
     def predict(self) -> "Trainer":
         """Predict values for the model."""
-        assert self._pl_trainer, (
+        assert self.pl_trainer, (
             "trainer is not configured. did you forget to call `prepare()`"
             " method first?"
         )
-        self._pl_trainer.predict(self._model, datamodule=self._datamodule)
+        self._datamodule.setup("predict")
+        for i, pred_dataloader in enumerate(
+            self._datamodule.predict_dataloader()
+        ):
+            self._logger.info("Starting prediction for split %d...", i + 1)
+            self.pl_trainer.predict(
+                self.model_wrap.model, dataloaders=pred_dataloader
+            )
         return self
 
     def _new_metric_logger(self) -> pl_log.Logger:
         return self._conf.logging.metric_logger_type(
             **self._conf.logging.arguments
         )
 
     def _configure_datamodule(self) -> Kit4DLAbstractDataModule:
+        class_ = self._conf.dataset.datamodule_class
+        io_.assert_valid_class(class_, Kit4DLAbstractDataModule)
         return self._conf.dataset.datamodule_class(conf=self._conf.dataset)
 
-    def _configure_model(self) -> Kit4DLAbstractModule:
-        return self._conf.model.model_class(conf=self._conf).to(self._device)
+    def _wrap_model(self) -> Kit4DLModuleWrapper:
+        return Kit4DLModuleWrapper(conf=self._conf, device=self._device)
 
-    def _get_model_checkpoint(self) -> ModelCheckpoint:
+    def _get_model_checkpoint(self) -> pl_callbacks.ModelCheckpoint:
         assert self._conf.training.checkpoint, (
             "getting model checkpoint callback, but `checkpoint` was not"
             " defined in the configuration file"
         )
         chkp_conf = self._conf.training.checkpoint
         assert (not chkp_conf.every_n_epochs) or isinstance(
             chkp_conf.every_n_epochs, int
         ), (
             "wrong type of `every_n_epochs`. expected: `int`, provided:"
             f" {type(chkp_conf.every_n_epochs)}"
         )
-        return ModelCheckpoint(
+        return pl_callbacks.ModelCheckpoint(
             dirpath=chkp_conf.path,
             filename=chkp_conf.filename,
             monitor=chkp_conf.monitor_metric_name,
             save_top_k=chkp_conf.save_top_k,
             mode=chkp_conf.mode,
             save_weights_only=chkp_conf.save_weights_only,
             every_n_epochs=chkp_conf.every_n_epochs,
             save_on_train_epoch_end=chkp_conf.save_on_train_epoch_end,
         )
 
+    def _set_default_trainer_args(self):
+        self._conf.training.arguments.setdefault("deterministic", True)
+        self._conf.training.arguments.setdefault("enable_progress_bar", True)
+
     def _configure_trainer(self) -> pl.Trainer:
         accelerator_device, device = self._conf.base.accelerator_device_and_id
         callbacks: list[pl_callbacks.Callback] = [
-            MetricCallback()
+            MetricCallback(conf=self._conf.metrics_obj)
         ] + self._conf.training.preconfigured_callbacks
         if self._conf.training.checkpoint:
             callbacks.append(self._get_model_checkpoint())
         return pl.Trainer(
             accelerator=accelerator_device,
             devices=device,
             max_epochs=self._conf.training.epochs,
             check_val_every_n_epoch=self._conf.validation.run_every_epoch,
-            enable_progress_bar=True,
-            deterministic=True,
             logger=self._metric_logger,
             callbacks=callbacks,
             **self._conf.training.arguments,
         )
```

### Comparing `kit4dl-2023.9b2/kit4dl/nn/validators.py` & `kit4dl-2024.5b0/kit4dl/nn/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A module with resuable validators."""
+
 import warnings
 
 import torch
 import torchmetrics as tm
 
 import kit4dl.io as io_
 from kit4dl import Kit4DLCallback
```

### Comparing `kit4dl-2023.9b2/kit4dl/utils.py` & `kit4dl-2024.5b0/kit4dl/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module with utilities functions and structures."""
+
 import os
 import random
 from typing import Callable, Hashable
 
 import numpy as np
 import torch
```

### Comparing `kit4dl-2023.9b2/kit4dl.egg-info/PKG-INFO` & `kit4dl-2024.5b0/kit4dl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kit4dl
-Version: 2023.9b2
+Version: 2024.5b0
 Summary: Kit4DL - A quick way to start with machine and deep learning
 Author: Jakub Walczak, Marco Mancini, Mirko Stojiljkovic, Shahbaz Alvi
 License: MIT License
         
         Copyright (c) 2023 opengeokube
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,19 +40,19 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lightning<=2.1.0.rc0
-Requires-Dist: torch<2.1.0,>=1.11.0
-Requires-Dist: torchmetrics<1.1.0,>=0.7.0
+Requires-Dist: lightning>=2.2.4
+Requires-Dist: torch>=2.1.0
+Requires-Dist: torchmetrics>=1.1.0
 Requires-Dist: numpy<=1.25.3,>=1.17.2
-Requires-Dist: pydantic<2.2.0,>=2.0.0
+Requires-Dist: pydantic>2.4.0
 Requires-Dist: scikit-learn
 Requires-Dist: colormath
 Requires-Dist: tqdm<4.67.0,>=4.57.0
 Requires-Dist: typing-extensions<4.8.0,>=4.0.0; python_version <= "3.11"
 Requires-Dist: Jinja2<3.2.0
 Requires-Dist: typer[all]
 Requires-Dist: toml; python_version < "3.11"
@@ -89,39 +89,43 @@
 1. Jakub Walczak <a href="https://orcid.org/0000-0002-5632-9484"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Marco Macini <a href="https://orcid.org/0000-0002-9150-943X"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Mirko Stojiljkovic <a href="https://orcid.org/0000-0003-2256-1645"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 1. Shahbaz Alvi <a href="https://orcid.org/0000-0001-5779-8568"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png" width="16" height="16" /></a>
 
 ## 📜 Cite Us
 ```bibtex
-@SOFTWARE{kit4dl,
-  author = {Walczak, Jakub and
-            Mancini, Marco and
-            Stojiljković, Mirko and
-            Alvi, Shahbaz},
-  title = {Kit4DL},
-  month = sep,
-  year = 2023,
-  note = {{Available in GitHub: https://github.com/opengeokube/kit4dl}},
-  publisher = {Zenodo},
-  version = {2023.9b1},
-  doi = {10.5281/zenodo.8328176},
-  url = {https://doi.org/10.5281/zenodo.8328176}
+@ARTICLE{kit4dl,
+    author = {Jakub Walczak and Marco Mancini and Shahbaz Alvi},
+    title = {Kit4DL: Towards fast prototyping and experimentation in machine learning and deep learning},
+    journal = {SoftwareX},
+    volume = {26},
+    pages = {101707},
+    year = {2024},
+    issn = {2352-7110},
+    doi = {https://doi.org/10.1016/j.softx.2024.101707},
+    url = {https://www.sciencedirect.com/science/article/pii/S2352711024000785},
+    keywords = {Deep learning, Machine learning, Prototyping, Python framework},
 }
 ```
+## 📖 Documentation
+Read the official [Documentation](https://opengeokube.github.io/kit4dl/index.html) to learn Kit4DL!
+
 ## 🚧 Roadmap
 
 > **Warning**: Kit4DL is currently in its alpha stage. All recommendations are welcomed.
 
 - [ ] add handling sklearn-like models
 - [ ] add functionality to serve the model
 - [x] enable custom metrics
 - [x] enable using callbacks (also custom ones)
 - [ ] write more unit tests
+- [ ] enable overwritting parameters with command line
 
+## 🙏 Acknowledgement
+This work has received fundings from the Polish National Centre for Research and Development under the LIDER XI program [grant number 0092/L-11/2019, "Semantic analysis of 3D point clouds"] and from the European Union’s Horizon 2020 Research and Innovation programme [SILVANUS Project - grant agreement number 101037247].
 
 ## 🎬 Quickstart
 
 ### Getting started
 
 #### Installation
 ```bash
@@ -201,14 +205,15 @@
 1. [Configuring optimizer](#configuring-optimizer)
 1. [Configuring criterion](#configuring-criterion)
 1. [Configuring metrics](#configuring-metrics)
 1. [Configuring checkpoint](#configuring-checkpoint)
 1. [Defining `target`](#defining-target)
 1. [Substitutable symbols](#substitutable-symbols)
 1. [Context constants](#context-constants)
+1. [Sensitive data obfuscating](#sensitive-data-obfuscating)
 
 #### Configuring base setup
 Most of the training/validation procedure is managed by a configuration file in the TOML format (recommended name is `conf.toml`).
 Each aspect is covered by separate sections. The general one is called `[base]`.
 It has the following properties:
 
 |   **Property** 	|  **Type**        |                                                   **Details**                                          	|
@@ -272,15 +277,15 @@
 In the `configure` method, the architecture of the network should be defined. 
 In `run_step` method, it turn, the logic for single forward pass should be implemented.
 
 ##### ✍️ Example
 ```python
 import torch
 from torch import nn
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 class SimpleCNN(Kit4DLAbstractModule):
     def configure(self, input_dims, output_dims) -> None:
         self.l1 = nn.Sequential(
             nn.Conv2d(
                 input_dims, 16, kernel_size=3, padding="same", bias=True
             ),
@@ -312,15 +317,15 @@
 
 If a forward pass for your model differs for the training, validation, test, or prediction stages, you can define separate methods for them:
 
 ##### ✍️ Example
 ```python
 import torch
 from torch import nn
-from kit4dl import Kit4DLAbstractModule
+from kit4dl.nn.base import Kit4DLAbstractModule
 
 class SimpleCNN(Kit4DLAbstractModule):
     ...
     def run_val_step(self, batch, batch_idx) -> tuple[torch.Tensor, torch.Tensor]:
         pass
 
     def run_test_step(self, batch, batch_idx) -> tuple[torch.Tensor, torch.Tensor]:
@@ -331,27 +336,27 @@
 ```
 
 > **Note**: If you need more customization of the process, you can always override the existing methods according to your needs.
 
 #### Defining datamodule
 Similarily to the model, datamodule instance is fully defined by the Python class and its configuration.
 The datamodule need to be a subclass of the `Kit4DLAbstractDataModule` abstract class from the `kit4dl` package.
-The class has to implement, at least, `prepare_trainvaldataset` (if preparing is the same for the train and validation splits) or `prepare_traindataset` and `prepare_valdataset` (if preparing data differs). Besides those, you can define `prepare_testdataset` and `prepare_predictdataset`, for test and prediction, respectively.
+The class has to implement, at least, `prepare_trainvaldatasets` (if preparing is the same for the train and validation splits) or `prepare_traindatasets` and `prepare_valdatasets` (if preparing data differs). Besides those, you can define `prepare_testdataset` and `prepare_predictdataset`, for test and prediction, respectively.
 
 ##### ✍️ Example
 ```python
 from torch.utils.data import Dataset, random_split
 from torchvision import transforms
 from torchvision.datasets import MNIST
 
-from kit4dl import Kit4DLAbstractDataModule
+from kit4dl.dataset import Kit4DLAbstractDataModule
 
 
 class MNISTCustomDatamodule(Kit4DLAbstractDataModule):
-    def prepare_trainvaldataset(
+    def prepare_trainvaldatasets(
         self, root_dir: str
     ) -> tuple[Dataset, Dataset]:
         dset = MNIST(
             root=root_dir,
             train=True,
             download=True,
             transform=transforms.ToTensor(),
@@ -436,16 +441,16 @@
 batch_size = 150
 shuffle = false
 num_workers = 4
 ```
 
 In the root `[dataset]` you should define `target` property being a path to the subclass of the `Kit4DLAbstractDataModule` module (see [Defining `target`](#defining-target)).
 Then, you need to define either `[dataset.trainval]` section or two separate sections: `[dataset.train]`, `[dataset.validation]`. There are also optional sections: `[dataset.test]` and `[dataset.predict]`.
-In `[dataset.trainval]` you pass values for parameters of the `prepare_trainvaldataset` method.
-Respectively, in the `[dataset.train]` you pass values for the parameters of the `prepare_traindataset` method, in `[dataset.validation]` — `prepare_valdataset`, `[dataset.test]` — `prepare_testdataset`, `[dataset.predict]` — `prepare_predictdataset`.
+In `[dataset.trainval]` you pass values for parameters of the `prepare_trainvaldatasets` method.
+Respectively, in the `[dataset.train]` you pass values for the parameters of the `prepare_traindatasets` method, in `[dataset.validation]` — `prepare_valdatasets`, `[dataset.test]` — `prepare_testdataset`, `[dataset.predict]` — `prepare_predictdataset`.
 
 Besides dataset configuration, you need to specify data loader arguments as indicated in the PyTorch docs [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader).
 
 > **Warning**: You **cannot** specify loader arguments for in the `[dataset.trainval.loader]`. Loaders should be defined for each split separately.
 
 
 #### Configuring training
@@ -476,15 +481,15 @@
 ```python
 import os
 from typing import Any
 
 import lightning.pytorch as pl
 import torchmetrics as tm
 
-from kit4dl import Kit4DLCallback, StepOutput
+from kit4dl import Kit4DLCallback
 
 
 class SaveConfusionMatrixCallback(Kit4DLCallback):
     _cm: tm.ConfusionMatrix
     _num_classes: int
     _task: str
     _save_dir: str
@@ -503,20 +508,20 @@
             task=self._task, num_classes=self._num_classes
         )
 
     def on_validation_batch_end(
         self,
         trainer: pl.Trainer,
         pl_module: pl.LightningModule,
-        outputs: StepOutput,
+        outputs: dict,
         batch: Any,
         batch_idx: int,
         dataloader_idx: int = 0,
     ) -> None:
-        self._cm.update(outputs.predictions, outputs.labels)
+        self._cm.update(outputs['pred'], outputs['true'])
 
     def on_validation_epoch_end(
         self, trainer: pl.Trainer, pl_module: pl.LightningModule
     ) -> None:
         """Called when the val epoch ends."""
         fig, _ = self._cm.plot()
         target_file = os.path.join(
@@ -699,7 +704,22 @@
 |   **Symbol** 	|            **Meaning of the symbol**                                   	|          **Example**                  |
 |-------------	|-----------------------------------------------------------------------	| -----------------------------------	|
 | `PROJECT_DIR`	| the home directory of the TOML configuration file (project directory) 	| `context.PROJECT_DIR`                 |
 | `LOG_LEVEL`	| logging level as defined in the configuration TOML file                	| `context.LOG_LEVEL`                   |
 | `LOG_FORMAT`	| logging message format as defined in the configuration TOML file      	| `context.LOG_FORMAT`                  |
 |  `VERSION`	| the current version of the package                                      	| `context.VERSION`                     |
 
+#### Sensitive data obfuscating
+It might happen, some sensitive data are stored in the configuration file. 
+We should prevent those data from being logged as hyperparameters. This is the reason why
+Kit4DL supports sensitive data obfuscating. By default, all values whose keys contain `key` string
+will be obfuscated with `***`. Both, sensitive data key and obfuscating value can be customized by
+a user, by setting environmental variables accordingly. To obfuscate all
+values containig `url` (e.g.`api-url`, `url-2`, etc.) with `^^^`, just use
+the following code.
+
+##### ✍️ Example
+```python
+import os
+os.environ["KIT4DL_KEY_TO_OBFUSCATE"] = "url"
+os.environ["KIT4DL_OBFUSCATING_VALUE"] = "^^^"
+```
```

### Comparing `kit4dl-2023.9b2/kit4dl.egg-info/SOURCES.txt` & `kit4dl-2024.5b0/kit4dl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 examples/cnn_mnist_classification/conf.toml
 examples/cnn_s3dis_segmentation/conf.toml
 kit4dl/__init__.py
 kit4dl/_version.py
 kit4dl/context.py
-kit4dl/dataset.py
 kit4dl/formatting.py
 kit4dl/io.py
 kit4dl/kit4dl_types.py
 kit4dl/metric.py
 kit4dl/mixins.py
 kit4dl/stages.py
 kit4dl/utils.py
@@ -26,23 +25,25 @@
 kit4dl/cli/_templates/project/conf.toml
 kit4dl/cli/_templates/project/datamodule.py
 kit4dl/cli/_templates/project/model.py
 kit4dl/nn/__init__.py
 kit4dl/nn/base.py
 kit4dl/nn/callbacks.py
 kit4dl/nn/confmodels.py
+kit4dl/nn/dataset.py
 kit4dl/nn/trainer.py
 kit4dl/nn/validators.py
 tests/__init__.py
 tests/dummy_module.py
 tests/dummy_module2.py
 tests/fixtures.py
 tests/test_context.py
 tests/test_datamodule.py
 tests/test_formatting.py
+tests/test_init.py
 tests/test_io.py
 tests/test_metrics.py
 tests/test_mixins.py
 tests/utils.py
 tests/cli/__init__.py
 tests/cli/test_app.py
 tests/nn/__init__.py
```

### Comparing `kit4dl-2023.9b2/pyproject.toml` & `kit4dl-2024.5b0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     "Intended Audience :: End Users/Desktop",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-    "lightning<=2.1.0.rc0",
-    "torch>=1.11.0,<2.1.0",
-    "torchmetrics>=0.7.0,<1.1.0",
+    "lightning>=2.2.4",
+    "torch>=2.1.0",
+    "torchmetrics>=1.1.0",
     "numpy>=1.17.2,<=1.25.3",
-    "pydantic>=2.0.0,<2.2.0",
+    "pydantic>2.4.0",
     "scikit-learn",
     "colormath",
     "tqdm>=4.57.0,<4.67.0",
     "typing-extensions>=4.0.0,<4.8.0; python_version<='3.11'",
     "Jinja2<3.2.0",
     "typer[all]",
     "toml; python_version<'3.11'"
@@ -71,16 +71,16 @@
 line_length = 79
 preview = true
 
 [tool.mypy]
 files = [
     "kit4dl", "."
 ]
-exclude = ["tests/", "examples/"]
+exclude = ["tests/", "examples/", "kit4dl/nn/callbacks"]
 
 [project.scripts]
 kit4dl = "kit4dl.cli.app:run"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning"
-]
+]
```

### Comparing `kit4dl-2023.9b2/tests/cli/test_app.py` & `kit4dl-2024.5b0/tests/cli/test_app.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/tests/dummy_module.py` & `kit4dl-2024.5b0/tests/dummy_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torchmetrics as tm
 
-from kit4dl.dataset import Kit4DLAbstractDataModule
+from kit4dl.nn.dataset import Kit4DLAbstractDataModule
 from kit4dl.nn.base import Kit4DLAbstractModule
 
 
 class A:
     pass
```

### Comparing `kit4dl-2023.9b2/tests/fixtures.py` & `kit4dl-2024.5b0/tests/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,33 +22,37 @@
     conf.base.accelerator_device_and_id = PropertyMock(
         return_value="cuda"
     ), PropertyMock(return_value=0)
     conf.logging.level = "INFO"
     conf.logging.format_ = (
         "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
-    conf.base.seed = 0
+
     conf.model = PropertyMock()
     conf.model.arguments = {"input_dims": 10, "output_dims": 1}
     conf.metrics_obj = {
         "Precision": tm.Precision(task="binary"),
         "FBetaScore": tm.FBetaScore(task="binary"),
     }
     conf.training = PropertyMock()
     conf.training.optimizer = PropertyMock()
     conf.training.optimizer.optimizer = torch.optim.SGD
     conf.training.checkpoint.mode = "max"
+    conf.training.callback = []
 
     conf.model.model_class = PropertyMock()
 
     conf.dataset = PropertyMock()
     conf.dataset.datamodule_class = PropertyMock()
 
     conf.dict = Mock()
     conf.dict.return_value = {}
+    conf.obfuscated_dict = Mock()
+    conf.obfuscated_dict.return_value = {}
+    conf.base.seed = 0
     yield conf
 
 
 @pytest.fixture
 def true_conf():
     yield Conf(
         root_dir=os.path.join(os.getcwd(), "tests", "resources"),
```

### Comparing `kit4dl-2023.9b2/tests/nn/test_base.py` & `kit4dl-2024.5b0/tests/nn/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 
 class TestBaseMLModel:
     @pytest.fixture
     def custom_module(self, conf):
         class CustomModule(Kit4DLAbstractModule):
             configure = MagicMock()
             run_step = MagicMock()
+            _conf = conf
+            _logger = MagicMock()
 
-        obj = CustomModule(conf=conf)
+        obj = CustomModule(**conf.model.arguments)
         yield obj
 
     @pytest.fixture
     def module(self):
         from torch import nn
 
         class Module(Kit4DLAbstractModule):
@@ -55,14 +57,18 @@
             ) -> tuple[torch.Tensor, torch.Tensor]:
                 x, cat, instance = batch
                 res = self.l1(x.permute(0, 2, 1))
                 return cat, res
 
         return Module
 
+    @pytest.mark.skip(
+        "MetricTracker is not located in Kit4DLAbstractModule anymore. See"
+        " Issue #40"
+    )
     def test_setup_metric_trackers(self, custom_module):
         assert custom_module.train_metric_tracker is not None
         assert custom_module.val_metric_tracker is not None
         assert custom_module.test_metric_tracker is not None
 
     def test_setup_called(self, custom_module, conf):
         custom_module.configure.assert_called_with(**conf.model.arguments)
```

### Comparing `kit4dl-2023.9b2/tests/nn/test_confmodels.py` & `kit4dl-2024.5b0/tests/nn/test_confmodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,17 @@
             layers = 4
             dropout = 0.1
             output_dims = 10
         """
         conf = ModelConf(**toml.loads(load))
         assert issubclass(conf.model_class, Kit4DLAbstractModule)
 
+    @pytest.mark.skip(
+        reason="checking subclass was moved from confmodels to Trainer"
+    )
     def test_get_model_failed_on_wrong_parent_class(self):
         load = """
             target = "tests.dummy_module::A"
         """
         with pytest.raises(ValidationError):
             _ = ModelConf(**toml.loads(load))
 
@@ -289,15 +292,15 @@
     def test_criterion_weight_passed(self):
         load = """
             target = "torch.nn::NLLLoss"
             weight = [0.1, 0.1]
         """
         conf = CriterionConf(**toml.loads(load))
         conf.target == "torch.nn.NLLLoss"
-        assert conf.weight == [0.1, 0.1]
+        assert conf.arguments["weight"] == [0.1, 0.1]
 
     @pytest.mark.skip(reason="weights values are not validated anymore")
     def test_criterion_failed_on_negative_weight(self):
         load = """
             target = "torch.nn::NLLLoss"
             weight = [-0.1, 0.1]
         """
@@ -313,20 +316,26 @@
 
     def test_get_criterion_failed_on_wrong_parent_class(self):
         load = """
             target = "tests.dummy_module::A"
         """
         with pytest.raises(
             ValidationError,
-            match=r"target class of the criterion must be a subclass of*",
+            match=(
+                r"target class of the criterion must be a function or a"
+                r" subclass of torch.nn.Module class!"
+            ),
         ):
             _ = CriterionConf(**toml.loads(load))
 
 
 class TestDatasetConf:
+    @pytest.mark.skip(
+        reason="checking subclass was moved from confmodels to Trainer"
+    )
     def test_get_dataset_fail_on_wrong_parent_class(self):
         load = """
             target = "tests.dummy_module::DummyDatasetModuleWrong"
         """
         with pytest.raises(
             ValidationError,
             match=r"target class of the dataset module must be a subclass of*",
@@ -545,14 +554,17 @@
         conf = Conf(**toml.loads(load))
         assert "name" in conf.logging.arguments
         assert (
             conf.logging.arguments["name"]
             == "handwritten_digit_classification"
         )
 
+    @pytest.mark.skip(
+        reason="Name is overwriten by experiment_name since version 2024.5b1"
+    )
     def test_dont_override_exp_name_with_base_if_provided(
         self, base_conf_txt_full
     ):
         load = base_conf_txt_full + """
         [logging]
         type = "csv"
         name = "logging_exp_name"
@@ -653,14 +665,17 @@
         load = f"""
             type = "{log_nick}"
         """
         conf = LoggingConf(**toml.loads(load))
         conf.maybe_update_experiment_name(EXP_NAME)
         assert conf.arguments[attr_name] == EXP_NAME
 
+    @pytest.mark.skip(
+        reason="Name is overwriten by experiment_name since version 2024.5b1"
+    )
     @pytest.mark.parametrize(
         "log_nick, attr_name",
         [
             ("comet", "experiment_name"),
             ("csv", "name"),
             ("mlflow", "experiment_name"),
             ("neptune", "name"),
```

### Comparing `kit4dl-2023.9b2/tests/nn/test_trainer.py` & `kit4dl-2024.5b0/tests/nn/test_trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unittest.mock import MagicMixin, patch
+from unittest.mock import MagicMixin, PropertyMock, patch
 
 import pytest
 
 from kit4dl.nn.trainer import Trainer, set_seed
 from tests.fixtures import conf, true_conf
 
 
@@ -24,22 +24,21 @@
         arr2 = np.random.rand(1000)
         ten2 = torch.rand(10, 20, 30)
         assert np.allclose(arr1, arr2)
         assert torch.allclose(ten1, ten2)
 
     @patch("kit4dl.nn.trainer.Trainer._configure_trainer")
     @patch("kit4dl.nn.trainer.Trainer._configure_datamodule")
+    @patch("kit4dl.io.assert_valid_class", return_value=True)
     def test_configure_model(
-        self, mock_conf_trainer, mock_conf_datamodule, conf
+        self, mock_assert, mock_conf_trainer, mock_conf_datamodule, conf
     ):
         Trainer(conf).prepare()
-        conf.model.model_class.assert_called_once_with(conf=conf)
+        conf.model.model_class.assert_called_once_with(**conf.model.arguments)
 
     @patch("kit4dl.nn.trainer.Trainer._configure_trainer")
-    @patch("kit4dl.nn.trainer.Trainer._configure_model")
-    def test_configure_datamodule(
-        self, mock_conf_trainer, mock_conf_model, conf
-    ):
+    @patch("kit4dl.io.assert_valid_class", return_value=True)
+    def test_configure_datamodule(self, mock_assert, mock_conf_trainer, conf):
         Trainer(conf).prepare()
         conf.dataset.datamodule_class.assert_called_once_with(
             conf=conf.dataset
         )
```

### Comparing `kit4dl-2023.9b2/tests/nn/test_validators.py` & `kit4dl-2024.5b0/tests/nn/test_validators.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/tests/resources/dataset.py` & `kit4dl-2024.5b0/tests/resources/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from torch.utils.data import random_split
 from torchvision.datasets import MNIST
 
 from kit4dl import Kit4DLAbstractDataModule
 
 
 class MNISTCustomDataset(Kit4DLAbstractDataModule):
-    def prepare_trainvaldataset(self, root_dir: str):
+    def prepare_trainvaldatasets(self, root_dir: str):
         dset = MNIST(root=root_dir, train=True, download=True)
         train_dset, val_dset = random_split(dset, [0.8, 0.2])
         return (train_dset, val_dset)
 
     def prepare_testdataset(self, root_dir: str):
         return MNIST(root=root_dir, train=False, download=True)
```

### Comparing `kit4dl-2023.9b2/tests/resources/model.py` & `kit4dl-2024.5b0/tests/resources/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Exemple module with simple convlution neural network"""
+
 import torch
 import torch.nn as nn
 
 from kit4dl import Kit4DLAbstractModule
 
 
 class SimpleCNN(Kit4DLAbstractModule):
```

### Comparing `kit4dl-2023.9b2/tests/resources/test_file.toml` & `kit4dl-2024.5b0/tests/resources/test_file.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/tests/test_context.py` & `kit4dl-2024.5b0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/tests/test_formatting.py` & `kit4dl-2024.5b0/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/tests/test_io.py` & `kit4dl-2024.5b0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b2/tests/test_metrics.py` & `kit4dl-2024.5b0/tests/test_metrics.py`

 * *Files identical despite different names*

