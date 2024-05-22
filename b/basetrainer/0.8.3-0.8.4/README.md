# Comparing `tmp/basetrainer-0.8.3.tar.gz` & `tmp/basetrainer-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basetrainer-0.8.3.tar", last modified: Wed May 15 09:01:24 2024, max compression
+gzip compressed data, was "basetrainer-0.8.4.tar", last modified: Wed May 22 11:21:58 2024, max compression
```

## Comparing `basetrainer-0.8.3.tar` & `basetrainer-0.8.4.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/
--rwxrwx---   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 basetrainer-0.8.3/LICENCE
--rw-r-----   0 PKing     (1000) PKing     (1000)      254 2024-05-15 09:01:14.000000 basetrainer-0.8.3/PKG-INFO
--rw-r-----   0 PKing     (1000) PKing     (1000)    17572 2023-08-24 03:00:36.000000 basetrainer-0.8.3/README.rst
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/
--rw-r-----   0 PKing     (1000) PKing     (1000)      141 2024-05-15 09:01:07.000000 basetrainer-0.8.3/basetrainer/__init__.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/callbacks/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/callbacks/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1166 2022-01-26 04:35:31.000000 basetrainer-0.8.3/basetrainer/callbacks/callbacks.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     3127 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/callbacks/log_history.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1497 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/callbacks/losses_recorder.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     7368 2024-02-21 04:38:14.000000 basetrainer-0.8.3/basetrainer/callbacks/model_checkpoint.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3208 2022-02-08 08:35:30.000000 basetrainer-0.8.3/basetrainer/callbacks/multi_losses_recorder.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/criterion/
--rwxrwx---   0 PKing     (1000) PKing     (1000)        1 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/criterion/__init__.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     4592 2023-03-17 10:16:56.000000 basetrainer-0.8.3/basetrainer/criterion/criterion.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/dataloader/
--rw-r-----   0 PKing     (1000) PKing     (1000)      114 2024-03-25 00:30:25.000000 basetrainer-0.8.3/basetrainer/dataloader/__init__.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     8310 2024-03-25 00:31:08.000000 basetrainer-0.8.3/basetrainer/dataloader/data_resample.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/engine/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/engine/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1510 2022-01-26 04:35:31.000000 basetrainer-0.8.3/basetrainer/engine/base.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     7863 2022-01-17 09:22:27.000000 basetrainer-0.8.3/basetrainer/engine/comm.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     5377 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/engine/engine.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3920 2022-01-17 09:22:27.000000 basetrainer-0.8.3/basetrainer/engine/launch.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     3082 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/engine/onnx_engine.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     5101 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/engine/trainer.py
--rw-r-----   0 PKing     (1000) PKing     (1000)    12287 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/engine/trt_engine.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/metric/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/__init__.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     4328 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/accuracy_recorder.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/
--rwxrwx---   0 PKing     (1000) PKing     (1000)      168 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/__init__.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     3122 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/acc.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     5457 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/classification_report.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     6586 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/eval_utils.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     1634 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/evaluate.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     2071 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/iou.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     4905 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/metrics.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     1424 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/pandas_tools.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     9529 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/pr.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     2469 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/psnr.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     7712 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/roc.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     7781 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/verification.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/
--rw-r-----   0 PKing     (1000) PKing     (1000)      114 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/__init__.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/
--rw-r-----   0 PKing     (1000) PKing     (1000)      119 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/__init__.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     7291 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/bboxes_match.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     2741 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/iou.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)    10147 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     6100 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval_torch.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     6477 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/map_metric.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/models/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2022-01-17 09:46:24.000000 basetrainer-0.8.3/basetrainer/models/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3339 2023-12-18 08:57:10.000000 basetrainer-0.8.3/basetrainer/models/build_models.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/optimizer/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/optimizer/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2588 2023-03-17 10:16:56.000000 basetrainer-0.8.3/basetrainer/optimizer/build_optimizer.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/pruning/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/pruning/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)    11795 2024-02-20 01:18:45.000000 basetrainer-0.8.3/basetrainer/pruning/nni_pruning.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2693 2022-01-17 09:22:27.000000 basetrainer-0.8.3/basetrainer/pruning/slim_pruning.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     6843 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/pruning/torch_pruning.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/scheduler/
--rw-rw----   0 PKing     (1000) PKing     (1000)     2981 2023-12-20 01:45:34.000000 basetrainer-0.8.3/basetrainer/scheduler/CosineAnnealingLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2141 2023-12-26 11:07:58.000000 basetrainer-0.8.3/basetrainer/scheduler/ExponentialLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2633 2022-12-16 02:49:37.000000 basetrainer-0.8.3/basetrainer/scheduler/LambdaLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3018 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/scheduler/MultiStepLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     4378 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/scheduler/MultiStepValue.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1657 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/scheduler/WarmUpLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/scheduler/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2150 2022-12-16 02:49:37.000000 basetrainer-0.8.3/basetrainer/scheduler/build_scheduler.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/utils/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/utils/__init__.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/utils/converter/
--rw-rw----   0 PKing     (1000) PKing     (1000)      130 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/converter/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2764 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/converter/onnx2trt.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3147 2023-12-28 02:54:06.000000 basetrainer-0.8.3/basetrainer/utils/converter/pytorch2onnx.py
--rw-r-----   0 PKing     (1000) PKing     (1000)      151 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/utils/file_utils.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     5722 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/utils/heatmap_utils.py
--rw-r-----   0 PKing     (1000) PKing     (1000)      152 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/utils/image_utils.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     6849 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/log.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     3781 2022-01-26 04:35:31.000000 basetrainer-0.8.3/basetrainer/utils/plot_utils.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     5037 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/utils/setup_config.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1399 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/utils/summary.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     4171 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/torch_data.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)    17572 2024-05-15 09:01:07.000000 basetrainer-0.8.3/basetrainer/utils/torch_tools.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     6261 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/utils/torchcam_utils.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/
--rw-r-----   0 PKing     (1000) PKing     (1000)      254 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/PKG-INFO
--rw-r-----   0 PKing     (1000) PKing     (1000)     2842 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/SOURCES.txt
--rw-r-----   0 PKing     (1000) PKing     (1000)        1 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/dependency_links.txt
--rw-r-----   0 PKing     (1000) PKing     (1000)        1 2023-08-23 09:06:15.000000 basetrainer-0.8.3/basetrainer.egg-info/not-zip-safe
--rw-r-----   0 PKing     (1000) PKing     (1000)       12 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/top_level.txt
--rw-r-----   0 PKing     (1000) PKing     (1000)       38 2024-05-15 09:01:14.000000 basetrainer-0.8.3/setup.cfg
--rwxr-x---   0 PKing     (1000) PKing     (1000)     2115 2023-08-24 03:00:36.000000 basetrainer-0.8.3/setup.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/test/
--rw-rw----   0 PKing     (1000) PKing     (1000)     3179 2023-12-26 11:08:42.000000 basetrainer-0.8.3/test/test_scheduler.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:49.000000 basetrainer-0.8.4/
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 basetrainer-0.8.4/LICENCE
+-rw-r-----   0 PKing     (1000) PKing     (1000)      254 2024-05-22 11:21:49.000000 basetrainer-0.8.4/PKG-INFO
+-rw-r-----   0 PKing     (1000) PKing     (1000)    17572 2023-08-24 03:00:36.000000 basetrainer-0.8.4/README.rst
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      141 2024-05-22 11:21:40.000000 basetrainer-0.8.4/basetrainer/__init__.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer/callbacks/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/callbacks/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1166 2022-01-26 04:35:31.000000 basetrainer-0.8.4/basetrainer/callbacks/callbacks.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     3127 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/callbacks/log_history.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1497 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/callbacks/losses_recorder.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     7368 2024-02-21 04:38:14.000000 basetrainer-0.8.4/basetrainer/callbacks/model_checkpoint.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3208 2022-02-08 08:35:30.000000 basetrainer-0.8.4/basetrainer/callbacks/multi_losses_recorder.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer/criterion/
+-rwxrwx---   0 PKing     (1000) PKing     (1000)        1 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/criterion/__init__.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     4592 2023-03-17 10:16:56.000000 basetrainer-0.8.4/basetrainer/criterion/criterion.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer/dataloader/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      114 2024-03-25 00:30:25.000000 basetrainer-0.8.4/basetrainer/dataloader/__init__.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     8310 2024-03-25 00:31:08.000000 basetrainer-0.8.4/basetrainer/dataloader/data_resample.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/engine/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/engine/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1510 2022-01-26 04:35:31.000000 basetrainer-0.8.4/basetrainer/engine/base.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     7863 2022-01-17 09:22:27.000000 basetrainer-0.8.4/basetrainer/engine/comm.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     5377 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/engine/engine.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3920 2022-01-17 09:22:27.000000 basetrainer-0.8.4/basetrainer/engine/launch.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     3082 2023-12-18 08:58:42.000000 basetrainer-0.8.4/basetrainer/engine/onnx_engine.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     5101 2023-12-18 08:58:42.000000 basetrainer-0.8.4/basetrainer/engine/trainer.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     4924 2024-05-22 11:09:07.000000 basetrainer-0.8.4/basetrainer/engine/trt_calibrator.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)    14980 2024-05-22 11:20:46.000000 basetrainer-0.8.4/basetrainer/engine/trt_engine.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/metric/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/__init__.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     4328 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/accuracy_recorder.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/
+-rwxrwx---   0 PKing     (1000) PKing     (1000)      168 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/__init__.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     3122 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/acc.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     5457 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/classification_report.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     6586 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/eval_utils.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     1634 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/evaluate.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     2071 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/iou.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     4905 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/metrics.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     1424 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/pandas_tools.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     9529 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/pr.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     2469 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/psnr.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     7712 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/roc.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     7781 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/metric/eval_tools/verification.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      114 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/__init__.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      119 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/__init__.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     7291 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/bboxes_match.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     2741 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/iou.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)    10147 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/map_eval.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     6100 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/map_eval_torch.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     6477 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/metric/map_tools/map_metric.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/models/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2022-01-17 09:46:24.000000 basetrainer-0.8.4/basetrainer/models/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3339 2023-12-18 08:57:10.000000 basetrainer-0.8.4/basetrainer/models/build_models.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/optimizer/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/optimizer/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2588 2023-03-17 10:16:56.000000 basetrainer-0.8.4/basetrainer/optimizer/build_optimizer.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/pruning/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/pruning/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)    11795 2024-02-20 01:18:45.000000 basetrainer-0.8.4/basetrainer/pruning/nni_pruning.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2693 2022-01-17 09:22:27.000000 basetrainer-0.8.4/basetrainer/pruning/slim_pruning.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     6843 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/pruning/torch_pruning.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:48.000000 basetrainer-0.8.4/basetrainer/scheduler/
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2981 2023-12-20 01:45:34.000000 basetrainer-0.8.4/basetrainer/scheduler/CosineAnnealingLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2141 2023-12-26 11:07:58.000000 basetrainer-0.8.4/basetrainer/scheduler/ExponentialLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2633 2022-12-16 02:49:37.000000 basetrainer-0.8.4/basetrainer/scheduler/LambdaLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3018 2021-12-28 07:55:23.000000 basetrainer-0.8.4/basetrainer/scheduler/MultiStepLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     4378 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/scheduler/MultiStepValue.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1657 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/scheduler/WarmUpLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/scheduler/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2150 2022-12-16 02:49:37.000000 basetrainer-0.8.4/basetrainer/scheduler/build_scheduler.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:49.000000 basetrainer-0.8.4/basetrainer/utils/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/utils/__init__.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:49.000000 basetrainer-0.8.4/basetrainer/utils/converter/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      130 2023-01-05 11:21:37.000000 basetrainer-0.8.4/basetrainer/utils/converter/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2764 2023-01-05 11:21:37.000000 basetrainer-0.8.4/basetrainer/utils/converter/onnx2trt.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3147 2023-12-28 02:54:06.000000 basetrainer-0.8.4/basetrainer/utils/converter/pytorch2onnx.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)      151 2023-12-18 08:58:42.000000 basetrainer-0.8.4/basetrainer/utils/file_utils.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     5722 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/utils/heatmap_utils.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)      152 2023-12-18 08:58:42.000000 basetrainer-0.8.4/basetrainer/utils/image_utils.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     6849 2023-01-05 11:21:37.000000 basetrainer-0.8.4/basetrainer/utils/log.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     3781 2022-01-26 04:35:31.000000 basetrainer-0.8.4/basetrainer/utils/plot_utils.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     5037 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/utils/setup_config.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1399 2021-12-28 07:55:24.000000 basetrainer-0.8.4/basetrainer/utils/summary.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     4171 2023-01-05 11:21:37.000000 basetrainer-0.8.4/basetrainer/utils/torch_data.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)    17572 2024-05-15 09:01:07.000000 basetrainer-0.8.4/basetrainer/utils/torch_tools.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     6261 2023-08-24 03:00:36.000000 basetrainer-0.8.4/basetrainer/utils/torchcam_utils.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer.egg-info/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      254 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer.egg-info/PKG-INFO
+-rw-r-----   0 PKing     (1000) PKing     (1000)     2879 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer.egg-info/SOURCES.txt
+-rw-r-----   0 PKing     (1000) PKing     (1000)        1 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer.egg-info/dependency_links.txt
+-rw-r-----   0 PKing     (1000) PKing     (1000)        1 2023-08-23 09:06:15.000000 basetrainer-0.8.4/basetrainer.egg-info/not-zip-safe
+-rw-r-----   0 PKing     (1000) PKing     (1000)       12 2024-05-22 11:21:47.000000 basetrainer-0.8.4/basetrainer.egg-info/top_level.txt
+-rw-r-----   0 PKing     (1000) PKing     (1000)       38 2024-05-22 11:21:49.000000 basetrainer-0.8.4/setup.cfg
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     2115 2023-08-24 03:00:36.000000 basetrainer-0.8.4/setup.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-22 11:21:49.000000 basetrainer-0.8.4/test/
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3179 2023-12-26 11:08:42.000000 basetrainer-0.8.4/test/test_scheduler.py
```

### Comparing `basetrainer-0.8.3/LICENCE` & `basetrainer-0.8.4/LICENCE`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/README.rst` & `basetrainer-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/callbacks/callbacks.py` & `basetrainer-0.8.4/basetrainer/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/callbacks/log_history.py` & `basetrainer-0.8.4/basetrainer/callbacks/log_history.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/callbacks/losses_recorder.py` & `basetrainer-0.8.4/basetrainer/callbacks/losses_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/callbacks/model_checkpoint.py` & `basetrainer-0.8.4/basetrainer/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/callbacks/multi_losses_recorder.py` & `basetrainer-0.8.4/basetrainer/callbacks/multi_losses_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/criterion/criterion.py` & `basetrainer-0.8.4/basetrainer/criterion/criterion.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/dataloader/data_resample.py` & `basetrainer-0.8.4/basetrainer/dataloader/data_resample.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/base.py` & `basetrainer-0.8.4/basetrainer/engine/base.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/comm.py` & `basetrainer-0.8.4/basetrainer/engine/comm.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/engine.py` & `basetrainer-0.8.4/basetrainer/engine/engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/launch.py` & `basetrainer-0.8.4/basetrainer/engine/launch.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/onnx_engine.py` & `basetrainer-0.8.4/basetrainer/engine/onnx_engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/trainer.py` & `basetrainer-0.8.4/basetrainer/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/engine/trt_engine.py` & `basetrainer-0.8.4/basetrainer/engine/trt_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,50 @@
 """
     @Author : PKing
     @E-mail : 390737991@qq.com
     @Date   : 2022-12-23 14:45:13
     @Brief  :常见问题：
     (1) TRT多模型推理时，Pytorch模型可能会出现冲突，建议Pytorch模型不要使用DataParallel加载模型推理
     (2) 推理输入数据batch_size>1时，需要在转换ONNX模型时，设置dynamic=True
+    (3) 多次`import pycuda.autoinit` 可能出现异常:Error Code 1: Cask (Cask convolution execution)
 """
 import os
 import cv2
 import numpy as np
 import pycuda.driver as cuda
+import pycuda.autoinit
 import tensorrt as trt
+import traceback
 from typing import Tuple, List
 
 cuda.init()
 device_context = cuda.Device(0).make_context()
 TRT_LOGGER = trt.Logger(trt.Logger.ERROR)  # TRT_LOGGER = trt.Logger(trt.Logger.WARNING)
 
 
 class TRTEngine(object):
     """TensorRT引擎"""
 
-    def __init__(self, model_file: str, input_shape: tuple):
+    def __init__(self, model_file: str, input_shape: tuple, quant=1, calibrator=None):
         """
         https://www.jianshu.com/p/36ff0e224112
         :param model_file: 模型文件，可以是*.trt或者*.onnx文件
         :param input_shape:输入维度(B, C, H, W)
+        :param quant: 0:不进行量化，1:进行半精度量化(FP16)，2:进行INT8量化(INT8)
+        :param calibrator: 校准模块，INT8量化时需要
         """
         print("tensorrt:{}".format(trt.__version__))  # 8.4.1.5
         assert len(input_shape) == 4
         B, C, H, W = input_shape
         self.input_size = (W, H)
         self.batch_size = B
+        self.calibrator = calibrator
         self.input_shape = input_shape
         # Load a serialized engine into memory
-        # self.engine = self.load_engine(model_file)  # 加载序列化的cuda引擎
-        self.engine = self.build_engine_onnx(model_file=model_file, input_shape=self.input_shape)
+        self.engine = self.load_model(model_file=model_file, input_shape=self.input_shape, quant=quant)
         # Create context, this can be re-used  创建 执行环境
         self.context = self.engine.create_execution_context()
         # Profile 0 (first profile) is used by default  context可以设置多个profile， 这里选择第一个，也是默认的profile，其中规定了输入尺寸的变化区间
         self.context.active_optimization_profile = 0
         print("Active Optimization Profile: {}".format(self.context.active_optimization_profile))
         # These binding_idxs can change if either the context or the
         # active_optimization_profile are changed  获得输入输出变量名对应profile的idx
@@ -57,42 +62,54 @@
         print("\tInput names: {}".format(self.input_names))
         # 获得输出变量的变量名
         print("Output Metadata")
         self.output_names = [self.engine.get_binding_name(binding_idx) for binding_idx in self.output_binding_idxs]
         print("\tNumber of Outputs: {}".format(len(self.output_binding_idxs)))
         print("\tOutput names     : {}".format(self.output_names))
         print("\tOutput Bindings for Profile {}: {}\n".format(self.context.active_optimization_profile,
-                                                              self.output_binding_idxs), flush=True)
-        print("\tTRT model loaded successfully:{}".format(model_file.replace(".onnx", ".trt")))
+                                                              self.output_binding_idxs))
+        print("TRT model loaded successfully:{}".format(model_file.replace(".onnx", ".trt")))
+        print('-----------' * 5, flush=True)
 
-    @staticmethod
-    def build_engine_onnx(model_file: str, input_shape, fp16=True):
+    def load_model(self, model_file: str, input_shape, quant=1):
         """
-        :param model_file: onnx file or trt file
-        :param batch_size:
-        :param fp16_mode:
-        :param max_workspace:
+        :param model_file: ONNX或TRT模型文件
+        :param input_shape: 模型输入维度
+        :param quant: 0:不进行量化，1:进行半精度量化，2:进行INT8量化
         :return:
         """
-        if model_file.endswith("trt") and os.path.exists(model_file):
-            trt_file = model_file
-            print('Reload engine file: {}'.format(trt_file))
-            engine = TRTEngine.load_engine(trt_file)
-            return engine
-        elif model_file.endswith("onnx"):
-            onnx_file = model_file
-            trt_file = model_file[:-len("onnx")] + "trt"
-        else:
-            raise Exception("model_file:{}".format(model_file))
-        print("Completed parsing of ONNX file")
-        print("convert ONNX file to TRT Engine")
-        print("load ONNX  file:{}".format(onnx_file))
-        engine = onnx2trt(onnx_file, trt_file=trt_file, input_shape=input_shape, fp16=fp16)
+        print('-----------' * 5)
+        engine = None
+        if model_file.endswith(".trt"):
+            try:
+                print('Load TRT model file         : {}'.format(model_file))
+                engine = TRTEngine.load_engine(model_file)
+                assert engine is not None, Exception('Load TRT model failed       : {}'.format(model_file))
+                print('Load TRT Engine successfully: {}'.format(model_file))
+            except Exception as e:
+                traceback.print_exc()
+                print('Load TRT model failed       : {}'.format(model_file), flush=True)
+                model_file = model_file.replace(".trt", ".onnx")
+        # TODO 如果TRT模型加载失败，则尝试从ONNX文件编译模型
+        if model_file.endswith(".onnx") and os.path.exists(model_file):
+            trt_file = model_file.replace(".onnx", ".trt")
+            print('Try to build TRT Engine from ONNX file:{}'.format(model_file))
+            engine = onnx2trt(model_file, trt_file=trt_file, input_shape=input_shape,
+                              quant=quant, calibrator=self.calibrator)
+            print("Completed parsing of ONNX file")
+            print('Load TRT Engine successfully: {}'.format(trt_file))
+        print('-----------' * 5, flush=True)
         return engine
 
+    @staticmethod
+    def load_engine(filename: str):
+        # Load serialized engine file into memory 加载序列化的cuda引擎并进行反序列化
+        with open(filename, "rb") as f, trt.Runtime(TRT_LOGGER) as runtime:
+            return runtime.deserialize_cuda_engine(f.read())
+
     def __call__(self, input_tensor):
         return self.inference(input_tensor)
 
     def inference(self, image_tensor):
         """
         image_tensor = image.transpose(2, 0, 1)
         image_tensor = image_tensor[np.newaxis, :]
@@ -128,20 +145,14 @@
             cuda.memcpy_dtoh(h_output, d_output)
         # 释放显存
         for b in bindings: b.free()
         device_context.pop()
         return host_outputs
 
     @staticmethod
-    def load_engine(filename: str):
-        # Load serialized engine file into memory 加载序列化的cuda引擎并进行反序列化
-        with open(filename, "rb") as f, trt.Runtime(TRT_LOGGER) as runtime:
-            return runtime.deserialize_cuda_engine(f.read())
-
-    @staticmethod
     def get_binding_idxs(engine: trt.ICudaEngine, profile_index: int):
         # Calculate start/end binding indices for current context's profile
         num_bindings_per_profile = engine.num_bindings // engine.num_optimization_profiles
         start_binding = profile_index * num_bindings_per_profile
         end_binding = start_binding + num_bindings_per_profile
         print("Engine/Binding Metadata")
         print("\tNumber of optimization profiles: {}".format(engine.num_optimization_profiles))
@@ -182,20 +193,21 @@
             buffer = np.empty(output_shape, dtype=np.float32)
             host_outputs.append(buffer)
             # Allocate output buffers on device
             device_outputs.append(cuda.mem_alloc(buffer.nbytes))
         return host_outputs, device_outputs
 
 
-def onnx2trt(onnx_file, trt_file=None, input_shape=(1, 3, 160, 160), max_batch_size=8, fp16=True):
+def onnx2trt(onnx_file, trt_file=None, input_shape=(1, 3, 160, 160), max_batch_size=8, quant=1, calibrator=None):
     """
     :param onnx_file: ONNX模型文件
     :param trt_file: 输出TRT模型文件，默认为onnx_file同目录
     :param input_shape: 模型输入维度
-    :param fp16: 是否进行半精度量化
+    :param quant: 0:不进行量化，1:进行半精度量化，2:进行INT8量化
+    :param calibrator: 校准模块，INT8量化时需要
     :return:
     """
 
     def GiB(val):
         return val * 1 << 30
 
     if not trt_file: trt_file = onnx_file[:-len("onnx")] + "trt"
@@ -203,39 +215,79 @@
     explicit_batch = 1 << (int)(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH)
     with trt.Builder(TRT_LOGGER) as builder, \
             builder.create_network(explicit_batch) as network, \
             trt.OnnxParser(network, TRT_LOGGER) as parser:
         builder.max_batch_size = max_batch_size  # trt推理时最大支持的batchsize
         config = builder.create_builder_config()
         config.max_workspace_size = GiB(4)
-        if fp16: config.set_flag(trt.BuilderFlag.FP16)
-        # if int8:config.set_flag(trt.BuilderFlag.INT8)
+        if quant == 1:
+            # assert (builder.platform_has_fast_fp16 == True), 'not support fp16'
+            config.set_flag(trt.BuilderFlag.FP16)
+        elif quant == 2:
+            # assert (builder.platform_has_fast_int8 == True), 'not support int8'
+            config.set_flag(trt.BuilderFlag.INT8)
+            config.int8_calibrator = calibrator
         print('Loading ONNX file from path {}...'.format(onnx_file))
         with open(onnx_file, 'rb') as model:
             print('Beginning ONNX file parsing')
             parser.parse(model.read())
         print('Completed parsing of ONNX file')
         print('Building an engine from file {}; this may take a while...'.format(onnx_file))
         profile = builder.create_optimization_profile()  # 动态输入时候需要 分别为最小输入、常规输入、最大输入
         # 有几个输入就要写几个profile.set_shape 名字和转onnx的时候要对应
-        # tensorrt6以后的版本是支持动态输入的，需要给每个动态输入绑定一个profile，用于指定最小值，常规值和最大值，如果超出这个范围会报异常。
-        profile.set_shape("input", (1, C, H, W), (batch_size, C, H, W), (batch_size * 2, C, H, W))
+        # tensorrt6以后的版本是支持动态输入的，需要给每个动态输入绑定一个profile，
+        # 用于指定最小值常规值和最大值，如果超出这个范围会报异常。
+        # min=(1, C, H, W), opt=(batch_size, C, H, W),max=(batch_size, C, H, W)
+        inputs = [network.get_input(i) for i in range(network.num_inputs)]
+        for inp in inputs:
+            profile.set_shape(inp.name, (1, C, H, W), (batch_size, C, H, W), (batch_size, C, H, W))
         config.add_optimization_profile(profile)
+        config.set_calibration_profile(profile)
         engine = builder.build_engine(network, config)
     print("Completed creating Engine")
     # 保存engine文件
     with open(trt_file, "wb") as f:
         f.write(engine.serialize())
     print("save TRT file:{}".format(trt_file))
     return engine
 
 
+def test_performance(image_dir="./test.png", itera=10000):
+    from pybaseutils import file_utils, time_utils
+    input_size = (518, 518)
+    # model_file = "./yolov5s_640_640.trt"
+    model_file = "./yolov5s_640_640_fp16.trt"
+    # model_file = "./yolov5s_640_640_int8.trt"
+    input_shape = (1, 3, input_size[1], input_size[0])  # (B,C,H,W)
+    engine = TRTEngine(model_file, input_shape=input_shape, quant=2, calibrator=None)
+    image_list = file_utils.get_files_lists(file_dir=image_dir)
+    image_list = image_list * itera
+    for i in range(itera):
+        image = cv2.imread(image_list[i])
+        image = cv2.resize(image, (input_size[1], input_size[0]))
+        image = image.transpose((2, 0, 1)).astype(np.float32) / 255.0
+        inp_tensor = np.array([image], dtype=np.float32)
+        with time_utils.Performance() as p:
+            out_tensor = engine(inp_tensor)[0]
+        print("inp_tensor:{}".format(inp_tensor.shape))
+        print("out_tensor:{}".format(out_tensor.shape))
+
+
+def test_example():
+    from basetrainer.engine.trt_calibrator import ImageDataset, Calibrator, build_transform
+    input_size = (640, 640)
+    image_dir = '/home/PKing/nasdata/tmp/tmp/face_person/VOC/VOC2012/JPEGImages'
+    dataset = ImageDataset(image_dir=image_dir, transform=build_transform, input_size=input_size)
+    calibrator = Calibrator(dataset, cache_file="./calibration.cache")
+
+    model_file = "./yolov5s_640_640.onnx"
+    input_shape = (1, 3, input_size[1], input_size[0])
+    engine = TRTEngine(model_file, input_shape=input_shape, quant=2, calibrator=calibrator)
+    inp_tensor = np.ones(shape=input_shape, dtype=np.float32)
+    out_tensor = engine(inp_tensor)[0]
+    print("inp_tensor:{}".format(inp_tensor.shape))
+    print("out_tensor:{}".format(out_tensor.shape))
+
+
 if __name__ == "__main__":
-    trt_file = "/home/dm/nasdata/release/handwriting/daip-calligraphy-hard/calligraphy-hard-recognizer/app/infercore/resource/resnet18_160_160_c3594_7.onnx"
-    # trt_file = "/home/dm/nasdata/release/handwriting/daip-calligraphy-hard/calligraphy-hard-recognizer/app/infercore/resource/resnet18_160_160_c3594_7.trt"
-    input_shape = (16, 3, 160, 160)  # (B,C,H,W)
-    trt = TRTEngine(trt_file, input_shape=input_shape)
-    image = np.ones(shape=input_shape)
-    input_tensor = np.asarray(image, dtype=np.float32)
-    outputs, = trt(input_tensor)
-    print("input_tensor:{}".format(input_tensor.shape))
-    print("output      :{}={}".format(outputs.shape, outputs))
+    test_performance()
+    # test_example()
```

