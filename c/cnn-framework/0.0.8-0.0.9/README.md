# Comparing `tmp/cnn_framework-0.0.8.tar.gz` & `tmp/cnn_framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnn_framework-0.0.8.tar", last modified: Wed Nov  8 13:50:15 2023, max compression
+gzip compressed data, was "cnn_framework-0.0.9.tar", last modified: Fri Nov 24 11:05:01 2023, max compression
```

## Comparing `cnn_framework-0.0.8.tar` & `cnn_framework-0.0.9.tar`

### file list

```diff
@@ -1,116 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.340900 cnn_framework-0.0.8/
--rw-rw-rw-   0        0        0     1513 2023-10-04 14:04:22.000000 cnn_framework-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1888 2023-11-08 13:50:15.336898 cnn_framework-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      999 2023-10-05 14:48:39.000000 cnn_framework-0.0.8/README.md
--rw-rw-rw-   0        0        0       86 2023-10-05 13:36:16.000000 cnn_framework-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       71 2023-11-08 13:50:15.342899 cnn_framework-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1169 2023-11-08 10:20:42.000000 cnn_framework-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.868113 cnn_framework-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.900113 cnn_framework-0.0.8/src/cnn_framework/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:41:28.000000 cnn_framework-0.0.8/src/cnn_framework/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.935932 cnn_framework-0.0.8/src/cnn_framework/dummy_cnn/
--rw-rw-rw-   0        0        0        0 2023-09-12 16:30:07.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_cnn/__init__.py
--rw-rw-rw-   0        0        0     2134 2023-10-20 09:30:57.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_cnn/data_set.py
--rw-rw-rw-   0        0        0      685 2023-04-27 08:48:45.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_cnn/model.py
--rw-rw-rw-   0        0        0      613 2023-10-20 09:31:15.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_cnn/model_params.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.952860 cnn_framework-0.0.8/src/cnn_framework/dummy_regression_cnn/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:41:52.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_regression_cnn/__init__.py
--rw-rw-rw-   0        0        0     2310 2023-10-20 09:31:34.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_regression_cnn/data_set.py
--rw-rw-rw-   0        0        0      685 2023-08-04 13:21:15.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_regression_cnn/model.py
--rw-rw-rw-   0        0        0      575 2023-10-20 09:31:44.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_regression_cnn/model_params.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.970231 cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/
--rw-rw-rw-   0        0        0        0 2023-09-04 08:23:07.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/data_set.py
--rw-rw-rw-   0        0        0      570 2023-09-04 08:21:18.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/model.py
--rw-rw-rw-   0        0        0      550 2023-10-20 09:31:52.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/model_params.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.992232 cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/
--rw-rw-rw-   0        0        0        0 2023-09-28 09:31:58.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/__init__.py
--rw-rw-rw-   0        0        0     1920 2023-10-20 09:32:08.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/data_set.py
--rw-rw-rw-   0        0        0     1130 2023-09-28 09:37:23.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/model.py
--rw-rw-rw-   0        0        0      715 2023-10-20 09:32:20.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/model_params.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.016231 cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:41:45.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/data_set.py
--rw-rw-rw-   0        0        0     2597 2023-10-20 09:32:42.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/decoder.py
--rw-rw-rw-   0        0        0     1343 2023-10-20 09:32:49.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/encoder.py
--rw-rw-rw-   0        0        0     1009 2023-10-20 09:34:55.000000 cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/model_params.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.053234 cnn_framework-0.0.8/src/cnn_framework/utils/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:42:51.000000 cnn_framework-0.0.8/src/cnn_framework/utils/__init__.py
--rw-rw-rw-   0        0        0     2847 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/create_dummy_data_set.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.069935 cnn_framework-0.0.8/src/cnn_framework/utils/data_loader_generators/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:02.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_loader_generators/__init__.py
--rw-rw-rw-   0        0        0     2013 2023-10-05 13:05:55.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_loader_generators/classifier_data_loader_generator.py
--rw-rw-rw-   0        0        0     6066 2023-10-20 09:33:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_loader_generators/data_loader_generator.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.084935 cnn_framework-0.0.8/src/cnn_framework/utils/data_managers/
--rw-rw-rw-   0        0        0        0 2023-10-06 10:48:38.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_managers/__init__.py
--rw-rw-rw-   0        0        0     2300 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_managers/abstract_data_manager.py
--rw-rw-rw-   0        0        0      306 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_managers/default_data_manager.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.106936 cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:05.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/__init__.py
--rw-rw-rw-   0        0        0     6276 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/abstract_data_set.py
--rw-rw-rw-   0        0        0     2757 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/dataset_output.py
--rw-rw-rw-   0        0        0     1773 2023-09-05 12:30:38.000000 cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/detection_data_set.py
--rw-rw-rw-   0        0        0     2278 2022-11-03 17:10:50.000000 cnn_framework-0.0.8/src/cnn_framework/utils/dimensions.py
--rw-rw-rw-   0        0        0     5996 2023-08-31 13:43:43.000000 cnn_framework-0.0.8/src/cnn_framework/utils/display_tools.py
--rw-rw-rw-   0        0        0      350 2023-09-22 09:10:49.000000 cnn_framework-0.0.8/src/cnn_framework/utils/enum.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.136935 cnn_framework-0.0.8/src/cnn_framework/utils/losses/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:09.000000 cnn_framework-0.0.8/src/cnn_framework/utils/losses/__init__.py
--rw-rw-rw-   0        0        0      720 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/losses/dice_loss.py
--rw-rw-rw-   0        0        0     5637 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/losses/focal_loss.py
--rw-rw-rw-   0        0        0      617 2023-09-28 10:04:07.000000 cnn_framework-0.0.8/src/cnn_framework/utils/losses/info_nce_loss.py
--rw-rw-rw-   0        0        0      364 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/losses/jaccard_loss.py
--rw-rw-rw-   0        0        0     1044 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/losses/loss_manager.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.145935 cnn_framework-0.0.8/src/cnn_framework/utils/lr_schedulers/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:11.000000 cnn_framework-0.0.8/src/cnn_framework/utils/lr_schedulers/__init__.py
--rw-rw-rw-   0        0        0     6254 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/lr_schedulers/linear_warmup_cosine_annealing_lr.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.180408 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/
--rw-rw-rw-   0        0        0        0 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/__init__.py
--rw-rw-rw-   0        0        0      531 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/abstract_metric.py
--rw-rw-rw-   0        0        0     1408 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/classification_accuracy.py
--rw-rw-rw-   0        0        0      683 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/mean_error_metric.py
--rw-rw-rw-   0        0        0      703 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/mean_squared_error_metric.py
--rw-rw-rw-   0        0        0      645 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/pcc.py
--rw-rw-rw-   0        0        0     1066 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/metrics/positive_pair_matching_metric.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.222898 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:16.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/__init__.py
--rw-rw-rw-   0        0        0     4186 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/cnn_model_manager.py
--rw-rw-rw-   0        0        0     4275 2023-09-28 10:20:04.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/contrastive_model_manager.py
--rw-rw-rw-   0        0        0     3912 2023-10-05 13:11:34.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/custom_get_encoder.py
--rw-rw-rw-   0        0        0    23828 2023-10-20 09:33:29.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/model_manager.py
--rw-rw-rw-   0        0        0     3849 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/regression_model_manager.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.241898 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/utils/
--rw-rw-rw-   0        0        0        0 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/utils/__init__.py
--rw-rw-rw-   0        0        0     3874 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/utils/custom_get_encoder.py
--rw-rw-rw-   0        0        0     1371 2023-11-08 10:12:25.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/utils/training_information.py
--rw-rw-rw-   0        0        0     6345 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/vae_model_manager.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.258899 cnn_framework-0.0.8/src/cnn_framework/utils/model_params/
--rw-rw-rw-   0        0        0        0 2023-10-06 10:49:27.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_params/__init__.py
--rw-rw-rw-   0        0        0    11509 2023-10-20 12:17:07.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_params/base_model_params.py
--rw-rw-rw-   0        0        0     2443 2023-10-20 09:33:53.000000 cnn_framework-0.0.8/src/cnn_framework/utils/model_params/vae_model_params.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.267898 cnn_framework-0.0.8/src/cnn_framework/utils/optimizers/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:19.000000 cnn_framework-0.0.8/src/cnn_framework/utils/optimizers/__init__.py
--rw-rw-rw-   0        0        0     6333 2023-09-28 09:43:44.000000 cnn_framework-0.0.8/src/cnn_framework/utils/optimizers/lars.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.287898 cnn_framework-0.0.8/src/cnn_framework/utils/parsers/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:23.000000 cnn_framework-0.0.8/src/cnn_framework/utils/parsers/__init__.py
--rw-rw-rw-   0        0        0     3315 2023-10-20 09:58:51.000000 cnn_framework-0.0.8/src/cnn_framework/utils/parsers/cnn_parser.py
--rw-rw-rw-   0        0        0      327 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/parsers/transfer_parser.py
--rw-rw-rw-   0        0        0      981 2023-09-27 15:09:57.000000 cnn_framework-0.0.8/src/cnn_framework/utils/parsers/vae_parser.py
--rw-rw-rw-   0        0        0     2529 2023-08-31 10:20:57.000000 cnn_framework-0.0.8/src/cnn_framework/utils/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.320898 cnn_framework-0.0.8/src/cnn_framework/utils/readers/
--rw-rw-rw-   0        0        0        0 2023-08-31 15:43:36.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-10-23 12:18:07.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/abstract_reader.py
--rw-rw-rw-   0        0        0     4621 2023-09-05 10:11:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/ciz_reader.py
--rw-rw-rw-   0        0        0     2389 2023-10-19 16:12:10.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/images_reader.py
--rw-rw-rw-   0        0        0     1775 2023-09-06 08:54:17.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/png_reader.py
--rw-rw-rw-   0        0        0     3401 2023-10-20 07:49:47.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/tiff_reader.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:15.333898 cnn_framework-0.0.8/src/cnn_framework/utils/readers/utils/
--rw-rw-rw-   0        0        0        0 2023-10-06 10:49:14.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/utils/__init__.py
--rw-rw-rw-   0        0        0      170 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/utils/normalization.py
--rw-rw-rw-   0        0        0      357 2023-09-18 08:10:40.000000 cnn_framework-0.0.8/src/cnn_framework/utils/readers/utils/projection.py
--rw-rw-rw-   0        0        0     3298 2023-08-31 11:50:10.000000 cnn_framework-0.0.8/src/cnn_framework/utils/tools.py
-drwxrwxrwx   0        0        0        0 2023-11-08 13:50:14.918932 cnn_framework-0.0.8/src/cnn_framework.egg-info/
--rw-rw-rw-   0        0        0     1888 2023-11-08 13:50:14.000000 cnn_framework-0.0.8/src/cnn_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4393 2023-11-08 13:50:14.000000 cnn_framework-0.0.8/src/cnn_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-08 13:50:14.000000 cnn_framework-0.0.8/src/cnn_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      243 2023-11-08 13:50:14.000000 cnn_framework-0.0.8/src/cnn_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-11-08 13:50:14.000000 cnn_framework-0.0.8/src/cnn_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.511098 cnn_framework-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.483097 cnn_framework-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-11-24 11:05:01.507097 cnn_framework-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.487097 cnn_framework-0.0.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/scripts/dummy_cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_cnn/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_cnn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/scripts/dummy_regression_cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_regression_cnn/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_regression_cnn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/scripts/dummy_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_segmentation/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_segmentation/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/scripts/dummy_sim_clr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_sim_clr/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_sim_clr/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/scripts/dummy_vae_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/scripts/dummy_vae_model/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-11-24 11:05:01.511098 cnn_framework-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.487097 cnn_framework-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/src/cnn_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/src/cnn_framework/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/_tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/_tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-24 11:05:01.000000 cnn_framework-0.0.9/src/cnn_framework/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.491097 cnn_framework-0.0.9/src/cnn_framework/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/data/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.495097 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.495097 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.495097 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.495097 cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/model_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.499097 cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/model_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.499097 cnn_framework-0.0.9/src/cnn_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/create_dummy_data_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.499097 cnn_framework-0.0.9/src/cnn_framework/utils/data_loader_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_loader_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_loader_generators/classifier_data_loader_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_loader_generators/data_loader_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.499097 cnn_framework-0.0.9/src/cnn_framework/utils/data_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_managers/abstract_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_managers/default_data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.499097 cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/abstract_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/dataset_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/detection_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/display_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.499097 cnn_framework-0.0.9/src/cnn_framework/utils/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/info_nce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/jaccard_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/loss_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/losses/ssim_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.503097 cnn_framework-0.0.9/src/cnn_framework/utils/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/lr_schedulers/linear_warmup_cosine_annealing_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.503097 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/abstract_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/classification_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/mean_error_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/mean_squared_error_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/pcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/metrics/positive_pair_matching_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.503097 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/cnn_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/contrastive_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/custom_get_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25931 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/regression_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.503097 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/utils/custom_get_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/utils/training_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/vae_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.503097 cnn_framework-0.0.9/src/cnn_framework/utils/model_params/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_params/base_model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/model_params/vae_model_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.503097 cnn_framework-0.0.9/src/cnn_framework/utils/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/optimizers/lars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.507097 cnn_framework-0.0.9/src/cnn_framework/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/parsers/cnn_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/parsers/transfer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/parsers/vae_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.507097 cnn_framework-0.0.9/src/cnn_framework/utils/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/abstract_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/ciz_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/images_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/png_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/tiff_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.507097 cnn_framework-0.0.9/src/cnn_framework/utils/readers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/utils/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/readers/utils/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/src/cnn_framework/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.507097 cnn_framework-0.0.9/src/cnn_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-11-24 11:05:01.000000 cnn_framework-0.0.9/src/cnn_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-11-24 11:05:01.000000 cnn_framework-0.0.9/src/cnn_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-24 11:05:01.000000 cnn_framework-0.0.9/src/cnn_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-24 11:05:01.000000 cnn_framework-0.0.9/src/cnn_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-24 11:05:01.000000 cnn_framework-0.0.9/src/cnn_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 11:05:01.507097 cnn_framework-0.0.9/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   179142 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/tutorials/classification.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/tutorials/contrastive_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   141922 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/tutorials/regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    79058 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/tutorials/segmentation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    71826 2023-11-24 11:04:43.000000 cnn_framework-0.0.9/tutorials/vae.ipynb
```

### Comparing `cnn_framework-0.0.8/LICENSE` & `cnn_framework-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Copyright (c) 2023, Thomas Bonte
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-- Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-- Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-- Neither the name of copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2023, Thomas Bonte
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+- Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+- Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+- Neither the name of copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `cnn_framework-0.0.8/PKG-INFO` & `cnn_framework-0.0.9/src/cnn_framework.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,84 @@
-Metadata-Version: 2.1
-Name: cnn_framework
-Version: 0.0.8
-Summary: CNN framework
-Home-page: https://https://github.com/15bonte/cnn_framework
-Author: Thomas Bonte
-Author-email: thomas.bonte@mines-paristech.fr
-Project-URL: Bug Tracker, https://https://github.com/15bonte/cnn_framework/issues
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=1.12.1
-Requires-Dist: scikit-image>=0.19.3
-Requires-Dist: matplotlib
-Requires-Dist: scikit-learn>=1.2.2
-Requires-Dist: pint>=0.19.2
-Requires-Dist: torchvision>=0.13.1
-Requires-Dist: albumentations==1.3.0
-Requires-Dist: torchmetrics>=0.11.4
-Requires-Dist: big-fish>=0.6.2
-Requires-Dist: pillow>=9.2.0
-Requires-Dist: segmentation-models-pytorch>=0.3.0
-Requires-Dist: protobuf==3.20.*
-Requires-Dist: tensorboard==2.8.0
-
-# CNN framework
-
-Run CNN models for classification, regression, segmentation, VAE, contrastive learning with any data set.
-
-## Installation
-
-First, create a dedicated conda environment using Python 3.9
-
-```bash
-conda create -n cnn_framework python=3.9
-conda activate cnn_framework
-```
-
-To install the latest github version of this library run the following using pip
-
-```bash
-pip install git+https://github.com/15bonte/cnn_framework
-```
-
-or alternatively you can clone the github repository
-
-```bash
-git clone https://github.com/15bonte/cnn_framework.git
-cd cnn_framework
-pip install -e .
-```
-
-If you want to run jupyter tutorials, you also need to install ipykernel
-
-```bash
-pip install ipykernel
-```
-
-If you want to work with VAE, you must also install [Pythae](https://github.com/clementchadebec/benchmark_VAE/tree/main) and [WandB](https://wandb.ai/home), which is not the case by default.
-
-```bash
-pip install pythae
-```
-
-```bash
-pip install wandb
-```
+Metadata-Version: 2.1
+Name: cnn-framework
+Version: 0.0.9
+Summary: CNN framework
+Home-page: https://github.com/15bonte/cnn_framework
+Author: Thomas Bonte
+Author-email: thomas.bonte@mines-paristech.fr
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/15bonte/cnn_detector/issues
+Project-URL: Documentation, https://github.com/15bonte/cnn_detector#README.md
+Project-URL: Source Code, https://github.com/15bonte/cnn_detector
+Project-URL: User Support, https://github.com/15bonte/cnn_detector/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch>=1.12.1
+Requires-Dist: scikit-image>=0.19.3
+Requires-Dist: matplotlib
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: pint>=0.19.2
+Requires-Dist: torchvision>=0.13.1
+Requires-Dist: albumentations==1.3.0
+Requires-Dist: torchmetrics>=0.11.4
+Requires-Dist: big-fish>=0.6.2
+Requires-Dist: pillow>=9.2.0
+Requires-Dist: segmentation-models-pytorch>=0.3.0
+Requires-Dist: protobuf==3.20.*
+Requires-Dist: tensorboard==2.8.0
+Requires-Dist: aicsimageio>=4.12.1
+Requires-Dist: tensorflow==2.8.0
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
+
+# CNN framework
+
+[![codecov](https://codecov.io/gh/15bonte/cnn_framework/branch/main/graph/badge.svg)](https://codecov.io/gh/15bonte/cnn_framework)
+[![tests](https://github.com/15bonte/cnn_framework/workflows/tests/badge.svg)](https://github.com/15bonte/cnn_framework/actions)
+
+Run CNN models for classification, regression, segmentation, VAE, contrastive learning with any data set.
+
+## Installation
+
+First, create a dedicated conda environment using Python 3.9
+
+```bash
+conda create -n cnn_framework python=3.9
+conda activate cnn_framework
+```
+
+To install the latest github version of this library run the following using pip
+
+```bash
+pip install git+https://github.com/15bonte/cnn_framework
+```
+
+or alternatively you can clone the github repository
+
+```bash
+git clone https://github.com/15bonte/cnn_framework.git
+cd cnn_framework
+pip install -e .
+```
+
+If you want to run jupyter tutorials, you also need to install ipykernel
+
+```bash
+pip install ipykernel
+```
+
+If you want to work with VAE, you must also install [Pythae](https://github.com/clementchadebec/benchmark_VAE/tree/main) and [WandB](https://wandb.ai/home), which is not the case by default.
+
+```bash
+pip install pythae
+```
+
+```bash
+pip install wandb
+```
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_cnn/data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_cnn/data_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,70 @@
-import albumentations as A
-
-from ..utils.readers.utils.projection import Projection
-from ..utils.readers.images_reader import ImagesReader
-from ..utils.data_sets.abstract_data_set import AbstractDataSet
-from ..utils.data_sets.dataset_output import DatasetOutput
-from ..utils.enum import ProjectMethods
-
-
-class DummyCnnDataSet(AbstractDataSet):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Data sources
-        self.input_data_source = ImagesReader(
-            [self.data_manager.get_microscopy_image_path],
-            [[Projection(method=ProjectMethods.Channel, channels=self.params.c_indexes, axis=2)]],
-        )
-
-    def set_transforms(self):
-        height, width = self.params.input_dimensions.to_tuple(False)
-        if self.is_train:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                    A.Rotate(border_mode=0, p=1, value=1),
-                    A.HorizontalFlip(p=0.5),
-                    A.VerticalFlip(p=0.5),
-                    A.GaussianBlur(),
-                ]
-            )
-        else:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        mean=self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                ]
-            )
-
-    def generate_raw_images(self, filename):
-        # Output
-        probabilities = self.read_output(filename)
-
-        return DatasetOutput(
-            input=self.input_data_source.get_image(filename, axis_to_merge=2),
-            target_array=probabilities,
-        )
+import albumentations as A
+
+from ..utils.readers.utils.projection import Projection
+from ..utils.readers.images_reader import ImagesReader
+from ..utils.data_sets.abstract_data_set import AbstractDataSet
+from ..utils.data_sets.dataset_output import DatasetOutput
+from ..utils.enum import ProjectMethods
+
+
+class DummyCnnDataSet(AbstractDataSet):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Data sources
+        self.input_data_source = ImagesReader(
+            [self.data_manager.get_microscopy_image_path],
+            [
+                [
+                    Projection(
+                        method=ProjectMethods.Channel,
+                        channels=self.params.c_indexes,
+                        axis=-1,
+                    )
+                ]
+            ],
+        )
+
+    def set_transforms(self):
+        height, width = self.params.input_dimensions.to_tuple(False)
+        if self.is_train:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                    A.Rotate(border_mode=0, p=1, value=1),
+                    A.HorizontalFlip(p=0.5),
+                    A.VerticalFlip(p=0.5),
+                    A.GaussianBlur(),
+                ]
+            )
+        else:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        mean=self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                ]
+            )
+
+    def generate_raw_images(self, filename):
+        # Output
+        probabilities = self.read_output(filename)
+
+        return DatasetOutput(
+            input=self.input_data_source.get_image(filename, axis_to_merge=-1),
+            target_array=probabilities,
+        )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_regression_cnn/data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_regression_cnn/data_set.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,75 @@
-import albumentations as A
-import numpy as np
-
-from ..utils.readers.utils.projection import Projection
-from ..utils.data_sets.abstract_data_set import AbstractDataSet
-from ..utils.readers.images_reader import ImagesReader
-from ..utils.data_sets.dataset_output import DatasetOutput
-from ..utils.enum import ProjectMethods
-
-
-class DummyRegressionCnnDataSet(AbstractDataSet):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Data sources
-        self.input_data_source = ImagesReader(
-            [self.data_manager.get_microscopy_image_path],
-            [[Projection(method=ProjectMethods.Channel, channels=self.params.c_indexes, axis=2)]],
-        )
-
-    def set_transforms(self):
-        height, width = self.params.input_dimensions.to_tuple(False)
-        if self.is_train:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                    # A.Rotate(border_mode=0, p=1, value=1),
-                    A.HorizontalFlip(p=0.5),
-                    A.VerticalFlip(p=0.5),
-                    A.GaussianBlur(),
-                ]
-            )
-        else:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        mean=self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                ]
-            )
-
-    def generate_raw_images(self, filename):
-        # Output
-        input_image = self.input_data_source.get_image(filename, axis_to_merge=2)
-        non_zero_area = np.count_nonzero(input_image) / 3
-
-        return DatasetOutput(
-            input=input_image,
-            target_array=np.array([non_zero_area]),
-            additional=self.additional_data_source.get_image(filename, axis_to_merge=2),
-        )
+import albumentations as A
+import numpy as np
+
+from ..utils.readers.utils.projection import Projection
+from ..utils.data_sets.abstract_data_set import AbstractDataSet
+from ..utils.readers.images_reader import ImagesReader
+from ..utils.data_sets.dataset_output import DatasetOutput
+from ..utils.enum import ProjectMethods
+
+
+class DummyRegressionCnnDataSet(AbstractDataSet):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Data sources
+        self.input_data_source = ImagesReader(
+            [self.data_manager.get_microscopy_image_path],
+            [
+                [
+                    Projection(
+                        method=ProjectMethods.Channel,
+                        channels=self.params.c_indexes,
+                        axis=-1,
+                    )
+                ]
+            ],
+        )
+
+    def set_transforms(self):
+        height, width = self.params.input_dimensions.to_tuple(False)
+        if self.is_train:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                    # A.Rotate(border_mode=0, p=1, value=1),
+                    A.HorizontalFlip(p=0.5),
+                    A.VerticalFlip(p=0.5),
+                    A.GaussianBlur(),
+                ]
+            )
+        else:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        mean=self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                ]
+            )
+
+    def generate_raw_images(self, filename):
+        # Output
+        input_image = self.input_data_source.get_image(filename, axis_to_merge=-1)
+        non_zero_area = np.count_nonzero(input_image) / 3
+
+        return DatasetOutput(
+            input=input_image,
+            target_array=np.array([non_zero_area]),
+            additional=self.additional_data_source.get_image(
+                filename, axis_to_merge=-1
+            ),
+        )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/data_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,80 @@
-import albumentations as A
-
-from ..utils.readers.utils.projection import Projection
-from ..utils.data_sets.dataset_output import DatasetOutput
-from ..utils.enum import ProjectMethods
-from ..utils.data_sets.abstract_data_set import AbstractDataSet
-from ..utils.readers.images_reader import ImagesReader
-
-
-class DummyDataSet(AbstractDataSet):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Data sources
-        self.input_data_source = ImagesReader(
-            [self.data_manager.get_microscopy_image_path],
-            [[Projection(method=ProjectMethods.Channel, channels=[0, 1, 2], axis=2)]],
-        )
-
-        # First channel is always 255
-        self.output_data_source = ImagesReader(
-            [self.data_manager.get_microscopy_image_path],
-            [[Projection(method=ProjectMethods.Channel, channels=[0], axis=2)]],
-        )
-
-    def set_transforms(self):
-        height, width = self.params.input_dimensions.to_tuple(False)
-        if self.is_train:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                    A.Rotate(border_mode=0),
-                    A.HorizontalFlip(),
-                    A.VerticalFlip(),
-                ]
-            )
-        else:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                ]
-            )
-
-    def generate_raw_images(self, filename):
-        return DatasetOutput(
-            input=self.input_data_source.get_image(filename, axis_to_merge=2),
-            target_image=self.output_data_source.get_image(filename, axis_to_merge=2),
-        )
+import albumentations as A
+
+from ..utils.readers.utils.projection import Projection
+from ..utils.data_sets.dataset_output import DatasetOutput
+from ..utils.enum import ProjectMethods
+from ..utils.data_sets.abstract_data_set import AbstractDataSet
+from ..utils.readers.images_reader import ImagesReader
+
+
+class DummyDataSet(AbstractDataSet):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Data sources
+        self.input_data_source = ImagesReader(
+            [self.data_manager.get_microscopy_image_path],
+            [
+                [
+                    Projection(
+                        method=ProjectMethods.Channel,
+                        channels=self.params.c_indexes,
+                        axis=-1,
+                    )
+                ]
+            ],
+        )
+
+        # First channel is always 255
+        self.output_data_source = ImagesReader(
+            [self.data_manager.get_microscopy_image_path],
+            [
+                [
+                    Projection(
+                        method=ProjectMethods.Channel,
+                        channels=[0],
+                        axis=-1,
+                    )
+                ]
+            ],
+        )
+
+    def set_transforms(self):
+        height, width = self.params.input_dimensions.to_tuple(False)
+        if self.is_train:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                    A.Rotate(border_mode=0),
+                    A.HorizontalFlip(),
+                    A.VerticalFlip(),
+                ]
+            )
+        else:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                ]
+            )
+
+    def generate_raw_images(self, filename):
+        return DatasetOutput(
+            input=self.input_data_source.get_image(filename, axis_to_merge=-1),
+            target_image=self.output_data_source.get_image(filename, axis_to_merge=-1),
+        )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_segmentation/model.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_segmentation/model.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import segmentation_models_pytorch as smp
-
-
-class UNet(smp.Unet):
-    def __init__(self, nb_classes, nb_input_channels):
-        super().__init__(
-            encoder_name="resnet18",  # choose encoder, e.g. mobilenet_v2 or efficientnet-b7
-            encoder_weights="imagenet",  # use `imagenet` pre-trained weights for encoder initialization
-            in_channels=nb_input_channels,  # model input channels (1 for gray-scale images, 3 for RGB, etc.)
-            classes=nb_classes,  # model output channels (number of classes in your dataset),
-        )
+import segmentation_models_pytorch as smp
+
+
+class UNet(smp.Unet):
+    def __init__(self, nb_classes, nb_input_channels):
+        super().__init__(
+            encoder_name="resnet18",  # choose encoder, e.g. mobilenet_v2 or efficientnet-b7
+            encoder_weights="imagenet",  # use `imagenet` pre-trained weights for encoder initialization
+            in_channels=nb_input_channels,  # model input channels (1 for gray-scale images, 3 for RGB, etc.)
+            classes=nb_classes,  # model output channels (number of classes in your dataset),
+        )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/data_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-import albumentations as A
-import numpy as np
-
-from ..utils.data_sets.abstract_data_set import AbstractDataSet
-from ..utils.readers.images_reader import ImagesReader
-from ..utils.data_sets.dataset_output import DatasetOutput
-from ..utils.enum import ProjectMethods
-from ..utils.readers.utils.projection import Projection
-
-
-class SimCLRDataSet(AbstractDataSet):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Data sources
-        self.input_data_source = ImagesReader(
-            [self.data_manager.get_microscopy_image_path],
-            [[Projection(method=ProjectMethods.Channel, channels=self.params.c_indexes, axis=2)]],
-        )
-
-    def set_transforms(self):
-        height, width = self.params.input_dimensions.to_tuple(False)
-        # NB: ColorJitter is is not suited for our dummy data set, but should be used for real data
-        self.transforms = A.Compose(
-            [
-                A.RandomCrop(height=height, width=width, p=1),
-                A.HorizontalFlip(),
-                A.VerticalFlip(),
-                # A.ColorJitter(brightness=0.2, contrast=0.2, saturation=0.2, hue=0.2, p=0.5),
-                A.Normalize(self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1),
-                A.GaussianBlur(),
-            ]
-        )
-
-    def generate_raw_images(self, filename):
-        return DatasetOutput(
-            input=self.input_data_source.get_image(filename, axis_to_merge=2),
-        )
-
-
-class SimCLRDataSetWithoutTransforms(SimCLRDataSet):
-    def set_transforms(self):
-        height, width = self.params.input_dimensions.to_tuple(False)
-        self.transforms = A.Compose(
-            [
-                A.Normalize(self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1),
-                A.CenterCrop(height=height, width=width, p=1),
-            ]
-        )
+import albumentations as A
+import numpy as np
+
+from ..utils.data_sets.abstract_data_set import AbstractDataSet
+from ..utils.readers.images_reader import ImagesReader
+from ..utils.data_sets.dataset_output import DatasetOutput
+from ..utils.enum import ProjectMethods
+from ..utils.readers.utils.projection import Projection
+
+
+class SimCLRDataSet(AbstractDataSet):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Data sources
+        self.input_data_source = ImagesReader(
+            [self.data_manager.get_microscopy_image_path],
+            [
+                [
+                    Projection(
+                        method=ProjectMethods.Channel,
+                        channels=self.params.c_indexes,
+                        axis=-1,
+                    )
+                ]
+            ],
+        )
+
+    def set_transforms(self):
+        height, width = self.params.input_dimensions.to_tuple(False)
+        # NB: ColorJitter is is not suited for our dummy data set, but should be used for real data
+        self.transforms = A.Compose(
+            [
+                A.RandomCrop(height=height, width=width, p=1),
+                A.HorizontalFlip(),
+                A.VerticalFlip(),
+                # A.ColorJitter(brightness=0.2, contrast=0.2, saturation=0.2, hue=0.2, p=0.5),
+                A.Normalize(
+                    self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
+                ),
+                A.GaussianBlur(),
+            ]
+        )
+
+    def generate_raw_images(self, filename):
+        return DatasetOutput(
+            input=self.input_data_source.get_image(filename, axis_to_merge=-1),
+        )
+
+
+class SimCLRDataSetWithoutTransforms(SimCLRDataSet):
+    def set_transforms(self):
+        height, width = self.params.input_dimensions.to_tuple(False)
+        self.transforms = A.Compose(
+            [
+                A.Normalize(
+                    self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
+                ),
+                A.CenterCrop(height=height, width=width, p=1),
+            ]
+        )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_sim_clr/model.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_sim_clr/model.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import torch.nn as nn
-from torchvision.models import resnet50, ResNet50_Weights
-
-
-class ResNetSimCLR(nn.Module):
-    """
-    ResNet backbone with MLP head for SimCLR
-    Here, f outputs a dim_mlp-dim vector and g outputs a out_dim-dim vector in the latent space.
-
-    f is the ResNet without its final fc layer.
-    g is this final fc layer, a MLP with 2 hidden layers.
-    """
-
-    def __init__(self, nb_input_channels, out_dim=128, **kwargs):
-        super().__init__()
-
-        self.backbone = resnet50(weights=ResNet50_Weights.DEFAULT)
-
-        # Modify first layer to accept input channels number
-        self.backbone.conv1 = nn.Conv2d(
-            nb_input_channels, 64, kernel_size=7, stride=2, padding=3, bias=False
-        )
-        # Modify fc to match out_dim
-        dim_mlp = self.backbone.fc.in_features
-        self.backbone.fc = nn.Linear(self.backbone.fc.in_features, out_dim, bias=True)
-
-        # Add mlp projection head
-        self.backbone.fc = nn.Sequential(nn.Linear(dim_mlp, dim_mlp), nn.ReLU(), self.backbone.fc)
-
-    def forward(self, x):
-        return self.backbone(x)
+import torch.nn as nn
+from torchvision.models import resnet50, ResNet50_Weights
+
+
+class ResNetSimCLR(nn.Module):
+    """
+    ResNet backbone with MLP head for SimCLR
+    Here, f outputs a dim_mlp-dim vector and g outputs a out_dim-dim vector in the latent space.
+
+    f is the ResNet without its final fc layer.
+    g is this final fc layer, a MLP with 2 hidden layers.
+    """
+
+    def __init__(self, nb_input_channels, out_dim=128, **kwargs):
+        super().__init__()
+
+        self.backbone = resnet50(weights=ResNet50_Weights.DEFAULT)
+
+        # Modify first layer to accept input channels number
+        self.backbone.conv1 = nn.Conv2d(
+            nb_input_channels, 64, kernel_size=7, stride=2, padding=3, bias=False
+        )
+        # Modify fc to match out_dim
+        dim_mlp = self.backbone.fc.in_features
+        self.backbone.fc = nn.Linear(self.backbone.fc.in_features, out_dim, bias=True)
+
+        # Add mlp projection head
+        self.backbone.fc = nn.Sequential(nn.Linear(dim_mlp, dim_mlp), nn.ReLU(), self.backbone.fc)
+
+    def forward(self, x):
+        return self.backbone(x)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/data_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,89 @@
-import albumentations as A
-import numpy as np
-
-from pythae.data.datasets import DatasetOutput as DatasetOutputVAE
-
-from ..utils.readers.utils.projection import Projection
-from ..utils.data_sets.dataset_output import DatasetOutput
-from ..utils.enum import ProjectMethods
-from ..utils.data_sets.abstract_data_set import AbstractDataSet
-from ..utils.readers.images_reader import ImagesReader
-
-
-class DummyVAEDataSet(AbstractDataSet):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # Data sources
-        self.input_data_source = ImagesReader(
-            [self.data_manager.get_microscopy_image_path],
-            [[Projection(method=ProjectMethods.Channel, channels=[0, 1, 2], axis=2)]],
-        )
-
-    def set_transforms(self):
-        height, width = self.params.input_dimensions.to_tuple(False)
-        if self.is_train:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                    A.Rotate(border_mode=0),
-                    A.HorizontalFlip(),
-                    A.VerticalFlip(),
-                ]
-            )
-        else:
-            self.transforms = A.Compose(
-                [
-                    A.Normalize(
-                        self.mean_std["mean"], std=self.mean_std["std"], max_pixel_value=1
-                    ),
-                    A.PadIfNeeded(min_height=height, min_width=width, border_mode=0, value=0, p=1),
-                    A.CenterCrop(height=height, width=width, p=1),
-                ]
-            )
-
-    def generate_raw_images(self, filename):
-        return DatasetOutput(
-            input=self.input_data_source.get_image(filename, axis_to_merge=2),
-        )
-
-    def __getitem__(self, idx):
-        # Read file and generate images
-        filename = self.names[idx]
-        raw_inputs = self.generate_raw_images(filename)
-
-        # Category (0 for squares, 1 for circles)
-        one_hot_probabilities = self.read_output(filename, one_hot=True)
-        if np.max(one_hot_probabilities) == 0:
-            category = -1
-        else:
-            category = np.argmax(one_hot_probabilities)
-
-        # Apply transforms
-        self.apply_transforms(raw_inputs)
-
-        return DatasetOutputVAE(
-            data=raw_inputs.input,
-            id=idx,
-            category=category,
-        )
+import albumentations as A
+import numpy as np
+
+from pythae.data.datasets import DatasetOutput as DatasetOutputVAE
+
+from ..utils.readers.utils.projection import Projection
+from ..utils.data_sets.dataset_output import DatasetOutput
+from ..utils.enum import ProjectMethods
+from ..utils.data_sets.abstract_data_set import AbstractDataSet
+from ..utils.readers.images_reader import ImagesReader
+
+
+class DummyVAEDataSet(AbstractDataSet):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Data sources
+        self.input_data_source = ImagesReader(
+            [self.data_manager.get_microscopy_image_path],
+            [
+                [
+                    Projection(
+                        method=ProjectMethods.Channel,
+                        channels=self.params.c_indexes,
+                        axis=-1,
+                    )
+                ]
+            ],
+        )
+
+    def set_transforms(self):
+        height, width = self.params.input_dimensions.to_tuple(False)
+        if self.is_train:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                    A.Rotate(border_mode=0),
+                    A.HorizontalFlip(),
+                    A.VerticalFlip(),
+                ]
+            )
+        else:
+            self.transforms = A.Compose(
+                [
+                    A.Normalize(
+                        self.mean_std["mean"],
+                        std=self.mean_std["std"],
+                        max_pixel_value=1,
+                    ),
+                    A.PadIfNeeded(
+                        min_height=height, min_width=width, border_mode=0, value=0, p=1
+                    ),
+                    A.CenterCrop(height=height, width=width, p=1),
+                ]
+            )
+
+    def generate_raw_images(self, filename):
+        return DatasetOutput(
+            input=self.input_data_source.get_image(filename, axis_to_merge=-1),
+        )
+
+    def __getitem__(self, idx):
+        # Read file and generate images
+        filename = self.names[idx]
+        raw_inputs = self.generate_raw_images(filename)
+
+        # Category (0 for squares, 1 for circles)
+        one_hot_probabilities = self.read_output(filename, one_hot=True)
+        if np.max(one_hot_probabilities) == 0:
+            category = -1
+        else:
+            category = np.argmax(one_hot_probabilities)
+
+        # Apply transforms
+        self.apply_transforms(raw_inputs)
+
+        return DatasetOutputVAE(
+            data=raw_inputs.input,
+            id=idx,
+            category=category,
+        )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/dummy_vae_model/decoder.py` & `cnn_framework-0.0.9/src/cnn_framework/dummy_vae_model/decoder.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import numpy as np
-
-from torch import nn
-import torch
-import torch.nn.functional as F
-
-from segmentation_models_pytorch.base.heads import SegmentationHead
-from segmentation_models_pytorch.base import modules as md
-
-from pythae.models.nn import BaseDecoder
-from pythae.models.base.base_utils import ModelOutput
-
-
-class DecoderBlock(nn.Module):
-    """
-    Inspired by segmentation_models_pytorch
-    """
-
-    def __init__(self, in_channels, out_channels, use_batchnorm):
-        super().__init__()
-        self.conv1 = md.Conv2dReLU(
-            in_channels,
-            out_channels,
-            kernel_size=3,
-            padding=1,
-            use_batchnorm=use_batchnorm,
-        )
-        self.conv2 = md.Conv2dReLU(
-            out_channels,
-            out_channels,
-            kernel_size=3,
-            padding=1,
-            use_batchnorm=use_batchnorm,
-        )
-
-    def forward(self, x):
-        x = F.interpolate(x, scale_factor=2, mode="nearest")
-        x = self.conv1(x)
-        x = self.conv2(x)
-        return x
-
-
-class CustomDecoder(BaseDecoder):
-    def __init__(self, params, args):
-        BaseDecoder.__init__(self)
-
-        self.head_channels = 512
-        out_channels = np.array([256, 128, 64, 32, 16])
-        in_channels = [self.head_channels] + list(out_channels[:-1])
-
-        # Infer size of images after convolutions
-        self.first_square_size = params.input_dimensions.height
-        for _ in range(len(out_channels)):
-            self.first_square_size = self.first_square_size // 2
-
-        self.fc = nn.Linear(
-            args.latent_dim,
-            self.head_channels * self.first_square_size * self.first_square_size,
-        )
-        blocks = [
-            DecoderBlock(in_ch, out_ch, use_batchnorm=True)
-            for in_ch, out_ch in zip(in_channels, out_channels)
-        ]
-        self.blocks = nn.ModuleList(blocks)
-
-        # Reconstruction
-        self.segmentation_head = SegmentationHead(
-            in_channels=out_channels[-1],
-            out_channels=len(params.c_indexes) * len(params.z_indexes),
-            activation=None,
-            kernel_size=3,
-        )
-
-    def forward(self, z: torch.Tensor):
-        x = self.fc(z).reshape(
-            z.shape[0], self.head_channels, self.first_square_size, self.first_square_size
-        )
-
-        for decoder_block in self.blocks:
-            x = decoder_block(x)
-
-        reconstruction = self.segmentation_head(x)
-        output = ModelOutput(reconstruction=reconstruction)
-
-        return output
+import numpy as np
+
+from torch import nn
+import torch
+import torch.nn.functional as F
+
+from segmentation_models_pytorch.base.heads import SegmentationHead
+from segmentation_models_pytorch.base import modules as md
+
+from pythae.models.nn import BaseDecoder
+from pythae.models.base.base_utils import ModelOutput
+
+
+class DecoderBlock(nn.Module):
+    """
+    Inspired by segmentation_models_pytorch
+    """
+
+    def __init__(self, in_channels, out_channels, use_batchnorm):
+        super().__init__()
+        self.conv1 = md.Conv2dReLU(
+            in_channels,
+            out_channels,
+            kernel_size=3,
+            padding=1,
+            use_batchnorm=use_batchnorm,
+        )
+        self.conv2 = md.Conv2dReLU(
+            out_channels,
+            out_channels,
+            kernel_size=3,
+            padding=1,
+            use_batchnorm=use_batchnorm,
+        )
+
+    def forward(self, x):
+        x = F.interpolate(x, scale_factor=2, mode="nearest")
+        x = self.conv1(x)
+        x = self.conv2(x)
+        return x
+
+
+class CustomDecoder(BaseDecoder):
+    def __init__(self, params, args):
+        BaseDecoder.__init__(self)
+
+        self.head_channels = 512
+        out_channels = np.array([256, 128, 64, 32, 16])
+        in_channels = [self.head_channels] + list(out_channels[:-1])
+
+        # Infer size of images after convolutions
+        self.first_square_size = params.input_dimensions.height
+        for _ in range(len(out_channels)):
+            self.first_square_size = self.first_square_size // 2
+
+        self.fc = nn.Linear(
+            args.latent_dim,
+            self.head_channels * self.first_square_size * self.first_square_size,
+        )
+        blocks = [
+            DecoderBlock(in_ch, out_ch, use_batchnorm=True)
+            for in_ch, out_ch in zip(in_channels, out_channels)
+        ]
+        self.blocks = nn.ModuleList(blocks)
+
+        # Reconstruction
+        self.segmentation_head = SegmentationHead(
+            in_channels=out_channels[-1],
+            out_channels=len(params.c_indexes) * len(params.z_indexes),
+            activation=None,
+            kernel_size=3,
+        )
+
+    def forward(self, z: torch.Tensor):
+        x = self.fc(z).reshape(
+            z.shape[0], self.head_channels, self.first_square_size, self.first_square_size
+        )
+
+        for decoder_block in self.blocks:
+            x = decoder_block(x)
+
+        reconstruction = self.segmentation_head(x)
+        output = ModelOutput(reconstruction=reconstruction)
+
+        return output
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/create_dummy_data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/create_dummy_data_set.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import os
-import warnings
-import numpy as np
-from skimage import io
-
-
-def generate_square(image_size, nb_channels, color):
-    # Create black image with square in the middle
-    image = np.zeros((image_size, image_size, nb_channels), dtype=np.uint8)
-
-    # Square
-    square_size = np.random.randint(2 * image_size / 5, 2 * image_size / 3)
-
-    # Top left random corner
-    random_x = np.random.randint(0, image_size - square_size)
-    random_y = np.random.randint(0, image_size - square_size)
-
-    if color is None:
-        # First channel is always 255 as it is used for segmentation
-        color = [255, np.random.randint(0, 255), np.random.randint(0, 255)]
-
-    image[
-        random_y : random_y + square_size,
-        random_x : random_x + square_size,
-        :,
-    ] = [255, np.random.randint(0, 255), np.random.randint(0, 255)]
-
-    return image
-
-
-def generate_circle(image_size, nb_channels, color):
-    # Create black image with circle in the middle
-    image = np.zeros((image_size, image_size, nb_channels), dtype=np.uint8)
-
-    # Circle
-
-    # Radius
-    radius = np.random.randint(image_size / 5, image_size / 3)
-
-    # Center
-    center_x = np.random.randint(radius, image_size - radius)
-    center_y = np.random.randint(radius, image_size - radius)
-
-    if color is None:
-        color = [255, np.random.randint(0, 255), np.random.randint(0, 255)]
-
-    for channel, channel_color in enumerate(color):
-        image[:, :, channel] = channel_color
-        for x in range(image_size):
-            for y in range(image_size):
-                if (x - center_x) ** 2 + (y - center_y) ** 2 > radius**2:
-                    image[y, x, channel] = 0
-
-    return image
-
-
-def generate_data_set(
-    save_dir,
-    image_size=128,
-    nb_channels=3,
-    nb_elements_per_class=100,
-    extension="tiff",
-    same_color=False,  # if True, square are all yellow and circle are all purple, if False, random colors
-):
-    # Create save_dir if it does not exist
-    if not os.path.exists(save_dir):
-        os.makedirs(save_dir)
-
-    for idx in range(nb_elements_per_class):
-        square_image = generate_square(
-            image_size, nb_channels, color=[255, 255, 0] if same_color else None
-        )
-        # Save image without warnings
-        with warnings.catch_warnings():
-            warnings.filterwarnings(action="ignore", category=UserWarning)
-            io.imsave(f"{save_dir}/random_{idx}_c0.{extension}", square_image)
-
-        circle_image = generate_circle(
-            image_size, nb_channels, color=[255, 0, 255] if same_color else None
-        )
-        with warnings.catch_warnings():
-            warnings.filterwarnings(action="ignore", category=UserWarning)
-            io.imsave(f"{save_dir}/random_{idx}_c1.{extension}", circle_image)
+import os
+import warnings
+import numpy as np
+from skimage import io
+
+
+def generate_square(image_size, nb_channels, color):
+    # Create black image with square in the middle
+    image = np.zeros((image_size, image_size, nb_channels), dtype=np.uint8)
+
+    # Square
+    square_size = np.random.randint(2 * image_size / 5, 2 * image_size / 3)
+
+    # Top left random corner
+    random_x = np.random.randint(0, image_size - square_size)
+    random_y = np.random.randint(0, image_size - square_size)
+
+    if color is None:
+        # First channel is always 255 as it is used for segmentation
+        color = [255, np.random.randint(0, 255), np.random.randint(0, 255)]
+
+    image[
+        random_y : random_y + square_size,
+        random_x : random_x + square_size,
+        :,
+    ] = [255, np.random.randint(0, 255), np.random.randint(0, 255)]
+
+    return image
+
+
+def generate_circle(image_size, nb_channels, color):
+    # Create black image with circle in the middle
+    image = np.zeros((image_size, image_size, nb_channels), dtype=np.uint8)
+
+    # Circle
+
+    # Radius
+    radius = np.random.randint(image_size / 5, image_size / 3)
+
+    # Center
+    center_x = np.random.randint(radius, image_size - radius)
+    center_y = np.random.randint(radius, image_size - radius)
+
+    if color is None:
+        color = [255, np.random.randint(0, 255), np.random.randint(0, 255)]
+
+    for channel, channel_color in enumerate(color):
+        image[:, :, channel] = channel_color
+        for x in range(image_size):
+            for y in range(image_size):
+                if (x - center_x) ** 2 + (y - center_y) ** 2 > radius**2:
+                    image[y, x, channel] = 0
+
+    return image
+
+
+def generate_data_set(
+    save_dir,
+    image_size=32,
+    nb_channels=3,
+    nb_elements_per_class=1000,
+    extension="tiff",
+    same_color=False,  # if True, square are all yellow and circle are all purple, if False, random colors
+):
+    # Create save_dir if it does not exist
+    if not os.path.exists(save_dir):
+        os.makedirs(save_dir)
+
+    for idx in range(nb_elements_per_class):
+        square_image = generate_square(
+            image_size, nb_channels, color=[255, 255, 0] if same_color else None
+        )
+        # Save image without warnings
+        with warnings.catch_warnings():
+            warnings.filterwarnings(action="ignore", category=UserWarning)
+            io.imsave(f"{save_dir}/random_{idx}_c0.{extension}", square_image)
+
+        circle_image = generate_circle(
+            image_size, nb_channels, color=[255, 0, 255] if same_color else None
+        )
+        with warnings.catch_warnings():
+            warnings.filterwarnings(action="ignore", category=UserWarning)
+            io.imsave(f"{save_dir}/random_{idx}_c1.{extension}", circle_image)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/data_loader_generators/classifier_data_loader_generator.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/data_loader_generators/classifier_data_loader_generator.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import random
-from collections import Counter
-import numpy as np
-
-from .data_loader_generator import DataLoaderGenerator
-
-
-constant_seeded_rd = random.Random(10)
-
-
-class ClassifierDataLoaderGenerator(DataLoaderGenerator):
-    """
-    Class used to generate data loaders from params and data folder.
-    Specific for CNN classifier.
-    """
-
-    def generate_train_weights(self, data_set_train, data_set_val, data_set_test):
-        """
-        For train, remove all images with label > number of classes, and balance dataset.
-        For val, test, keep as it is.
-        """
-        for set_name, data_set in zip(
-            ["train", "val", "test"], [data_set_train, data_set_val, data_set_test]
-        ):
-            if len(data_set.names) == 0:
-                if set_name == "train":
-                    weights_train = []
-                continue
-            # Create list of class ids
-            class_probabilities = np.array([data_set.read_output(name) for name in data_set.names])
-            class_ids = np.argmax(class_probabilities, axis=1)
-            # Count occurrences/sum of probabilities of each class
-            count = np.sum(class_probabilities, axis=0)
-            # Create weights for each class
-            if set_name == "train":  # oversampling for train set
-                weights_train = [
-                    1.0 / count[class_id] if count[class_id] > 0 else 0 for class_id in class_ids
-                ]
-
-            # Print information
-            count = Counter(class_ids)
-            class_counts = ", ".join(
-                [f"{count[class_id]} images for class {class_id}" for class_id in sorted(count)]
-            )
-            oversampling_message = " (oversampling applied)" if set_name == "train" else ""
-            print(
-                f"{set_name} has {class_counts}, total {len(data_set.names)} images{oversampling_message}"
-            )
-
-        print("###################")
-
-        return weights_train
+import random
+from collections import Counter
+import numpy as np
+
+from .data_loader_generator import DataLoaderGenerator
+
+
+constant_seeded_rd = random.Random(10)
+
+
+class ClassifierDataLoaderGenerator(DataLoaderGenerator):
+    """
+    Class used to generate data loaders from params and data folder.
+    Specific for CNN classifier.
+    """
+
+    def generate_train_weights(self, data_set_train, data_set_val, data_set_test):
+        """
+        For train, remove all images with label > number of classes, and balance dataset.
+        For val, test, keep as it is.
+        """
+        for set_name, data_set in zip(
+            ["train", "val", "test"], [data_set_train, data_set_val, data_set_test]
+        ):
+            if len(data_set.names) == 0:
+                if set_name == "train":
+                    weights_train = []
+                continue
+            # Create list of class ids
+            class_probabilities = np.array([data_set.read_output(name) for name in data_set.names])
+            class_ids = np.argmax(class_probabilities, axis=1)
+            # Count occurrences/sum of probabilities of each class
+            count = np.sum(class_probabilities, axis=0)
+            # Create weights for each class
+            if set_name == "train":  # oversampling for train set
+                weights_train = [
+                    1.0 / count[class_id] if count[class_id] > 0 else 0 for class_id in class_ids
+                ]
+
+            # Print information
+            count = Counter(class_ids)
+            class_counts = ", ".join(
+                [f"{count[class_id]} images for class {class_id}" for class_id in sorted(count)]
+            )
+            oversampling_message = " (oversampling applied)" if set_name == "train" else ""
+            print(
+                f"{set_name} has {class_counts}, total {len(data_set.names)} images{oversampling_message}"
+            )
+
+        print("###################")
+
+        return weights_train
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/data_loader_generators/data_loader_generator.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/data_loader_generators/data_loader_generator.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import numpy as np
-import torch
-from torch.utils.data import DataLoader, WeightedRandomSampler
-from torch.utils.data._utils.collate import default_collate
-
-from ..data_managers.default_data_manager import DefaultDataManager
-from ..model_params.base_model_params import DataSplit
-from ..data_sets.dataset_output import DatasetOutput
-from ..tools import handle_image_type
-
-
-def check_dimensions_order(params, dataset_output):
-    assert dataset_output.input.shape[-1] == len(params.c_indexes) * len(params.z_indexes)
-    if dataset_output.target_is_image():
-        assert dataset_output.target.shape[-1] == params.out_channels
-
-
-def get_mean_and_std(data_loaders):
-    """
-    Args:
-        dataloader: DataLoader with a mil dataset
-
-    Returns:
-        Mean and std of images in dataloader.
-    """
-
-    # Initialize mean and std
-    params = data_loaders[0].dataset.params
-    in_channels = len(params.c_indexes) * len(params.z_indexes)
-    channels = in_channels + params.out_channels
-    channels_sum, channels_squared_sum = np.zeros(channels), np.zeros(channels)
-    num_imgs = 0
-
-    for data_loader in data_loaders:
-        for filename in data_loader.dataset.names:
-            dataset_output = data_loader.dataset.generate_raw_images(filename)  # H, W, C
-            check_dimensions_order(params, dataset_output)
-            img, target = dataset_output.input, dataset_output.target
-            # If target is image, concatenate it to img to compute its mean and std
-            if dataset_output.target_is_image():
-                img = np.concatenate([img, target], axis=-1)
-            # Handle type
-            img = handle_image_type(img)
-            # Cast img to float32 to avoid overflow
-            img = img.astype("float32")
-            channels_sum += np.mean(img, axis=(0, 1))
-            channels_squared_sum += np.mean(np.square(img), axis=(0, 1))
-            num_imgs += 1
-
-    mean = channels_sum / num_imgs
-    std = np.sqrt((channels_squared_sum / num_imgs - np.square(mean)))
-
-    return {"mean": list(mean), "std": list(std)}
-
-
-def collate_dataset_output(batch):
-    """Collate function that treats the `DatasetOutput` class correctly."""
-    if isinstance(batch[0], DatasetOutput):
-        # `default_collate` returns a dict for older versions of PyTorch.
-        return DatasetOutput(**default_collate([element.to_dict() for element in batch]))
-    else:
-        return default_collate(batch)
-
-
-class DataLoaderGenerator:
-    """
-    Class used to generate data loaders from params and data folder.
-    Note DATA_SET_CLASS is related to the MODEL,
-    while the DATA_MANAGER is related to the DATA.
-    """
-
-    def __init__(
-        self,
-        params,
-        data_set_class,
-        data_manager_class=DefaultDataManager,
-        collate_fn=collate_dataset_output,
-    ):
-        self.data_set_class = data_set_class
-        self.data_manager = data_manager_class(params.data_dir)
-        self.params = params
-        self.collate_fn = collate_fn
-
-    def generate_train_weights(self, data_set_train, data_set_val, data_set_test):
-        # Print data sets size
-        for set_name, data_set in zip(
-            ["train", "val", "test"], [data_set_train, data_set_val, data_set_test]
-        ):
-            print(f"{set_name} has {len(data_set.names)} images.")
-
-        print("###################")
-
-        # By default, no oversampling is applied
-        return [1 for _ in data_set_train.names]
-
-    def generate_data_loader(self, single_image_test_batch=False, train_as_test=False):
-        """
-        single_image_test_batch should be set to True to force batch_size=1 for test set.
-        Useful to enable extraction of multi sub images for testing, for detection models.
-
-        If train_as_test is True, train is not shuffled and no augmentation is applied.
-        """
-        files = self.data_manager.get_distinct_files()
-        files.sort()
-
-        data_split = DataSplit(self.params, files)
-        names_train, names_val, names_test = data_split.generate_train_val_test_list(
-            files, self.params.data_dir
-        )
-
-        self.params.names_train = names_train
-        self.params.names_val = names_val
-        self.params.names_test = names_test
-
-        # Data sets
-        dataset_train = self.data_set_class(
-            (not train_as_test), names_train, self.data_manager, self.params
-        )
-        dataset_val = self.data_set_class(False, names_val, self.data_manager, self.params)
-        dataset_test = self.data_set_class(False, names_test, self.data_manager, self.params)
-
-        # Generate weights for train set (i.e. oversampling of some images)
-        weights_train = self.generate_train_weights(dataset_train, dataset_val, dataset_test)
-
-        # Train
-        sampler_train = (
-            WeightedRandomSampler(torch.DoubleTensor(weights_train), len(names_train))
-            if len(names_train) and not train_as_test
-            else None
-        )
-        train_dl = DataLoader(
-            dataset_train,
-            batch_size=self.params.batch_size,
-            sampler=sampler_train,
-            collate_fn=self.collate_fn,
-            num_workers=self.params.num_workers,
-            persistent_workers=True if self.params.num_workers else False,
-            pin_memory=True,
-        )
-
-        # Val
-        val_dl = DataLoader(
-            dataset_val,
-            batch_size=self.params.batch_size,
-            collate_fn=self.collate_fn,
-            num_workers=self.params.num_workers,
-            persistent_workers=True if self.params.num_workers else False,
-            pin_memory=True,
-        )
-
-        # Test (no sampler to keep order)
-        test_dl = DataLoader(
-            dataset_test,
-            batch_size=1 if single_image_test_batch else self.params.batch_size,
-            collate_fn=self.collate_fn,
-            pin_memory=True,
-        )
-
-        return train_dl, val_dl, test_dl
+import numpy as np
+import torch
+from torch.utils.data import DataLoader, WeightedRandomSampler
+from torch.utils.data._utils.collate import default_collate
+
+from ..data_managers.default_data_manager import DefaultDataManager
+from ..model_params.base_model_params import DataSplit
+from ..data_sets.dataset_output import DatasetOutput
+from ..tools import handle_image_type
+
+
+def check_dimensions_order(params, dataset_output):
+    assert dataset_output.input.shape[-1] == len(params.c_indexes) * len(params.z_indexes)
+    if dataset_output.target_is_image():
+        assert dataset_output.target.shape[-1] == params.out_channels
+
+
+def get_mean_and_std(data_loaders):
+    """
+    Args:
+        dataloader: DataLoader with a mil dataset
+
+    Returns:
+        Mean and std of images in dataloader.
+    """
+
+    # Initialize mean and std
+    params = data_loaders[0].dataset.params
+    in_channels = len(params.c_indexes) * len(params.z_indexes)
+    channels = in_channels + params.out_channels
+    channels_sum, channels_squared_sum = np.zeros(channels), np.zeros(channels)
+    num_imgs = 0
+
+    for data_loader in data_loaders:
+        for filename in data_loader.dataset.names:
+            dataset_output = data_loader.dataset.generate_raw_images(filename)  # H, W, C
+            check_dimensions_order(params, dataset_output)
+            img, target = dataset_output.input, dataset_output.target
+            # If target is image, concatenate it to img to compute its mean and std
+            if dataset_output.target_is_image():
+                img = np.concatenate([img, target], axis=-1)
+            # Handle type
+            img = handle_image_type(img)
+            # Cast img to float32 to avoid overflow
+            img = img.astype("float32")
+            channels_sum += np.mean(img, axis=(0, 1))
+            channels_squared_sum += np.mean(np.square(img), axis=(0, 1))
+            num_imgs += 1
+
+    mean = channels_sum / num_imgs
+    std = np.sqrt((channels_squared_sum / num_imgs - np.square(mean)))
+
+    return {"mean": list(mean), "std": list(std)}
+
+
+def collate_dataset_output(batch):
+    """Collate function that treats the `DatasetOutput` class correctly."""
+    if isinstance(batch[0], DatasetOutput):
+        # `default_collate` returns a dict for older versions of PyTorch.
+        return DatasetOutput(**default_collate([element.to_dict() for element in batch]))
+    else:
+        return default_collate(batch)
+
+
+class DataLoaderGenerator:
+    """
+    Class used to generate data loaders from params and data folder.
+    Note DATA_SET_CLASS is related to the MODEL,
+    while the DATA_MANAGER is related to the DATA.
+    """
+
+    def __init__(
+        self,
+        params,
+        data_set_class,
+        data_manager_class=DefaultDataManager,
+        collate_fn=collate_dataset_output,
+    ):
+        self.data_set_class = data_set_class
+        self.data_manager = data_manager_class(params.data_dir)
+        self.params = params
+        self.collate_fn = collate_fn
+
+    def generate_train_weights(self, data_set_train, data_set_val, data_set_test):
+        # Print data sets size
+        for set_name, data_set in zip(
+            ["train", "val", "test"], [data_set_train, data_set_val, data_set_test]
+        ):
+            print(f"{set_name} has {len(data_set.names)} images.")
+
+        print("###################")
+
+        # By default, no oversampling is applied
+        return [1 for _ in data_set_train.names]
+
+    def generate_data_loader(self, single_image_test_batch=False, train_as_test=False):
+        """
+        single_image_test_batch should be set to True to force batch_size=1 for test set.
+        Useful to enable extraction of multi sub images for testing, for detection models.
+
+        If train_as_test is True, train is not shuffled and no augmentation is applied.
+        """
+        files = self.data_manager.get_distinct_files()
+        files.sort()
+
+        data_split = DataSplit(self.params, files)
+        names_train, names_val, names_test = data_split.generate_train_val_test_list(
+            files, self.params.data_dir
+        )
+
+        self.params.names_train = names_train
+        self.params.names_val = names_val
+        self.params.names_test = names_test
+
+        # Data sets
+        dataset_train = self.data_set_class(
+            (not train_as_test), names_train, self.data_manager, self.params
+        )
+        dataset_val = self.data_set_class(False, names_val, self.data_manager, self.params)
+        dataset_test = self.data_set_class(False, names_test, self.data_manager, self.params)
+
+        # Generate weights for train set (i.e. oversampling of some images)
+        weights_train = self.generate_train_weights(dataset_train, dataset_val, dataset_test)
+
+        # Train
+        sampler_train = (
+            WeightedRandomSampler(torch.DoubleTensor(weights_train), len(names_train))
+            if len(names_train) and not train_as_test
+            else None
+        )
+        train_dl = DataLoader(
+            dataset_train,
+            batch_size=self.params.batch_size,
+            sampler=sampler_train,
+            collate_fn=self.collate_fn,
+            num_workers=self.params.num_workers,
+            persistent_workers=True if self.params.num_workers else False,
+            pin_memory=True,
+        )
+
+        # Val
+        val_dl = DataLoader(
+            dataset_val,
+            batch_size=self.params.batch_size,
+            collate_fn=self.collate_fn,
+            num_workers=self.params.num_workers,
+            persistent_workers=True if self.params.num_workers else False,
+            pin_memory=True,
+        )
+
+        # Test (no sampler to keep order)
+        test_dl = DataLoader(
+            dataset_test,
+            batch_size=1 if single_image_test_batch else self.params.batch_size,
+            collate_fn=self.collate_fn,
+            pin_memory=True,
+        )
+
+        return train_dl, val_dl, test_dl
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/abstract_data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/abstract_data_set.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-from abc import abstractmethod
-from typing import Optional
-
-import numpy as np
-from torch.utils.data import Dataset
-from albumentations import Compose
-
-from ...utils.readers.images_reader import ImagesReader
-from .dataset_output import DatasetOutput
-from ..tools import read_categories_probability_from_name, to_one_hot
-
-
-class AbstractDataSet(Dataset):
-    def __init__(self, is_train, names, data_manager, params):
-        # Is train (not val or test)
-        self.is_train = is_train
-        # Files names
-        self.names = names
-        # Model parameters
-        self.params = params
-        # Data manager
-        self.data_manager = data_manager
-        # Transforms
-        self.transforms: Optional[Compose] = None
-        # Initialize means and standard deviations as None, will be set afterwards
-        self.mean_std = None
-        # Create empty data sources
-        self.input_data_source = ImagesReader()
-        self.output_data_source = ImagesReader()
-        self.additional_data_source = ImagesReader()
-
-    def set_transforms(self):
-        # No transforms
-        pass
-
-    def check_order(self):
-        # Check if order of transforms makes sense
-        transform_names = [transform.__class__.__name__ for transform in self.transforms]
-        # Transform that have to be BEFORE and AFTER Normalize
-        before_normalize = ["ColorJitter", "GaussNoise"]  # because they clip to 0-MAX_TYPE_VALUE
-        after_normalize = ["GaussianBlur", "Rotate", "PadIfNeeded"]
-        # Ignore if Normalize is not in transforms
-        if "Normalize" not in transform_names:
-            return
-        # Check if transforms are in the right order
-        normalize_seen = False
-        for transform in transform_names:
-            if transform == "Normalize":
-                normalize_seen = True
-            if not normalize_seen:
-                assert transform not in after_normalize
-            else:
-                assert transform not in before_normalize
-
-    def initialize_transforms(self):
-        self.set_transforms()
-        self.check_order()
-
-    @abstractmethod
-    def generate_raw_images(self, filename) -> DatasetOutput:
-        raise NotImplementedError
-
-    def read_output(self, filename, one_hot=False):
-        """
-        Used for classification models.
-        Read category and/or probabilities from file name
-        """
-        # Read category from name
-        categories_and_probabilities = filename.split(".")[0].split("_c")[1:]
-        category = int(categories_and_probabilities[0])
-        # Are there probabilities for classes?
-        if len(categories_and_probabilities) > 1 and not one_hot:
-            _, probabilities = read_categories_probability_from_name(filename)
-        else:
-            # Case where class is set to -1
-            probabilities = to_one_hot(category, self.params.nb_classes) if category > -1 else None
-
-        if probabilities is None:
-            return np.zeros(self.params.nb_classes)
-
-        # Length of probabilities has to be equal to number of classes
-        assert self.params.nb_classes == len(probabilities)
-
-        # Category has to be the index of the highest probability
-        assert category == np.argmax(probabilities)
-
-        return np.asarray(probabilities)
-
-    @staticmethod
-    def pass_image(image_x, image_y, image_z):
-        return False
-
-    # shape of inputs in the dataset
-    def __len__(self):
-        return len(self.names)
-
-    def apply_transforms(self, data_set_output: DatasetOutput) -> None:
-        # Transforms are not yet defined
-        if self.transforms is None:
-            return data_set_output
-
-        # No target or additional images
-        if not data_set_output.target_is_image() and not data_set_output.additional_is_image():
-            transformed = self.transforms(image=data_set_output.input)
-            data_set_output.input = np.moveaxis(transformed["image"], 2, 0)
-        # Target and no additional images
-        elif data_set_output.target_is_image() and not data_set_output.additional_is_image():
-            fake_input = np.concatenate((data_set_output.input, data_set_output.target), axis=-1)
-            transformed = self.transforms(image=fake_input)
-            # Split image and target
-            transformed_input = transformed["image"][:, :, : data_set_output.input.shape[-1]]
-            transformed_target = transformed["image"][:, :, data_set_output.input.shape[-1] :]
-            data_set_output.input = np.moveaxis(transformed_input, 2, 0)
-            data_set_output.target = np.moveaxis(transformed_target, 2, 0)
-        # No target and additional images
-        elif not data_set_output.target_is_image() and data_set_output.additional_is_image():
-            transformed = self.transforms(
-                image=data_set_output.input, mask=data_set_output.additional
-            )
-            data_set_output.input = np.moveaxis(transformed["image"], 2, 0)
-            data_set_output.additional = np.moveaxis(transformed["mask"], 2, 0)
-        # Target and additional images
-        elif data_set_output.target_is_image() and data_set_output.additional_is_image():
-            fake_input = np.concatenate((data_set_output.input, data_set_output.target), axis=-1)
-            transformed = self.transforms(image=fake_input, mask=data_set_output.additional)
-            # Split image and target
-            transformed_input = transformed["image"][:, :, : data_set_output.input.shape[-1]]
-            transformed_target = transformed["image"][:, :, data_set_output.input.shape[-1] :]
-            data_set_output.input = np.moveaxis(transformed_input, 2, 0)
-            data_set_output.target = np.moveaxis(transformed_target, 2, 0)
-            data_set_output.additional = np.moveaxis(transformed["mask"], 2, 0)
-
-    def __getitem__(self, idx):
-        # Read file and generate images
-        data_set_output = self.generate_raw_images(self.names[idx])
-
-        # Apply transforms
-        self.apply_transforms(data_set_output)
-        data_set_output.index = idx
-
-        # Set to torch tensors
-        data_set_output.to_torch()
-
-        return data_set_output
+from abc import abstractmethod
+from typing import Optional
+
+import numpy as np
+from torch.utils.data import Dataset
+from albumentations import Compose
+
+from ...utils.readers.images_reader import ImagesReader
+from .dataset_output import DatasetOutput
+from ..tools import read_categories_probability_from_name, to_one_hot
+
+
+class AbstractDataSet(Dataset):
+    def __init__(self, is_train, names, data_manager, params):
+        # Is train (not val or test)
+        self.is_train = is_train
+        # Files names
+        self.names = names
+        # Model parameters
+        self.params = params
+        # Data manager
+        self.data_manager = data_manager
+        # Transforms
+        self.transforms: Optional[Compose] = None
+        # Initialize means and standard deviations as None, will be set afterwards
+        self.mean_std = None
+        # Create empty data sources
+        self.input_data_source = ImagesReader()
+        self.output_data_source = ImagesReader()
+        self.additional_data_source = ImagesReader()
+
+    def set_transforms(self):
+        # No transforms
+        pass
+
+    def check_order(self):
+        # Check if order of transforms makes sense
+        transform_names = [transform.__class__.__name__ for transform in self.transforms]
+        # Transform that have to be BEFORE and AFTER Normalize
+        before_normalize = ["ColorJitter", "GaussNoise"]  # because they clip to 0-MAX_TYPE_VALUE
+        after_normalize = ["GaussianBlur", "Rotate", "PadIfNeeded"]
+        # Ignore if Normalize is not in transforms
+        if "Normalize" not in transform_names:
+            return
+        # Check if transforms are in the right order
+        normalize_seen = False
+        for transform in transform_names:
+            if transform == "Normalize":
+                normalize_seen = True
+            if not normalize_seen:
+                assert transform not in after_normalize
+            else:
+                assert transform not in before_normalize
+
+    def initialize_transforms(self):
+        self.set_transforms()
+        self.check_order()
+
+    @abstractmethod
+    def generate_raw_images(self, filename) -> DatasetOutput:
+        raise NotImplementedError
+
+    def read_output(self, filename, one_hot=False):
+        """
+        Used for classification models.
+        Read category and/or probabilities from file name
+        """
+        # Read category from name
+        categories_and_probabilities = filename.split(".")[0].split("_c")[1:]
+        category = int(categories_and_probabilities[0])
+        # Are there probabilities for classes?
+        if len(categories_and_probabilities) > 1 and not one_hot:
+            _, probabilities = read_categories_probability_from_name(filename)
+        else:
+            # Case where class is set to -1
+            probabilities = to_one_hot(category, self.params.nb_classes) if category > -1 else None
+
+        if probabilities is None:
+            return np.zeros(self.params.nb_classes)
+
+        # Length of probabilities has to be equal to number of classes
+        assert self.params.nb_classes == len(probabilities)
+
+        # Category has to be the index of the highest probability
+        assert category == np.argmax(probabilities)
+
+        return np.asarray(probabilities)
+
+    @staticmethod
+    def pass_image(image_x, image_y, image_z):
+        return False
+
+    # shape of inputs in the dataset
+    def __len__(self):
+        return len(self.names)
+
+    def apply_transforms(self, data_set_output: DatasetOutput) -> None:
+        # Transforms are not yet defined
+        if self.transforms is None:
+            return data_set_output
+
+        # No target or additional images
+        if not data_set_output.target_is_image() and not data_set_output.additional_is_image():
+            transformed = self.transforms(image=data_set_output.input)
+            data_set_output.input = np.moveaxis(transformed["image"], 2, 0)
+        # Target and no additional images
+        elif data_set_output.target_is_image() and not data_set_output.additional_is_image():
+            fake_input = np.concatenate((data_set_output.input, data_set_output.target), axis=-1)
+            transformed = self.transforms(image=fake_input)
+            # Split image and target
+            transformed_input = transformed["image"][:, :, : data_set_output.input.shape[-1]]
+            transformed_target = transformed["image"][:, :, data_set_output.input.shape[-1] :]
+            data_set_output.input = np.moveaxis(transformed_input, 2, 0)
+            data_set_output.target = np.moveaxis(transformed_target, 2, 0)
+        # No target and additional images
+        elif not data_set_output.target_is_image() and data_set_output.additional_is_image():
+            transformed = self.transforms(
+                image=data_set_output.input, mask=data_set_output.additional
+            )
+            data_set_output.input = np.moveaxis(transformed["image"], 2, 0)
+            data_set_output.additional = np.moveaxis(transformed["mask"], 2, 0)
+        # Target and additional images
+        elif data_set_output.target_is_image() and data_set_output.additional_is_image():
+            fake_input = np.concatenate((data_set_output.input, data_set_output.target), axis=-1)
+            transformed = self.transforms(image=fake_input, mask=data_set_output.additional)
+            # Split image and target
+            transformed_input = transformed["image"][:, :, : data_set_output.input.shape[-1]]
+            transformed_target = transformed["image"][:, :, data_set_output.input.shape[-1] :]
+            data_set_output.input = np.moveaxis(transformed_input, 2, 0)
+            data_set_output.target = np.moveaxis(transformed_target, 2, 0)
+            data_set_output.additional = np.moveaxis(transformed["mask"], 2, 0)
+
+    def __getitem__(self, idx):
+        # Read file and generate images
+        data_set_output = self.generate_raw_images(self.names[idx])
+
+        # Apply transforms
+        self.apply_transforms(data_set_output)
+        data_set_output.index = idx
+
+        # Set to torch tensors
+        data_set_output.to_torch()
+
+        return data_set_output
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/dataset_output.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/dataset_output.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from typing import Optional
-import numpy as np
-import torch
-
-from ..tools import torch_from_numpy
-
-
-class DatasetOutput:
-    """
-    Class to handle the output of a dataset.
-    """
-
-    def __init__(
-        self,
-        index: Optional[int] = None,
-        input: Optional[np.array] = None,
-        target_image: Optional[np.array] = None,
-        target_array: Optional[np.array] = None,
-        additional: Optional[np.array] = None,
-        prediction: Optional[np.array] = None,
-    ):
-        self.index = index
-        self.input = input
-
-        # Make sure only one target is specified
-        assert (target_image is None) or (target_array is None)
-
-        self.target_image = target_image
-        self.target_array = target_array
-
-        self.additional = additional
-        self.prediction = prediction
-
-    @property
-    def target(self):
-        return self.target_image if self.target_is_image() else self.target_array
-
-    @target.setter
-    def target(self, new_target: np.array):
-        if self.target_image is not None:
-            self.target_image = new_target
-        else:
-            self.target_array = new_target
-
-    def __getitem__(self, idx):
-        item_dict = {
-            key: value[idx, ...].squeeze()
-            for key, value in self.__dict__.items()
-            if value is not None and key != "target"
-        }
-        return DatasetOutput(**item_dict)
-
-    def to_torch(self) -> None:
-        self.index = torch.tensor(self.index)
-        self.input = torch_from_numpy(self.input)
-        self.target = torch_from_numpy(self.target)
-        self.additional = torch_from_numpy(self.additional)
-        self.prediction = torch_from_numpy(self.prediction)
-
-    def to_dict(self) -> dict:
-        return {
-            key: value
-            for key, value in self.__dict__.items()
-            if value is not None and key != "target"
-        }
-
-    def to_device(self, device) -> None:
-        self.index = self.index.to(device)
-        self.input = self.input.to(device)
-        self.target = self.target.to(device)
-        self.additional = self.additional.to(device) if self.additional_is_image() else None
-        self.prediction = self.prediction.to(device) if self.prediction is not None else None
-
-    def get_numpy_dataset_output(self):
-        numpy_dict = {
-            key: value.detach().cpu().numpy()
-            for key, value in self.__dict__.items()
-            if value is not None and key != "target"
-        }
-        return DatasetOutput(**numpy_dict)
-
-    def target_is_image(self):
-        return self.target_image is not None
-
-    def additional_is_image(self):
-        return self.additional is not None
+from typing import Optional
+import numpy as np
+import torch
+
+from ..tools import torch_from_numpy
+
+
+class DatasetOutput:
+    """
+    Class to handle the output of a dataset.
+    """
+
+    def __init__(
+        self,
+        index: Optional[int] = None,
+        input: Optional[np.array] = None,
+        target_image: Optional[np.array] = None,
+        target_array: Optional[np.array] = None,
+        additional: Optional[np.array] = None,
+        prediction: Optional[np.array] = None,
+    ):
+        self.index = index
+        self.input = input
+
+        # Make sure only one target is specified
+        assert (target_image is None) or (target_array is None)
+
+        self.target_image = target_image
+        self.target_array = target_array
+
+        self.additional = additional
+        self.prediction = prediction
+
+    @property
+    def target(self):
+        return self.target_image if self.target_is_image() else self.target_array
+
+    @target.setter
+    def target(self, new_target: np.array):
+        if self.target_image is not None:
+            self.target_image = new_target
+        else:
+            self.target_array = new_target
+
+    def __getitem__(self, idx):
+        item_dict = {
+            key: value[idx, ...].squeeze()
+            for key, value in self.__dict__.items()
+            if value is not None and key != "target"
+        }
+        return DatasetOutput(**item_dict)
+
+    def to_torch(self) -> None:
+        self.index = torch.tensor(self.index)
+        self.input = torch_from_numpy(self.input)
+        self.target = torch_from_numpy(self.target)
+        self.additional = torch_from_numpy(self.additional)
+        self.prediction = torch_from_numpy(self.prediction)
+
+    def to_dict(self) -> dict:
+        return {
+            key: value
+            for key, value in self.__dict__.items()
+            if value is not None and key != "target"
+        }
+
+    def to_device(self, device) -> None:
+        self.index = self.index.to(device)
+        self.input = self.input.to(device)
+        self.target = self.target.to(device)
+        self.additional = self.additional.to(device) if self.additional_is_image() else None
+        self.prediction = self.prediction.to(device) if self.prediction is not None else None
+
+    def get_numpy_dataset_output(self):
+        numpy_dict = {
+            key: value.detach().cpu().numpy()
+            for key, value in self.__dict__.items()
+            if value is not None and key != "target"
+        }
+        return DatasetOutput(**numpy_dict)
+
+    def target_is_image(self):
+        return self.target_image is not None
+
+    def additional_is_image(self):
+        return self.additional is not None
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/data_sets/detection_data_set.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/data_sets/detection_data_set.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import json
-from abc import abstractmethod
-
-from .abstract_data_set import AbstractDataSet
-
-
-class DetectionDataSet(AbstractDataSet):
-    @abstractmethod
-    def generate_raw_images(self, filename):
-        raise NotImplementedError
-
-    @staticmethod
-    def get_image_id(annotations, filename):  # extension not included
-        for image in annotations["images"]:
-            if image["file_name"] == filename:
-                return image["id"]
-        raise ValueError(f"Image {filename} not found in JSON annotation file.")
-
-    def get_target(self, annotations, image_id):
-        boxes, labels = [], []
-        for annotation in annotations["annotations"]:
-            if annotation["image_id"] != image_id:
-                continue
-            boxes.append(annotation["bbox"])
-            labels.append(annotation["category_id"])
-        return {
-            "boxes": boxes,
-            "labels": labels,
-            "image_id": image_id,
-        }
-
-    def get_image_file_name_from_id(self, image_id):
-        """
-        Returns file name without extension.
-        """
-        bounding_boxes_reader = self.data_manager.get_bounding_boxes_path()
-        json_reader = open(bounding_boxes_reader)
-        annotations = json.load(json_reader)
-
-        # Get image path from image_id
-        for image in annotations["images"]:
-            if image["id"] == image_id:
-                return image["file_name"]
-        raise ValueError(f"Image {image_id} not found in JSON annotation file.")
-
-    def __getitem__(self, idx):
-        _, raw_img_input, raw_img_output, _ = super().__getitem__(idx)
-
-        # Image index and additional data are ignored for train_one_epoch
-        return raw_img_input, raw_img_output
+import json
+from abc import abstractmethod
+
+from .abstract_data_set import AbstractDataSet
+
+
+class DetectionDataSet(AbstractDataSet):
+    @abstractmethod
+    def generate_raw_images(self, filename):
+        raise NotImplementedError
+
+    @staticmethod
+    def get_image_id(annotations, filename):  # extension not included
+        for image in annotations["images"]:
+            if image["file_name"] == filename:
+                return image["id"]
+        raise ValueError(f"Image {filename} not found in JSON annotation file.")
+
+    def get_target(self, annotations, image_id):
+        boxes, labels = [], []
+        for annotation in annotations["annotations"]:
+            if annotation["image_id"] != image_id:
+                continue
+            boxes.append(annotation["bbox"])
+            labels.append(annotation["category_id"])
+        return {
+            "boxes": boxes,
+            "labels": labels,
+            "image_id": image_id,
+        }
+
+    def get_image_file_name_from_id(self, image_id):
+        """
+        Returns file name without extension.
+        """
+        bounding_boxes_reader = self.data_manager.get_bounding_boxes_path()
+        json_reader = open(bounding_boxes_reader)
+        annotations = json.load(json_reader)
+
+        # Get image path from image_id
+        for image in annotations["images"]:
+            if image["id"] == image_id:
+                return image["file_name"]
+        raise ValueError(f"Image {image_id} not found in JSON annotation file.")
+
+    def __getitem__(self, idx):
+        _, raw_img_input, raw_img_output, _ = super().__getitem__(idx)
+
+        # Image index and additional data are ignored for train_one_epoch
+        return raw_img_input, raw_img_output
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/losses/dice_loss.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/losses/dice_loss.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import torch.nn as nn
-
-# Taken from https://www.kaggle.com/code/bigironsphere/loss-function-library-keras-pytorch
-
-
-class DiceLoss(nn.Module):
-    def __init__(self, weight=None, size_average=True):
-        super(DiceLoss, self).__init__()
-
-    def forward(self, inputs, targets, smooth=1):
-
-        # comment out if your model contains a sigmoid or equivalent activation layer
-        # inputs = F.sigmoid(inputs)
-
-        # flatten label and prediction tensors
-        inputs = inputs.reshape(-1)
-        targets = targets.reshape(-1)
-
-        intersection = (inputs * targets).sum()
-        dice = (2.0 * intersection + smooth) / (inputs.sum() + targets.sum() + smooth)
-
-        return 1 - dice
+import torch.nn as nn
+
+# Taken from https://www.kaggle.com/code/bigironsphere/loss-function-library-keras-pytorch
+
+
+class DiceLoss(nn.Module):
+    def __init__(self, weight=None, size_average=True):
+        super(DiceLoss, self).__init__()
+
+    def forward(self, inputs, targets, smooth=1):
+
+        # comment out if your model contains a sigmoid or equivalent activation layer
+        # inputs = F.sigmoid(inputs)
+
+        # flatten label and prediction tensors
+        inputs = inputs.reshape(-1)
+        targets = targets.reshape(-1)
+
+        intersection = (inputs * targets).sum()
+        dice = (2.0 * intersection + smooth) / (inputs.sum() + targets.sum() + smooth)
+
+        return 1 - dice
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/losses/focal_loss.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/losses/focal_loss.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-from typing import Optional
-import torch
-from torch import Tensor
-from torch import nn
-from torch.nn import functional as F
-
-# Taken from https://github.com/AdeelH/pytorch-multi-class-focal-loss/blob/master/focal_loss.py
-
-
-class FocalLossAdeelH(nn.Module):
-    """ Focal Loss, as described in https://arxiv.org/abs/1708.02002.
-    It is essentially an enhancement to cross entropy loss and is
-    useful for classification tasks when there is a large class imbalance.
-    x is expected to contain raw, unnormalized scores for each class.
-    y is expected to contain class labels.
-    Shape:
-        - x: (batch_size, C) or (batch_size, C, d1, d2, ..., dK), K > 0.
-        - y: (batch_size,) or (batch_size, d1, d2, ..., dK), K > 0.
-    """
-
-    def __init__(
-        self,
-        alpha: Optional[Tensor] = None,
-        gamma: float = 0.0,
-        reduction: str = "mean",
-        ignore_index: int = -100,
-    ):
-        """Constructor.
-        Args:
-            alpha (Tensor, optional): Weights for each class. Defaults to None.
-            gamma (float, optional): A constant, as described in the paper.
-                Defaults to 0.
-            reduction (str, optional): 'mean', 'sum' or 'none'.
-                Defaults to 'mean'.
-            ignore_index (int, optional): class label to ignore.
-                Defaults to -100.
-        """
-        if reduction not in ("mean", "sum", "none"):
-            raise ValueError('Reduction must be one of: "mean", "sum", "none".')
-
-        super().__init__()
-        self.alpha = alpha
-        self.gamma = gamma
-        self.ignore_index = ignore_index
-        self.reduction = reduction
-
-        self.nll_loss = nn.NLLLoss(weight=alpha, reduction="none", ignore_index=ignore_index)
-
-    def __repr__(self):
-        arg_keys = ["alpha", "gamma", "ignore_index", "reduction"]
-        arg_vals = [self.__dict__[k] for k in arg_keys]
-        arg_vals = [f"'{v}'" if isinstance(v, str) else v for v in arg_vals]
-        arg_strs = [f"{k}={v}" for k, v in zip(arg_keys, arg_vals)]
-        arg_str = ", ".join(arg_strs)
-        return f"{type(self).__name__}({arg_str})"
-
-    def forward(self, x: Tensor, y: Tensor) -> Tensor:
-        if x.ndim > 2:
-            # (N, C, d1, d2, ..., dK) --> (N * d1 * ... * dK, C)
-            c = x.shape[1]
-            x = x.permute(0, *range(2, x.ndim), 1).reshape(-1, c)
-            # (N, d1, d2, ..., dK) --> (N * d1 * ... * dK,)
-            y = y.view(-1)
-
-        unignored_mask = y != self.ignore_index
-        y = y[unignored_mask]
-        if len(y) == 0:
-            return torch.tensor(0.0)
-        x = x[unignored_mask]
-
-        # compute weighted cross entropy term: -alpha * log(pt)
-        # (alpha is already part of self.nll_loss)
-        log_p = F.log_softmax(x, dim=-1)
-        ce = self.nll_loss(log_p, y)
-
-        # get true class column from each row
-        all_rows = torch.arange(len(x))
-        log_pt = log_p[all_rows, y]
-
-        # compute focal term: (1 - pt)^gamma
-        pt = log_pt.exp()
-        focal_term = (1 - pt) ** self.gamma
-
-        # the full loss: -alpha * ((1 - pt)^gamma) * log(pt)
-        loss = focal_term * ce
-
-        if self.reduction == "mean":
-            loss = loss.mean()
-        elif self.reduction == "sum":
-            loss = loss.sum()
-
-        return loss
-
-
-class FocalLoss(nn.Module):
-    r"""Implementation of the `focal loss <https://arxiv.org/pdf/1708.02002.pdf>`
-    Implements FocalLoss with either probabilities or logits.
-    ----------
-    alpha: float
-        Focal Loss ``alpha`` parameter
-        If negative, balance is ignored.
-    gamma: float
-        Focal Loss ``gamma`` parameter
-    """
-
-    def __init__(self, alpha: float = 0.25, gamma: float = 2.0):
-        super().__init__()
-        self.alpha = alpha
-        self.gamma = gamma
-        self.use_cuda = torch.cuda.is_available()
-
-        self.softmax = nn.Softmax(dim=-1)
-        self.log_soft_max = nn.LogSoftmax(dim=-1)
-
-    def forward(self, scores: Tensor, target: Tensor) -> Tensor:
-        r"""
-        Parameters
-        ----------
-        input: Tensor
-            input tensor with scores
-        target: Tensor
-            target tensor with the actual classes or probabilities
-            B or (B, C)
-        --------
-        """
-
-        # Get useful dimensions
-        num_batch = scores.size(0)
-        num_class = scores.size(1)
-
-        # Convert target to one-hot if necessary
-        if len(target.shape) == 1:
-            target = target.view(-1, 1).squeeze()
-            # Adapt to special case of one batch
-            if num_batch == 1:
-                target = torch.unsqueeze(target, 0)
-            target = torch.eye(num_class)[target]  # B, C
-
-        # Adapt to special case of one batch
-        if num_batch == 1:
-            scores = torch.unsqueeze(scores, 0)
-
-        # Move to GPU if possible
-        if self.use_cuda:
-            target = target.cuda()
-            scores = scores.cuda()
-
-        target = target.contiguous()
-
-        # Compute weights is alpha is positive
-        if self.alpha > 0:
-            balanced_weights = self.alpha * target + (1 - self.alpha) * (1 - target)
-        else:
-            balanced_weights = 1
-
-        probabilities = self.softmax(scores)
-        weights = (balanced_weights * (1 - probabilities).pow(self.gamma)).detach()
-        logs = self.log_soft_max(scores)
-
-        cross_entropy_loss = -weights * logs * target  # B, C
-
-        return torch.sum(cross_entropy_loss) / num_batch
+from typing import Optional
+import torch
+from torch import Tensor
+from torch import nn
+from torch.nn import functional as F
+
+# Taken from https://github.com/AdeelH/pytorch-multi-class-focal-loss/blob/master/focal_loss.py
+
+
+class FocalLossAdeelH(nn.Module):
+    """ Focal Loss, as described in https://arxiv.org/abs/1708.02002.
+    It is essentially an enhancement to cross entropy loss and is
+    useful for classification tasks when there is a large class imbalance.
+    x is expected to contain raw, unnormalized scores for each class.
+    y is expected to contain class labels.
+    Shape:
+        - x: (batch_size, C) or (batch_size, C, d1, d2, ..., dK), K > 0.
+        - y: (batch_size,) or (batch_size, d1, d2, ..., dK), K > 0.
+    """
+
+    def __init__(
+        self,
+        alpha: Optional[Tensor] = None,
+        gamma: float = 0.0,
+        reduction: str = "mean",
+        ignore_index: int = -100,
+    ):
+        """Constructor.
+        Args:
+            alpha (Tensor, optional): Weights for each class. Defaults to None.
+            gamma (float, optional): A constant, as described in the paper.
+                Defaults to 0.
+            reduction (str, optional): 'mean', 'sum' or 'none'.
+                Defaults to 'mean'.
+            ignore_index (int, optional): class label to ignore.
+                Defaults to -100.
+        """
+        if reduction not in ("mean", "sum", "none"):
+            raise ValueError('Reduction must be one of: "mean", "sum", "none".')
+
+        super().__init__()
+        self.alpha = alpha
+        self.gamma = gamma
+        self.ignore_index = ignore_index
+        self.reduction = reduction
+
+        self.nll_loss = nn.NLLLoss(weight=alpha, reduction="none", ignore_index=ignore_index)
+
+    def __repr__(self):
+        arg_keys = ["alpha", "gamma", "ignore_index", "reduction"]
+        arg_vals = [self.__dict__[k] for k in arg_keys]
+        arg_vals = [f"'{v}'" if isinstance(v, str) else v for v in arg_vals]
+        arg_strs = [f"{k}={v}" for k, v in zip(arg_keys, arg_vals)]
+        arg_str = ", ".join(arg_strs)
+        return f"{type(self).__name__}({arg_str})"
+
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        if x.ndim > 2:
+            # (N, C, d1, d2, ..., dK) --> (N * d1 * ... * dK, C)
+            c = x.shape[1]
+            x = x.permute(0, *range(2, x.ndim), 1).reshape(-1, c)
+            # (N, d1, d2, ..., dK) --> (N * d1 * ... * dK,)
+            y = y.view(-1)
+
+        unignored_mask = y != self.ignore_index
+        y = y[unignored_mask]
+        if len(y) == 0:
+            return torch.tensor(0.0)
+        x = x[unignored_mask]
+
+        # compute weighted cross entropy term: -alpha * log(pt)
+        # (alpha is already part of self.nll_loss)
+        log_p = F.log_softmax(x, dim=-1)
+        ce = self.nll_loss(log_p, y)
+
+        # get true class column from each row
+        all_rows = torch.arange(len(x))
+        log_pt = log_p[all_rows, y]
+
+        # compute focal term: (1 - pt)^gamma
+        pt = log_pt.exp()
+        focal_term = (1 - pt) ** self.gamma
+
+        # the full loss: -alpha * ((1 - pt)^gamma) * log(pt)
+        loss = focal_term * ce
+
+        if self.reduction == "mean":
+            loss = loss.mean()
+        elif self.reduction == "sum":
+            loss = loss.sum()
+
+        return loss
+
+
+class FocalLoss(nn.Module):
+    r"""Implementation of the `focal loss <https://arxiv.org/pdf/1708.02002.pdf>`
+    Implements FocalLoss with either probabilities or logits.
+    ----------
+    alpha: float
+        Focal Loss ``alpha`` parameter
+        If negative, balance is ignored.
+    gamma: float
+        Focal Loss ``gamma`` parameter
+    """
+
+    def __init__(self, alpha: float = 0.25, gamma: float = 2.0):
+        super().__init__()
+        self.alpha = alpha
+        self.gamma = gamma
+        self.use_cuda = torch.cuda.is_available()
+
+        self.softmax = nn.Softmax(dim=-1)
+        self.log_soft_max = nn.LogSoftmax(dim=-1)
+
+    def forward(self, scores: Tensor, target: Tensor) -> Tensor:
+        r"""
+        Parameters
+        ----------
+        input: Tensor
+            input tensor with scores
+        target: Tensor
+            target tensor with the actual classes or probabilities
+            B or (B, C)
+        --------
+        """
+
+        # Get useful dimensions
+        num_batch = scores.size(0)
+        num_class = scores.size(1)
+
+        # Convert target to one-hot if necessary
+        if len(target.shape) == 1:
+            target = target.view(-1, 1).squeeze()
+            # Adapt to special case of one batch
+            if num_batch == 1:
+                target = torch.unsqueeze(target, 0)
+            target = torch.eye(num_class)[target]  # B, C
+
+        # Adapt to special case of one batch
+        if num_batch == 1:
+            scores = torch.unsqueeze(scores, 0)
+
+        # Move to GPU if possible
+        if self.use_cuda:
+            target = target.cuda()
+            scores = scores.cuda()
+
+        target = target.contiguous()
+
+        # Compute weights is alpha is positive
+        if self.alpha > 0:
+            balanced_weights = self.alpha * target + (1 - self.alpha) * (1 - target)
+        else:
+            balanced_weights = 1
+
+        probabilities = self.softmax(scores)
+        weights = (balanced_weights * (1 - probabilities).pow(self.gamma)).detach()
+        logs = self.log_soft_max(scores)
+
+        cross_entropy_loss = -weights * logs * target  # B, C
+
+        return torch.sum(cross_entropy_loss) / num_batch
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/losses/info_nce_loss.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/losses/info_nce_loss.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import torch.nn as nn
-import torch
-
-
-class InfoNceLoss(nn.Module):
-    """
-    Loss function for contrastive learning.
-    Taken from https://github.com/sthalles/SimCLR/blob/1848fc934ad844ae630e6c452300433fe99acfd9/simclr.py#L76.
-    """
-
-    def __init__(self, device, temperature):
-        super().__init__()
-        self.device = device
-        self.temperature = temperature
-        self.criterion = torch.nn.CrossEntropyLoss().to(self.device)
-
-    def forward(self, logits, labels):
-        logits = logits / self.temperature
-        loss = self.criterion(logits, labels)
-        return loss
+import torch.nn as nn
+import torch
+
+
+class InfoNceLoss(nn.Module):
+    """
+    Loss function for contrastive learning.
+    Taken from https://github.com/sthalles/SimCLR/blob/1848fc934ad844ae630e6c452300433fe99acfd9/simclr.py#L76.
+    """
+
+    def __init__(self, device, temperature):
+        super().__init__()
+        self.device = device
+        self.temperature = temperature
+        self.criterion = torch.nn.CrossEntropyLoss().to(self.device)
+
+    def forward(self, logits, labels):
+        logits = logits / self.temperature
+        loss = self.criterion(logits, labels)
+        return loss
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/losses/loss_manager.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/losses/loss_manager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import List
-import torch.nn as nn
-
-
-class LossManager:
-    def __init__(self, *args) -> None:
-        self.losses_function: List[nn.Module] = args
-        self.running_losses = [0] * len(self.losses_function)
-
-    def __call__(self, *args, **kwargs):
-        # First compute main loss
-        main_loss = self.losses_function[0](*args, **kwargs)
-        self.running_losses[0] += main_loss
-        # Then compute other losses, used only for logging
-        for i, loss_function in enumerate(self.losses_function[1:]):
-            self.running_losses[i + 1] += loss_function(*args, **kwargs)
-        return main_loss
-
-    def get_running_losses(self):
-        """
-        Return a list of tuples (loss_name, loss_value)
-        """
-        named_running_losses = []
-        for i, loss_function in enumerate(self.losses_function):
-            named_running_losses.append((loss_function.__class__.__name__, self.running_losses[i]))
-            self.running_losses[i] = 0
-        return named_running_losses
+from typing import List
+import torch.nn as nn
+
+
+class LossManager:
+    def __init__(self, *args) -> None:
+        self.losses_function: List[nn.Module] = args
+        self.running_losses = [0] * len(self.losses_function)
+
+    def __call__(self, *args, **kwargs):
+        # First compute main loss
+        main_loss = self.losses_function[0](*args, **kwargs)
+        self.running_losses[0] += main_loss
+        # Then compute other losses, used only for logging
+        for i, loss_function in enumerate(self.losses_function[1:]):
+            self.running_losses[i + 1] += loss_function(*args, **kwargs)
+        return main_loss
+
+    def get_running_losses(self):
+        """
+        Return a list of tuples (loss_name, loss_value)
+        """
+        named_running_losses = []
+        for i, loss_function in enumerate(self.losses_function):
+            named_running_losses.append((loss_function.__class__.__name__, self.running_losses[i]))
+            self.running_losses[i] = 0
+        return named_running_losses
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/lr_schedulers/linear_warmup_cosine_annealing_lr.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/lr_schedulers/linear_warmup_cosine_annealing_lr.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import math
-from typing import List
-from torch.optim import Optimizer
-from torch.optim.lr_scheduler import _LRScheduler
-
-# from https://lightning-flash.readthedocs.io/en/stable/_modules/flash/core/optimizers/lr_scheduler.html#LinearWarmupCosineAnnealingLR
-
-
-class LinearWarmupCosineAnnealingLR(_LRScheduler):
-    """Sets the learning rate of each parameter group to follow a linear warmup schedule between warmup_start_lr
-    and base_lr followed by a cosine annealing schedule between base_lr and eta_min.
-
-    .. warning::
-        It is recommended to call :func:`.step()` for :class:`LinearWarmupCosineAnnealingLR`
-        after each iteration as calling it after each epoch will keep the starting lr at
-        warmup_start_lr for the first epoch which is 0 in most cases.
-
-    .. warning::
-        passing epoch to :func:`.step()` is being deprecated and comes with an EPOCH_DEPRECATION_WARNING.
-        It calls the :func:`_get_closed_form_lr()` method for this scheduler instead of
-        :func:`get_lr()`. Though this does not change the behavior of the scheduler, when passing
-        epoch param to :func:`.step()`, the user should call the :func:`.step()` function before calling
-        train and validation methods.
-
-    Example:
-        >>> layer = nn.Linear(10, 1)
-        >>> optimizer = Adam(layer.parameters(), lr=0.02)
-        >>> scheduler = LinearWarmupCosineAnnealingLR(optimizer, warmup_epochs=10, max_epochs=40)
-        >>> #
-        >>> # the default case
-        >>> for epoch in range(40):
-        ...     # train(...)
-        ...     # validate(...)
-        ...     scheduler.step()
-        >>> #
-        >>> # passing epoch param case
-        >>> for epoch in range(40):
-        ...     scheduler.step(epoch)
-        ...     # train(...)
-        ...     # validate(...)
-    """
-
-    def __init__(
-        self,
-        optimizer: Optimizer,
-        warmup_epochs: int,
-        max_epochs: int,
-        warmup_start_lr: float = 0.0,
-        eta_min: float = 0.0,
-        last_epoch: int = -1,
-    ) -> None:
-        """
-        Args:
-            optimizer (Optimizer): Wrapped optimizer.
-            warmup_epochs (int): Maximum number of iterations for linear warmup
-            max_epochs (int): Maximum number of iterations
-            warmup_start_lr (float): Learning rate to start the linear warmup. Default: 0.
-            eta_min (float): Minimum learning rate. Default: 0.
-            last_epoch (int): The index of last epoch. Default: -1.
-        """
-        self.warmup_epochs = warmup_epochs
-        self.max_epochs = max_epochs
-        self.warmup_start_lr = warmup_start_lr
-        self.eta_min = eta_min
-
-        super().__init__(optimizer, last_epoch)
-
-    def get_lr(self) -> List[float]:
-        """Compute learning rate using chainable form of the scheduler."""
-        # if not self._get_lr_called_within_step:
-        #     warnings.warn(
-        #         "To get the last learning rate computed by the scheduler, "
-        #         "please use `get_last_lr()`.",
-        #         UserWarning,
-        #     )
-
-        if self.last_epoch == 0:
-            return [self.warmup_start_lr] * len(self.base_lrs)
-        if self.last_epoch < self.warmup_epochs:
-            return [
-                group["lr"] + (base_lr - self.warmup_start_lr) / (self.warmup_epochs - 1)
-                for base_lr, group in zip(self.base_lrs, self.optimizer.param_groups)
-            ]
-        if self.last_epoch == self.warmup_epochs:
-            return self.base_lrs
-        if (self.last_epoch - 1 - self.max_epochs) % (
-            2 * (self.max_epochs - self.warmup_epochs)
-        ) == 0:
-            return [
-                group["lr"]
-                + (base_lr - self.eta_min)
-                * (1 - math.cos(math.pi / (self.max_epochs - self.warmup_epochs)))
-                / 2
-                for base_lr, group in zip(self.base_lrs, self.optimizer.param_groups)
-            ]
-
-        return [
-            (
-                1
-                + math.cos(
-                    math.pi
-                    * (self.last_epoch - self.warmup_epochs)
-                    / (self.max_epochs - self.warmup_epochs)
-                )
-            )
-            / (
-                1
-                + math.cos(
-                    math.pi
-                    * (self.last_epoch - self.warmup_epochs - 1)
-                    / (self.max_epochs - self.warmup_epochs)
-                )
-            )
-            * (group["lr"] - self.eta_min)
-            + self.eta_min
-            for group in self.optimizer.param_groups
-        ]
-
-    def _get_closed_form_lr(self) -> List[float]:
-        """Called when epoch is passed as a param to the `step` function of the scheduler."""
-        if self.last_epoch < self.warmup_epochs:
-            return [
-                self.warmup_start_lr
-                + self.last_epoch * (base_lr - self.warmup_start_lr) / (self.warmup_epochs - 1)
-                for base_lr in self.base_lrs
-            ]
-
-        return [
-            self.eta_min
-            + 0.5
-            * (base_lr - self.eta_min)
-            * (
-                1
-                + math.cos(
-                    math.pi
-                    * (self.last_epoch - self.warmup_epochs)
-                    / (self.max_epochs - self.warmup_epochs)
-                )
-            )
-            for base_lr in self.base_lrs
-        ]
-
-
-# warmup + decay as a function
-def linear_warmup_decay(warmup_steps, total_steps, cosine=True, linear=False):
-    """Linear warmup for warmup_steps, optionally with cosine annealing or linear decay to 0 at total_steps."""
-    assert not (linear and cosine)
-
-    def fn(step):
-        if step < warmup_steps:
-            return float(step) / float(max(1, warmup_steps))
-
-        if not (cosine or linear):
-            # no decay
-            return 1.0
-
-        progress = float(step - warmup_steps) / float(max(1, total_steps - warmup_steps))
-        if cosine:
-            # cosine decay
-            return 0.5 * (1.0 + math.cos(math.pi * progress))
-
-        # linear decay
-        return 1.0 - progress
-
-    return fn
+import math
+from typing import List
+from torch.optim import Optimizer
+from torch.optim.lr_scheduler import _LRScheduler
+
+# from https://lightning-flash.readthedocs.io/en/stable/_modules/flash/core/optimizers/lr_scheduler.html#LinearWarmupCosineAnnealingLR
+
+
+class LinearWarmupCosineAnnealingLR(_LRScheduler):
+    """Sets the learning rate of each parameter group to follow a linear warmup schedule between warmup_start_lr
+    and base_lr followed by a cosine annealing schedule between base_lr and eta_min.
+
+    .. warning::
+        It is recommended to call :func:`.step()` for :class:`LinearWarmupCosineAnnealingLR`
+        after each iteration as calling it after each epoch will keep the starting lr at
+        warmup_start_lr for the first epoch which is 0 in most cases.
+
+    .. warning::
+        passing epoch to :func:`.step()` is being deprecated and comes with an EPOCH_DEPRECATION_WARNING.
+        It calls the :func:`_get_closed_form_lr()` method for this scheduler instead of
+        :func:`get_lr()`. Though this does not change the behavior of the scheduler, when passing
+        epoch param to :func:`.step()`, the user should call the :func:`.step()` function before calling
+        train and validation methods.
+
+    Example:
+        >>> layer = nn.Linear(10, 1)
+        >>> optimizer = Adam(layer.parameters(), lr=0.02)
+        >>> scheduler = LinearWarmupCosineAnnealingLR(optimizer, warmup_epochs=10, max_epochs=40)
+        >>> #
+        >>> # the default case
+        >>> for epoch in range(40):
+        ...     # train(...)
+        ...     # validate(...)
+        ...     scheduler.step()
+        >>> #
+        >>> # passing epoch param case
+        >>> for epoch in range(40):
+        ...     scheduler.step(epoch)
+        ...     # train(...)
+        ...     # validate(...)
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        warmup_epochs: int,
+        max_epochs: int,
+        warmup_start_lr: float = 0.0,
+        eta_min: float = 0.0,
+        last_epoch: int = -1,
+    ) -> None:
+        """
+        Args:
+            optimizer (Optimizer): Wrapped optimizer.
+            warmup_epochs (int): Maximum number of iterations for linear warmup
+            max_epochs (int): Maximum number of iterations
+            warmup_start_lr (float): Learning rate to start the linear warmup. Default: 0.
+            eta_min (float): Minimum learning rate. Default: 0.
+            last_epoch (int): The index of last epoch. Default: -1.
+        """
+        self.warmup_epochs = warmup_epochs
+        self.max_epochs = max_epochs
+        self.warmup_start_lr = warmup_start_lr
+        self.eta_min = eta_min
+
+        super().__init__(optimizer, last_epoch)
+
+    def get_lr(self) -> List[float]:
+        """Compute learning rate using chainable form of the scheduler."""
+        # if not self._get_lr_called_within_step:
+        #     warnings.warn(
+        #         "To get the last learning rate computed by the scheduler, "
+        #         "please use `get_last_lr()`.",
+        #         UserWarning,
+        #     )
+
+        if self.last_epoch == 0:
+            return [self.warmup_start_lr] * len(self.base_lrs)
+        if self.last_epoch < self.warmup_epochs:
+            return [
+                group["lr"] + (base_lr - self.warmup_start_lr) / (self.warmup_epochs - 1)
+                for base_lr, group in zip(self.base_lrs, self.optimizer.param_groups)
+            ]
+        if self.last_epoch == self.warmup_epochs:
+            return self.base_lrs
+        if (self.last_epoch - 1 - self.max_epochs) % (
+            2 * (self.max_epochs - self.warmup_epochs)
+        ) == 0:
+            return [
+                group["lr"]
+                + (base_lr - self.eta_min)
+                * (1 - math.cos(math.pi / (self.max_epochs - self.warmup_epochs)))
+                / 2
+                for base_lr, group in zip(self.base_lrs, self.optimizer.param_groups)
+            ]
+
+        return [
+            (
+                1
+                + math.cos(
+                    math.pi
+                    * (self.last_epoch - self.warmup_epochs)
+                    / (self.max_epochs - self.warmup_epochs)
+                )
+            )
+            / (
+                1
+                + math.cos(
+                    math.pi
+                    * (self.last_epoch - self.warmup_epochs - 1)
+                    / (self.max_epochs - self.warmup_epochs)
+                )
+            )
+            * (group["lr"] - self.eta_min)
+            + self.eta_min
+            for group in self.optimizer.param_groups
+        ]
+
+    def _get_closed_form_lr(self) -> List[float]:
+        """Called when epoch is passed as a param to the `step` function of the scheduler."""
+        if self.last_epoch < self.warmup_epochs:
+            return [
+                self.warmup_start_lr
+                + self.last_epoch * (base_lr - self.warmup_start_lr) / (self.warmup_epochs - 1)
+                for base_lr in self.base_lrs
+            ]
+
+        return [
+            self.eta_min
+            + 0.5
+            * (base_lr - self.eta_min)
+            * (
+                1
+                + math.cos(
+                    math.pi
+                    * (self.last_epoch - self.warmup_epochs)
+                    / (self.max_epochs - self.warmup_epochs)
+                )
+            )
+            for base_lr in self.base_lrs
+        ]
+
+
+# warmup + decay as a function
+def linear_warmup_decay(warmup_steps, total_steps, cosine=True, linear=False):
+    """Linear warmup for warmup_steps, optionally with cosine annealing or linear decay to 0 at total_steps."""
+    assert not (linear and cosine)
+
+    def fn(step):
+        if step < warmup_steps:
+            return float(step) / float(max(1, warmup_steps))
+
+        if not (cosine or linear):
+            # no decay
+            return 1.0
+
+        progress = float(step - warmup_steps) / float(max(1, total_steps - warmup_steps))
+        if cosine:
+            # cosine decay
+            return 0.5 * (1.0 + math.cos(math.pi * progress))
+
+        # linear decay
+        return 1.0 - progress
+
+    return fn
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/metrics/classification_accuracy.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/metrics/classification_accuracy.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import torch
-from torchmetrics.classification import Accuracy
-
-from .abstract_metric import AbstractMetric
-
-
-class ClassificationAccuracy(AbstractMetric):
-    """
-    Classification accuracy.
-    """
-
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.name = "ClassificationAccuracy"
-        self.true, self.pred = torch.empty(0).to(self.device), torch.empty(0).to(self.device)
-        self.metric = Accuracy(
-            task="multiclass", num_classes=self.num_classes, average="macro"
-        ).to(self.device)
-
-    def update(self, predictions, targets, _=None):
-        # From vector to classification
-        predictions_argmax = torch.argmax(predictions, dim=1)
-        targets_argmax = torch.argmax(targets, dim=1)
-        # Update metric
-        self.metric.update(
-            predictions_argmax,
-            targets_argmax,
-        )
-        # Update current values
-        self.true = torch.cat((self.true, targets_argmax))
-        self.pred = torch.cat((self.pred, predictions_argmax))
-
-    def get_score(self):
-        return self.metric.compute().item(), (self.true, self.pred)
-
-    def reset(self):
-        self.metric = Accuracy(
-            task="multiclass", num_classes=self.num_classes, average="macro"
-        ).to(self.device)
-        self.true, self.pred = torch.empty(0).to(self.device), torch.empty(0).to(self.device)
+import torch
+from torchmetrics.classification import Accuracy
+
+from .abstract_metric import AbstractMetric
+
+
+class ClassificationAccuracy(AbstractMetric):
+    """
+    Classification accuracy.
+    """
+
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.name = "ClassificationAccuracy"
+        self.true, self.pred = torch.empty(0).to(self.device), torch.empty(0).to(self.device)
+        self.metric = Accuracy(
+            task="multiclass", num_classes=self.num_classes, average="macro"
+        ).to(self.device)
+
+    def update(self, predictions, targets, _=None):
+        # From vector to classification
+        predictions_argmax = torch.argmax(predictions, dim=1)
+        targets_argmax = torch.argmax(targets, dim=1)
+        # Update metric
+        self.metric.update(
+            predictions_argmax,
+            targets_argmax,
+        )
+        # Update current values
+        self.true = torch.cat((self.true, targets_argmax))
+        self.pred = torch.cat((self.pred, predictions_argmax))
+
+    def get_score(self):
+        return self.metric.compute().item(), (self.true, self.pred)
+
+    def reset(self):
+        self.metric = Accuracy(
+            task="multiclass", num_classes=self.num_classes, average="macro"
+        ).to(self.device)
+        self.true, self.pred = torch.empty(0).to(self.device), torch.empty(0).to(self.device)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/metrics/mean_error_metric.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/metrics/mean_error_metric.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from torchmetrics import MeanSquaredError
-
-from .abstract_metric import AbstractMetric
-
-
-class MeanErrorMetric(AbstractMetric):
-    """
-    Mean Error.
-    """
-
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.name = "MeanError"
-        self.metric = MeanSquaredError(squared=False).to(self.device)
-
-    def update(self, predictions, targets, _=None):
-        # Update metric
-        self.metric.update(
-            predictions,
-            targets,
-        )
-
-    def get_score(self):
-        return -self.metric.compute().item(), None
-
-    def reset(self):
-        self.metric = MeanSquaredError(squared=False).to(self.device)
+from torchmetrics import MeanSquaredError
+
+from .abstract_metric import AbstractMetric
+
+
+class MeanErrorMetric(AbstractMetric):
+    """
+    Mean Error.
+    """
+
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.name = "MeanError"
+        self.metric = MeanSquaredError(squared=False).to(self.device)
+
+    def update(self, predictions, targets, _=None):
+        # Update metric
+        self.metric.update(
+            predictions,
+            targets,
+        )
+
+    def get_score(self):
+        return -self.metric.compute().item(), None
+
+    def reset(self):
+        self.metric = MeanSquaredError(squared=False).to(self.device)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/metrics/mean_squared_error_metric.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/metrics/mean_squared_error_metric.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from torchmetrics import MeanSquaredError
-
-from .abstract_metric import AbstractMetric
-
-
-class MeanSquaredErrorMetric(AbstractMetric):
-    """
-    Mean Squared Error.
-    """
-
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.name = "MeanSquaredError"
-        self.metric = MeanSquaredError(squared=True).to(self.device)
-
-    def update(self, predictions, targets, _=None):
-        # Update metric
-        self.metric.update(
-            predictions,
-            targets,
-        )
-
-    def get_score(self):
-        return -self.metric.compute().item(), None
-
-    def reset(self):
-        self.metric = MeanSquaredError(squared=True).to(self.device)
+from torchmetrics import MeanSquaredError
+
+from .abstract_metric import AbstractMetric
+
+
+class MeanSquaredErrorMetric(AbstractMetric):
+    """
+    Mean Squared Error.
+    """
+
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.name = "MeanSquaredError"
+        self.metric = MeanSquaredError(squared=True).to(self.device)
+
+    def update(self, predictions, targets, _=None):
+        # Update metric
+        self.metric.update(
+            predictions,
+            targets,
+        )
+
+    def get_score(self):
+        return -self.metric.compute().item(), None
+
+    def reset(self):
+        self.metric = MeanSquaredError(squared=True).to(self.device)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/metrics/pcc.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/metrics/pcc.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import torch
-from torchmetrics import PearsonCorrCoef
-
-from .abstract_metric import AbstractMetric
-
-
-class PCC(AbstractMetric):
-    """
-    Pearson Correlation Coefficient.
-    """
-
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.metric = PearsonCorrCoef().to(self.device)
-        self.name = "PCC"
-
-    def update(self, predictions, targets, _=None):
-        self.metric.update(torch.flatten(predictions), torch.flatten(targets).float())
-
-    def get_score(self):
-        return self.metric.compute().item(), None
-
-    def reset(self):
-        self.metric = PearsonCorrCoef().to(self.device)
+import torch
+from torchmetrics import PearsonCorrCoef
+
+from .abstract_metric import AbstractMetric
+
+
+class PCC(AbstractMetric):
+    """
+    Pearson Correlation Coefficient.
+    """
+
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.metric = PearsonCorrCoef().to(self.device)
+        self.name = "PCC"
+
+    def update(self, predictions, targets, _=None):
+        self.metric.update(torch.flatten(predictions), torch.flatten(targets).float())
+
+    def get_score(self):
+        return self.metric.compute().item(), None
+
+    def reset(self):
+        self.metric = PearsonCorrCoef().to(self.device)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/metrics/positive_pair_matching_metric.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/metrics/positive_pair_matching_metric.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import torch
-import numpy as np
-
-from .abstract_metric import AbstractMetric
-
-
-class PositivePairMatchingMetric(AbstractMetric):
-    """
-    Computes the accuracy over the k top predictions for the specified values of k.
-    """
-
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.name = "PositivePairMatchingMetric"
-        self.local_matchings = []
-
-    def update(self, predictions, targets, ___=None):
-        topk = (1,)
-
-        with torch.no_grad():
-            maxk = topk[0]
-            batch_size = targets.size(0)
-
-            _, pred = predictions.topk(maxk, 1, True, True)
-            pred = pred.t()
-            correct = pred.eq(targets.view(1, -1).expand_as(pred))
-
-            correct_k = correct[:maxk].reshape(-1).float().sum(0, keepdim=True)
-            matching = correct_k.div_(batch_size)[0].item()
-            self.local_matchings.append(matching)
-
-    def get_score(self):
-        return np.mean(self.local_matchings), None
-
-    def reset(self):
-        self.local_matchings = []
+import torch
+import numpy as np
+
+from .abstract_metric import AbstractMetric
+
+
+class PositivePairMatchingMetric(AbstractMetric):
+    """
+    Computes the accuracy over the k top predictions for the specified values of k.
+    """
+
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.name = "PositivePairMatchingMetric"
+        self.local_matchings = []
+
+    def update(self, predictions, targets, ___=None):
+        topk = (1,)
+
+        with torch.no_grad():
+            maxk = topk[0]
+            batch_size = targets.size(0)
+
+            _, pred = predictions.topk(maxk, 1, True, True)
+            pred = pred.t()
+            correct = pred.eq(targets.view(1, -1).expand_as(pred))
+
+            correct_k = correct[:maxk].reshape(-1).float().sum(0, keepdim=True)
+            matching = correct_k.div_(batch_size)[0].item()
+            self.local_matchings.append(matching)
+
+    def get_score(self):
+        return np.mean(self.local_matchings), None
+
+    def reset(self):
+        self.local_matchings = []
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/cnn_model_manager.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/regression_model_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,100 @@
-import os
-import warnings
-from matplotlib import pyplot as plt
-from skimage import io
-import numpy as np
-import torch
-
-from ..metrics.abstract_metric import AbstractMetric
-from ..data_sets.dataset_output import DatasetOutput
-from .model_manager import ModelManager
-from ..display_tools import (
-    display_confusion_matrix,
-    make_image_matplotlib_displayable,
-    make_image_tiff_displayable,
-)
-
-
-class CnnModelManager(ModelManager):
-    def save_results(self, name: str, dl_element: DatasetOutput, mean_std):
-        input_np = dl_element.input
-        target_np = dl_element.target
-        prediction_np = dl_element.prediction
-        add_np = dl_element.additional
-
-        prediction_class = np.argmax(prediction_np, axis=0)
-        ground_truth_class = np.argmax(target_np, axis=0)
-
-        # Choose folder to save
-        folder_to_save = (
-            os.path.join(self.params.output_dir, "right")
-            if prediction_class == ground_truth_class
-            else os.path.join(self.params.output_dir, "wrong")
-        )
-        os.makedirs(folder_to_save, exist_ok=True)
-
-        # Save inputs, targets & predictions as tiff images
-        for data_image, data_type, data_mean_std in zip(
-            [input_np, add_np],
-            ["input", "additional"],
-            [mean_std, None],  # No normalization for additional data
-        ):
-            if data_image is None:  # case when additional data is None
-                continue
-            image_to_save = make_image_tiff_displayable(data_image, data_mean_std)
-
-            # Save inputs with prediction and ground truth in name
-            with warnings.catch_warnings():
-                warnings.filterwarnings(action="ignore", category=UserWarning)
-                io.imsave(
-                    f"{folder_to_save}/{name}_{data_type}_g{ground_truth_class}_p{prediction_class}.tiff",
-                    image_to_save,
-                )
-
-    def write_images_to_tensorboard(
-        self,
-        current_batch: int,
-        dl_element: DatasetOutput,
-        name: str,
-    ):
-        # Get numpy arrays
-        numpy_dl_element = dl_element.get_numpy_dataset_output()
-
-        # Get images name
-        current_dl_file_names = [
-            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
-        ]
-        image_names = [
-            current_dl_file_names[image_index] for image_index in numpy_dl_element.index
-        ]
-
-        # Log the results images
-        for i, (input_np, target_np, prediction_np, image_name) in enumerate(
-            zip(
-                numpy_dl_element.input,
-                numpy_dl_element.target,
-                numpy_dl_element.prediction,
-                image_names,
-            )
-        ):
-            # Do not save too many images
-            if i == self.params.nb_tensorboard_images_max:
-                break
-            # Get class with max probability
-            prediction = np.argmax(prediction_np, axis=0)
-            ground_truth = np.argmax(target_np, axis=0)
-
-            # Log input image
-            plt.title(f"Ground truth {ground_truth} - Predicted {prediction}")
-            input_mat = make_image_matplotlib_displayable(input_np, self.dl[name].dataset.mean_std)
-            plt.imshow(input_mat)
-            self.writer.add_figure(
-                f"{name}/{image_name}",
-                plt.gcf(),
-                current_batch,
-            )
-
-    def model_prediction(self, dl_element: DatasetOutput, dl_metric: AbstractMetric, _) -> None:
-        """
-        Function to generate outputs from inputs for given model
-        Careful, softmax is applied here and not in the model.
-        """
-        dl_element.to_device(self.device)
-
-        predictions = torch.softmax(self.model(dl_element.input.float()), dim=-1)
-        dl_element.prediction = predictions
-
-        # Update metric
-        dl_metric.update(predictions, dl_element.target, dl_element.additional)
-
-    def plot_confusion_matrix(self, results) -> None:
-        display_confusion_matrix(results, self.params.class_names, self.params.output_dir)
+import warnings
+from matplotlib import pyplot as plt
+from skimage import io
+import numpy as np
+
+from ..data_sets.dataset_output import DatasetOutput
+from .model_manager import ModelManager
+from ..display_tools import (
+    make_image_matplotlib_displayable,
+    make_image_tiff_displayable,
+)
+
+
+class RegressionModelManager(ModelManager):
+    def save_results(self, name, dl_element: DatasetOutput, mean_std):
+        input_np = dl_element.input
+        target_np = dl_element.target
+        prediction_np = dl_element.prediction
+        add_np = dl_element.additional
+
+        # Save inputs, targets & predictions as tiff images
+        for data_image, data_type, data_mean_std in zip(
+            [input_np, add_np],
+            ["input", "additional"],
+            [mean_std, None],  # No normalization for additional data
+        ):
+            if data_image is None:
+                continue
+            image_to_save = make_image_tiff_displayable(data_image, data_mean_std)
+
+            # Save inputs with prediction and ground truth in name
+            if len(target_np.shape) == 0:  # case where regression predicts only one value
+                target_np = np.array([target_np])
+                prediction_np = np.array([prediction_np])
+            ground_truth = "_".join([str(local_target) for local_target in target_np])
+            prediction = "_".join([str(local_prediction) for local_prediction in prediction_np])
+            with warnings.catch_warnings():
+                warnings.filterwarnings(action="ignore", category=UserWarning)
+                io.imsave(
+                    f"{self.params.output_dir}/{name}_{data_type}_g{ground_truth}_p{prediction}.tiff",
+                    image_to_save,
+                )
+
+    def write_images_to_tensorboard(
+        self,
+        current_batch,
+        dl_element,
+        name,
+    ):
+        # Get numpy arrays
+        numpy_dl_element = dl_element.get_numpy_dataset_output()
+
+        # Get images name
+        current_dl_file_names = [
+            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
+        ]
+        image_names = [
+            current_dl_file_names[image_index] for image_index in numpy_dl_element.index
+        ]
+
+        # Log the results images
+        for i, (input_np, target_np, prediction_np, image_name) in enumerate(
+            zip(
+                numpy_dl_element.input,
+                numpy_dl_element.target,
+                numpy_dl_element.prediction,
+                image_names,
+            )
+        ):
+            # Do not save too many images
+            if i == self.params.nb_tensorboard_images_max:
+                break
+            # Get class with max probability
+            ground_truth = ",".join([str(int(local_target)) for local_target in target_np])
+            prediction = ",".join(
+                [str(int(local_prediction)) for local_prediction in prediction_np]
+            )
+
+            # Log input image
+            plt.title(f"Ground truth {ground_truth} - Predicted {prediction}")
+            input_mat = make_image_matplotlib_displayable(input_np, self.dl[name].dataset.mean_std)
+            plt.imshow(input_mat)
+            self.writer.add_figure(
+                f"{name}/{image_name}",
+                plt.gcf(),
+                current_batch,
+            )
+
+    def model_prediction(self, dl_element, dl_metric, _):
+        """
+        Function to generate outputs from inputs for given model.
+        No softmax is applied here.
+        """
+        dl_element.to_device(self.device)
+
+        predictions = self.model(dl_element.input.float())
+        dl_element.prediction = predictions
+
+        # Update metric
+        dl_metric.update(predictions, dl_element.target, dl_element.additional)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/contrastive_model_manager.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/contrastive_model_manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from typing import Optional
-from matplotlib import pyplot as plt
-import torch
-import torch.nn.functional as F
-
-from ..losses.loss_manager import LossManager
-from ..data_sets.dataset_output import DatasetOutput
-from ..display_tools import make_image_matplotlib_displayable
-from ..metrics.abstract_metric import AbstractMetric
-from .model_manager import ModelManager
-
-
-class ContrastiveModelManager(ModelManager):
-    def compute_loss(
-        self,
-        dl_element: DatasetOutput,
-        dl_metric: AbstractMetric,
-        loss_manager: Optional[LossManager] = None,
-        data_loader=None,
-    ):
-        # Read data loader element
-        inputs = dl_element.input
-        batch_size = inputs.shape[0]
-
-        # Construct all_inputs: [input[0], input[1], input[2], ..., input_bis[0], input_bis[1], input_bis[2], ...]
-        all_inputs = torch.zeros((inputs.shape[0] * self.params.n_views, *inputs.shape[1:]))
-        for input_index, image_index in enumerate(dl_element.index):
-            dl_element_bis = data_loader.dataset[image_index.item()]
-            assert dl_element_bis.index == image_index
-            # Fill input
-            all_inputs[input_index] = inputs[input_index]
-            all_inputs[input_index + batch_size] = dl_element_bis.input
-
-        all_inputs = all_inputs.to(self.device).float()
-        features = self.model(all_inputs)
-
-        # Define labels
-        labels = torch.cat([torch.arange(batch_size) for i in range(self.params.n_views)], dim=0)
-        labels = (labels.unsqueeze(0) == labels.unsqueeze(1)).float()
-        labels = labels.to(self.device)
-
-        features = F.normalize(features, dim=1)
-
-        similarity_matrix = torch.matmul(features, features.T)
-
-        # Discard the main diagonal from both: labels and similarities matrix
-        mask = torch.eye(labels.shape[0], dtype=torch.bool).to(self.device)
-        labels = labels[~mask].view(labels.shape[0], -1)
-        similarity_matrix = similarity_matrix[~mask].view(similarity_matrix.shape[0], -1)
-
-        # Select and combine multiple positives
-        positives = similarity_matrix[labels.bool()].view(labels.shape[0], -1)
-
-        # Select only the negatives the negatives
-        negatives = similarity_matrix[~labels.bool()].view(similarity_matrix.shape[0], -1)
-
-        logits = torch.cat([positives, negatives], dim=1)
-        labels = torch.zeros(logits.shape[0], dtype=torch.long).to(self.device)
-
-        # Update metric
-        dl_metric.update(logits, labels)
-
-        # Use other inputs as fake predictions
-        dl_element.prediction = all_inputs[batch_size:]
-
-        # Compute loss if possible
-        if loss_manager is None:
-            return None
-        loss = loss_manager(logits, labels)
-
-        return loss
-
-    def write_images_to_tensorboard(self, current_batch, dl_element, name):
-        # Get numpy arrays
-        numpy_dl_element = dl_element.get_numpy_dataset_output()
-
-        # Get images name
-        current_dl_file_names = [
-            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
-        ]
-        image_names = [
-            current_dl_file_names[image_index] for image_index in numpy_dl_element.index
-        ]
-
-        # Current data set mean & std
-        mean_std = self.dl[name].dataset.mean_std
-
-        # Log the results images
-        for i, (input_np, input_np_bis, image_name) in enumerate(
-            zip(numpy_dl_element.input, numpy_dl_element.prediction, image_names)
-        ):
-            # Do not save too many images
-            if i == self.params.nb_tensorboard_images_max:
-                break
-            plt.imshow(make_image_matplotlib_displayable(input_np, mean_std=mean_std))
-            self.writer.add_figure(
-                f"{name}/{image_name}/first_transformed",
-                plt.gcf(),
-                current_batch,
-            )
-
-            plt.imshow(make_image_matplotlib_displayable(input_np_bis, mean_std=mean_std))
-            self.writer.add_figure(
-                f"{name}/{image_name}/second_transformed",
-                plt.gcf(),
-                current_batch,
-            )
-
-    def save_results(self, _, __, ___):
-        pass
+from typing import Optional
+from matplotlib import pyplot as plt
+import torch
+import torch.nn.functional as F
+
+from ..losses.loss_manager import LossManager
+from ..data_sets.dataset_output import DatasetOutput
+from ..display_tools import make_image_matplotlib_displayable
+from ..metrics.abstract_metric import AbstractMetric
+from .model_manager import ModelManager
+
+
+class ContrastiveModelManager(ModelManager):
+    def compute_loss(
+        self,
+        dl_element: DatasetOutput,
+        dl_metric: AbstractMetric,
+        loss_manager: Optional[LossManager] = None,
+        data_loader=None,
+    ):
+        # Read data loader element
+        inputs = dl_element.input
+        batch_size = inputs.shape[0]
+
+        # Construct all_inputs: [input[0], input[1], input[2], ..., input_bis[0], input_bis[1], input_bis[2], ...]
+        all_inputs = torch.zeros((inputs.shape[0] * self.params.n_views, *inputs.shape[1:]))
+        for input_index, image_index in enumerate(dl_element.index):
+            dl_element_bis = data_loader.dataset[image_index.item()]
+            assert dl_element_bis.index == image_index
+            # Fill input
+            all_inputs[input_index] = inputs[input_index]
+            all_inputs[input_index + batch_size] = dl_element_bis.input
+
+        all_inputs = all_inputs.to(self.device).float()
+        features = self.model(all_inputs)
+
+        # Define labels
+        labels = torch.cat([torch.arange(batch_size) for i in range(self.params.n_views)], dim=0)
+        labels = (labels.unsqueeze(0) == labels.unsqueeze(1)).float()
+        labels = labels.to(self.device)
+
+        features = F.normalize(features, dim=1)
+
+        similarity_matrix = torch.matmul(features, features.T)
+
+        # Discard the main diagonal from both: labels and similarities matrix
+        mask = torch.eye(labels.shape[0], dtype=torch.bool).to(self.device)
+        labels = labels[~mask].view(labels.shape[0], -1)
+        similarity_matrix = similarity_matrix[~mask].view(similarity_matrix.shape[0], -1)
+
+        # Select and combine multiple positives
+        positives = similarity_matrix[labels.bool()].view(labels.shape[0], -1)
+
+        # Select only the negatives the negatives
+        negatives = similarity_matrix[~labels.bool()].view(similarity_matrix.shape[0], -1)
+
+        logits = torch.cat([positives, negatives], dim=1)
+        labels = torch.zeros(logits.shape[0], dtype=torch.long).to(self.device)
+
+        # Update metric
+        dl_metric.update(logits, labels)
+
+        # Use other inputs as fake predictions
+        dl_element.prediction = all_inputs[batch_size:]
+
+        # Compute loss if possible
+        if loss_manager is None:
+            return None
+        loss = loss_manager(logits, labels)
+
+        return loss
+
+    def write_images_to_tensorboard(self, current_batch, dl_element, name):
+        # Get numpy arrays
+        numpy_dl_element = dl_element.get_numpy_dataset_output()
+
+        # Get images name
+        current_dl_file_names = [
+            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
+        ]
+        image_names = [
+            current_dl_file_names[image_index] for image_index in numpy_dl_element.index
+        ]
+
+        # Current data set mean & std
+        mean_std = self.dl[name].dataset.mean_std
+
+        # Log the results images
+        for i, (input_np, input_np_bis, image_name) in enumerate(
+            zip(numpy_dl_element.input, numpy_dl_element.prediction, image_names)
+        ):
+            # Do not save too many images
+            if i == self.params.nb_tensorboard_images_max:
+                break
+            plt.imshow(make_image_matplotlib_displayable(input_np, mean_std=mean_std))
+            self.writer.add_figure(
+                f"{name}/{image_name}/first_transformed",
+                plt.gcf(),
+                current_batch,
+            )
+
+            plt.imshow(make_image_matplotlib_displayable(input_np_bis, mean_std=mean_std))
+            self.writer.add_figure(
+                f"{name}/{image_name}/second_transformed",
+                plt.gcf(),
+                current_batch,
+            )
+
+    def save_results(self, _, __, ___):
+        pass
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/custom_get_encoder.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/custom_get_encoder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import torch.utils.model_zoo as model_zoo
-
-from segmentation_models_pytorch.encoders.resnet import resnet_encoders
-from segmentation_models_pytorch.encoders.dpn import dpn_encoders
-from segmentation_models_pytorch.encoders.vgg import vgg_encoders
-from segmentation_models_pytorch.encoders.senet import senet_encoders
-from segmentation_models_pytorch.encoders.densenet import densenet_encoders
-from segmentation_models_pytorch.encoders.inceptionresnetv2 import inceptionresnetv2_encoders
-from segmentation_models_pytorch.encoders.inceptionv4 import inceptionv4_encoders
-from segmentation_models_pytorch.encoders.efficientnet import efficient_net_encoders
-from segmentation_models_pytorch.encoders.mobilenet import mobilenet_encoders
-from segmentation_models_pytorch.encoders.xception import xception_encoders
-from segmentation_models_pytorch.encoders.timm_efficientnet import timm_efficientnet_encoders
-from segmentation_models_pytorch.encoders.timm_resnest import timm_resnest_encoders
-from segmentation_models_pytorch.encoders.timm_res2net import timm_res2net_encoders
-from segmentation_models_pytorch.encoders.timm_regnet import timm_regnet_encoders
-from segmentation_models_pytorch.encoders.timm_sknet import timm_sknet_encoders
-from segmentation_models_pytorch.encoders.timm_mobilenetv3 import timm_mobilenetv3_encoders
-from segmentation_models_pytorch.encoders.timm_gernet import timm_gernet_encoders
-
-from segmentation_models_pytorch.encoders.timm_universal import TimmUniversalEncoder
-
-# Modified from segmentation_models_pytorch to enable drop_out parameter change
-# Look for "Only change from original code"
-
-encoders = {}
-encoders.update(resnet_encoders)
-encoders.update(dpn_encoders)
-encoders.update(vgg_encoders)
-encoders.update(senet_encoders)
-encoders.update(densenet_encoders)
-encoders.update(inceptionresnetv2_encoders)
-encoders.update(inceptionv4_encoders)
-encoders.update(efficient_net_encoders)
-encoders.update(mobilenet_encoders)
-encoders.update(xception_encoders)
-encoders.update(timm_efficientnet_encoders)
-encoders.update(timm_resnest_encoders)
-encoders.update(timm_res2net_encoders)
-encoders.update(timm_regnet_encoders)
-encoders.update(timm_sknet_encoders)
-encoders.update(timm_mobilenetv3_encoders)
-encoders.update(timm_gernet_encoders)
-
-
-def get_encoder(
-    name, in_channels=3, depth=5, drop_rate=0.2, weights=None, output_stride=32, **kwargs
-):
-    if name.startswith("tu-"):
-        name = name[3:]
-        encoder = TimmUniversalEncoder(
-            name=name,
-            in_channels=in_channels,
-            depth=depth,
-            output_stride=output_stride,
-            pretrained=weights is not None,
-            **kwargs,
-        )
-        return encoder
-
-    try:
-        Encoder = encoders[name]["encoder"]
-    except KeyError:
-        raise KeyError(
-            "Wrong encoder name `{}`, supported encoders: {}".format(name, list(encoders.keys()))
-        )
-
-    params = encoders[name]["params"]
-    params.update(depth=depth)
-
-    # Only change from original code - update drop_rate only if it is in params
-    if "drop_rate" in params:
-        params.update(drop_rate=drop_rate)
-
-    encoder = Encoder(**params)
-
-    if weights is not None:
-        try:
-            settings = encoders[name]["pretrained_settings"][weights]
-        except KeyError:
-            raise KeyError(
-                "Wrong pretrained weights `{}` for encoder `{}`. Available options are: {}".format(
-                    weights,
-                    name,
-                    list(encoders[name]["pretrained_settings"].keys()),
-                )
-            )
-        encoder.load_state_dict(model_zoo.load_url(settings["url"]))
-
-    encoder.set_in_channels(in_channels, pretrained=weights is not None)
-    if output_stride != 32:
-        encoder.make_dilated(output_stride)
-
-    return encoder
+import torch.utils.model_zoo as model_zoo
+
+from segmentation_models_pytorch.encoders.resnet import resnet_encoders
+from segmentation_models_pytorch.encoders.dpn import dpn_encoders
+from segmentation_models_pytorch.encoders.vgg import vgg_encoders
+from segmentation_models_pytorch.encoders.senet import senet_encoders
+from segmentation_models_pytorch.encoders.densenet import densenet_encoders
+from segmentation_models_pytorch.encoders.inceptionresnetv2 import inceptionresnetv2_encoders
+from segmentation_models_pytorch.encoders.inceptionv4 import inceptionv4_encoders
+from segmentation_models_pytorch.encoders.efficientnet import efficient_net_encoders
+from segmentation_models_pytorch.encoders.mobilenet import mobilenet_encoders
+from segmentation_models_pytorch.encoders.xception import xception_encoders
+from segmentation_models_pytorch.encoders.timm_efficientnet import timm_efficientnet_encoders
+from segmentation_models_pytorch.encoders.timm_resnest import timm_resnest_encoders
+from segmentation_models_pytorch.encoders.timm_res2net import timm_res2net_encoders
+from segmentation_models_pytorch.encoders.timm_regnet import timm_regnet_encoders
+from segmentation_models_pytorch.encoders.timm_sknet import timm_sknet_encoders
+from segmentation_models_pytorch.encoders.timm_mobilenetv3 import timm_mobilenetv3_encoders
+from segmentation_models_pytorch.encoders.timm_gernet import timm_gernet_encoders
+
+from segmentation_models_pytorch.encoders.timm_universal import TimmUniversalEncoder
+
+# Modified from segmentation_models_pytorch to enable drop_out parameter change
+# Look for "Only change from original code"
+
+encoders = {}
+encoders.update(resnet_encoders)
+encoders.update(dpn_encoders)
+encoders.update(vgg_encoders)
+encoders.update(senet_encoders)
+encoders.update(densenet_encoders)
+encoders.update(inceptionresnetv2_encoders)
+encoders.update(inceptionv4_encoders)
+encoders.update(efficient_net_encoders)
+encoders.update(mobilenet_encoders)
+encoders.update(xception_encoders)
+encoders.update(timm_efficientnet_encoders)
+encoders.update(timm_resnest_encoders)
+encoders.update(timm_res2net_encoders)
+encoders.update(timm_regnet_encoders)
+encoders.update(timm_sknet_encoders)
+encoders.update(timm_mobilenetv3_encoders)
+encoders.update(timm_gernet_encoders)
+
+
+def get_encoder(
+    name, in_channels=3, depth=5, drop_rate=0.2, weights=None, output_stride=32, **kwargs
+):
+    if name.startswith("tu-"):
+        name = name[3:]
+        encoder = TimmUniversalEncoder(
+            name=name,
+            in_channels=in_channels,
+            depth=depth,
+            output_stride=output_stride,
+            pretrained=weights is not None,
+            **kwargs,
+        )
+        return encoder
+
+    try:
+        Encoder = encoders[name]["encoder"]
+    except KeyError:
+        raise KeyError(
+            "Wrong encoder name `{}`, supported encoders: {}".format(name, list(encoders.keys()))
+        )
+
+    params = encoders[name]["params"]
+    params.update(depth=depth)
+
+    # Only change from original code - update drop_rate only if it is in params
+    if "drop_rate" in params:
+        params.update(drop_rate=drop_rate)
+
+    encoder = Encoder(**params)
+
+    if weights is not None:
+        try:
+            settings = encoders[name]["pretrained_settings"][weights]
+        except KeyError:
+            raise KeyError(
+                "Wrong pretrained weights `{}` for encoder `{}`. Available options are: {}".format(
+                    weights,
+                    name,
+                    list(encoders[name]["pretrained_settings"].keys()),
+                )
+            )
+        encoder.load_state_dict(model_zoo.load_url(settings["url"]))
+
+    encoder.set_in_channels(in_channels, pretrained=weights is not None)
+    if output_stride != 32:
+        encoder.make_dilated(output_stride)
+
+    return encoder
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/model_manager.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/model_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,594 +1,691 @@
-from pathlib import Path
-import warnings
-import datetime
-import json
-import os
-import time
-from typing import Optional
-from matplotlib import pyplot as plt
-import numpy as np
-from skimage import io
-
-import torch
-from torch.utils.tensorboard import SummaryWriter
-from torch.cuda.amp import GradScaler, autocast
-from torch.optim.lr_scheduler import StepLR
-import torch.nn as nn
-from torch.utils.data import DataLoader
-from torch.optim.optimizer import Optimizer
-
-from .utils.training_information import TrainingInformation
-from ..enum import PredictMode
-from ..losses.loss_manager import LossManager
-from ..model_params.base_model_params import BaseModelParams
-from ..data_sets.dataset_output import DatasetOutput
-from ..metrics.abstract_metric import AbstractMetric
-from ..tools import random_sample
-from ..data_loader_generators.data_loader_generator import get_mean_and_std
-from ..display_tools import (
-    display_progress,
-    make_image_tiff_displayable,
-)
-
-
-def adapt_mean_std(mean_std):
-    """
-    Used to read old fashioned mean_std files
-    """
-
-    # If "mean" is already a key, nothing to change
-    if "mean" in mean_std:
-        return mean_std
-
-    # Else, adapt accordingly
-    mean = [mean_std[str(idx)]["mean"] for idx in range(len(mean_std))]
-    std = [mean_std[str(idx)]["std"] for idx in range(len(mean_std))]
-
-    return {"mean": mean, "std": std}
-
-
-class ModelManager:
-    """
-    Class with all useful functions to train, test, ... a CNN-based model
-    """
-
-    def __init__(
-        self, model: nn.Module, params: BaseModelParams, metric_class: type[AbstractMetric]
-    ):
-        # Device to train model
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
-        self.model = model.float()
-        self.model.to(self.device)
-
-        self.params = params
-
-        self.metric_class = metric_class
-
-        self.parameters_path = os.path.join(self.params.models_folder, "parameters.csv")
-
-        # Display current git hash to follow up
-
-        # Used in prediction
-        self.image_index = 0
-        # Used in training
-        self.train_loss_manager = None
-        self.val_loss_manager = None
-        self.lr_scheduler = None
-
-        # Useful information
-        self.dl = {}  # data loaders dictionary
-        self.training_information = TrainingInformation(int(self.params.num_epochs))
-
-        # Tensorboard writer
-        os.makedirs(self.params.tensorboard_folder_path, exist_ok=True)
-        self.writer = SummaryWriter(self.params.tensorboard_folder_path)
-        self.model_save_path = f"{self.params.models_folder}/{self.params.model_save_name}"
-        self.model_save_path_early_stopping = (
-            f"{self.params.models_folder}/early_stopping_{self.params.model_save_name}"
-        )
-
-    def write_images_to_tensorboard(
-        self, current_batch: int, dl_element: DatasetOutput, name: str
-    ) -> None:
-        # Get numpy arrays
-        numpy_dl_element = dl_element.get_numpy_dataset_output()
-
-        # Get images name
-        current_dl_file_names = [
-            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
-        ]
-        image_names = [
-            current_dl_file_names[image_index] for image_index in numpy_dl_element.index
-        ]
-
-        # Log the results images
-        for i, (prediction_np, target_np, image_name) in enumerate(
-            zip(numpy_dl_element.prediction, numpy_dl_element.target, image_names)
-        ):
-            # Do not save too many images
-            if i == self.params.nb_tensorboard_images_max:
-                break
-            for channel in range(target_np.shape[0]):
-                # ... log the ground truth image
-                plt.imshow(target_np[channel], cmap="gray")
-                self.writer.add_figure(
-                    f"{name}/{image_name}/{channel}/groundtruth",
-                    plt.gcf(),
-                    current_batch,
-                )
-
-                plt.imshow(prediction_np[channel], cmap="gray")
-                # ... log the model output image
-                self.writer.add_figure(
-                    f"{name}/{image_name}/{channel}/predicted",
-                    plt.gcf(),
-                    current_batch,
-                )
-
-    def compute_loss(
-        self,
-        dl_element: DatasetOutput,
-        dl_metric: AbstractMetric,
-        loss_manager: Optional[LossManager] = None,
-        _=None,
-    ):
-        inputs = dl_element.input.to(self.device)  # B, C, H, W
-        targets = dl_element.target.to(self.device)
-
-        # Compute the model output
-        predictions = self.model(inputs.float())
-        dl_element.prediction = predictions
-
-        # Update metric
-        dl_metric.update(predictions, targets, dl_element.additional)
-
-        # No need to compute loss if used in test
-        if loss_manager is None:
-            return None
-
-        # Compute loss
-        loss = loss_manager(predictions, targets.float())
-        return loss
-
-    def log_train_progress(self, train_metric: AbstractMetric) -> None:
-        current_batch = self.training_information.get_current_batch()
-        # Graphs
-        plot_step = int(self.params.plot_step)
-        if current_batch % plot_step == plot_step - 1:  # every plot_step mini-batches...
-            # ... log the running loss
-            running_losses = self.train_loss_manager.get_running_losses()
-            for name, loss in running_losses:
-                self.writer.add_scalar(
-                    f"train/{name}",
-                    loss.item() / plot_step,
-                    current_batch,
-                )
-
-            # ... log running metric
-            score, _ = train_metric.get_score()
-            self.writer.add_scalar(f"train/{train_metric.get_name()}", score, current_batch)
-            train_metric.reset()
-
-    def log_val_progress(self, val_metric: AbstractMetric) -> None:
-        current_batch = self.training_information.get_current_batch()
-
-        # ...log the running loss
-        running_losses = self.val_loss_manager.get_running_losses()
-        for name, loss in running_losses:
-            val_dl_length = len(self.dl["val"])
-            self.writer.add_scalar(f"val/{name}", loss.item() / val_dl_length, current_batch)
-
-        # ...log the running metric
-        score, _ = val_metric.get_score()
-        self.writer.add_scalar(f"val/{val_metric.get_name()}", score, current_batch)
-        return score
-
-    def log_images(self, dl_element: DatasetOutput, name: str) -> None:
-        # Get needed training information
-        current_batch = self.training_information.get_current_batch()
-        num_batches_train = self.training_information.num_batches_train
-        batch_index = self.training_information.batch_index
-        epoch = self.training_information.epoch
-
-        epochs_to_plot = np.linspace(
-            1, self.training_information.num_epochs, self.params.nb_plot_images, dtype=int
-        )
-
-        # Condition to apply only for training
-        batch_condition = True if name == "val" else batch_index == num_batches_train - 1
-        if epoch in epochs_to_plot and batch_condition:
-            # Plot last training batch of epoch
-            self.write_images_to_tensorboard(current_batch, dl_element, name)
-
-    def fit_core(self, optimizer: Optimizer) -> None:
-        # Batch information
-        self.training_information.num_batches_train = len(self.dl["train"])
-        best_val_loss, best_val_score = np.Infinity, -np.Infinity
-        model_epoch = -1
-
-        # Create train metric
-        train_metric = self.metric_class(self.device, self.params.nb_classes)
-
-        # Define scaler
-        scaler = GradScaler(enabled=self.params.fp16_precision)
-
-        for epoch in range(self.training_information.num_epochs):
-            self.training_information.epoch = epoch + 1
-            # Enumerate mini batches
-            self.model.train()  # set model to train mode
-            for batch_index, dl_element in enumerate(
-                self.dl["train"]
-            ):  # indexes, inputs, targets, adds
-                self.training_information.batch_index = batch_index + 1
-
-                # Perform training loop
-                with autocast(enabled=self.params.fp16_precision):
-                    loss = self.compute_loss(
-                        dl_element, train_metric, self.train_loss_manager, self.dl["train"]
-                    )
-
-                # Clear the gradients
-                optimizer.zero_grad()
-                # Credit assignment
-                scaler.scale(loss).backward()
-                # Update model weights
-                scaler.step(optimizer)
-                scaler.update()
-
-                # Log progress
-                self.log_train_progress(train_metric)
-                self.log_images(dl_element, "train")
-                display_progress(
-                    "Training in progress",
-                    self.training_information.get_current_batch(),
-                    self.training_information.get_total_batches(),
-                    additional_message=f"Local step {self.training_information.batch_index} | Epoch {self.training_information.epoch}",
-                )
-
-            # Start by lr_scheduler as warmup starts by 0 otherwise
-            self.lr_scheduler.step()
-
-            evaluate = len(self.dl["val"]) > 0
-            val_loss, val_score = 0, 0
-            # If val_dl is not empty then perform evaluation and compute loss
-            if evaluate:
-                val_metric = self.metric_class(self.device, self.params.nb_classes)
-                self.model.eval()  # set model to evaluation mode
-                with torch.no_grad():
-                    for dl_element in self.dl["val"]:
-                        loss = self.compute_loss(
-                            dl_element,
-                            val_metric,
-                            self.val_loss_manager,
-                            self.dl["val"],
-                        )
-                        val_loss += loss
-
-                    # Log progress
-                    val_score = self.log_val_progress(val_metric)
-                    self.log_images(dl_element, "val")
-
-            # Save only if better than current best loss, or if no evaluation is possible
-            if (
-                (not evaluate)
-                or (val_score >= best_val_score)  # best model is model with highest val score
-                or (
-                    val_score == best_val_score and val_loss < best_val_loss
-                )  # or lowest val loss if val score is constant
-            ):
-                torch.save(self.model.state_dict(), self.model_save_path_early_stopping)
-                best_val_loss = val_loss
-                best_val_score = val_score
-                model_epoch = self.training_information.epoch
-
-        # Save model at last epoch
-        torch.save(self.model.state_dict(), self.model_save_path)
-
-        # Best model epoch
-        self.training_information.best_model_epoch = model_epoch
-        print(f"\nBest model saved at epoch {model_epoch}.")
-
-    def compute_and_save_mean_std(self, train_dl: DataLoader, val_dl: DataLoader) -> None:
-        # Compute mean and std
-        data_set_mean_std = get_mean_and_std([train_dl, val_dl])
-
-        # Save in model folder
-        mean_std_file = os.path.join(self.params.models_folder, "mean_std.json")
-        with open(mean_std_file, "w") as write_file:
-            json.dump(data_set_mean_std, write_file, indent=4)
-
-        # Update train and val accordingly
-        train_dl.dataset.mean_std = data_set_mean_std
-        val_dl.dataset.mean_std = data_set_mean_std
-
-    def fit(
-        self,
-        train_dl: DataLoader,
-        val_dl: DataLoader,
-        optimizer: Optimizer,
-        loss_function,
-        lr_scheduler=None,
-    ) -> None:
-        # Create folder to save model
-        os.makedirs(self.params.models_folder, exist_ok=True)
-
-        # Create csv file with all parameters
-        with open(self.parameters_path, "a") as f:
-            for key in self.params.__dict__.keys():
-                f.write("%s;%s\n" % (key, self.params.__dict__[key]))
-        f.close()
-
-        # Compute mean and std of dataset
-        self.compute_and_save_mean_std(train_dl, val_dl)
-
-        if len(train_dl) == 0:
-            raise ValueError("No data to train.")
-
-        # Initialise transforms before prediction
-        train_dl.dataset.initialize_transforms()
-        val_dl.dataset.initialize_transforms()
-
-        # Define data loaders names
-        self.dl["train"] = train_dl
-        self.dl["val"] = val_dl
-
-        # Define lr_scheduler
-        if lr_scheduler is None:
-            self.lr_scheduler = StepLR(optimizer, step_size=1, gamma=1)  # Constant lr
-        else:
-            self.lr_scheduler = lr_scheduler
-
-        # Monitor training time
-        start = time.time()
-
-        # Loss managers initializer
-        if isinstance(loss_function, list):
-            self.train_loss_manager = LossManager(*loss_function)
-            self.val_loss_manager = LossManager(*loss_function)
-        else:
-            self.train_loss_manager = LossManager(loss_function)
-            self.val_loss_manager = LossManager(loss_function)
-
-        # Core fit function with training loop
-        self.fit_core(optimizer)
-
-        self.writer.close()
-        end = time.time()
-
-        # Training time
-        training_time = end - start
-        self.training_information.training_time = training_time
-        print(
-            f"\nTraining successfully finished in {datetime.timedelta(seconds = training_time)}."
-        )
-
-        # Update model with saved one
-        self.model.load_state_dict(torch.load(self.model_save_path))
-
-    def model_prediction(
-        self, dl_element: DatasetOutput, dl_metric: AbstractMetric, data_loader: DataLoader
-    ) -> None:
-        """
-        Function to generate outputs from inputs for given model.
-        By default, does the same thing as compute_loss.
-        """
-        self.compute_loss(dl_element, dl_metric, None, data_loader)
-
-    def save_results(self, name: str, dl_element: DatasetOutput, mean_std) -> None:
-        # Possible target normalization
-        target_mean_std = None
-        # Save inputs, targets & predictions as tiff images
-        for data_image, data_type in zip(
-            [dl_element.input, dl_element.target, dl_element.prediction, dl_element.additional],
-            ["input", "groundtruth", "predicted", "additional"],
-        ):
-            # C, H, W for data_image
-            if data_image is None:  # case when additional data is None
-                continue
-            if data_type == "input" and mean_std is not None:  # input has been normalized
-                # Case where both input and target have been normalized
-                if data_image.shape[0] != len(mean_std["mean"]):
-                    nb_input_channels = (
-                        len(params.c_indexes) * len(params.z_indexes)
-                    )
-                    input_mean_std = {
-                        "mean": mean_std["mean"][:nb_input_channels],
-                        "std": mean_std["std"][:nb_input_channels],
-                    }
-                    target_mean_std = {
-                        "mean": mean_std["mean"][nb_input_channels:],
-                        "std": mean_std["std"][nb_input_channels:],
-                    }
-                else:
-                    input_mean_std = mean_std
-                image_to_save = make_image_tiff_displayable(data_image, input_mean_std)
-            elif data_type in ["groundtruth", "predicted"] and target_mean_std is not None:
-                image_to_save = make_image_tiff_displayable(data_image, target_mean_std)
-            else:
-                image_to_save = make_image_tiff_displayable(data_image, None)
-            with warnings.catch_warnings():
-                warnings.filterwarnings(action="ignore", category=UserWarning)
-                io.imsave(
-                    f"{self.params.output_dir}/{name}_{data_type}.tiff",
-                    image_to_save,
-                )
-
-    def batch_predict(
-        self,
-        test_dl: DataLoader,
-        images_to_save: list[int],
-        num_batches_test: int,
-        test_metric: AbstractMetric,
-        predict_mode: PredictMode,
-    ):
-        all_predictions_np = []
-        for batch_idx, dl_element in enumerate(test_dl):
-            # Reshape in case of multiple images stacked together
-            # Transform shape to (S, C, H, W) to mimic (B, C, H, W)
-            if len(dl_element.input.shape) == 5:  # (B, S, C, H, W) = (1, S, C, H, W)
-                dl_element.input = dl_element.input.view(
-                    *dl_element.input.shape[:0], -1, *dl_element.input.shape[2:]
-                )  # (S, C, H, W)
-                dl_element.target = dl_element.target.view(
-                    *dl_element.target.shape[:0], -1, *dl_element.target.shape[2:]
-                )
-                dl_element.additional = dl_element.additional.view(
-                    *dl_element.additional.shape[:0], -1, *dl_element.additional.shape[2:]
-                )
-
-            # Run prediction
-            self.model_prediction(dl_element, test_metric, test_dl)
-
-            # Get numpy elements
-            dl_element_numpy = dl_element.get_numpy_dataset_output()
-            all_predictions_np = all_predictions_np + [*dl_element_numpy.prediction]
-
-            if predict_mode == PredictMode.Standard and dl_element.target is not None:
-                # Save few images
-                for idx in range(dl_element.target.shape[0]):
-                    if self.image_index in images_to_save:
-                        image_id = (batch_idx * test_dl.batch_size) + idx
-                        image_name = test_dl.dataset.names[image_id].split(".")[0]
-
-                        self.save_results(
-                            f"{image_name}_{self.image_index}",
-                            dl_element_numpy[idx],
-                            test_dl.dataset.mean_std,
-                        )
-                    self.image_index += 1
-
-            display_progress(
-                "Model evaluation in progress",
-                batch_idx + 1,
-                num_batches_test,
-                additional_message=f"Batch #{batch_idx}",
-            )
-
-        return all_predictions_np
-
-    def plot_confusion_matrix(self, _) -> None:
-        # Only used for classification models
-        return
-
-    def read_mean_std(self, test_dl: DataLoader) -> None:
-        # Get mean and standard deviation from saved file
-        # Either from model that have just been trained
-        if os.path.exists(self.params.models_folder):
-            mean_std_path = f"{self.params.models_folder}/mean_std.json"
-        # Or from model that have been loaded from model_load_path
-        else:
-            # mean_std may be saved in parent folders
-            # Iterate over parent folders to find mean_std.json
-            mean_std_path = None
-            potential_paths = [
-                self.params.model_load_path,
-            ] + list(Path(self.params.model_load_path).parents)
-            for parent_folder in potential_paths:
-                mean_std_path = f"{parent_folder}/mean_std.json"
-                if os.path.isfile(mean_std_path):
-                    break
-
-        if os.path.isfile(mean_std_path):
-            with open(mean_std_path, "r") as mean_std_file:
-                raw_mean_std = json.load(mean_std_file)
-                mean_std = adapt_mean_std(raw_mean_std)
-                test_dl.dataset.mean_std = mean_std
-
-    def predict(
-        self,
-        test_dl: DataLoader,
-        predict_mode=PredictMode.Standard,
-        nb_images_to_save=10,
-        compute_own_mean_std=False,
-    ) -> Optional[list]:
-        """
-        Parameters
-        ----------
-        test_dl : DataLoader
-            DataLoader for test set
-        predict_mode : PredictMode, optional
-            By default, do not return predictions
-        nb_images_to_save : int, optional
-            Number of images to save, by default 10
-            nb_images_to_save == -1 => save all images
-
-        """
-
-        # Create folder to save predictions
-        os.makedirs(self.params.output_dir, exist_ok=True)
-
-        # Update test_dl with saved mean and std
-        if compute_own_mean_std:
-            mean_std = get_mean_and_std([test_dl])
-            test_dl.dataset.mean_std = mean_std
-        else:
-            self.read_mean_std(test_dl)
-
-        # Initialise transforms before prediction
-        test_dl.dataset.initialize_transforms()
-
-        self.model.eval()  # Set eval mode for model
-
-        # Create list with images indexes to save predictions, to avoid saving all
-        num_batches_test = len(test_dl)
-        total_images = num_batches_test * test_dl.batch_size
-        if nb_images_to_save == -1:
-            nb_images_to_save = total_images
-        else:
-            nb_images_to_save = min(total_images, nb_images_to_save)
-        images_to_save = random_sample(range(total_images), nb_images_to_save)
-
-        # Reset metric
-        test_metric = self.metric_class(self.device, self.params.nb_classes)
-
-        with torch.no_grad():
-            # Use trained model to predict on test set
-            predictions = self.batch_predict(
-                test_dl, images_to_save, num_batches_test, test_metric, predict_mode
-            )
-
-        if predict_mode != PredictMode.Standard:
-            return predictions
-
-        # Display box plot
-        score, additional_results = test_metric.get_score()
-
-        self.plot_confusion_matrix(additional_results)
-
-        # Compute accuracy
-        accuracy_message = f"Average {test_metric.name}: {round(score, 2)}"
-        print("\n" + accuracy_message)
-        self.training_information.score = score
-
-    def write_useful_information(self) -> None:
-        # Update parameters file with all useful information
-        os.makedirs(self.params.models_folder, exist_ok=True)
-        with open(self.parameters_path, "a") as f:
-            for attribute, value in vars(self.training_information).items():
-                f.write("%s;%s\n" % (attribute, value))
-        f.close()
-
-        if self.params.global_results_path == "":
-            return
-
-        # If global results file does not exist, create it
-        if not os.path.exists(self.params.global_results_path):
-            with open(self.params.global_results_path, "w") as f:
-                f.write(
-                    "model;model id;train set size;val set size;test set size;epochs;learning rate;training_time;score;\n"
-                )
-            f.close()
-
-        # Store useful results in global results file
-        with open(self.params.global_results_path, "a") as f:
-            f.write(f"{self.params.name};")
-            f.write(f"{self.params.format_now};")
-            f.write(f"{self.params.train_number};")
-            f.write(f"{self.params.val_number};")
-            f.write(f"{self.params.test_number};")
-            f.write(f"{self.params.num_epochs};")
-            f.write(f"{self.params.learning_rate};")
-            f.write(f"{self.training_information.training_time};")
-            f.write(f"{self.training_information.score};\n")
-        f.close()
+import math
+from pathlib import Path
+import warnings
+import datetime
+import json
+import os
+import time
+from typing import Optional
+from matplotlib import pyplot as plt
+import numpy as np
+from skimage import io
+from tensorboard.backend.event_processing.event_accumulator import EventAccumulator
+import tensorflow as tf
+
+import torch
+from torch.utils.tensorboard import SummaryWriter
+from torch.cuda.amp import GradScaler, autocast
+from torch.optim.lr_scheduler import StepLR
+import torch.nn as nn
+from torch.utils.data import DataLoader
+from torch.optim.optimizer import Optimizer
+
+from .utils.training_information import TrainingInformation
+from ..enum import PredictMode
+from ..losses.loss_manager import LossManager
+from ..model_params.base_model_params import BaseModelParams
+from ..data_sets.dataset_output import DatasetOutput
+from ..metrics.abstract_metric import AbstractMetric
+from ..tools import extract_patterns, random_sample
+from ..data_loader_generators.data_loader_generator import get_mean_and_std
+from ..display_tools import (
+    display_progress,
+    make_image_tiff_displayable,
+)
+
+
+def adapt_mean_std(mean_std):
+    """
+    Used to read old fashioned mean_std files
+    """
+
+    # If "mean" is already a key, nothing to change
+    if "mean" in mean_std:
+        return mean_std
+
+    # Else, adapt accordingly
+    mean = [mean_std[str(idx)]["mean"] for idx in range(len(mean_std))]
+    std = [mean_std[str(idx)]["std"] for idx in range(len(mean_std))]
+
+    return {"mean": mean, "std": std}
+
+
+class ModelManager:
+    """
+    Class with all useful functions to train, test, ... a CNN-based model
+    """
+
+    def __init__(
+        self,
+        model: nn.Module,
+        params: BaseModelParams,
+        metric_class: type[AbstractMetric],
+    ):
+        # Device to train model
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+        self.model = model.float()
+        self.model.to(self.device)
+
+        self.params = params
+
+        self.metric_class = metric_class
+
+        self.parameters_path = os.path.join(self.params.models_folder, "parameters.csv")
+
+        # Display current git hash to follow up
+
+        # Used in prediction
+        self.image_index = 0
+        # Used in training
+        self.train_loss_manager = None
+        self.val_loss_manager = None
+        self.lr_scheduler = None
+
+        # Useful information
+        self.dl = {}  # data loaders dictionary
+        self.training_information = TrainingInformation(int(self.params.num_epochs))
+
+        # Tensorboard writer
+        os.makedirs(self.params.tensorboard_folder_path, exist_ok=True)
+        self.writer = SummaryWriter(self.params.tensorboard_folder_path)
+        self.model_save_path = (
+            f"{self.params.models_folder}/{self.params.model_save_name}"
+        )
+        self.model_save_path_early_stopping = (
+            f"{self.params.models_folder}/early_stopping_{self.params.model_save_name}"
+        )
+
+    def write_images_to_tensorboard(
+        self, current_batch: int, dl_element: DatasetOutput, name: str
+    ) -> None:
+        # Get numpy arrays
+        numpy_dl_element = dl_element.get_numpy_dataset_output()
+
+        # Get images name
+        current_dl_file_names = [
+            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
+        ]
+        image_names = [
+            current_dl_file_names[image_index] for image_index in numpy_dl_element.index
+        ]
+
+        # Log the results images
+        for i, (prediction_np, target_np, image_name) in enumerate(
+            zip(numpy_dl_element.prediction, numpy_dl_element.target, image_names)
+        ):
+            # Do not save too many images
+            if i == self.params.nb_tensorboard_images_max:
+                break
+            for channel in range(target_np.shape[0]):
+                # ... log the ground truth image
+                plt.imshow(target_np[channel], cmap="gray")
+                self.writer.add_figure(
+                    f"{name}/{image_name}/{channel}/groundtruth",
+                    plt.gcf(),
+                    current_batch,
+                )
+
+                plt.imshow(prediction_np[channel], cmap="gray")
+                # ... log the model output image
+                self.writer.add_figure(
+                    f"{name}/{image_name}/{channel}/predicted",
+                    plt.gcf(),
+                    current_batch,
+                )
+
+    def compute_loss(
+        self,
+        dl_element: DatasetOutput,
+        dl_metric: AbstractMetric,
+        loss_manager: Optional[LossManager] = None,
+        _=None,
+    ):
+        inputs = dl_element.input.to(self.device)  # B, C, H, W
+        targets = dl_element.target.to(self.device)
+
+        # Compute the model output
+        predictions = self.model(inputs.float())
+        dl_element.prediction = predictions
+
+        # Update metric
+        dl_metric.update(predictions, targets, dl_element.additional)
+
+        # No need to compute loss if used in test
+        if loss_manager is None:
+            return None
+
+        # Compute loss
+        loss = loss_manager(predictions, targets.float())
+        return loss
+
+    def log_train_progress(self, train_metric: AbstractMetric) -> None:
+        current_batch = self.training_information.get_current_batch()
+        # Graphs
+        plot_step = int(self.params.plot_step)
+        if (
+            current_batch % plot_step == plot_step - 1
+        ):  # every plot_step mini-batches...
+            # ... log the running loss
+            running_losses = self.train_loss_manager.get_running_losses()
+            for name, loss in running_losses:
+                self.writer.add_scalar(
+                    f"train/{name}",
+                    loss.item() / plot_step,
+                    current_batch,
+                )
+
+            # ... log running metric
+            score, _ = train_metric.get_score()
+            self.writer.add_scalar(
+                f"train/{train_metric.get_name()}", score, current_batch
+            )
+            train_metric.reset()
+
+    def log_val_progress(self, val_metric: AbstractMetric) -> None:
+        current_batch = self.training_information.get_current_batch()
+
+        # ...log the running loss
+        running_losses = self.val_loss_manager.get_running_losses()
+        for name, loss in running_losses:
+            val_dl_length = len(self.dl["val"])
+            self.writer.add_scalar(
+                f"val/{name}", loss.item() / val_dl_length, current_batch
+            )
+
+        # ...log the running metric
+        score, _ = val_metric.get_score()
+        self.writer.add_scalar(f"val/{val_metric.get_name()}", score, current_batch)
+        return score
+
+    def log_images(self, dl_element: DatasetOutput, name: str) -> None:
+        # Get needed training information
+        current_batch = self.training_information.get_current_batch()
+        num_batches_train = self.training_information.num_batches_train
+        batch_index = self.training_information.batch_index
+        epoch = self.training_information.epoch
+
+        epochs_to_plot = np.linspace(
+            1,
+            self.training_information.num_epochs,
+            self.params.nb_plot_images,
+            dtype=int,
+        )
+
+        # Condition to apply only for training
+        batch_condition = (
+            True if name == "val" else batch_index == num_batches_train - 1
+        )
+        if epoch in epochs_to_plot and batch_condition:
+            # Plot last training batch of epoch
+            self.write_images_to_tensorboard(current_batch, dl_element, name)
+
+    def fit_core(self, optimizer: Optimizer) -> None:
+        # Batch information
+        self.training_information.num_batches_train = len(self.dl["train"])
+        best_val_loss, best_val_score = np.Infinity, -np.Infinity
+        model_epoch = -1
+
+        # Create train metric
+        train_metric = self.metric_class(self.device, self.params.nb_classes)
+
+        # Define scaler
+        scaler = GradScaler(enabled=self.params.fp16_precision)
+
+        for epoch in range(self.training_information.num_epochs):
+            self.training_information.epoch = epoch + 1
+            # Enumerate mini batches
+            self.model.train()  # set model to train mode
+            for batch_index, dl_element in enumerate(
+                self.dl["train"]
+            ):  # indexes, inputs, targets, adds
+                self.training_information.batch_index = batch_index + 1
+
+                # Perform training loop
+                with autocast(enabled=self.params.fp16_precision):
+                    loss = self.compute_loss(
+                        dl_element,
+                        train_metric,
+                        self.train_loss_manager,
+                        self.dl["train"],
+                    )
+
+                # Clear the gradients
+                optimizer.zero_grad()
+                # Credit assignment
+                scaler.scale(loss).backward()
+                # Update model weights
+                scaler.step(optimizer)
+                scaler.update()
+
+                # Log progress
+                self.log_train_progress(train_metric)
+                self.log_images(dl_element, "train")
+                display_progress(
+                    "Training in progress",
+                    self.training_information.get_current_batch(),
+                    self.training_information.get_total_batches(),
+                    additional_message=f"Local step {self.training_information.batch_index} | Epoch {self.training_information.epoch}",
+                )
+
+            # Start by lr_scheduler as warmup starts by 0 otherwise
+            self.lr_scheduler.step()
+
+            evaluate = len(self.dl["val"]) > 0
+            val_loss, val_score = 0, 0
+            # If val_dl is not empty then perform evaluation and compute loss
+            if evaluate:
+                val_metric = self.metric_class(self.device, self.params.nb_classes)
+                self.model.eval()  # set model to evaluation mode
+                with torch.no_grad():
+                    for dl_element in self.dl["val"]:
+                        loss = self.compute_loss(
+                            dl_element,
+                            val_metric,
+                            self.val_loss_manager,
+                            self.dl["val"],
+                        )
+                        val_loss += loss
+
+                    # Log progress
+                    val_score = self.log_val_progress(val_metric)
+                    self.log_images(dl_element, "val")
+
+            # Save only if better than current best loss, or if no evaluation is possible
+            if (
+                (not evaluate)
+                or (
+                    val_score >= best_val_score
+                )  # best model is model with highest val score
+                or (
+                    val_score == best_val_score and val_loss < best_val_loss
+                )  # or lowest val loss if val score is constant
+            ):
+                torch.save(self.model.state_dict(), self.model_save_path_early_stopping)
+                best_val_loss = val_loss
+                best_val_score = val_score
+                model_epoch = self.training_information.epoch
+
+        # Save model at last epoch
+        torch.save(self.model.state_dict(), self.model_save_path)
+
+        # Best model epoch
+        self.training_information.best_model_epoch = model_epoch
+        print(f"\nBest model saved at epoch {model_epoch}.")
+
+    def compute_and_save_mean_std(
+        self, train_dl: DataLoader, val_dl: DataLoader
+    ) -> dict[str, list[float]]:
+        """
+        Compute mean and std.
+        """
+        data_set_mean_std = get_mean_and_std([train_dl, val_dl])
+
+        # Save in model folder
+        mean_std_file = os.path.join(self.params.models_folder, "mean_std.json")
+        with open(mean_std_file, "w") as write_file:
+            json.dump(data_set_mean_std, write_file, indent=4)
+
+        # Update train and val accordingly
+        train_dl.dataset.mean_std = data_set_mean_std
+        val_dl.dataset.mean_std = data_set_mean_std
+
+        return data_set_mean_std
+
+    def fit(
+        self,
+        train_dl: DataLoader,
+        val_dl: DataLoader,
+        optimizer: Optimizer,
+        loss_function,
+        lr_scheduler=None,
+    ) -> None:
+        # Create folder to save model
+        os.makedirs(self.params.models_folder, exist_ok=True)
+
+        # Create csv file with all parameters
+        with open(self.parameters_path, "a") as f:
+            for key in self.params.__dict__.keys():
+                f.write("%s;%s\n" % (key, self.params.__dict__[key]))
+        f.close()
+
+        # Compute mean and std of dataset
+        self.compute_and_save_mean_std(train_dl, val_dl)
+
+        if len(train_dl) == 0:
+            raise ValueError("No data to train.")
+
+        # Initialise transforms before prediction
+        train_dl.dataset.initialize_transforms()
+        val_dl.dataset.initialize_transforms()
+
+        # Define data loaders names
+        self.dl["train"] = train_dl
+        self.dl["val"] = val_dl
+
+        # Define lr_scheduler
+        if lr_scheduler is None:
+            self.lr_scheduler = StepLR(optimizer, step_size=1, gamma=1)  # Constant lr
+        else:
+            self.lr_scheduler = lr_scheduler
+
+        # Monitor training time
+        start = time.time()
+
+        # Loss managers initializer
+        if isinstance(loss_function, list):
+            self.train_loss_manager = LossManager(*loss_function)
+            self.val_loss_manager = LossManager(*loss_function)
+        else:
+            self.train_loss_manager = LossManager(loss_function)
+            self.val_loss_manager = LossManager(loss_function)
+
+        # Core fit function with training loop
+        self.fit_core(optimizer)
+
+        self.writer.close()
+        end = time.time()
+
+        # Training time
+        training_time = end - start
+        self.training_information.training_time = training_time
+        print(
+            f"\nTraining successfully finished in {datetime.timedelta(seconds = training_time)}."
+        )
+
+        # Update model with saved one
+        self.model.load_state_dict(torch.load(self.model_save_path))
+
+    def model_prediction(
+        self,
+        dl_element: DatasetOutput,
+        dl_metric: AbstractMetric,
+        data_loader: DataLoader,
+    ) -> None:
+        """
+        Function to generate outputs from inputs for given model.
+        By default, does the same thing as compute_loss.
+        """
+        self.compute_loss(dl_element, dl_metric, None, data_loader)
+
+    def save_results(self, name: str, dl_element: DatasetOutput, mean_std) -> None:
+        # Possible target normalization
+        target_mean_std = None
+        # Save inputs, targets & predictions as tiff images
+        for data_image, data_type in zip(
+            [
+                dl_element.input,
+                dl_element.target,
+                dl_element.prediction,
+                dl_element.additional,
+            ],
+            ["input", "groundtruth", "predicted", "additional"],
+        ):
+            # C, H, W for data_image
+            if data_image is None:  # case when additional data is None
+                continue
+            if (
+                data_type == "input" and mean_std is not None
+            ):  # input has been normalized
+                # Case where both input and target have been normalized
+                if data_image.shape[0] != len(mean_std["mean"]):
+                    nb_input_channels = len(self.params.c_indexes) * len(
+                        self.params.z_indexes
+                    )
+                    input_mean_std = {
+                        "mean": mean_std["mean"][:nb_input_channels],
+                        "std": mean_std["std"][:nb_input_channels],
+                    }
+                    target_mean_std = {
+                        "mean": mean_std["mean"][nb_input_channels:],
+                        "std": mean_std["std"][nb_input_channels:],
+                    }
+                else:
+                    input_mean_std = mean_std
+                image_to_save = make_image_tiff_displayable(data_image, input_mean_std)
+            elif (
+                data_type in ["groundtruth", "predicted"]
+                and target_mean_std is not None
+            ):
+                image_to_save = make_image_tiff_displayable(data_image, target_mean_std)
+            else:
+                image_to_save = make_image_tiff_displayable(data_image, None)
+            if len(image_to_save) == 0:  # protect against empty image
+                continue
+            with warnings.catch_warnings():
+                warnings.filterwarnings(action="ignore", category=UserWarning)
+                io.imsave(
+                    f"{self.params.output_dir}/{name}_{data_type}.tiff",
+                    image_to_save,
+                )
+
+    def batch_predict(
+        self,
+        test_dl: DataLoader,
+        images_to_save: list[int],
+        num_batches_test: int,
+        test_metric: AbstractMetric,
+        predict_mode: PredictMode,
+    ):
+        all_predictions_np = []
+        for batch_idx, dl_element in enumerate(test_dl):
+            # Reshape in case of multiple images stacked together
+            # Transform shape to (S, C, H, W) to mimic (B, C, H, W)
+            if len(dl_element.input.shape) == 5:  # (B, S, C, H, W) = (1, S, C, H, W)
+                dl_element.input = dl_element.input.view(
+                    *dl_element.input.shape[:0], -1, *dl_element.input.shape[2:]
+                )  # (S, C, H, W)
+                dl_element.target = dl_element.target.view(
+                    *dl_element.target.shape[:0], -1, *dl_element.target.shape[2:]
+                )
+                dl_element.additional = dl_element.additional.view(
+                    *dl_element.additional.shape[:0],
+                    -1,
+                    *dl_element.additional.shape[2:],
+                )
+
+            # Run prediction
+            self.model_prediction(dl_element, test_metric, test_dl)
+
+            # Get numpy elements
+            dl_element_numpy = dl_element.get_numpy_dataset_output()
+            all_predictions_np = all_predictions_np + [*dl_element_numpy.prediction]
+
+            if predict_mode == PredictMode.Standard and dl_element.target is not None:
+                # Save few images
+                for idx in range(dl_element.target.shape[0]):
+                    if self.image_index in images_to_save:
+                        image_id = (batch_idx * test_dl.batch_size) + idx
+                        image_name = test_dl.dataset.names[image_id].split(".")[0]
+
+                        self.save_results(
+                            f"{image_name}_{self.image_index}",
+                            dl_element_numpy[idx],
+                            test_dl.dataset.mean_std,
+                        )
+                    self.image_index += 1
+
+            display_progress(
+                "Model evaluation in progress",
+                batch_idx + 1,
+                num_batches_test,
+                additional_message=f"Batch #{batch_idx}",
+            )
+
+        return all_predictions_np
+
+    def plot_confusion_matrix(self, _) -> None:
+        # Only used for classification models
+        return
+
+    def read_mean_std(self, test_dl: DataLoader) -> None:
+        # Get mean and standard deviation from saved file
+        # Either from model that have just been trained
+        if os.path.exists(self.params.models_folder):
+            mean_std_path = f"{self.params.models_folder}/mean_std.json"
+        # Or from model that have been loaded from model_load_path
+        else:
+            # mean_std may be saved in parent folders
+            # Iterate over parent folders to find mean_std.json
+            mean_std_path = None
+            potential_paths = [
+                self.params.model_load_path,
+            ] + list(Path(self.params.model_load_path).parents)
+            for parent_folder in potential_paths:
+                mean_std_path = f"{parent_folder}/mean_std.json"
+                if os.path.isfile(mean_std_path):
+                    break
+
+        if os.path.isfile(mean_std_path):
+            with open(mean_std_path, "r") as mean_std_file:
+                raw_mean_std = json.load(mean_std_file)
+                mean_std = adapt_mean_std(raw_mean_std)
+                test_dl.dataset.mean_std = mean_std
+
+    def predict(
+        self,
+        test_dl: DataLoader,
+        predict_mode=PredictMode.Standard,
+        nb_images_to_save=10,
+        compute_own_mean_std=False,
+    ) -> Optional[list]:
+        """
+        Parameters
+        ----------
+        test_dl : DataLoader
+            DataLoader for test set
+        predict_mode : PredictMode, optional
+            By default, do not return predictions
+        nb_images_to_save : int, optional
+            Number of images to save, by default 10
+            nb_images_to_save == -1 => save all images
+
+        """
+
+        # Create folder to save predictions
+        os.makedirs(self.params.output_dir, exist_ok=True)
+
+        # Update test_dl with saved mean and std
+        if compute_own_mean_std:
+            mean_std = get_mean_and_std([test_dl])
+            test_dl.dataset.mean_std = mean_std
+        else:
+            self.read_mean_std(test_dl)
+
+        # Initialise transforms before prediction
+        test_dl.dataset.initialize_transforms()
+
+        self.model.eval()  # Set eval mode for model
+
+        # Create list with images indexes to save predictions, to avoid saving all
+        num_batches_test = len(test_dl)
+        total_images = num_batches_test * test_dl.batch_size
+        if nb_images_to_save == -1:
+            nb_images_to_save = total_images
+        else:
+            nb_images_to_save = min(total_images, nb_images_to_save)
+        images_to_save = random_sample(range(total_images), nb_images_to_save)
+
+        # Reset metric
+        test_metric = self.metric_class(self.device, self.params.nb_classes)
+
+        with torch.no_grad():
+            # Use trained model to predict on test set
+            predictions = self.batch_predict(
+                test_dl, images_to_save, num_batches_test, test_metric, predict_mode
+            )
+
+        if predict_mode != PredictMode.Standard:
+            return predictions
+
+        # Display box plot
+        score, additional_results = test_metric.get_score()
+
+        self.plot_confusion_matrix(additional_results)
+
+        # Compute accuracy
+        accuracy_message = f"Average {test_metric.name}: {round(score, 2)}"
+        print("\n" + accuracy_message)
+        self.training_information.score = score
+
+    def write_useful_information(self) -> None:
+        # Update parameters file with all useful information
+        os.makedirs(self.params.models_folder, exist_ok=True)
+        with open(self.parameters_path, "a") as f:
+            for attribute, value in vars(self.training_information).items():
+                f.write("%s;%s\n" % (attribute, value))
+        f.close()
+
+        if self.params.global_results_path == "":
+            return
+
+        # If global results file does not exist, create it
+        if not os.path.exists(self.params.global_results_path):
+            with open(self.params.global_results_path, "w") as f:
+                f.write(
+                    "model;model id;train set size;val set size;test set size;epochs;learning rate;training_time;score;\n"
+                )
+            f.close()
+
+        # Store useful results in global results file
+        with open(self.params.global_results_path, "a") as f:
+            f.write(f"{self.params.name};")
+            f.write(f"{self.params.format_now};")
+            f.write(f"{self.params.train_number};")
+            f.write(f"{self.params.val_number};")
+            f.write(f"{self.params.test_number};")
+            f.write(f"{self.params.num_epochs};")
+            f.write(f"{self.params.learning_rate};")
+            f.write(f"{self.training_information.training_time};")
+            f.write(f"{self.training_information.score};\n")
+        f.close()
+
+    def display_training_curves(self):
+        """
+        Show tensorboard curves in a matplotlib figure.
+        """
+        event_acc = EventAccumulator(self.params.tensorboard_folder_path)
+        event_acc.Reload()
+        scalar_tags = event_acc.Tags()["scalars"]
+
+        fig = plt.figure(figsize=(12, 12))
+
+        nb_columns = 2
+        nb_lines = math.ceil(len(scalar_tags) / nb_columns)
+        for idx, scalar_tag in enumerate(scalar_tags):
+            _, step_nums, vals = zip(*event_acc.Scalars(scalar_tag))
+            ax = fig.add_subplot(nb_lines, nb_columns, idx + 1)
+            ax.plot(step_nums, vals)
+            ax.set_title(scalar_tag)
+            ax.set_xlabel("Steps")
+
+        plt.show()
+
+    def display_training_images(self, patterns: Optional[list[str]] = None):
+        """
+        Show tensorboard images in a matplotlib figure.
+        Plot first 8 images, last printed to tensorboard.
+        """
+        if patterns is None:
+            patterns = ["val*"]
+
+        event_acc = EventAccumulator(self.params.tensorboard_folder_path)
+        event_acc.Reload()
+        image_tags = event_acc.Tags()["images"]
+        filtered_images_tags = extract_patterns(image_tags, patterns)
+
+        fig = plt.figure(figsize=(4, 6))
+
+        for idx, image_tag in enumerate(filtered_images_tags):
+            if idx == 6:
+                break
+            is_ground_truth = idx % 2 == 0
+            _, _, encoded_string, _, _ = zip(*event_acc.Images(image_tag))
+            # -1 for last image (most recent)
+            image = tf.image.decode_image(encoded_string[-1], channels=1).numpy()
+            ax = fig.add_subplot(3, 2, idx + 1)
+            ax.imshow(image, cmap="gray")
+            ax.axis("off")
+            ax.set_title("Ground truth mask" if is_ground_truth else "Predicted mask")
+
+        plt.show()
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/utils/custom_get_encoder.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/utils/custom_get_encoder.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import torch.utils.model_zoo as model_zoo
-
-from segmentation_models_pytorch.encoders.resnet import resnet_encoders
-from segmentation_models_pytorch.encoders.dpn import dpn_encoders
-from segmentation_models_pytorch.encoders.vgg import vgg_encoders
-from segmentation_models_pytorch.encoders.senet import senet_encoders
-from segmentation_models_pytorch.encoders.densenet import densenet_encoders
-from segmentation_models_pytorch.encoders.inceptionresnetv2 import inceptionresnetv2_encoders
-from segmentation_models_pytorch.encoders.inceptionv4 import inceptionv4_encoders
-from segmentation_models_pytorch.encoders.efficientnet import efficient_net_encoders
-from segmentation_models_pytorch.encoders.mobilenet import mobilenet_encoders
-from segmentation_models_pytorch.encoders.xception import xception_encoders
-from segmentation_models_pytorch.encoders.timm_efficientnet import timm_efficientnet_encoders
-from segmentation_models_pytorch.encoders.timm_resnest import timm_resnest_encoders
-from segmentation_models_pytorch.encoders.timm_res2net import timm_res2net_encoders
-from segmentation_models_pytorch.encoders.timm_regnet import timm_regnet_encoders
-from segmentation_models_pytorch.encoders.timm_sknet import timm_sknet_encoders
-from segmentation_models_pytorch.encoders.timm_mobilenetv3 import timm_mobilenetv3_encoders
-from segmentation_models_pytorch.encoders.timm_gernet import timm_gernet_encoders
-
-from segmentation_models_pytorch.encoders.timm_universal import TimmUniversalEncoder
-
-# Modified from segmentation_models_pytorch to enable drop_out parameter change 
-# Look for "Only change from original code" 
-
-encoders = {}
-encoders.update(resnet_encoders)
-encoders.update(dpn_encoders)
-encoders.update(vgg_encoders)
-encoders.update(senet_encoders)
-encoders.update(densenet_encoders)
-encoders.update(inceptionresnetv2_encoders)
-encoders.update(inceptionv4_encoders)
-encoders.update(efficient_net_encoders)
-encoders.update(mobilenet_encoders)
-encoders.update(xception_encoders)
-encoders.update(timm_efficientnet_encoders)
-encoders.update(timm_resnest_encoders)
-encoders.update(timm_res2net_encoders)
-encoders.update(timm_regnet_encoders)
-encoders.update(timm_sknet_encoders)
-encoders.update(timm_mobilenetv3_encoders)
-encoders.update(timm_gernet_encoders)
-
-
-def get_encoder(
-    name, in_channels=3, depth=5, drop_rate=0.2, weights=None, output_stride=32, **kwargs
-):
-
-    if name.startswith("tu-"):
-        name = name[3:]
-        encoder = TimmUniversalEncoder(
-            name=name,
-            in_channels=in_channels,
-            depth=depth,
-            output_stride=output_stride,
-            pretrained=weights is not None,
-            **kwargs,
-        )
-        return encoder
-
-    try:
-        Encoder = encoders[name]["encoder"]
-    except KeyError:
-        raise KeyError(
-            "Wrong encoder name `{}`, supported encoders: {}".format(name, list(encoders.keys()))
-        )
-
-    params = encoders[name]["params"]
-    params.update(depth=depth)
-
-    # Only change from original code - update drop_rate only if it is in params
-    if "drop_rate" in params:
-        params.update(drop_rate=drop_rate)
-
-    encoder = Encoder(**params)
-
-    if weights is not None:
-        try:
-            settings = encoders[name]["pretrained_settings"][weights]
-        except KeyError:
-            raise KeyError(
-                "Wrong pretrained weights `{}` for encoder `{}`. Available options are: {}".format(
-                    weights, name, list(encoders[name]["pretrained_settings"].keys()),
-                )
-            )
-        encoder.load_state_dict(model_zoo.load_url(settings["url"]))
-
-    encoder.set_in_channels(in_channels, pretrained=weights is not None)
-    if output_stride != 32:
-        encoder.make_dilated(output_stride)
-
-    return encoder
+import torch.utils.model_zoo as model_zoo
+
+from segmentation_models_pytorch.encoders.resnet import resnet_encoders
+from segmentation_models_pytorch.encoders.dpn import dpn_encoders
+from segmentation_models_pytorch.encoders.vgg import vgg_encoders
+from segmentation_models_pytorch.encoders.senet import senet_encoders
+from segmentation_models_pytorch.encoders.densenet import densenet_encoders
+from segmentation_models_pytorch.encoders.inceptionresnetv2 import inceptionresnetv2_encoders
+from segmentation_models_pytorch.encoders.inceptionv4 import inceptionv4_encoders
+from segmentation_models_pytorch.encoders.efficientnet import efficient_net_encoders
+from segmentation_models_pytorch.encoders.mobilenet import mobilenet_encoders
+from segmentation_models_pytorch.encoders.xception import xception_encoders
+from segmentation_models_pytorch.encoders.timm_efficientnet import timm_efficientnet_encoders
+from segmentation_models_pytorch.encoders.timm_resnest import timm_resnest_encoders
+from segmentation_models_pytorch.encoders.timm_res2net import timm_res2net_encoders
+from segmentation_models_pytorch.encoders.timm_regnet import timm_regnet_encoders
+from segmentation_models_pytorch.encoders.timm_sknet import timm_sknet_encoders
+from segmentation_models_pytorch.encoders.timm_mobilenetv3 import timm_mobilenetv3_encoders
+from segmentation_models_pytorch.encoders.timm_gernet import timm_gernet_encoders
+
+from segmentation_models_pytorch.encoders.timm_universal import TimmUniversalEncoder
+
+# Modified from segmentation_models_pytorch to enable drop_out parameter change 
+# Look for "Only change from original code" 
+
+encoders = {}
+encoders.update(resnet_encoders)
+encoders.update(dpn_encoders)
+encoders.update(vgg_encoders)
+encoders.update(senet_encoders)
+encoders.update(densenet_encoders)
+encoders.update(inceptionresnetv2_encoders)
+encoders.update(inceptionv4_encoders)
+encoders.update(efficient_net_encoders)
+encoders.update(mobilenet_encoders)
+encoders.update(xception_encoders)
+encoders.update(timm_efficientnet_encoders)
+encoders.update(timm_resnest_encoders)
+encoders.update(timm_res2net_encoders)
+encoders.update(timm_regnet_encoders)
+encoders.update(timm_sknet_encoders)
+encoders.update(timm_mobilenetv3_encoders)
+encoders.update(timm_gernet_encoders)
+
+
+def get_encoder(
+    name, in_channels=3, depth=5, drop_rate=0.2, weights=None, output_stride=32, **kwargs
+):
+
+    if name.startswith("tu-"):
+        name = name[3:]
+        encoder = TimmUniversalEncoder(
+            name=name,
+            in_channels=in_channels,
+            depth=depth,
+            output_stride=output_stride,
+            pretrained=weights is not None,
+            **kwargs,
+        )
+        return encoder
+
+    try:
+        Encoder = encoders[name]["encoder"]
+    except KeyError:
+        raise KeyError(
+            "Wrong encoder name `{}`, supported encoders: {}".format(name, list(encoders.keys()))
+        )
+
+    params = encoders[name]["params"]
+    params.update(depth=depth)
+
+    # Only change from original code - update drop_rate only if it is in params
+    if "drop_rate" in params:
+        params.update(drop_rate=drop_rate)
+
+    encoder = Encoder(**params)
+
+    if weights is not None:
+        try:
+            settings = encoders[name]["pretrained_settings"][weights]
+        except KeyError:
+            raise KeyError(
+                "Wrong pretrained weights `{}` for encoder `{}`. Available options are: {}".format(
+                    weights, name, list(encoders[name]["pretrained_settings"].keys()),
+                )
+            )
+        encoder.load_state_dict(model_zoo.load_url(settings["url"]))
+
+    encoder.set_in_channels(in_channels, pretrained=weights is not None)
+    if output_stride != 32:
+        encoder.make_dilated(output_stride)
+
+    return encoder
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/utils/training_information.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/utils/training_information.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from pathlib import Path
-
-
-class TrainingInformation:
-    """
-    Class to store training information.
-    """
-
-    def __init__(self, num_epochs: int) -> None:
-        # Global parameters
-        self.num_batches_train = None
-        self.num_epochs = num_epochs
-
-        # Training follow-up
-        self.epoch = 1  # starts at 1
-        self.batch_index = 1  # starts at 1
-        self.best_model_epoch = None
-        self.training_time = 0
-        self.score = None
-        self.additional_score = None
-
-        # Get git hash
-        try:
-            import git
-
-            current_file_path = Path(__file__).parent.resolve()
-            repo = git.Repo(current_file_path, search_parent_directories=True)
-            self.git_hash = repo.head.object.hexsha
-            print(f"Current commit hash: {self.git_hash}")
-        except:  # if not a git repository
-            self.git_hash = "unknown"
-
-    def check_validity(self) -> None:
-        if self.num_batches_train is None:
-            raise ValueError("Number of batches is not defined yet")
-
-    def get_total_batches(self) -> int:
-        self.check_validity()
-        return self.num_batches_train * self.num_epochs
-
-    def get_current_batch(self) -> int:
-        self.check_validity()
-        return (self.epoch - 1) * self.num_batches_train + self.batch_index
+from pathlib import Path
+
+
+class TrainingInformation:
+    """
+    Class to store training information.
+    """
+
+    def __init__(self, num_epochs: int) -> None:
+        # Global parameters
+        self.num_batches_train = None
+        self.num_epochs = num_epochs
+
+        # Training follow-up
+        self.epoch = 1  # starts at 1
+        self.batch_index = 1  # starts at 1
+        self.best_model_epoch = None
+        self.training_time = 0
+        self.score = None
+        self.additional_score = None
+
+        # Get git hash
+        try:
+            import git
+
+            current_file_path = Path(__file__).parent.resolve()
+            repo = git.Repo(current_file_path, search_parent_directories=True)
+            self.git_hash = repo.head.object.hexsha
+            print(f"Current commit hash: {self.git_hash}")
+        except:  # if not a git repository
+            self.git_hash = "unknown"
+
+    def check_validity(self) -> None:
+        if self.num_batches_train is None:
+            raise ValueError("Number of batches is not defined yet")
+
+    def get_total_batches(self) -> int:
+        self.check_validity()
+        return self.num_batches_train * self.num_epochs
+
+    def get_current_batch(self) -> int:
+        self.check_validity()
+        return (self.epoch - 1) * self.num_batches_train + self.batch_index
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_managers/vae_model_manager.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_managers/vae_model_manager.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import os
-from matplotlib import pyplot as plt
-
-from ..enum import PredictMode
-from ..data_sets.dataset_output import DatasetOutput
-from ..display_tools import display_progress
-from .model_manager import ModelManager
-
-
-class VAEModelManager(ModelManager):
-    def compute_loss(self, dl_element, dl_metric, _=None, __=None):
-        # Read data loader element
-        dl_element["data"] = dl_element["data"].to(self.device)
-        dl_element["category"] = dl_element["category"].to(self.device)
-
-        # Compute the model output
-        model_output = self.model(dl_element)
-        dl_element.prediction = model_output["recon_x"]
-
-        # Update metric
-        dl_metric.update(model_output["recon_x"], dl_element["data"])
-
-        return model_output["loss"]
-
-    def model_prediction(self, dl_element, dl_metric, _):
-        """
-        Function to generate outputs from inputs for given model.
-        """
-        # Read data loader element
-        dl_element["data"] = dl_element["data"].to(self.device)
-        dl_element["category"] = dl_element["category"].to(self.device)
-
-        # Compute the model output
-        model_output = self.model(dl_element)
-        dl_element.prediction = model_output
-
-        # Update metric
-        dl_metric.update(model_output["recon_x"], dl_element["data"])
-
-    def get_embedding(self, dl_element):
-        dl_element["data"] = dl_element["data"].to(self.device)
-        return self.model.encoder(dl_element["data"]).embedding
-
-    def batch_predict(
-        self, test_dl, images_to_save, num_batches_test, test_metric, predict_mode: PredictMode
-    ):
-        all_predictions_np = []
-        for batch_idx, dl_element in enumerate(test_dl):
-            # Run prediction
-            if predict_mode == PredictMode.Standard:  # standard use
-                self.model_prediction(dl_element, test_metric, test_dl)
-                predictions = dl_element.prediction["recon_x"]
-            else:  # return embedding
-                predictions = self.get_embedding(dl_element)
-
-            predictions_np = predictions.cpu().numpy()
-            all_predictions_np = all_predictions_np + [*predictions_np]
-
-            display_progress(
-                "Model evaluation in progress",
-                batch_idx + 1,
-                num_batches_test,
-                additional_message=f"Batch #{batch_idx}",
-            )
-
-            # Save few images
-            if predict_mode != PredictMode.Standard:
-                continue
-
-            # Get numpy elements
-            inputs_np = dl_element["data"].cpu().numpy()
-
-            for idx in range(dl_element["data"].shape[0]):
-                if self.image_index in images_to_save:
-                    image_id = (batch_idx * test_dl.batch_size) + idx
-                    image_name = test_dl.dataset.names[image_id].split(".")[0]
-
-                    # Get element at index
-                    input_np = inputs_np[idx, ...].squeeze()
-                    prediction_np = predictions_np[idx, ...].squeeze()
-
-                    dl_element_numpy = DatasetOutput(
-                        input=input_np,
-                        prediction=prediction_np,
-                    )
-
-                    self.save_results(
-                        f"{image_name}_{self.image_index}",
-                        dl_element_numpy,
-                        test_dl.dataset.mean_std,
-                    )
-
-                self.image_index += 1
-
-        return all_predictions_np
-
-    def write_useful_information(self):
-        # Update parameters file with all useful information
-        os.makedirs(self.params.models_folder, exist_ok=True)
-        with open(self.parameters_path, "a") as f:
-            for attribute, value in vars(self.training_information).items():
-                f.write("%s;%s\n" % (attribute, value))
-        f.close()
-
-        if self.params.global_results_path == "":
-            return
-
-        # If global results file does not exist, create it
-        if not os.path.exists(self.params.global_results_path):
-            with open(self.params.global_results_path, "w") as f:
-                f.write(
-                    "data;id;latent dim;learning rate;beta;gamma;delta;git hash;score;weight_decay;batch size;drop out;encoder name;additional score\n"
-                )
-            f.close()
-
-        # Store useful results in global results file
-        with open(self.params.global_results_path, "a") as f:
-            f.write(f"{self.params.data_dir};")
-            f.write(f"{self.params.format_now};")
-            f.write(f"{self.params.latent_dim};")
-            f.write(f"{self.params.learning_rate};")
-            f.write(f"{self.params.beta};")
-            f.write(f"{self.params.gamma};")
-            f.write(f"{self.params.delta};")
-            f.write(f"{self.training_information.git_hash};")
-            f.write(f"{self.training_information.score};")
-            f.write(f"{self.params.weight_decay};")
-            f.write(f"{self.params.batch_size};")
-            f.write(f"{self.params.dropout};")
-            f.write(f"{self.params.encoder_name};")
-            f.write(f"{self.training_information.additional_score};\n")
-        f.close()
-
-    def write_images_to_tensorboard(self, current_batch, dl_element, name):
-        # Get numpy arrays
-        inputs_np = dl_element["data"]
-        image_indexes_np = dl_element["id"]
-
-        # Get images name
-        current_dl_file_names = [
-            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
-        ]
-        image_names = [current_dl_file_names[image_index] for image_index in image_indexes_np]
-
-        # Log the results images
-        for i, (input_np, image_name) in enumerate(zip(inputs_np, image_names)):
-            # Do not save too many images
-            if i == self.params.nb_tensorboard_images_max:
-                break
-            for channel in range(input_np.shape[0]):
-                # ... log the ground truth image
-                plt.imshow(input_np[channel], cmap="gray")
-                self.writer.add_figure(
-                    f"{name}/{image_name}/{channel}/input",
-                    plt.gcf(),
-                    current_batch,
-                )
+import os
+from matplotlib import pyplot as plt
+
+from ..enum import PredictMode
+from ..data_sets.dataset_output import DatasetOutput
+from ..display_tools import display_progress
+from .model_manager import ModelManager
+
+
+class VAEModelManager(ModelManager):
+    def compute_loss(self, dl_element, dl_metric, _=None, __=None):
+        # Read data loader element
+        dl_element["data"] = dl_element["data"].to(self.device)
+        dl_element["category"] = dl_element["category"].to(self.device)
+
+        # Compute the model output
+        model_output = self.model(dl_element)
+        dl_element.prediction = model_output["recon_x"]
+
+        # Update metric
+        dl_metric.update(model_output["recon_x"], dl_element["data"])
+
+        return model_output["loss"]
+
+    def model_prediction(self, dl_element, dl_metric, _):
+        """
+        Function to generate outputs from inputs for given model.
+        """
+        # Read data loader element
+        dl_element["data"] = dl_element["data"].to(self.device)
+        dl_element["category"] = dl_element["category"].to(self.device)
+
+        # Compute the model output
+        model_output = self.model(dl_element)
+        dl_element.prediction = model_output
+
+        # Update metric
+        dl_metric.update(model_output["recon_x"], dl_element["data"])
+
+    def get_embedding(self, dl_element):
+        dl_element["data"] = dl_element["data"].to(self.device)
+        return self.model.encoder(dl_element["data"]).embedding
+
+    def batch_predict(
+        self, test_dl, images_to_save, num_batches_test, test_metric, predict_mode: PredictMode
+    ):
+        all_predictions_np = []
+        for batch_idx, dl_element in enumerate(test_dl):
+            # Run prediction
+            if predict_mode == PredictMode.Standard:  # standard use
+                self.model_prediction(dl_element, test_metric, test_dl)
+                predictions = dl_element.prediction["recon_x"]
+            else:  # return embedding
+                predictions = self.get_embedding(dl_element)
+
+            predictions_np = predictions.cpu().numpy()
+            all_predictions_np = all_predictions_np + [*predictions_np]
+
+            display_progress(
+                "Model evaluation in progress",
+                batch_idx + 1,
+                num_batches_test,
+                additional_message=f"Batch #{batch_idx}",
+            )
+
+            # Save few images
+            if predict_mode != PredictMode.Standard:
+                continue
+
+            # Get numpy elements
+            inputs_np = dl_element["data"].cpu().numpy()
+
+            for idx in range(dl_element["data"].shape[0]):
+                if self.image_index in images_to_save:
+                    image_id = (batch_idx * test_dl.batch_size) + idx
+                    image_name = test_dl.dataset.names[image_id].split(".")[0]
+
+                    # Get element at index
+                    input_np = inputs_np[idx, ...].squeeze()
+                    prediction_np = predictions_np[idx, ...].squeeze()
+
+                    dl_element_numpy = DatasetOutput(
+                        input=input_np,
+                        prediction=prediction_np,
+                    )
+
+                    self.save_results(
+                        f"{image_name}_{self.image_index}",
+                        dl_element_numpy,
+                        test_dl.dataset.mean_std,
+                    )
+
+                self.image_index += 1
+
+        return all_predictions_np
+
+    def write_useful_information(self):
+        # Update parameters file with all useful information
+        os.makedirs(self.params.models_folder, exist_ok=True)
+        with open(self.parameters_path, "a") as f:
+            for attribute, value in vars(self.training_information).items():
+                f.write("%s;%s\n" % (attribute, value))
+        f.close()
+
+        if self.params.global_results_path == "":
+            return
+
+        # If global results file does not exist, create it
+        if not os.path.exists(self.params.global_results_path):
+            with open(self.params.global_results_path, "w") as f:
+                f.write(
+                    "data;id;latent dim;learning rate;beta;gamma;delta;git hash;score;weight_decay;batch size;drop out;encoder name;additional score\n"
+                )
+            f.close()
+
+        # Store useful results in global results file
+        with open(self.params.global_results_path, "a") as f:
+            f.write(f"{self.params.data_dir};")
+            f.write(f"{self.params.format_now};")
+            f.write(f"{self.params.latent_dim};")
+            f.write(f"{self.params.learning_rate};")
+            f.write(f"{self.params.beta};")
+            f.write(f"{self.params.gamma};")
+            f.write(f"{self.params.delta};")
+            f.write(f"{self.training_information.git_hash};")
+            f.write(f"{self.training_information.score};")
+            f.write(f"{self.params.weight_decay};")
+            f.write(f"{self.params.batch_size};")
+            f.write(f"{self.params.dropout};")
+            f.write(f"{self.params.encoder_name};")
+            f.write(f"{self.training_information.additional_score};\n")
+        f.close()
+
+    def write_images_to_tensorboard(self, current_batch, dl_element, name):
+        # Get numpy arrays
+        inputs_np = dl_element["data"]
+        image_indexes_np = dl_element["id"]
+
+        # Get images name
+        current_dl_file_names = [
+            file_name.split(".")[0] for file_name in self.dl[name].dataset.names
+        ]
+        image_names = [current_dl_file_names[image_index] for image_index in image_indexes_np]
+
+        # Log the results images
+        for i, (input_np, image_name) in enumerate(zip(inputs_np, image_names)):
+            # Do not save too many images
+            if i == self.params.nb_tensorboard_images_max:
+                break
+            for channel in range(input_np.shape[0]):
+                # ... log the ground truth image
+                plt.imshow(input_np[channel], cmap="gray")
+                self.writer.add_figure(
+                    f"{name}/{image_name}/{channel}/input",
+                    plt.gcf(),
+                    current_batch,
+                )
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_params/base_model_params.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_params/base_model_params.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,284 +1,290 @@
-from pathlib import Path
-import random
-from datetime import datetime
-import os
-
-from ..dimensions import Dimensions
-from ..tools import extract_patterns
-
-
-class DataSplit:
-    """
-    Split the dataset into train, validation and test.
-    """
-
-    def __init__(self, params, distinct_files):
-        """
-        distinct_files: All distinct files in the data folder. Names in file_name should be in this list.
-        """
-        self.data_sets = {
-            "train": {
-                "ratio": params.train_ratio,
-                "number": params.train_number,
-                "possible_files": [],
-                "files": [],
-                "file_name": params.train_file,
-            },
-            "val": {
-                "ratio": params.val_ratio,
-                "number": params.val_number,
-                "possible_files": [],
-                "files": [],
-                "file_name": params.val_file,
-            },
-            "test": {
-                "ratio": params.test_ratio,
-                "number": params.test_number,
-                "possible_files": [],
-                "files": [],
-                "file_name": params.test_file,
-            },
-        }
-
-        for name, data_set in self.data_sets.items():
-            # Either number or ratio must be provided, not both
-            if data_set["ratio"] * data_set["number"] != 0:
-                raise ValueError(
-                    f"Both {name} ratio and number are not null, choice is ambiguous."
-                )
-            # If file name is provided, then possible elements are the ones written in the file
-            current_filename = data_set["file_name"]
-            if current_filename == "":
-                continue
-            if os.path.isfile(current_filename):
-                with open(current_filename, "r") as f:
-                    patterns = f.read().splitlines()
-                data_set["possible_files"] = extract_patterns(distinct_files, patterns)
-                # In this case, if neither ratio nor number is provided, then ratio is 100%
-                if data_set["ratio"] == 0 and data_set["number"] == 0:
-                    data_set["ratio"] = 1
-            else:
-                raise ValueError(f"{current_filename} does not exist.")
-
-    @staticmethod
-    def display_loading_source(name, data_set, dir_src):
-        source_path = data_set["file_name"] if data_set["file_name"] != "" else dir_src
-        number_ratio_message = "All elements"
-        if data_set["ratio"] > 1:
-            raise ValueError(f"{name} ratio is greater than 1.")
-        if data_set["number"] == 0 and data_set["ratio"] == 0:
-            print(f"No data is loaded for {name}")
-        else:
-            if data_set["ratio"] > 0:
-                number_ratio_message = f"{int(data_set['ratio'] * 100)}% elements"
-            elif data_set["number"] > 0:
-                number_ratio_message = f"{data_set['number']} elements"
-            print(f"{name} data is loaded from {source_path} - {number_ratio_message}")
-
-    def generate_train_val_test_list(self, files, dir_src):
-        print("### Data source ###")
-        for name, data_set in self.data_sets.items():
-            # Display information about the source of the data
-            self.display_loading_source(name, data_set, dir_src)
-            # If missing possible_files, consider the ones provided
-            if len(data_set["possible_files"]) == 0:
-                data_set["possible_files"] = files[:]
-            # Replace ratio by number to only consider number in the following
-            if data_set["ratio"] > 0:
-                data_set["number"] = int(data_set["ratio"] * len(data_set["possible_files"]))
-        print("###################")
-
-        # Return data set names, sorted by priority
-        def sort_data_sets():
-            # Train is always last as it uses random with no seed
-            # Between test and val, first select the one having a file name
-            if self.data_sets["test"]["file_name"] > self.data_sets["val"]["file_name"]:
-                return ["test", "val", "train"]
-            return ["val", "test", "train"]
-
-        sorted_data_sets = sort_data_sets()
-        for name in sorted_data_sets:
-            data_set = self.data_sets[name]
-            # Raise error if too many elements are required
-            if data_set["number"] > len(data_set["possible_files"]):
-                raise ValueError(f"Not enough files for {name}...")
-            # Randomly sample indices
-            # Keep same val and test images at each run
-            rd_generator = random.Random(None if name == "train" else 10)
-            indices = rd_generator.sample(
-                range(len(data_set["possible_files"])), data_set["number"]
-            )
-            data_set["files"] = [data_set["possible_files"][i] for i in indices]
-            # Remove the files from the possible files for other data sets
-            for file in data_set["files"]:
-                for other_data_set in self.data_sets.values():
-                    if file in other_data_set["possible_files"]:
-                        other_data_set["possible_files"].remove(file)
-
-        # Sort files before returning
-        return (
-            sorted(self.data_sets["train"]["files"]),
-            sorted(self.data_sets["val"]["files"]),
-            sorted(self.data_sets["test"]["files"]),
-        )
-
-
-class BaseModelParams:
-    """
-    Model params base class.
-    """
-
-    def __init__(self, name):
-        self.name = name
-
-        # Input dimensions to the model
-        self.input_dimensions = Dimensions(height=None, width=None, depth=None)
-
-        # Optimizer
-        self.beta1 = 0.9  # exponential decay rate for the first moment estimates
-        self.beta2 = 0.999  # exponential decay rate for the second moment estimates
-        self.weight_decay = 0.0  # weight decay (L2 penalty)
-        self.dropout = 0.0  # dropout rate
-
-        # Training parameters
-        self.num_epochs = 50
-        self.batch_size = 32
-        self.learning_rate = 0.1
-        self.fp16_precision = False
-        self.nb_warmup_epochs = 10
-        self.num_workers = 4
-
-        self.nb_classes = None
-        self.class_names = []
-        self.model_index = 0
-        self.c_indexes = [0]  # channels selected as input
-        self.z_indexes = [0]  # heights selected as input
-        self.out_channels = 0  # output
-
-        # Input data set
-        self.data_dir = os.path.join(str(Path.home()), "data", "dummy")
-
-        # Data split
-        self.train_ratio = 0
-        self.train_number = 0
-        self.train_file = ""
-
-        self.val_ratio = 0
-        self.val_number = 0
-        self.val_file = ""
-
-        self.test_ratio = 0
-        self.test_number = 0
-        self.test_file = ""
-
-        self.cross_validation_dir = ""
-
-        # Tensorboard parameters
-        self.tensorboard_folder_path = os.path.join(str(Path.home()), "tensorboard/local")
-        self.plot_step = 10
-        # Number of different epochs where to plot images
-        self.nb_plot_images = 2
-        self.nb_tensorboard_images_max = 8
-
-        # Output folders - models & predictions
-        self.models_folder = os.path.join(str(Path.home()), "models/local")
-        self.model_save_name = f"{self.name}.pt"
-        self.output_dir = os.path.join(str(Path.home()), "predictions/local")
-
-        # Path to load model to predict
-        self.model_load_path = ""
-
-        # Date
-        self.format_now = ""
-        self.job_id = "local"
-
-        # Global results path
-        self.global_results_path = ""
-
-        # Files loaded - do not set, to be modified during data loading
-        self.names_train = []
-        self.names_val = []
-        self.names_test = []
-
-        # Weights and biases parameters
-        self.wandb_project = "vae-dummy"
-        self.wandb_entity = "cbio-bis"
-
-    def get_useful_training_parameters(self):
-        return f"epochs {self.num_epochs} | batch {self.batch_size} | lr {self.learning_rate} | weight decay {self.weight_decay} | dropout {self.dropout} | c {self.c_indexes} | z {self.z_indexes}"
-
-    def update(self, args=None):
-        if args is not None:
-            if args.job_id:
-                self.job_id = args.job_id
-            if args.data_dir:
-                self.data_dir = args.data_dir
-            if args.tb_dir:
-                self.tensorboard_folder_path = args.tb_dir
-            if args.model_path:
-                self.models_folder = args.model_path
-            if args.lr:
-                self.learning_rate = float(args.lr)
-            if args.epochs:
-                self.num_epochs = int(args.epochs)
-            if args.plot_step:
-                self.plot_step = int(args.plot_step)
-            if args.output_dir:
-                self.output_dir = args.output_dir
-            if args.batch_size:
-                self.batch_size = int(args.batch_size)
-            if args.train_ratio:
-                self.train_ratio = float(args.train_ratio)
-            if args.val_ratio:
-                self.val_ratio = float(args.val_ratio)
-            if args.test_ratio:
-                self.test_ratio = float(args.test_ratio)
-            if args.train_number:
-                self.train_number = int(args.train_number)
-            if args.val_number:
-                self.val_number = int(args.val_number)
-            if args.test_number:
-                self.test_number = int(args.test_number)
-            if args.train_file:
-                self.train_file = args.train_file
-            if args.val_file:
-                self.val_file = args.val_file
-            if args.test_file:
-                self.test_file = args.test_file
-            if args.model_load_path:
-                self.model_load_path = args.model_load_path
-            if args.global_results_path:
-                self.global_results_path = args.global_results_path
-            if args.model_index:
-                self.model_index = int(args.model_index)
-            if args.image_height:
-                self.input_dimensions.height = int(args.image_height)
-            if args.image_width:
-                self.input_dimensions.width = int(args.image_width)
-            if args.weight_decay:
-                self.weight_decay = float(args.weight_decay)
-            if args.num_workers:
-                self.num_workers = int(args.num_workers)
-            if args.dropout:
-                self.dropout = float(args.dropout)
-            if args.c_indexes:
-                self.c_indexes = args.c_indexes
-            if args.z_indexes:
-                self.z_indexes = args.z_indexes
-            if args.cross_validation_dir:
-                self.cross_validation_dir = args.cross_validation_dir
-
-        # Create folders dedicated to current run
-        now = datetime.now()
-        self.format_now = now.strftime("%Y%m%d-%H%M%S") + "-" + self.job_id
-
-        print(f"Model time id: {self.format_now}")
-        print(self.get_useful_training_parameters())
-
-        self.tensorboard_folder_path = (
-            f"{self.tensorboard_folder_path}/{self.format_now}_{self.name}"
-        )
-
-        self.models_folder = f"{self.models_folder}/{self.name}/{self.format_now}"
-
-        self.output_dir = f"{self.output_dir}/{self.name}/{self.format_now}"
+from pathlib import Path
+import random
+from datetime import datetime
+import os
+
+
+from ..dimensions import Dimensions
+from ..tools import extract_patterns
+from ...data.tools import get_folder_path
+
+
+class DataSplit:
+    """
+    Split the dataset into train, validation and test.
+    """
+
+    def __init__(self, params, distinct_files):
+        """
+        distinct_files: All distinct files in the data folder. Names in file_name should be in this list.
+        """
+        self.data_sets = {
+            "train": {
+                "ratio": params.train_ratio,
+                "number": params.train_number,
+                "possible_files": [],
+                "files": [],
+                "file_name": params.train_file,
+            },
+            "val": {
+                "ratio": params.val_ratio,
+                "number": params.val_number,
+                "possible_files": [],
+                "files": [],
+                "file_name": params.val_file,
+            },
+            "test": {
+                "ratio": params.test_ratio,
+                "number": params.test_number,
+                "possible_files": [],
+                "files": [],
+                "file_name": params.test_file,
+            },
+        }
+
+        for name, data_set in self.data_sets.items():
+            # Either number or ratio must be provided, not both
+            if data_set["ratio"] * data_set["number"] != 0:
+                raise ValueError(
+                    f"Both {name} ratio and number are not null, choice is ambiguous."
+                )
+            # If file name is provided, then possible elements are the ones written in the file
+            current_filename = data_set["file_name"]
+            if current_filename == "":
+                continue
+            if os.path.isfile(current_filename):
+                with open(current_filename, "r") as f:
+                    patterns = f.read().splitlines()
+                data_set["possible_files"] = extract_patterns(distinct_files, patterns)
+                # In this case, if neither ratio nor number is provided, then ratio is 100%
+                if data_set["ratio"] == 0 and data_set["number"] == 0:
+                    data_set["ratio"] = 1
+            else:
+                raise ValueError(f"{current_filename} does not exist.")
+
+    @staticmethod
+    def display_loading_source(name, data_set, dir_src):
+        source_path = data_set["file_name"] if data_set["file_name"] != "" else dir_src
+        number_ratio_message = "All elements"
+        if data_set["ratio"] > 1:
+            raise ValueError(f"{name} ratio is greater than 1.")
+        if data_set["number"] == 0 and data_set["ratio"] == 0:
+            print(f"No data is loaded for {name}")
+        else:
+            if data_set["ratio"] > 0:
+                number_ratio_message = f"{int(data_set['ratio'] * 100)}% elements"
+            elif data_set["number"] > 0:
+                number_ratio_message = f"{data_set['number']} elements"
+            print(f"{name} data is loaded from {source_path} - {number_ratio_message}")
+
+    def generate_train_val_test_list(self, files, dir_src):
+        print("### Data source ###")
+        for name, data_set in self.data_sets.items():
+            # Display information about the source of the data
+            self.display_loading_source(name, data_set, dir_src)
+            # If missing possible_files, consider the ones provided
+            if len(data_set["possible_files"]) == 0:
+                data_set["possible_files"] = files[:]
+            # Replace ratio by number to only consider number in the following
+            if data_set["ratio"] > 0:
+                data_set["number"] = int(
+                    data_set["ratio"] * len(data_set["possible_files"])
+                )
+        print("###################")
+
+        # Return data set names, sorted by priority
+        def sort_data_sets():
+            # Train is always last as it uses random with no seed
+            # Between test and val, first select the one having a file name
+            if self.data_sets["test"]["file_name"] > self.data_sets["val"]["file_name"]:
+                return ["test", "val", "train"]
+            return ["val", "test", "train"]
+
+        sorted_data_sets = sort_data_sets()
+        for name in sorted_data_sets:
+            data_set = self.data_sets[name]
+            # Raise error if too many elements are required
+            if data_set["number"] > len(data_set["possible_files"]):
+                raise ValueError(f"Not enough files for {name}...")
+            # Randomly sample indices
+            # Keep same val and test images at each run
+            rd_generator = random.Random(None if name == "train" else 10)
+            indices = rd_generator.sample(
+                range(len(data_set["possible_files"])), data_set["number"]
+            )
+            data_set["files"] = [data_set["possible_files"][i] for i in indices]
+            # Remove the files from the possible files for other data sets
+            for file in data_set["files"]:
+                for other_data_set in self.data_sets.values():
+                    if file in other_data_set["possible_files"]:
+                        other_data_set["possible_files"].remove(file)
+
+        # Sort files before returning
+        return (
+            sorted(self.data_sets["train"]["files"]),
+            sorted(self.data_sets["val"]["files"]),
+            sorted(self.data_sets["test"]["files"]),
+        )
+
+
+class BaseModelParams:
+    """
+    Model params base class.
+    """
+
+    def __init__(self, name):
+        self.name = name
+
+        # Input dimensions to the model
+        self.input_dimensions = Dimensions(height=32, width=32)
+
+        # Optimizer
+        self.beta1 = 0.9  # exponential decay rate for the first moment estimates
+        self.beta2 = 0.999  # exponential decay rate for the second moment estimates
+        self.weight_decay = 0.0  # weight decay (L2 penalty)
+        self.dropout = 0.0  # dropout rate
+
+        # Training parameters
+        self.num_epochs = 50
+        self.batch_size = 32
+        self.learning_rate = 0.1
+        self.fp16_precision = False
+        self.nb_warmup_epochs = 10
+        self.num_workers = 4
+
+        self.nb_classes = None
+        self.class_names = []
+        self.model_index = 0
+        self.c_indexes = [0]  # channels selected as input
+        self.z_indexes = [0]  # heights selected as input
+        self.out_channels = 0  # output
+
+        # Input data set
+        self.data_dir = get_folder_path("images")
+
+        # Data split
+        self.train_ratio = 0
+        self.train_number = 0
+        self.train_file = ""
+
+        self.val_ratio = 0
+        self.val_number = 0
+        self.val_file = ""
+
+        self.test_ratio = 0
+        self.test_number = 0
+        self.test_file = ""
+
+        self.cross_validation_dir = ""
+
+        # Tensorboard parameters
+        self.tensorboard_folder_path = get_folder_path("tensorboard")
+        self.plot_step = 10
+        # Number of different epochs where to plot images
+        self.nb_plot_images = 2
+        self.nb_tensorboard_images_max = 8
+
+        # Output folders - models & predictions
+        self.models_folder = get_folder_path("models")
+        self.model_save_name = f"{self.name}.pt"
+        self.output_dir = get_folder_path("predictions")
+
+        # Path to load model to predict
+        self.model_load_path = ""
+
+        # Date
+        self.format_now = ""
+        self.job_id = "local"
+
+        # Global results path
+        self.global_results_path = ""
+
+        # Files loaded - do not set, to be modified during data loading
+        self.names_train = []
+        self.names_val = []
+        self.names_test = []
+
+        # Weights and biases parameters
+        self.wandb_project = "vae-dummy"
+        self.wandb_entity = "cbio-bis"
+
+    def get_useful_training_parameters(self):
+        return f"epochs {self.num_epochs} | batch {self.batch_size} | lr {self.learning_rate} | weight decay {self.weight_decay} | dropout {self.dropout} | c {self.c_indexes} | z {self.z_indexes}"
+
+    def update(self, args=None):
+        if args is not None:
+            if args.job_id:
+                self.job_id = args.job_id
+            if args.data_dir:
+                self.data_dir = args.data_dir
+            if args.tb_dir:
+                self.tensorboard_folder_path = args.tb_dir
+            if args.model_path:
+                self.models_folder = args.model_path
+            if args.lr:
+                self.learning_rate = float(args.lr)
+            if args.epochs:
+                self.num_epochs = int(args.epochs)
+            if args.plot_step:
+                self.plot_step = int(args.plot_step)
+            if args.output_dir:
+                self.output_dir = args.output_dir
+            if args.batch_size:
+                self.batch_size = int(args.batch_size)
+            if args.train_ratio:
+                self.train_ratio = float(args.train_ratio)
+            if args.val_ratio:
+                self.val_ratio = float(args.val_ratio)
+            if args.test_ratio:
+                self.test_ratio = float(args.test_ratio)
+            if args.train_number:
+                self.train_number = int(args.train_number)
+            if args.val_number:
+                self.val_number = int(args.val_number)
+            if args.test_number:
+                self.test_number = int(args.test_number)
+            if args.train_file:
+                self.train_file = args.train_file
+            if args.val_file:
+                self.val_file = args.val_file
+            if args.test_file:
+                self.test_file = args.test_file
+            if args.model_load_path:
+                self.model_load_path = args.model_load_path
+            if args.global_results_path:
+                self.global_results_path = args.global_results_path
+            if args.model_index:
+                self.model_index = int(args.model_index)
+            if args.image_height:
+                self.input_dimensions.height = int(args.image_height)
+            if args.image_width:
+                self.input_dimensions.width = int(args.image_width)
+            if args.weight_decay:
+                self.weight_decay = float(args.weight_decay)
+            if args.num_workers:
+                self.num_workers = int(args.num_workers)
+            if args.dropout:
+                self.dropout = float(args.dropout)
+            if args.c_indexes:
+                self.c_indexes = args.c_indexes
+            if args.z_indexes:
+                self.z_indexes = args.z_indexes
+            if args.cross_validation_dir:
+                self.cross_validation_dir = args.cross_validation_dir
+            if args.out_channels:
+                self.out_channels = args.out_channels
+
+        # Create folders dedicated to current run
+        now = datetime.now()
+        self.format_now = now.strftime("%Y%m%d-%H%M%S") + "-" + self.job_id
+
+        print(f"Model time id: {self.format_now}")
+        print(self.get_useful_training_parameters())
+
+        self.tensorboard_folder_path = (
+            f"{self.tensorboard_folder_path}/{self.format_now}_{self.name}"
+        )
+
+        self.models_folder = f"{self.models_folder}/{self.name}/{self.format_now}"
+
+        self.output_dir = f"{self.output_dir}/{self.name}/{self.format_now}"
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/model_params/vae_model_params.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/model_params/vae_model_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,71 @@
-from .base_model_params import BaseModelParams
-from ..dimensions import Dimensions
-
-
-class VAEModelParams(BaseModelParams):
-    """
-    VAE model params.
-    """
-
-    def __init__(self, name="vae"):
-        super().__init__(name)
-
-        self.input_dimensions = Dimensions(height=160, width=160)
-
-        self.c_indexes = [0, 1]
-        self.z_indexes = [0]
-
-        self.nb_classes = 3  # G1, S, G2
-        self.depth = 5
-
-        self.learning_rate = 1e-3
-        self.weight_decay = 0.05
-        self.beta1 = 0.91
-        self.beta2 = 0.995
-        self.reconstruction_loss = "mse"  # "l1", "bce" or "mse"
-        self.kld_loss = "standard"  # "standard" or "cl-vae"
-        self.encoder_name = "timm-efficientnet-b0"
-
-        self.latent_dim = 256
-        self.beta = 1  # weight of KLD loss
-        self.gamma = 0  # weight of classification loss
-        self.delta = 0  # weight of segmentation loss
-
-        self.model_pretrained_path = ""
-
-    def update(self, args=None):
-        # Finish by parent class as it prints the parameters
-
-        if args is not None:
-            if args.latent_dim:
-                self.latent_dim = args.latent_dim
-            if args.beta:
-                self.beta = float(args.beta)
-            if args.gamma:
-                self.gamma = float(args.gamma)
-            if args.delta:
-                self.delta = float(args.delta)
-            if args.reconstruction_loss:
-                self.reconstruction_loss = args.reconstruction_loss
-            if args.model_pretrained_path:
-                self.model_pretrained_path = args.model_pretrained_path
-            if args.depth:
-                self.depth = int(args.depth)
-            if args.kld_loss:
-                self.kld_loss = args.kld_loss
-            if args.encoder_name:
-                self.encoder_name = args.encoder_name
-
-        super().update(args)
-
-    def get_useful_training_parameters(self):
-        parent_parameters = super().get_useful_training_parameters()
-        parameters = (
-            parent_parameters
-            + f" | latent dim {self.latent_dim}"
-            + f" | beta {self.beta}"
-            + f" | gamma {self.gamma}"
-            + f" | delta {self.delta}"
-            + f" | depth {self.depth}"
-            + f" | kld loss {self.kld_loss}"
-            + f" | encoder name {self.encoder_name}"
-        )
-        return parameters
+from .base_model_params import BaseModelParams
+from ..dimensions import Dimensions
+
+
+class VAEModelParams(BaseModelParams):
+    """
+    VAE model params.
+    """
+
+    def __init__(self, name="vae"):
+        super().__init__(name)
+
+        self.c_indexes = [0, 1]
+        self.z_indexes = [0]
+
+        self.nb_classes = 3  # G1, S, G2
+        self.depth = 5
+
+        self.learning_rate = 1e-3
+        self.weight_decay = 0.05
+        self.beta1 = 0.91
+        self.beta2 = 0.995
+        self.reconstruction_loss = "mse"  # "l1", "bce" or "mse"
+        self.kld_loss = "standard"  # "standard" or "cl-vae"
+        self.encoder_name = "timm-efficientnet-b0"
+
+        self.latent_dim = 256
+        self.beta = 1  # weight of KLD loss
+        self.gamma = 0  # weight of classification loss
+        self.delta = 0  # weight of segmentation loss
+
+        self.model_pretrained_path = ""
+
+    def update(self, args=None):
+        # Finish by parent class as it prints the parameters
+
+        if args is not None:
+            if args.latent_dim:
+                self.latent_dim = args.latent_dim
+            if args.beta:
+                self.beta = float(args.beta)
+            if args.gamma:
+                self.gamma = float(args.gamma)
+            if args.delta:
+                self.delta = float(args.delta)
+            if args.reconstruction_loss:
+                self.reconstruction_loss = args.reconstruction_loss
+            if args.model_pretrained_path:
+                self.model_pretrained_path = args.model_pretrained_path
+            if args.depth:
+                self.depth = int(args.depth)
+            if args.kld_loss:
+                self.kld_loss = args.kld_loss
+            if args.encoder_name:
+                self.encoder_name = args.encoder_name
+
+        super().update(args)
+
+    def get_useful_training_parameters(self):
+        parent_parameters = super().get_useful_training_parameters()
+        parameters = (
+            parent_parameters
+            + f" | latent dim {self.latent_dim}"
+            + f" | beta {self.beta}"
+            + f" | gamma {self.gamma}"
+            + f" | delta {self.delta}"
+            + f" | depth {self.depth}"
+            + f" | kld loss {self.kld_loss}"
+            + f" | encoder name {self.encoder_name}"
+        )
+        return parameters
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/parsers/vae_parser.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/parsers/vae_parser.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .cnn_parser import CnnParser
-
-
-class VAEParser(CnnParser):
-    """
-    VAE parsing class.
-    """
-
-    def __init__(self):
-        super().__init__()
-
-        self.arguments_parser.add_argument("--latent_dim", help="Latent space dimension")
-        self.arguments_parser.add_argument("--beta", help="KD loss weight")
-        self.arguments_parser.add_argument("--gamma", help="classification loss weight")
-        self.arguments_parser.add_argument("--delta", help="segmentation loss weight")
-        self.arguments_parser.add_argument("--reconstruction_loss", help="mse, bce or l1")
-        self.arguments_parser.add_argument(
-            "--model_pretrained_path", help="Path to pretrained model"
-        )
-        self.arguments_parser.add_argument("--depth", help="Depth of encoder")
-        self.arguments_parser.add_argument("--kld_loss", help="standard or cl-vae")
-        self.arguments_parser.add_argument("--encoder_name", help="Encoder name")
+from .cnn_parser import CnnParser
+
+
+class VAEParser(CnnParser):
+    """
+    VAE parsing class.
+    """
+
+    def __init__(self):
+        super().__init__()
+
+        self.arguments_parser.add_argument("--latent_dim", help="Latent space dimension")
+        self.arguments_parser.add_argument("--beta", help="KD loss weight")
+        self.arguments_parser.add_argument("--gamma", help="classification loss weight")
+        self.arguments_parser.add_argument("--delta", help="segmentation loss weight")
+        self.arguments_parser.add_argument("--reconstruction_loss", help="mse, bce or l1")
+        self.arguments_parser.add_argument(
+            "--model_pretrained_path", help="Path to pretrained model"
+        )
+        self.arguments_parser.add_argument("--depth", help="Depth of encoder")
+        self.arguments_parser.add_argument("--kld_loss", help="standard or cl-vae")
+        self.arguments_parser.add_argument("--encoder_name", help="Encoder name")
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/preprocessing.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/preprocessing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,78 @@
-import numpy as np
-from sklearn.preprocessing import MinMaxScaler
-
-
-def normalize_array(input_array, mean_std=None, reverse=False):
-    """
-    Works for both 2D and 3D arrays.
-    If reverse, then the normalization is reversed.
-
-    mean_std = dict(channel, dict(mean, std))
-    """
-
-    # Get number of channels
-    nb_channels = np.min(input_array.shape)
-
-    # Find channel axis
-    channel_axis = np.argmin(input_array.shape)
-    # Put channel axis in front
-    input_array = np.moveaxis(input_array, channel_axis, 0)
-
-    if mean_std is not None:  # custom mean and std
-        assert nb_channels == len(mean_std["mean"])
-        mean, std = mean_std["mean"], mean_std["std"]
-        for _ in range(2):  # 2 for H and W
-            mean = np.expand_dims(mean, -1)
-            std = np.expand_dims(std, -1)
-    else:  # compute mean and std
-        axes = tuple(range(1, len(input_array.shape)))
-        mean = np.mean(input_array, axis=axes, keepdims=True)
-        std = np.std(input_array, axis=axes, keepdims=True)
-
-    # If reverse, apply reverse normalization
-    if reverse:
-        mean = -mean / std
-        std = 1 / std
-
-    normalized_array = (input_array - mean) / std
-
-    # Cast to float32 as float64 is not supported by albumentations
-    normalized_array = normalized_array.astype(np.float32)
-
-    # Put channel axis back to original position
-    normalized_array = np.moveaxis(normalized_array, 0, channel_axis)
-
-    return normalized_array
-
-
-def zero_one_scaler(input_array, feature_range=(0, 1)):
-    """
-    Normalize array between 0 and 1.
-    Works for both 2D and 3D arrays.
-    """
-    # 2D
-    if len(input_array.shape) <= 2:
-        return MinMaxScaler().fit_transform(input_array)
-
-    # Find channel axis
-    channel_axis = np.argmin(input_array.shape)
-    nb_channels = input_array.shape[channel_axis]
-    # Put channel axis in back
-    new_input_array = np.moveaxis(input_array, channel_axis, -1)
-    # Reshape to 2D
-    as_columns = new_input_array.reshape(-1, nb_channels)
-    # Apply min max scaler
-    transformed_columns = MinMaxScaler(feature_range=feature_range).fit_transform(as_columns)
-    # Reshape to original shape
-    transformed = transformed_columns.reshape(new_input_array.shape)
-    # Put channel axis back to original position
-    transformed = np.moveaxis(transformed, -1, channel_axis)
-
-    # Make sure values are between 0 and 1
-    transformed = np.clip(transformed, 0, 1)
-
-    return transformed
+import numpy as np
+from sklearn.preprocessing import MinMaxScaler
+
+
+def normalize_array(input_array, mean_std=None, reverse=False, channel_axis=None):
+    """
+    Works for both 2D and 3D arrays.
+    If reverse, then the normalization is reversed.
+
+    mean_std = dict(channel, dict(mean, std))
+    """
+
+    # Get number of channels
+    nb_channels = np.min(input_array.shape)
+
+    # Find channel axis if not already given
+    if channel_axis is None:
+        channel_axis = np.argmin(input_array.shape)
+
+    # Put channel axis in front
+    input_array = np.moveaxis(input_array, channel_axis, 0)
+
+    if mean_std is not None:  # custom mean and std
+        assert nb_channels == len(mean_std["mean"])
+        mean, std = mean_std["mean"], mean_std["std"]
+        for _ in range(2):  # 2 for H and W
+            mean = np.expand_dims(mean, -1)
+            std = np.expand_dims(std, -1)
+    else:  # compute mean and std
+        axes = tuple(range(1, len(input_array.shape)))
+        mean = np.mean(input_array, axis=axes, keepdims=True)
+        std = np.std(input_array, axis=axes, keepdims=True)
+
+    # If reverse, apply reverse normalization
+    if reverse:
+        mean = -mean / std
+        std = 1 / std
+
+    normalized_array = (input_array - mean) / std
+
+    # Cast to float32 as float64 is not supported by albumentations
+    normalized_array = normalized_array.astype(np.float32)
+
+    # Put channel axis back to original position
+    normalized_array = np.moveaxis(normalized_array, 0, channel_axis)
+
+    return normalized_array
+
+
+def zero_one_scaler(input_array, feature_range=(0, 1)):
+    """
+    Normalize array between 0 and 1.
+    Works for both 2D and 3D arrays.
+    """
+    # 2D
+    if len(input_array.shape) <= 2:
+        return MinMaxScaler().fit_transform(input_array)
+
+    # Find channel axis
+    channel_axis = np.argmin(input_array.shape)
+    nb_channels = input_array.shape[channel_axis]
+    # Put channel axis in back
+    new_input_array = np.moveaxis(input_array, channel_axis, -1)
+    # Reshape to 2D
+    as_columns = new_input_array.reshape(-1, nb_channels)
+    # Apply min max scaler
+    transformed_columns = MinMaxScaler(feature_range=feature_range).fit_transform(
+        as_columns
+    )
+    # Reshape to original shape
+    transformed = transformed_columns.reshape(new_input_array.shape)
+    # Put channel axis back to original position
+    transformed = np.moveaxis(transformed, -1, channel_axis)
+
+    # Make sure values are between 0 and 1
+    transformed = np.clip(transformed, 0, 1)
+
+    return transformed
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/readers/abstract_reader.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/readers/abstract_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,121 @@
-from abc import abstractmethod
-from typing import List
-import numpy as np
-from bigfish import stack
-from skimage import io
-
-from .utils.normalization import Normalization
-from .utils.projection import Projection
-
-from ..enum import NormalizeMethods, ProjectMethods
-from ..preprocessing import (
-    zero_one_scaler,
-    normalize_array,
-)
-from ..tools import handle_image_type
-
-
-class AbstractReader:
-    """
-    Base class for readers
-
-    Parameters
-    ----------
-    file_path : str
-        Path to the file to read
-    normalize : Normalization
-        Method to normalize the image
-    project : List[Projection]
-        Method to project the image
-    respect_initial_type : bool
-        If True, the image will be kept in the same type as the original file.
-        If False, the image will be converted to be adapted to torch.
-    """
-
-    def __init__(
-        self,
-        file_path: str,
-        normalize: Normalization = Normalization(method=NormalizeMethods.none),
-        project: List[Projection] = [Projection(method=ProjectMethods.none)],
-        respect_initial_type=False,
-    ):
-        # Read image from file
-        self.image = io.imread(file_path)
-        # Type management
-        if not respect_initial_type:
-            self.image = handle_image_type(self.image)
-
-        self.respect_initial_type = respect_initial_type
-
-        self.preprocessing_done = False
-
-        self.normalize = normalize
-        self.project = project
-
-    def get_processed_image(self):
-        if not self.preprocessing_done:
-            # Project & normalize
-            self.project_image()
-            self.normalize_image()
-            self.preprocessing_done = True
-        return self.image
-
-    def get_dimensions(self):
-        return self.image.shape
-
-    def normalize_image(self):
-        if self.normalize.method == NormalizeMethods.none:
-            pass
-        elif self.normalize.method == NormalizeMethods.ZeroOneScaler:
-            self.image = zero_one_scaler(self.image)
-        elif self.normalize.method == NormalizeMethods.Standardize:
-            self.image = normalize_array(self.image)
-        elif self.normalize.method == NormalizeMethods.StandardizeImageNet:
-            type_factor = np.iinfo(self.image.dtype).max
-            mean_std = {
-                0: {"mean": 0.485 * type_factor, "std": 0.229 * type_factor},
-                1: {"mean": 0.456 * type_factor, "std": 0.224 * type_factor},
-                2: {"mean": 0.406 * type_factor, "std": 0.225 * type_factor},
-            }
-            self.image = normalize_array(self.image, mean_std) / type_factor
-        else:
-            raise ValueError("Unknown normalization method")
-
-    def project_image(self):
-        for projection in self.project:
-            # Apply projection
-            if projection.method == ProjectMethods.none:
-                pass
-            elif projection.method == ProjectMethods.Maximum:
-                self.image = self.image.max(axis=projection.axis)
-            elif projection.method == ProjectMethods.Mean:
-                self.image = self.image.mean(axis=projection.axis).astype(self.image.dtype)
-            elif projection.method == ProjectMethods.Focus:
-                self.image = stack.focus_projection(self.image, proportion=projection.proportion)
-            elif projection.method == ProjectMethods.Channel:
-                self.image = np.take(self.image, projection.channels, axis=projection.axis)
-            else:
-                raise ValueError("Unknown projection method")
-        # Squeeze as before, but after projection
-        self.image = np.squeeze(self.image)
-
-    @abstractmethod
-    def display_info(
-        self,
-        unit=None,
-        scale=None,
-        save_path="",
-        dimensions=None,
-        show=True,
-        verbose=True,
-    ):
-        pass
+from abc import abstractmethod
+from typing import List
+import numpy as np
+from bigfish import stack
+from skimage import io
+
+from .utils.normalization import Normalization
+from .utils.projection import Projection
+
+from ..enum import NormalizeMethods, ProjectMethods
+from ..preprocessing import (
+    zero_one_scaler,
+    normalize_array,
+)
+from ..tools import handle_image_type
+
+
+class AbstractReader:
+    """
+    Base class for readers
+
+    Parameters
+    ----------
+    file_path : str
+        Path to the file to read
+    normalize : Normalization
+        Method to normalize the image
+    project : List[Projection]
+        Method to project the image
+    respect_initial_type : bool
+        If True, the image will be kept in the same type as the original file.
+        If False, the image will be converted to be adapted to torch.
+    """
+
+    def __init__(
+        self,
+        file_path: str,
+        normalize: Normalization = Normalization(method=NormalizeMethods.none),
+        project: List[Projection] = [Projection(method=ProjectMethods.none)],
+        respect_initial_type=False,
+    ):
+        # Read image from file
+        self.image = self._read_image(file_path)
+        # Type management
+        if not respect_initial_type:
+            self.image = handle_image_type(self.image)
+
+        self.respect_initial_type = respect_initial_type
+
+        self.preprocessing_done = False
+
+        self.normalize = normalize
+        self.project = project
+
+    def _read_image(self, file_path: str) -> np.ndarray:
+        return io.imread(file_path)
+
+    def get_processed_image(self):
+        if not self.preprocessing_done:
+            # Project & normalize
+            self.project_image()
+            self.normalize_image()
+            self.preprocessing_done = True
+        return self.image
+
+    def get_dimensions(self):
+        return self.image.shape
+
+    def normalize_image(self):
+        if self.normalize.method == NormalizeMethods.none:
+            pass
+        elif self.normalize.method == NormalizeMethods.ZeroOneScaler:
+            self.image = zero_one_scaler(self.image)
+        elif self.normalize.method == NormalizeMethods.Standardize:
+            self.image = normalize_array(self.image, channel_axis=self.normalize.axis)
+        elif self.normalize.method == NormalizeMethods.StandardizeImageNet:
+            type_factor = np.iinfo(self.image.dtype).max
+            mean_std = {
+                0: {"mean": 0.485 * type_factor, "std": 0.229 * type_factor},
+                1: {"mean": 0.456 * type_factor, "std": 0.224 * type_factor},
+                2: {"mean": 0.406 * type_factor, "std": 0.225 * type_factor},
+            }
+            self.image = normalize_array(self.image, mean_std) / type_factor
+        else:
+            raise ValueError("Unknown normalization method")
+
+    def project_image(self):
+        for projection in self.project:
+            # Apply projection
+            if projection.method == ProjectMethods.none:
+                pass
+            elif projection.method == ProjectMethods.Maximum:
+                self.image = self.image.max(axis=projection.axis)
+                self.image = np.expand_dims(self.image, projection.axis)
+            elif projection.method == ProjectMethods.Mean:
+                self.image = self.image.mean(axis=projection.axis).astype(
+                    self.image.dtype
+                )
+                self.image = np.expand_dims(self.image, projection.axis)
+            elif projection.method == ProjectMethods.Focus:
+                self.image = stack.focus_projection(
+                    self.image, proportion=projection.proportion
+                )
+            elif projection.method == ProjectMethods.Channel:
+                self.image = np.take(
+                    self.image, projection.channels, axis=projection.axis
+                )
+            else:
+                raise ValueError("Unknown projection method")
+
+    @abstractmethod
+    def display_info(
+        self,
+        unit=None,
+        scale=None,
+        save_path="",
+        dimensions=None,
+        show=True,
+        verbose=True,
+    ):
+        pass
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/readers/ciz_reader.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/readers/ciz_reader.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import slideio
-import numpy as np
-import matplotlib.pyplot as plt
-
-from ..enum import NormalizeMethods, ProjectMethods
-from ..preprocessing import normalize_array
-
-
-class CIZReader:
-    """
-    Class to read CIZ file.
-    """
-
-    def __init__(
-        self, path, channels=None, normalize=NormalizeMethods.none, project=ProjectMethods.none
-    ):
-        print("May be deprecated because unused for a while.")
-        self.slide = slideio.open_slide(path, "CZI")
-        self.scene = self.slide.get_scene(0)
-
-        # Get all channels or only specified ones if asked
-        if channels is None:
-            self.channels_names = {
-                channel: f"{self.scene.get_channel_name(channel)}_{channel}"
-                for channel in range(self.scene.num_channels)
-            }
-        else:
-            self.channels_names = {}
-            for channel in channels:
-                index = int(channel.split("_")[-1])
-                self.channels_names[index] = channel
-
-        self.z_stacks = {}
-        self.image_preprocessed = False
-        self.normalize = normalize
-        self.project = project
-
-    def group_project_stacks(self, channel, name):
-        stacks = []
-        for z_slice in range(self.scene.num_z_slices):
-            block = self.scene.read_block(
-                channel_indices=[channel], slices=(z_slice, z_slice + 1)
-            )  # HW
-            stacks.append(block)
-        array_stacks = np.asarray(stacks)  # DHW
-        if name in self.project:  # Project only if asked
-            array_stacks = array_stacks.max(axis=0)  # HW
-            array_stacks = np.expand_dims(array_stacks, axis=0)  # DHW, D=1
-        return array_stacks
-
-    def preprocess_image(self):
-        # Iterate over CIZ channels
-        for channel in range(self.scene.num_channels):
-            # Ignore if not asked by user
-            if channel not in self.channels_names:
-                continue
-            # Group z-stacks together in DHW format & normalize
-            name = self.channels_names[channel]
-            z_stack_array = self.group_project_stacks(channel, name)  # DHW
-            # Normalize only if asked
-            if name in self.normalize:
-                z_stack_array = normalize_array(z_stack_array, None)
-            # Swap axes to match HWD format
-            if len(z_stack_array.shape) > 2:
-                z_stack_array = np.moveaxis(z_stack_array, 0, 2)  # HWD
-            # Force float64 type
-            if z_stack_array.dtype == np.uint16:
-                z_stack_array = z_stack_array * 1.0
-            # Store final result
-            self.z_stacks[name] = np.expand_dims(z_stack_array, axis=0)  # CHWD (gray-scale)
-        self.image_preprocessed = True
-
-    def get_processed_image(self, channel):
-        if not self.image_preprocessed:
-            self.preprocess_image()
-        if channel not in self.z_stacks:
-            raise ValueError(f"Channel {channel} does not exist in image.")
-        return self.z_stacks[channel]
-
-    def display_info(self, _=None, __=None, ___="", ____=None):
-        # Print some data information
-        print(f"Scenes: {self.slide.num_scenes} \nScene name: {self.scene.name}")
-        print(f"Rectangle: {self.scene.rect} \nChannels: {self.scene.num_channels}")
-        print(f"Resolution: {self.scene.resolution} \nZ-slices: {self.scene.num_z_slices}")
-        print(f"Channels names: {self.channels_names}")
-
-        z_slices_to_plot = [0, self.scene.num_z_slices // 2, self.scene.num_z_slices - 1]
-        rows, columns = len(z_slices_to_plot), self.scene.num_channels
-        fig = plt.figure()
-
-        for idx, z_slice in enumerate(z_slices_to_plot):
-            for scene_channel in range(self.scene.num_channels):
-                block = self.scene.read_block(
-                    channel_indices=[scene_channel], slices=(z_slice, z_slice + 1)
-                )
-                fig.add_subplot(rows, columns, idx * columns + scene_channel + 1)
-                plt.title(f"{self.channels_names[scene_channel]} - Z{z_slice}")
-                plt.imshow(block, cmap="gray")
-
-        plt.show()
-
-
-if __name__ == "__main__":
-    FILE_PATH = r"C:\Users\thoma\data\Data Allen\st6gal1.tar\st6gal1\3500001232_100X_20170825_2-Scene-04-P15-E05.czi"
-    ONLY_CHANNELS = ["H3342_5", "EGFP_3"]
-
-    reader = CIZReader(
-        FILE_PATH,
-        project=["CMDRP_0", "CMDRP_1", "EGFP_2", "EGFP_3", "H3342_4", "H3342_5", "Bright_6"],
-        channels=ONLY_CHANNELS,
-    )
-    reader.display_max_intensity_projection()
+import slideio
+import numpy as np
+import matplotlib.pyplot as plt
+
+from ..enum import NormalizeMethods, ProjectMethods
+from ..preprocessing import normalize_array
+
+
+class CIZReader:
+    """
+    Class to read CIZ file.
+    """
+
+    def __init__(
+        self, path, channels=None, normalize=NormalizeMethods.none, project=ProjectMethods.none
+    ):
+        print("May be deprecated because unused for a while.")
+        self.slide = slideio.open_slide(path, "CZI")
+        self.scene = self.slide.get_scene(0)
+
+        # Get all channels or only specified ones if asked
+        if channels is None:
+            self.channels_names = {
+                channel: f"{self.scene.get_channel_name(channel)}_{channel}"
+                for channel in range(self.scene.num_channels)
+            }
+        else:
+            self.channels_names = {}
+            for channel in channels:
+                index = int(channel.split("_")[-1])
+                self.channels_names[index] = channel
+
+        self.z_stacks = {}
+        self.image_preprocessed = False
+        self.normalize = normalize
+        self.project = project
+
+    def group_project_stacks(self, channel, name):
+        stacks = []
+        for z_slice in range(self.scene.num_z_slices):
+            block = self.scene.read_block(
+                channel_indices=[channel], slices=(z_slice, z_slice + 1)
+            )  # HW
+            stacks.append(block)
+        array_stacks = np.asarray(stacks)  # DHW
+        if name in self.project:  # Project only if asked
+            array_stacks = array_stacks.max(axis=0)  # HW
+            array_stacks = np.expand_dims(array_stacks, axis=0)  # DHW, D=1
+        return array_stacks
+
+    def preprocess_image(self):
+        # Iterate over CIZ channels
+        for channel in range(self.scene.num_channels):
+            # Ignore if not asked by user
+            if channel not in self.channels_names:
+                continue
+            # Group z-stacks together in DHW format & normalize
+            name = self.channels_names[channel]
+            z_stack_array = self.group_project_stacks(channel, name)  # DHW
+            # Normalize only if asked
+            if name in self.normalize:
+                z_stack_array = normalize_array(z_stack_array, None)
+            # Swap axes to match HWD format
+            if len(z_stack_array.shape) > 2:
+                z_stack_array = np.moveaxis(z_stack_array, 0, 2)  # HWD
+            # Force float64 type
+            if z_stack_array.dtype == np.uint16:
+                z_stack_array = z_stack_array * 1.0
+            # Store final result
+            self.z_stacks[name] = np.expand_dims(z_stack_array, axis=0)  # CHWD (gray-scale)
+        self.image_preprocessed = True
+
+    def get_processed_image(self, channel):
+        if not self.image_preprocessed:
+            self.preprocess_image()
+        if channel not in self.z_stacks:
+            raise ValueError(f"Channel {channel} does not exist in image.")
+        return self.z_stacks[channel]
+
+    def display_info(self, _=None, __=None, ___="", ____=None):
+        # Print some data information
+        print(f"Scenes: {self.slide.num_scenes} \nScene name: {self.scene.name}")
+        print(f"Rectangle: {self.scene.rect} \nChannels: {self.scene.num_channels}")
+        print(f"Resolution: {self.scene.resolution} \nZ-slices: {self.scene.num_z_slices}")
+        print(f"Channels names: {self.channels_names}")
+
+        z_slices_to_plot = [0, self.scene.num_z_slices // 2, self.scene.num_z_slices - 1]
+        rows, columns = len(z_slices_to_plot), self.scene.num_channels
+        fig = plt.figure()
+
+        for idx, z_slice in enumerate(z_slices_to_plot):
+            for scene_channel in range(self.scene.num_channels):
+                block = self.scene.read_block(
+                    channel_indices=[scene_channel], slices=(z_slice, z_slice + 1)
+                )
+                fig.add_subplot(rows, columns, idx * columns + scene_channel + 1)
+                plt.title(f"{self.channels_names[scene_channel]} - Z{z_slice}")
+                plt.imshow(block, cmap="gray")
+
+        plt.show()
+
+
+if __name__ == "__main__":
+    FILE_PATH = r"C:\Users\thoma\data\Data Allen\st6gal1.tar\st6gal1\3500001232_100X_20170825_2-Scene-04-P15-E05.czi"
+    ONLY_CHANNELS = ["H3342_5", "EGFP_3"]
+
+    reader = CIZReader(
+        FILE_PATH,
+        project=["CMDRP_0", "CMDRP_1", "EGFP_2", "EGFP_3", "H3342_4", "H3342_5", "Bright_6"],
+        channels=ONLY_CHANNELS,
+    )
+    reader.display_max_intensity_projection()
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework/utils/tools.py` & `cnn_framework-0.0.9/src/cnn_framework/utils/tools.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import random
-import numpy as np
-from albumentations.augmentations.utils import MAX_VALUES_BY_DTYPE
-import fnmatch
-import torch
-
-
-CONSTANT_SEEDED_RD = random.Random(10)
-BUFFER_RANDOM = None
-BUFFER_RANGE = 0
-
-
-def random_sample(range_sample, nb_sample):
-    global BUFFER_RANGE
-    global BUFFER_RANDOM
-
-    if BUFFER_RANDOM is None or nb_sample != len(BUFFER_RANDOM) or range_sample != BUFFER_RANGE:
-        BUFFER_RANGE = range_sample
-        BUFFER_RANDOM = CONSTANT_SEEDED_RD.sample(range_sample, nb_sample)
-    return BUFFER_RANDOM
-
-
-# function to generate one hot encoded vector from a label
-def to_one_hot(label, nb_classes):
-    """
-    label in [0, nb_classes-1]
-    """
-    one_hot_encoded = np.zeros(nb_classes)
-    one_hot_encoded[label] = 1
-    return one_hot_encoded
-
-
-def read_categories_probability_from_name(filename):
-    categories_and_probabilities = filename.split(".")[0].split("_c")[1:]
-    category = int(categories_and_probabilities[0])
-    probabilities = []
-    for i in range(len(categories_and_probabilities) - 1):
-        current_category_and_probability = categories_and_probabilities[i + 1]
-        current_category, current_probability = current_category_and_probability.split("_")[:2]
-        # Probabilities have to be given in order
-        assert int(current_category) == i
-        probabilities.append(int(current_probability) / 100)
-    return category, probabilities
-
-
-def handle_image_type(image):
-    """
-    Adapt image type to be used by torchvision.
-
-    float32 -> make sure values are between 0 and 1.0
-    float64 -> convert to float32
-
-    uint8 -> does nothing
-    uint16 -> convert to float32 as torchvision does not support uint16
-    """
-
-    if image.dtype == np.float64:
-        image = image.astype("float32")
-    if image.dtype == np.float32:
-        if image.max() > 1.0:
-            print("WARNING: float image should have values between 0 and 1.0")
-    elif image.dtype == np.uint16:
-        coef = MAX_VALUES_BY_DTYPE[image.dtype]
-        image = image.astype(np.float32) * (1 / coef)
-    elif image.dtype == np.uint8:  # to run VAE
-        coef = MAX_VALUES_BY_DTYPE[image.dtype]
-        image = image.astype(np.float32) * (1 / coef)
-
-    return image
-
-
-def extract_patterns(files, patterns):
-    """Return files that match any of the given patterns."""
-    result = []
-    for name in files:
-        for pattern in patterns:
-            if fnmatch.fnmatch(name, pattern):
-                result.append(name)
-                break
-    return result
-
-
-def get_image_type_max(image):
-    image_max_value = image.max()
-    # Float case
-    if image_max_value <= 1.0:
-        return 1.0
-    # Integer case
-    possible_types = [np.uint8, np.uint16]
-    for image_type in possible_types:
-        if image_max_value > np.iinfo(image_type).max:
-            continue
-        return float(np.iinfo(image_type).max)
-    raise ValueError("Image max value is too high to be encoded in uint8 or uint16")
-
-
-def torch_from_numpy(np_array):
-    if np_array is None:
-        return None
-    # uint16 not supported by torch.from_numpy
-    if np_array.dtype == np.uint16:
-        np_array = np_array.astype(np.int32)
+import random
+import numpy as np
+from albumentations.augmentations.utils import MAX_VALUES_BY_DTYPE
+import fnmatch
+import torch
+
+
+CONSTANT_SEEDED_RD = random.Random(10)
+BUFFER_RANDOM = None
+BUFFER_RANGE = 0
+
+
+def random_sample(range_sample, nb_sample):
+    global BUFFER_RANGE
+    global BUFFER_RANDOM
+
+    if BUFFER_RANDOM is None or nb_sample != len(BUFFER_RANDOM) or range_sample != BUFFER_RANGE:
+        BUFFER_RANGE = range_sample
+        BUFFER_RANDOM = CONSTANT_SEEDED_RD.sample(range_sample, nb_sample)
+    return BUFFER_RANDOM
+
+
+# function to generate one hot encoded vector from a label
+def to_one_hot(label, nb_classes):
+    """
+    label in [0, nb_classes-1]
+    """
+    one_hot_encoded = np.zeros(nb_classes)
+    one_hot_encoded[label] = 1
+    return one_hot_encoded
+
+
+def read_categories_probability_from_name(filename):
+    categories_and_probabilities = filename.split(".")[0].split("_c")[1:]
+    category = int(categories_and_probabilities[0])
+    probabilities = []
+    for i in range(len(categories_and_probabilities) - 1):
+        current_category_and_probability = categories_and_probabilities[i + 1]
+        current_category, current_probability = current_category_and_probability.split("_")[:2]
+        # Probabilities have to be given in order
+        assert int(current_category) == i
+        probabilities.append(int(current_probability) / 100)
+    return category, probabilities
+
+
+def handle_image_type(image):
+    """
+    Adapt image type to be used by torchvision.
+
+    float32 -> make sure values are between 0 and 1.0
+    float64 -> convert to float32
+
+    uint8 -> does nothing
+    uint16 -> convert to float32 as torchvision does not support uint16
+    """
+
+    if image.dtype == np.float64:
+        image = image.astype("float32")
+    if image.dtype == np.float32:
+        if image.max() > 1.0:
+            print("WARNING: float image should have values between 0 and 1.0")
+    elif image.dtype == np.uint16:
+        coef = MAX_VALUES_BY_DTYPE[image.dtype]
+        image = image.astype(np.float32) * (1 / coef)
+    elif image.dtype == np.uint8:  # to run VAE
+        coef = MAX_VALUES_BY_DTYPE[image.dtype]
+        image = image.astype(np.float32) * (1 / coef)
+
+    return image
+
+
+def extract_patterns(files, patterns):
+    """Return files that match any of the given patterns."""
+    result = []
+    for name in files:
+        for pattern in patterns:
+            if fnmatch.fnmatch(name, pattern):
+                result.append(name)
+                break
+    return result
+
+
+def get_image_type_max(image):
+    image_max_value = image.max()
+    # Float case
+    if image_max_value <= 1.0:
+        return 1.0
+    # Integer case
+    possible_types = [np.uint8, np.uint16]
+    for image_type in possible_types:
+        if image_max_value > np.iinfo(image_type).max:
+            continue
+        return float(np.iinfo(image_type).max)
+    raise ValueError("Image max value is too high to be encoded in uint8 or uint16")
+
+
+def torch_from_numpy(np_array):
+    if np_array is None:
+        return None
+    # uint16 not supported by torch.from_numpy
+    if np_array.dtype == np.uint16:
+        np_array = np_array.astype(np.int32)
     return torch.from_numpy(np_array)
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework.egg-info/PKG-INFO` & `cnn_framework-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,84 @@
-Metadata-Version: 2.1
-Name: cnn-framework
-Version: 0.0.8
-Summary: CNN framework
-Home-page: https://https://github.com/15bonte/cnn_framework
-Author: Thomas Bonte
-Author-email: thomas.bonte@mines-paristech.fr
-Project-URL: Bug Tracker, https://https://github.com/15bonte/cnn_framework/issues
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=1.12.1
-Requires-Dist: scikit-image>=0.19.3
-Requires-Dist: matplotlib
-Requires-Dist: scikit-learn>=1.2.2
-Requires-Dist: pint>=0.19.2
-Requires-Dist: torchvision>=0.13.1
-Requires-Dist: albumentations==1.3.0
-Requires-Dist: torchmetrics>=0.11.4
-Requires-Dist: big-fish>=0.6.2
-Requires-Dist: pillow>=9.2.0
-Requires-Dist: segmentation-models-pytorch>=0.3.0
-Requires-Dist: protobuf==3.20.*
-Requires-Dist: tensorboard==2.8.0
-
-# CNN framework
-
-Run CNN models for classification, regression, segmentation, VAE, contrastive learning with any data set.
-
-## Installation
-
-First, create a dedicated conda environment using Python 3.9
-
-```bash
-conda create -n cnn_framework python=3.9
-conda activate cnn_framework
-```
-
-To install the latest github version of this library run the following using pip
-
-```bash
-pip install git+https://github.com/15bonte/cnn_framework
-```
-
-or alternatively you can clone the github repository
-
-```bash
-git clone https://github.com/15bonte/cnn_framework.git
-cd cnn_framework
-pip install -e .
-```
-
-If you want to run jupyter tutorials, you also need to install ipykernel
-
-```bash
-pip install ipykernel
-```
-
-If you want to work with VAE, you must also install [Pythae](https://github.com/clementchadebec/benchmark_VAE/tree/main) and [WandB](https://wandb.ai/home), which is not the case by default.
-
-```bash
-pip install pythae
-```
-
-```bash
-pip install wandb
-```
+Metadata-Version: 2.1
+Name: cnn_framework
+Version: 0.0.9
+Summary: CNN framework
+Home-page: https://github.com/15bonte/cnn_framework
+Author: Thomas Bonte
+Author-email: thomas.bonte@mines-paristech.fr
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/15bonte/cnn_detector/issues
+Project-URL: Documentation, https://github.com/15bonte/cnn_detector#README.md
+Project-URL: Source Code, https://github.com/15bonte/cnn_detector
+Project-URL: User Support, https://github.com/15bonte/cnn_detector/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch>=1.12.1
+Requires-Dist: scikit-image>=0.19.3
+Requires-Dist: matplotlib
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: pint>=0.19.2
+Requires-Dist: torchvision>=0.13.1
+Requires-Dist: albumentations==1.3.0
+Requires-Dist: torchmetrics>=0.11.4
+Requires-Dist: big-fish>=0.6.2
+Requires-Dist: pillow>=9.2.0
+Requires-Dist: segmentation-models-pytorch>=0.3.0
+Requires-Dist: protobuf==3.20.*
+Requires-Dist: tensorboard==2.8.0
+Requires-Dist: aicsimageio>=4.12.1
+Requires-Dist: tensorflow==2.8.0
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
+
+# CNN framework
+
+[![codecov](https://codecov.io/gh/15bonte/cnn_framework/branch/main/graph/badge.svg)](https://codecov.io/gh/15bonte/cnn_framework)
+[![tests](https://github.com/15bonte/cnn_framework/workflows/tests/badge.svg)](https://github.com/15bonte/cnn_framework/actions)
+
+Run CNN models for classification, regression, segmentation, VAE, contrastive learning with any data set.
+
+## Installation
+
+First, create a dedicated conda environment using Python 3.9
+
+```bash
+conda create -n cnn_framework python=3.9
+conda activate cnn_framework
+```
+
+To install the latest github version of this library run the following using pip
+
+```bash
+pip install git+https://github.com/15bonte/cnn_framework
+```
+
+or alternatively you can clone the github repository
+
+```bash
+git clone https://github.com/15bonte/cnn_framework.git
+cd cnn_framework
+pip install -e .
+```
+
+If you want to run jupyter tutorials, you also need to install ipykernel
+
+```bash
+pip install ipykernel
+```
+
+If you want to work with VAE, you must also install [Pythae](https://github.com/clementchadebec/benchmark_VAE/tree/main) and [WandB](https://wandb.ai/home), which is not the case by default.
+
+```bash
+pip install pythae
+```
+
+```bash
+pip install wandb
+```
```

### Comparing `cnn_framework-0.0.8/src/cnn_framework.egg-info/SOURCES.txt` & `cnn_framework-0.0.9/src/cnn_framework.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,54 @@
+.gitignore
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
+tox.ini
+.github/workflows/test_and_deploy.yml
+scripts/dummy_cnn/test.py
+scripts/dummy_cnn/train.py
+scripts/dummy_regression_cnn/test.py
+scripts/dummy_regression_cnn/train.py
+scripts/dummy_segmentation/test.py
+scripts/dummy_segmentation/train.py
+scripts/dummy_sim_clr/test.py
+scripts/dummy_sim_clr/train.py
+scripts/dummy_vae_model/train.py
 src/cnn_framework/__init__.py
+src/cnn_framework/_version.py
 src/cnn_framework.egg-info/PKG-INFO
 src/cnn_framework.egg-info/SOURCES.txt
 src/cnn_framework.egg-info/dependency_links.txt
 src/cnn_framework.egg-info/requires.txt
 src/cnn_framework.egg-info/top_level.txt
+src/cnn_framework/_tests/__init__.py
+src/cnn_framework/_tests/test_classification.py
+src/cnn_framework/_tests/test_regression.py
+src/cnn_framework/data/__init__.py
+src/cnn_framework/data/tools.py
 src/cnn_framework/dummy_cnn/__init__.py
 src/cnn_framework/dummy_cnn/data_set.py
 src/cnn_framework/dummy_cnn/model.py
 src/cnn_framework/dummy_cnn/model_params.py
+src/cnn_framework/dummy_cnn/test.py
+src/cnn_framework/dummy_cnn/train.py
 src/cnn_framework/dummy_regression_cnn/__init__.py
 src/cnn_framework/dummy_regression_cnn/data_set.py
 src/cnn_framework/dummy_regression_cnn/model.py
 src/cnn_framework/dummy_regression_cnn/model_params.py
+src/cnn_framework/dummy_regression_cnn/test.py
+src/cnn_framework/dummy_regression_cnn/train.py
 src/cnn_framework/dummy_segmentation/__init__.py
 src/cnn_framework/dummy_segmentation/data_set.py
 src/cnn_framework/dummy_segmentation/model.py
 src/cnn_framework/dummy_segmentation/model_params.py
+src/cnn_framework/dummy_segmentation/test.py
+src/cnn_framework/dummy_segmentation/train.py
 src/cnn_framework/dummy_sim_clr/__init__.py
 src/cnn_framework/dummy_sim_clr/data_set.py
 src/cnn_framework/dummy_sim_clr/model.py
 src/cnn_framework/dummy_sim_clr/model_params.py
 src/cnn_framework/dummy_vae_model/__init__.py
 src/cnn_framework/dummy_vae_model/data_set.py
 src/cnn_framework/dummy_vae_model/decoder.py
@@ -49,14 +73,15 @@
 src/cnn_framework/utils/data_sets/detection_data_set.py
 src/cnn_framework/utils/losses/__init__.py
 src/cnn_framework/utils/losses/dice_loss.py
 src/cnn_framework/utils/losses/focal_loss.py
 src/cnn_framework/utils/losses/info_nce_loss.py
 src/cnn_framework/utils/losses/jaccard_loss.py
 src/cnn_framework/utils/losses/loss_manager.py
+src/cnn_framework/utils/losses/ssim_loss.py
 src/cnn_framework/utils/lr_schedulers/__init__.py
 src/cnn_framework/utils/lr_schedulers/linear_warmup_cosine_annealing_lr.py
 src/cnn_framework/utils/metrics/__init__.py
 src/cnn_framework/utils/metrics/abstract_metric.py
 src/cnn_framework/utils/metrics/classification_accuracy.py
 src/cnn_framework/utils/metrics/mean_error_metric.py
 src/cnn_framework/utils/metrics/mean_squared_error_metric.py
@@ -85,8 +110,13 @@
 src/cnn_framework/utils/readers/abstract_reader.py
 src/cnn_framework/utils/readers/ciz_reader.py
 src/cnn_framework/utils/readers/images_reader.py
 src/cnn_framework/utils/readers/png_reader.py
 src/cnn_framework/utils/readers/tiff_reader.py
 src/cnn_framework/utils/readers/utils/__init__.py
 src/cnn_framework/utils/readers/utils/normalization.py
-src/cnn_framework/utils/readers/utils/projection.py
+src/cnn_framework/utils/readers/utils/projection.py
+tutorials/classification.ipynb
+tutorials/contrastive_learning.ipynb
+tutorials/regression.ipynb
+tutorials/segmentation.ipynb
+tutorials/vae.ipynb
```

