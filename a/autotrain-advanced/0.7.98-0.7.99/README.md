# Comparing `tmp/autotrain-advanced-0.7.98.tar.gz` & `tmp/autotrain-advanced-0.7.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.98.tar", last modified: Tue May 21 08:35:44 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.99.tar", last modified: Tue May 21 10:26:05 2024, max compression
```

## Comparing `autotrain-advanced-0.7.98.tar` & `autotrain-advanced-0.7.99.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.307764 autotrain-advanced-0.7.98/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.98/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-21 08:35:44.307764 autotrain-advanced-0.7.98/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-21 08:35:44.307764 autotrain-advanced-0.7.98/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.271765 autotrain-advanced-0.7.98/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-21 08:35:23.000000 autotrain-advanced-0.7.98/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.98/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.98/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/app/colab.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.98/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.98/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1923 2024-05-17 06:28:50.000000 autotrain-advanced-0.7.98/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17665 2024-05-17 15:11:13.000000 autotrain-advanced-0.7.98/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3409 2024-05-17 06:28:48.000000 autotrain-advanced-0.7.98/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.275765 autotrain-advanced-0.7.98/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.98/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.98/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.98/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_object_detection.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.98/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.98/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.98/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.98/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.98/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.98/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20755 2024-05-21 08:33:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.279765 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4608 2024-05-21 08:33:42.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7743 2024-05-21 08:33:52.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1793 2024-05-21 08:34:03.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3460 2024-05-21 08:34:15.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2268 2024-05-21 08:34:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.283765 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1826 2024-05-21 08:34:34.000000 autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.98/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.287765 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-21 08:35:44.000000 autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 08:35:44.287765 autotrain-advanced-0.7.98/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.98/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.205342 autotrain-advanced-0.7.99/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.99/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-21 10:26:05.205342 autotrain-advanced-0.7.99/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.99/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-21 10:26:05.209342 autotrain-advanced-0.7.99/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.99/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.181342 autotrain-advanced-0.7.99/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-21 10:25:29.000000 autotrain-advanced-0.7.99/src/autotrain/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/app/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.99/src/autotrain/app/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.99/src/autotrain/app/api_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.99/src/autotrain/app/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.99/src/autotrain/app/colab.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.99/src/autotrain/app/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.99/src/autotrain/app/models.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.99/src/autotrain/app/oauth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.99/src/autotrain/app/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/app/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.99/src/autotrain/app/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/app/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.99/src/autotrain/app/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.99/src/autotrain/app/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.99/src/autotrain/app/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.99/src/autotrain/app/templates/login.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1923 2024-05-17 06:28:50.000000 autotrain-advanced-0.7.99/src/autotrain/app/training_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17665 2024-05-17 15:11:13.000000 autotrain-advanced-0.7.99/src/autotrain/app/ui_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3409 2024-05-17 06:28:48.000000 autotrain-advanced-0.7.99/src/autotrain/app/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/backends/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.99/src/autotrain/backends/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/backends/base.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.99/src/autotrain/backends/endpoints.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.99/src/autotrain/backends/local.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.99/src/autotrain/backends/ngc.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-17 06:24:42.000000 autotrain-advanced-0.7.99/src/autotrain/backends/nvcf.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.99/src/autotrain/backends/spaces.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.99/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_object_detection.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_text_regression.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.99/src/autotrain/cli/run_tools.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.99/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.99/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.99/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.99/src/autotrain/parser.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.99/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.99/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.99/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.99/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/tools/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.99/src/autotrain/tools/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.99/src/autotrain/tools/convert_to_kohya.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.99/src/autotrain/tools/merge_adapter.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.185342 autotrain-advanced-0.7.99/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_default.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_dpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_orpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_reward.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_sft.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21465 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-16 17:02:41.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/train.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/train_xl.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8207 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4608 2024-05-21 08:33:42.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7895 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7743 2024-05-21 08:33:52.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9654 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1793 2024-05-21 08:34:03.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13181 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8484 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3460 2024-05-21 08:34:15.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.189342 autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7765 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2268 2024-05-21 08:34:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.193342 autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8265 2024-05-21 10:25:21.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1826 2024-05-21 08:34:34.000000 autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.99/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.193342 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-21 10:26:05.000000 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-21 10:26:05.000000 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-21 10:26:05.000000 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-21 10:26:05.000000 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-21 10:26:05.000000 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-21 10:26:05.000000 autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-21 10:26:05.193342 autotrain-advanced-0.7.99/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.99/static/logo.png
```

### Comparing `autotrain-advanced-0.7.98/LICENSE` & `autotrain-advanced-0.7.99/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/PKG-INFO` & `autotrain-advanced-0.7.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.98
+Version: 0.7.99
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.98/README.md` & `autotrain-advanced-0.7.99/README.md`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/setup.py` & `autotrain-advanced-0.7.99/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/__init__.py` & `autotrain-advanced-0.7.99/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warnings.filterwarnings("ignore", category=UserWarning, module="peft")
 warnings.filterwarnings("ignore", category=UserWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="datasets")
 warnings.filterwarnings("ignore", category=FutureWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="huggingface_hub")
 
 logger = Logger().get_logger()
-__version__ = "0.7.98"
+__version__ = "0.7.99"
 
 
 def is_colab():
     try:
         import google.colab
 
         return True
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/api_routes.py` & `autotrain-advanced-0.7.99/src/autotrain/app/api_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/app.py` & `autotrain-advanced-0.7.99/src/autotrain/app/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/colab.py` & `autotrain-advanced-0.7.99/src/autotrain/app/colab.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/db.py` & `autotrain-advanced-0.7.99/src/autotrain/app/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/models.py` & `autotrain-advanced-0.7.99/src/autotrain/app/models.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.99/src/autotrain/app/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/params.py` & `autotrain-advanced-0.7.99/src/autotrain/app/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.99/src/autotrain/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.99/src/autotrain/app/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.99/src/autotrain/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.99/src/autotrain/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/templates/login.html` & `autotrain-advanced-0.7.99/src/autotrain/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.99/src/autotrain/app/training_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/ui_routes.py` & `autotrain-advanced-0.7.99/src/autotrain/app/ui_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/app/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/app/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/backends/base.py` & `autotrain-advanced-0.7.99/src/autotrain/backends/base.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/backends/endpoints.py` & `autotrain-advanced-0.7.99/src/autotrain/backends/endpoints.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/backends/ngc.py` & `autotrain-advanced-0.7.99/src/autotrain/backends/ngc.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/backends/nvcf.py` & `autotrain-advanced-0.7.99/src/autotrain/backends/nvcf.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/backends/spaces.py` & `autotrain-advanced-0.7.99/src/autotrain/backends/spaces.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_object_detection.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_object_detection.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_seq2seq.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_text_regression.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_text_regression.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_token_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/run_tools.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/run_tools.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/commands.py` & `autotrain-advanced-0.7.99/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/help.py` & `autotrain-advanced-0.7.99/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/logging.py` & `autotrain-advanced-0.7.99/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/parser.py` & `autotrain-advanced-0.7.99/src/autotrain/parser.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.99/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.99/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.99/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.99/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/project.py` & `autotrain-advanced-0.7.99/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/tasks.py` & `autotrain-advanced-0.7.99/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/tools/convert_to_kohya.py` & `autotrain-advanced-0.7.99/src/autotrain/tools/convert_to_kohya.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/tools/merge_adapter.py` & `autotrain-advanced-0.7.99/src/autotrain/tools/merge_adapter.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_default.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_dpo.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_dpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_orpo.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_orpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_reward.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_reward.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/train_clm_sft.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/train_clm_sft.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/clm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,38 +325,56 @@
 
 
 def process_input_data(config):
     if config.data_path == f"{config.project_name}/autotrain-data":
         logger.info("loading dataset from disk")
         train_data = load_from_disk(config.data_path)[config.train_split]
     else:
-        train_data = load_dataset(
-            config.data_path,
-            split=config.train_split,
-            token=config.token,
-        )
+        if ":" in config.train_split:
+            dataset_config_name, split = config.train_split.split(":")
+            train_data = load_dataset(
+                config.data_path,
+                name=dataset_config_name,
+                split=split,
+                token=config.token,
+            )
+        else:
+            train_data = load_dataset(
+                config.data_path,
+                split=config.train_split,
+                token=config.token,
+            )
     # rename columns for reward trainer
     if config.trainer in ("dpo", "reward", "orpo"):
         if not (config.text_column == "chosen" and config.text_column in train_data.column_names):
             train_data = train_data.rename_column(config.text_column, "chosen")
         if not (config.rejected_text_column == "rejected" and config.rejected_text_column in train_data.column_names):
             train_data = train_data.rename_column(config.rejected_text_column, "rejected")
     if config.trainer in ("dpo", "orpo"):
         if not (config.prompt_text_column == "prompt" and config.prompt_text_column in train_data.column_names):
             train_data = train_data.rename_column(config.prompt_text_column, "prompt")
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
         if config.trainer in ("dpo", "reward", "orpo"):
             if not (config.text_column == "chosen" and config.text_column in valid_data.column_names):
                 valid_data = valid_data.rename_column(config.text_column, "chosen")
             if not (
                 config.rejected_text_column == "rejected" and config.rejected_text_column in valid_data.column_names
             ):
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/common.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/train.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/train_xl.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/train_xl.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,29 +41,47 @@
     if isinstance(config, dict):
         config = ImageClassificationParams(**config)
 
     valid_data = None
     if config.data_path == f"{config.project_name}/autotrain-data":
         train_data = load_from_disk(config.data_path)[config.train_split]
     else:
-        train_data = load_dataset(
-            config.data_path,
-            split=config.train_split,
-            token=config.token,
-        )
+        if ":" in config.train_split:
+            dataset_config_name, split = config.train_split.split(":")
+            train_data = load_dataset(
+                config.data_path,
+                name=dataset_config_name,
+                split=split,
+                token=config.token,
+            )
+        else:
+            train_data = load_dataset(
+                config.data_path,
+                split=config.train_split,
+                token=config.token,
+            )
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
     logger.info(f"Train data: {train_data}")
     logger.info(f"Valid data: {valid_data}")
 
     classes = train_data.features[config.target_column].names
     logger.info(f"Classes: {classes}")
     label2id = {c: i for i, c in enumerate(classes)}
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,29 +42,47 @@
     if isinstance(config, dict):
         config = ObjectDetectionParams(**config)
 
     valid_data = None
     if config.data_path == f"{config.project_name}/autotrain-data":
         train_data = load_from_disk(config.data_path)[config.train_split]
     else:
-        train_data = load_dataset(
-            config.data_path,
-            split=config.train_split,
-            token=config.token,
-        )
+        if ":" in config.train_split:
+            dataset_config_name, split = config.train_split.split(":")
+            train_data = load_dataset(
+                config.data_path,
+                name=dataset_config_name,
+                split=split,
+                token=config.token,
+            )
+        else:
+            train_data = load_dataset(
+                config.data_path,
+                split=config.train_split,
+                token=config.token,
+            )
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
     logger.info(f"Train data: {train_data}")
     logger.info(f"Valid data: {valid_data}")
 
     categories = train_data.features[config.objects_column].feature["category"].names
     id2label = dict(enumerate(categories))
     label2id = {v: k for k, v in id2label.items()}
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/object_detection/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,30 +51,48 @@
     valid_data = None
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             train_data = load_from_disk(config.data_path)[config.train_split]
         else:
-            train_data = load_dataset(
-                config.data_path,
-                split=config.train_split,
-                token=config.token,
-            )
+            if ":" in config.train_split:
+                dataset_config_name, split = config.train_split.split(":")
+                train_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                train_data = load_dataset(
+                    config.data_path,
+                    split=config.train_split,
+                    token=config.token,
+                )
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
     tokenizer = AutoTokenizer.from_pretrained(config.model, token=config.token, trust_remote_code=ALLOW_REMOTE_CODE)
 
     train_data = Seq2SeqDataset(data=train_data, tokenizer=tokenizer, config=config)
     if config.valid_split is not None:
         valid_data = Seq2SeqDataset(data=valid_data, tokenizer=tokenizer, config=config)
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,31 +135,49 @@
 
     train_data = None
     valid_data = None
     if config.data_path == f"{config.project_name}/autotrain-data":
         logger.info("loading dataset from disk")
         train_data = load_from_disk(config.data_path)[config.train_split]
     else:
-        train_data = load_dataset(
-            config.data_path,
-            split=config.train_split,
-            token=config.token,
-        )
+        if ":" in config.train_split:
+            dataset_config_name, split = config.train_split.split(":")
+            train_data = load_dataset(
+                config.data_path,
+                name=dataset_config_name,
+                split=split,
+                token=config.token,
+            )
+        else:
+            train_data = load_dataset(
+                config.data_path,
+                split=config.train_split,
+                token=config.token,
+            )
     train_data = train_data.to_pandas()
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
         valid_data = valid_data.to_pandas()
 
     if valid_data is None:
         raise Exception("valid_data is None. Please provide a valid_split for tabular training.")
 
     # determine which columns are categorical
     if config.categorical_columns is None:
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,30 +46,48 @@
     valid_data = None
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             train_data = load_from_disk(config.data_path)[config.train_split]
         else:
-            train_data = load_dataset(
-                config.data_path,
-                split=config.train_split,
-                token=config.token,
-            )
+            if ":" in config.train_split:
+                dataset_config_name, split = config.train_split.split(":")
+                train_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                train_data = load_dataset(
+                    config.data_path,
+                    split=config.train_split,
+                    token=config.token,
+                )
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
     classes = train_data.features[config.target_column].names
     label2id = {c: i for i, c in enumerate(classes)}
     num_classes = len(classes)
 
     if num_classes < 2:
         raise ValueError("Invalid number of classes. Must be greater than 1.")
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,30 +46,48 @@
     valid_data = None
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             train_data = load_from_disk(config.data_path)[config.train_split]
         else:
-            train_data = load_dataset(
-                config.data_path,
-                split=config.train_split,
-                token=config.token,
-            )
+            if ":" in config.train_split:
+                dataset_config_name, split = config.train_split.split(":")
+                train_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                train_data = load_dataset(
+                    config.data_path,
+                    split=config.train_split,
+                    token=config.token,
+                )
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
     model_config = AutoConfig.from_pretrained(config.model, num_labels=1)
     model_config._num_labels = 1
     label2id = {"target": 0}
     model_config.label2id = label2id
     model_config.id2label = {v: k for k, v in label2id.items()}
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/text_regression/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/text_regression/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,30 +47,48 @@
     valid_data = None
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             train_data = load_from_disk(config.data_path)[config.train_split]
         else:
-            train_data = load_dataset(
-                config.data_path,
-                split=config.train_split,
-                token=config.token,
-            )
+            if ":" in config.train_split:
+                dataset_config_name, split = config.train_split.split(":")
+                train_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                train_data = load_dataset(
+                    config.data_path,
+                    split=config.train_split,
+                    token=config.token,
+                )
 
     if config.valid_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             valid_data = load_from_disk(config.data_path)[config.valid_split]
         else:
-            valid_data = load_dataset(
-                config.data_path,
-                split=config.valid_split,
-                token=config.token,
-            )
+            if ":" in config.valid_split:
+                dataset_config_name, split = config.valid_split.split(":")
+                valid_data = load_dataset(
+                    config.data_path,
+                    name=dataset_config_name,
+                    split=split,
+                    token=config.token,
+                )
+            else:
+                valid_data = load_dataset(
+                    config.data_path,
+                    split=config.valid_split,
+                    token=config.token,
+                )
 
     label_list = train_data.features[config.tags_column].feature.names
     num_classes = len(label_list)
 
     model_config = AutoConfig.from_pretrained(config.model, num_labels=num_classes)
     model_config._num_labels = num_classes
     model_config.label2id = {l: i for i, l in enumerate(label_list)}
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/trainers/token_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain/utils.py` & `autotrain-advanced-0.7.99/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.98
+Version: 0.7.99
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.99/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.98/static/logo.png` & `autotrain-advanced-0.7.99/static/logo.png`

 * *Files identical despite different names*