### Comparing `basetrainer-0.8.3/basetrainer/metric/accuracy_recorder.py` & `basetrainer-0.8.4/basetrainer/metric/accuracy_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/acc.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/acc.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/classification_report.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/classification_report.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/eval_utils.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/eval_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/evaluate.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/iou.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/iou.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/metrics.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/metrics.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/pandas_tools.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/pr.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/pr.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/psnr.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/psnr.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/roc.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/roc.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/eval_tools/verification.py` & `basetrainer-0.8.4/basetrainer/metric/eval_tools/verification.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/bboxes_match.py` & `basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/bboxes_match.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/iou.py` & `basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/iou.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval.py` & `basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/map_eval.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval_torch.py` & `basetrainer-0.8.4/basetrainer/metric/map_tools/evaluator/map_eval_torch.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/metric/map_tools/map_metric.py` & `basetrainer-0.8.4/basetrainer/metric/map_tools/map_metric.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/models/build_models.py` & `basetrainer-0.8.4/basetrainer/models/build_models.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/optimizer/build_optimizer.py` & `basetrainer-0.8.4/basetrainer/optimizer/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/pruning/nni_pruning.py` & `basetrainer-0.8.4/basetrainer/pruning/nni_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/pruning/slim_pruning.py` & `basetrainer-0.8.4/basetrainer/pruning/slim_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/pruning/torch_pruning.py` & `basetrainer-0.8.4/basetrainer/pruning/torch_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/CosineAnnealingLR.py` & `basetrainer-0.8.4/basetrainer/scheduler/CosineAnnealingLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/ExponentialLR.py` & `basetrainer-0.8.4/basetrainer/scheduler/ExponentialLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/LambdaLR.py` & `basetrainer-0.8.4/basetrainer/scheduler/LambdaLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/MultiStepLR.py` & `basetrainer-0.8.4/basetrainer/scheduler/MultiStepLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/MultiStepValue.py` & `basetrainer-0.8.4/basetrainer/scheduler/MultiStepValue.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/WarmUpLR.py` & `basetrainer-0.8.4/basetrainer/scheduler/WarmUpLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/scheduler/build_scheduler.py` & `basetrainer-0.8.4/basetrainer/scheduler/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/converter/onnx2trt.py` & `basetrainer-0.8.4/basetrainer/utils/converter/onnx2trt.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/converter/pytorch2onnx.py` & `basetrainer-0.8.4/basetrainer/utils/converter/pytorch2onnx.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/heatmap_utils.py` & `basetrainer-0.8.4/basetrainer/utils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/log.py` & `basetrainer-0.8.4/basetrainer/utils/log.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/plot_utils.py` & `basetrainer-0.8.4/basetrainer/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/setup_config.py` & `basetrainer-0.8.4/basetrainer/utils/setup_config.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/summary.py` & `basetrainer-0.8.4/basetrainer/utils/summary.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/torch_data.py` & `basetrainer-0.8.4/basetrainer/utils/torch_data.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/torch_tools.py` & `basetrainer-0.8.4/basetrainer/utils/torch_tools.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer/utils/torchcam_utils.py` & `basetrainer-0.8.4/basetrainer/utils/torchcam_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/basetrainer.egg-info/SOURCES.txt` & `basetrainer-0.8.4/basetrainer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 basetrainer/engine/__init__.py
 basetrainer/engine/base.py
 basetrainer/engine/comm.py
 basetrainer/engine/engine.py
 basetrainer/engine/launch.py
 basetrainer/engine/onnx_engine.py
 basetrainer/engine/trainer.py
+basetrainer/engine/trt_calibrator.py
 basetrainer/engine/trt_engine.py
 basetrainer/metric/__init__.py
 basetrainer/metric/accuracy_recorder.py
 basetrainer/metric/eval_tools/__init__.py
 basetrainer/metric/eval_tools/acc.py
 basetrainer/metric/eval_tools/classification_report.py
 basetrainer/metric/eval_tools/eval_utils.py
```

### Comparing `basetrainer-0.8.3/setup.py` & `basetrainer-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.3/test/test_scheduler.py` & `basetrainer-0.8.4/test/test_scheduler.py`

 * *Files identical despite different names*

