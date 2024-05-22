# Comparing `tmp/kit4dl-2024.5b0.tar.gz` & `tmp/kit4dl-2024.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kit4dl-2024.5b0.tar", last modified: Mon May 20 09:39:17 2024, max compression
+gzip compressed data, was "kit4dl-2024.5b1.tar", last modified: Wed May 22 07:49:49 2024, max compression
```

## Comparing `kit4dl-2024.5b0.tar` & `kit4dl-2024.5b1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    33014 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.322361 kit4dl-2024.5b0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/examples/cnn_mnist_classification/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/examples/cnn_mnist_classification/conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/examples/cnn_s3dis_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/examples/cnn_s3dis_segmentation/conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/kit4dl/
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.326361 kit4dl-2024.5b0/kit4dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.322361 kit4dl-2024.5b0/kit4dl/cli/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/kit4dl/cli/_templates/project/
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/_templates/project/conf.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/_templates/project/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/_templates/project/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/kit4dl_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/kit4dl/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/confmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/nn/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/kit4dl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/kit4dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33014 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 09:39:17.000000 kit4dl-2024.5b0/kit4dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.330361 kit4dl-2024.5b0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/cli/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/dummy_module2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/tests/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_confmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/nn/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:39:17.334361 kit4dl-2024.5b0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/resources/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/resources/test_file.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 09:39:12.000000 kit4dl-2024.5b0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.322246 kit4dl-2024.5b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32981 2024-05-22 07:49:49.322246 kit4dl-2024.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.310246 kit4dl-2024.5b1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.314246 kit4dl-2024.5b1/examples/cnn_mnist_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/examples/cnn_mnist_classification/conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.314246 kit4dl-2024.5b1/examples/cnn_s3dis_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/examples/cnn_s3dis_segmentation/conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.314246 kit4dl-2024.5b1/kit4dl/
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.318246 kit4dl-2024.5b1/kit4dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.310246 kit4dl-2024.5b1/kit4dl/cli/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.318246 kit4dl-2024.5b1/kit4dl/cli/_templates/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/cli/_templates/project/conf.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/cli/_templates/project/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/cli/_templates/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/kit4dl_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.318246 kit4dl-2024.5b1/kit4dl/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/confmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/nn/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/kit4dl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.322246 kit4dl-2024.5b1/kit4dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32981 2024-05-22 07:49:49.000000 kit4dl-2024.5b1/kit4dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-22 07:49:49.000000 kit4dl-2024.5b1/kit4dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:49:49.000000 kit4dl-2024.5b1/kit4dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 07:49:49.000000 kit4dl-2024.5b1/kit4dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 07:49:49.000000 kit4dl-2024.5b1/kit4dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 07:49:49.000000 kit4dl-2024.5b1/kit4dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:49:49.322246 kit4dl-2024.5b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.318246 kit4dl-2024.5b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.318246 kit4dl-2024.5b1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/cli/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/dummy_module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.322246 kit4dl-2024.5b1/tests/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/nn/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/nn/test_confmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/nn/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/nn/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:49:49.322246 kit4dl-2024.5b1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/resources/test_file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-22 07:49:45.000000 kit4dl-2024.5b1/tests/utils.py
```

### Comparing `kit4dl-2024.5b0/LICENSE` & `kit4dl-2024.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/PKG-INFO` & `kit4dl-2024.5b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kit4dl
-Version: 2024.5b0
+Version: 2024.5b1
 Summary: Kit4DL - A quick way to start with machine and deep learning
 Author: Jakub Walczak, Marco Mancini, Mirko Stojiljkovic, Shahbaz Alvi
 License: MIT License
         
         Copyright (c) 2023 opengeokube
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 Requires-Dist: torch>=2.1.0
 Requires-Dist: torchmetrics>=1.1.0
 Requires-Dist: numpy<=1.25.3,>=1.17.2
 Requires-Dist: pydantic>2.4.0
 Requires-Dist: scikit-learn
 Requires-Dist: colormath
 Requires-Dist: tqdm<4.67.0,>=4.57.0
-Requires-Dist: typing-extensions<4.8.0,>=4.0.0; python_version <= "3.11"
+Requires-Dist: typing-extensions>=4.8.0
 Requires-Dist: Jinja2<3.2.0
 Requires-Dist: typer[all]
 Requires-Dist: toml; python_version < "3.11"
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/opengeokube/ml-kit/56dc56c1be7f6332c0f75cdfb3160d29cebc3c58/static/logo.svg" width="20%" height="20%">
```

### Comparing `kit4dl-2024.5b0/README.md` & `kit4dl-2024.5b1/README.md`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/examples/cnn_mnist_classification/conf.toml` & `kit4dl-2024.5b1/examples/cnn_mnist_classification/conf.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/examples/cnn_s3dis_segmentation/conf.toml` & `kit4dl-2024.5b1/examples/cnn_s3dis_segmentation/conf.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/__init__.py` & `kit4dl-2024.5b1/kit4dl/__init__.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/cli/_templates/project/conf.toml` & `kit4dl-2024.5b1/kit4dl/cli/_templates/project/conf.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/cli/_templates/project/datamodule.py` & `kit4dl-2024.5b1/kit4dl/cli/_templates/project/datamodule.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/cli/_templates/project/model.py` & `kit4dl-2024.5b1/kit4dl/cli/_templates/project/model.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/cli/app.py` & `kit4dl-2024.5b1/kit4dl/cli/app.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/context.py` & `kit4dl-2024.5b1/kit4dl/context.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/formatting.py` & `kit4dl-2024.5b1/kit4dl/formatting.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/io.py` & `kit4dl-2024.5b1/kit4dl/io.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/metric.py` & `kit4dl-2024.5b1/kit4dl/metric.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/mixins.py` & `kit4dl-2024.5b1/kit4dl/mixins.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/nn/base.py` & `kit4dl-2024.5b1/kit4dl/nn/base.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/nn/callbacks.py` & `kit4dl-2024.5b1/kit4dl/nn/callbacks.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/nn/confmodels.py` & `kit4dl-2024.5b1/kit4dl/nn/confmodels.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/nn/dataset.py` & `kit4dl-2024.5b1/kit4dl/nn/dataset.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/nn/trainer.py` & `kit4dl-2024.5b1/kit4dl/nn/trainer.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/nn/validators.py` & `kit4dl-2024.5b1/kit4dl/nn/validators.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl/utils.py` & `kit4dl-2024.5b1/kit4dl/utils.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/kit4dl.egg-info/PKG-INFO` & `kit4dl-2024.5b1/kit4dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kit4dl
-Version: 2024.5b0
+Version: 2024.5b1
 Summary: Kit4DL - A quick way to start with machine and deep learning
 Author: Jakub Walczak, Marco Mancini, Mirko Stojiljkovic, Shahbaz Alvi
 License: MIT License
         
         Copyright (c) 2023 opengeokube
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 Requires-Dist: torch>=2.1.0
 Requires-Dist: torchmetrics>=1.1.0
 Requires-Dist: numpy<=1.25.3,>=1.17.2
 Requires-Dist: pydantic>2.4.0
 Requires-Dist: scikit-learn
 Requires-Dist: colormath
 Requires-Dist: tqdm<4.67.0,>=4.57.0
-Requires-Dist: typing-extensions<4.8.0,>=4.0.0; python_version <= "3.11"
+Requires-Dist: typing-extensions>=4.8.0
 Requires-Dist: Jinja2<3.2.0
 Requires-Dist: typer[all]
 Requires-Dist: toml; python_version < "3.11"
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/opengeokube/ml-kit/56dc56c1be7f6332c0f75cdfb3160d29cebc3c58/static/logo.svg" width="20%" height="20%">
```

### Comparing `kit4dl-2024.5b0/kit4dl.egg-info/SOURCES.txt` & `kit4dl-2024.5b1/kit4dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/pyproject.toml` & `kit4dl-2024.5b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "torch>=2.1.0",
     "torchmetrics>=1.1.0",
     "numpy>=1.17.2,<=1.25.3",
     "pydantic>2.4.0",
     "scikit-learn",
     "colormath",
     "tqdm>=4.57.0,<4.67.0",
-    "typing-extensions>=4.0.0,<4.8.0; python_version<='3.11'",
+    "typing-extensions>=4.8.0",
     "Jinja2<3.2.0",
     "typer[all]",
     "toml; python_version<'3.11'"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "kit4dl._version.__version__"}
@@ -79,8 +79,8 @@
 
 [project.scripts]
 kit4dl = "kit4dl.cli.app:run"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning"
-]
+]
```

### Comparing `kit4dl-2024.5b0/tests/cli/test_app.py` & `kit4dl-2024.5b1/tests/cli/test_app.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/dummy_module.py` & `kit4dl-2024.5b1/tests/dummy_module.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/fixtures.py` & `kit4dl-2024.5b1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/nn/test_base.py` & `kit4dl-2024.5b1/tests/nn/test_base.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/nn/test_confmodels.py` & `kit4dl-2024.5b1/tests/nn/test_confmodels.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/nn/test_trainer.py` & `kit4dl-2024.5b1/tests/nn/test_trainer.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/nn/test_validators.py` & `kit4dl-2024.5b1/tests/nn/test_validators.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/resources/dataset.py` & `kit4dl-2024.5b1/tests/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/resources/model.py` & `kit4dl-2024.5b1/tests/resources/model.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/resources/test_file.toml` & `kit4dl-2024.5b1/tests/resources/test_file.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/test_context.py` & `kit4dl-2024.5b1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/test_formatting.py` & `kit4dl-2024.5b1/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/test_init.py` & `kit4dl-2024.5b1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/test_io.py` & `kit4dl-2024.5b1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/test_metrics.py` & `kit4dl-2024.5b1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2024.5b0/tests/test_mixins.py` & `kit4dl-2024.5b1/tests/test_mixins.py`

 * *Files identical despite different names*

