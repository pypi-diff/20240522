# Comparing `tmp/torchtnt-0.2.3.tar.gz` & `tmp/torchtnt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-0.2.3.tar", last modified: Sat Feb 24 02:03:52 2024, max compression
+gzip compressed data, was "torchtnt-0.2.4.tar", last modified: Wed May 22 16:19:11 2024, max compression
```

## Comparing `torchtnt-0.2.3.tar` & `torchtnt-0.2.4.tar`

### file list

```diff
@@ -1,94 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.166326 torchtnt-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-24 02:01:27.000000 torchtnt-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-24 02:03:52.166326 torchtnt-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-24 02:01:27.000000 torchtnt-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-24 02:01:27.000000 torchtnt-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 02:03:52.166326 torchtnt-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-02-24 02:01:27.000000 torchtnt-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.154326 torchtnt-0.2.3/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.154326 torchtnt-0.2.3/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/_loop_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/_unit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35118 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.158326 torchtnt-0.2.3/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/_checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24423 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/base_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/checkpointer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/dcp_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/empty_cuda_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/iteration_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/memory_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.162326 torchtnt-0.2.3/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.166326 torchtnt-0.2.3/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/data/synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    22038 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.166326 torchtnt-0.2.3/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/memory_snapshot_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/prepare_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-24 02:01:27.000000 torchtnt-0.2.3/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:03:52.154326 torchtnt-0.2.3/torchtnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-24 02:03:52.000000 torchtnt-0.2.3/torchtnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-02-24 02:03:52.000000 torchtnt-0.2.3/torchtnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 02:03:52.000000 torchtnt-0.2.3/torchtnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-24 02:03:52.000000 torchtnt-0.2.3/torchtnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-24 02:03:52.000000 torchtnt-0.2.3/torchtnt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 02:03:52.000000 torchtnt-0.2.3/torchtnt.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.856754 torchtnt-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 16:17:08.000000 torchtnt-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-22 16:19:11.856754 torchtnt-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-22 16:17:08.000000 torchtnt-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 16:17:08.000000 torchtnt-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:19:11.860754 torchtnt-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-22 16:17:08.000000 torchtnt-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.844754 torchtnt-0.2.4/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.848754 torchtnt-0.2.4/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/_loop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/_unit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.852754 torchtnt-0.2.4/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/_checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/base_checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/checkpointer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/dcp_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/empty_cuda_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/iteration_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/memory_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/progress_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/slow_rank_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/throughput_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/time_limit_interrupter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/time_wait_for_batch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/torch_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.856754 torchtnt-0.2.4/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.856754 torchtnt-0.2.4/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/data/synthetic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23329 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/fsdp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.856754 torchtnt-0.2.4/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/memory_snapshot_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/prepare_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-22 16:17:08.000000 torchtnt-0.2.4/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:19:11.856754 torchtnt-0.2.4/torchtnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-22 16:19:11.000000 torchtnt-0.2.4/torchtnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-22 16:19:11.000000 torchtnt-0.2.4/torchtnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:19:11.000000 torchtnt-0.2.4/torchtnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 16:19:11.000000 torchtnt-0.2.4/torchtnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 16:19:11.000000 torchtnt-0.2.4/torchtnt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:19:11.000000 torchtnt-0.2.4/torchtnt.egg-info/zip-safe
```

### Comparing `torchtnt-0.2.3/LICENSE` & `torchtnt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-0.2.3/PKG-INFO` & `torchtnt-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt
-Version: 0.2.3
+Version: 0.2.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,15 +30,15 @@
 Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: parameterized; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: torchsnapshot-nightly; extra == "dev"
 Requires-Dist: pyre-check; extra == "dev"
-Requires-Dist: torchvision==0.16.2; extra == "dev"
+Requires-Dist: torchvision==0.15.2; extra == "dev"
 
 TNT
 ==========
 
 **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and utilities.
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt Version: 0.2.3 Summary: A lightweight
+Metadata-Version: 2.1 Name: torchtnt Version: 0.2.4 Summary: A lightweight
 library for PyTorch training tools and utilities Home-page: https://github.com/
 pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com License: BSD-
 3 Keywords: pytorch,torch,training,tools,utilities Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
@@ -10,15 +10,15 @@
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch
 Requires-Dist: numpy Requires-Dist: fsspec Requires-Dist: tensorboard Requires-
 Dist: packaging Requires-Dist: psutil Requires-Dist: pyre_extensions Requires-
 Dist: typing_extensions Requires-Dist: setuptools Requires-Dist: tqdm Requires-
 Dist: tabulate Provides-Extra: dev Requires-Dist: parameterized; extra == "dev"
 Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: torchsnapshot-nightly; extra == "dev" Requires-Dist: pyre-check;
-extra == "dev" Requires-Dist: torchvision==0.16.2; extra == "dev" TNT
+extra == "dev" Requires-Dist: torchvision==0.15.2; extra == "dev" TNT
 ========== **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and
 utilities.
  _[_b_u_i_l_d_ _s_t_a_t_u_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_p_y_p_i_ _n_i_g_h_t_l_y_ _v_e_r_s_i_o_n_]_[_c_o_d_e_c_o_v_]_[_b_s_d
                         _l_i_c_e_n_s_e_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_ _s_t_a_t_u_s_]
 ## Installation TNT can be installed with pip: ```buildoutcfg pip install
 torchtnt ``` Or, alternatively, via conda: ```buildoutcfg conda install -
 c conda-forge torchtnt ``` If you run into issues, make sure that Pytorch is
```

### Comparing `torchtnt-0.2.3/README.md` & `torchtnt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-0.2.3/setup.py` & `torchtnt-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.2.3/torchtnt/framework/__init__.py` & `torchtnt-0.2.4/torchtnt/framework/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from .auto_unit import AutoPredictUnit, AutoUnit
 from .callback import Callback
 from .evaluate import evaluate
 from .fit import fit
 from .predict import predict
 from .state import ActivePhase, EntryPoint, PhaseState, State
 from .train import train
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/_callback_handler.py` & `torchtnt-0.2.4/torchtnt/framework/_callback_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from functools import partial
 from typing import Dict, List, Type, Union
 from unittest.mock import Mock
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/_loop_utils.py` & `torchtnt-0.2.4/torchtnt/framework/_loop_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-import collections
-import inspect
+# pyre-strict
+
 import logging
-from typing import Callable, Dict, Iterable, Optional, TypeVar
+from typing import Dict, Iterable, Optional, Protocol, runtime_checkable, TypeVar
 
 import torch
 import torch.nn as nn
-import typing_extensions
-from torchtnt.framework.state import State
+from torch.nn.parallel.distributed import DistributedDataParallel
+
+_EXPORT_UTILS_AVAIL = True
+try:
+    from torch.ao.quantization.pt2e.export_utils import model_is_exported
+except Exception:
+    _EXPORT_UTILS_AVAIL = False
+
 from torchtnt.utils.progress import Progress
 
 _logger: logging.Logger = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 # Helper functions common across the loops
@@ -33,37 +39,57 @@
 ) -> bool:
     return (max_steps is not None and progress.num_steps_completed >= max_steps) or (
         max_steps_per_epoch is not None
         and progress.num_steps_completed_in_epoch >= max_steps_per_epoch
     )
 
 
+@runtime_checkable
+class _DistributedSampler(Protocol):
+    def set_epoch(self, epoch: int) -> None: ...
+
+
 def _maybe_set_distributed_sampler_epoch(
     dataloader: Iterable[object],
     current_epoch: int,
 ) -> None:
     """Set epoch of distributed sampler in dataloader, if applicable.
     See: https://pytorch.org/docs/stable/data.html#torch.utils.data.distributed.DistributedSampler
     """
     # Set current training epoch for any DistributedSampler in dataloader
     if isinstance(dataloader, torch.utils.data.DataLoader) and isinstance(
         dataloader.sampler,
-        torch.utils.data.distributed.DistributedSampler,
+        _DistributedSampler,
     ):
         dataloader.sampler.set_epoch(current_epoch)
 
 
 def _set_module_training_mode(
     modules: Dict[str, nn.Module], mode: bool
 ) -> Dict[str, bool]:
     """Returns states to allow for a reset at the end of the loop."""
     prior_module_train_states = {}
     for name, module in modules.items():
         prior_module_train_states[name] = module.training
-        module.train(mode)
+        is_ddp = isinstance(module, DistributedDataParallel)
+
+        if _EXPORT_UTILS_AVAIL and model_is_exported(
+            module.module if is_ddp else module
+        ):
+            if mode:
+                module = torch.ao.quantization.move_exported_model_to_train(
+                    module.module if is_ddp else module
+                )
+            else:
+                module = torch.ao.quantization.move_exported_model_to_eval(
+                    module.module if is_ddp else module
+                )
+        else:
+            module.train(mode)
+
     return prior_module_train_states
 
 
 def _reset_module_training_mode(
     modules: Dict[str, nn.Module], prior_modes: Dict[str, bool]
 ) -> None:
     # Reset training mode for modules at the end of the epoch
@@ -72,25 +98,7 @@
     for name, module in modules.items():
         if name in prior_modes:
             module.train(prior_modes[name])
 
 
 def _log_api_usage(entry_point: str) -> None:
     torch._C._log_api_usage_once(f"torchtnt.framework.{entry_point}")
-
-
-def _step_requires_iterator(step_func: Callable[[State, T], object]) -> bool:
-    """
-    Helper function to evaluate whether the loops should pass the data iterator to the `_step`
-    functions, or whether the loop should call `next(data_iter)` and pass a single batch to process.
-
-    This is closely tied to the Unit's corresponding step function signature.
-    """
-    argspec = inspect.getfullargspec(step_func)
-    annotations = argspec.annotations
-    if "data" not in annotations:
-        _logger.warning(
-            f"Expected step function to have an annotated argument named ``data``. Found {annotations}."
-        )
-        return False
-    annotated_type = annotations["data"]
-    return typing_extensions.get_origin(annotated_type) is collections.abc.Iterator
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/_test_utils.py` & `torchtnt-0.2.4/torchtnt/framework/_test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Iterable, Iterator, Optional, Tuple
 
 import torch
 from torch import nn, Tensor
 from torch.utils.data import DataLoader, Dataset, IterableDataset, TensorDataset
 from torchtnt.framework.auto_unit import AutoUnit
 from torchtnt.framework.state import EntryPoint, PhaseState, State
@@ -25,14 +27,27 @@
             dataloader=dataloader or [1, 2, 3, 4],
             max_epochs=1,
             max_steps=1,
             max_steps_per_epoch=1,
         ),
         timer=None,
     )
+
+
+def get_dummy_eval_state(dataloader: Optional[Iterable[object]] = None) -> State:
+    return State(
+        entry_point=EntryPoint.EVALUATE,
+        eval_state=PhaseState(
+            dataloader=dataloader or [1, 2, 3, 4],
+            max_epochs=1,
+            max_steps=1,
+            max_steps_per_epoch=1,
+        ),
+        timer=None,
+    )
 
 
 def get_dummy_fit_state() -> State:
     return State(
         entry_point=EntryPoint.FIT,
         train_state=PhaseState(
             dataloader=[1, 2, 3, 4],
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/_unit_utils.py` & `torchtnt-0.2.4/torchtnt/framework/_unit_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import collections
 import inspect
 import logging
 from typing import Callable, Dict, List, Tuple, TypeVar
 
 import torch
 import typing_extensions
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/auto_unit.py` & `torchtnt-0.2.4/torchtnt/framework/auto_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 
 import contextlib
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Generic, Iterator, List, Optional, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    ContextManager,
+    Generic,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import torch
 from pyre_extensions import none_throws
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim.swa_utils import SWALR
-from torchtnt.framework._loop_utils import _step_requires_iterator
+from torchtnt.framework._unit_utils import _step_requires_iterator
 from torchtnt.framework.state import ActivePhase, EntryPoint, State
 from torchtnt.framework.unit import EvalUnit, PredictUnit, TPredictData, TrainUnit
 from torchtnt.framework.utils import get_timing_context
 from torchtnt.utils.device import copy_data_to_device, record_data_in_stream
 from torchtnt.utils.env import init_from_env
 from torchtnt.utils.lr_scheduler import TLRScheduler
 from torchtnt.utils.precision import (
     convert_precision_str_to_dtype,
     get_grad_scaler_from_precision,
+    GradScaler,
 )
 from torchtnt.utils.prepare_module import (
     _is_fsdp_module,
     ActivationCheckpointParams,
     FSDPStrategy,
     prepare_fsdp,
     prepare_module,
     Strategy,
     TorchCompileParams,
 )
 from torchtnt.utils.swa import AveragedModel
-from torchtnt.utils.version import is_torch_version_ge_1_13_1
 from typing_extensions import Literal
 
 
 TData = TypeVar("TData")
 
 
 @dataclass
@@ -149,16 +161,14 @@
         module: torch.nn.Module,
         device: Optional[torch.device] = None,
         precision: Optional[Union[str, torch.dtype]] = None,
         detect_anomaly: Optional[bool] = None,
         torch_compile_params: Optional[TorchCompileParams] = None,
     ) -> None:
         super().__init__()
-        if torch_compile_params:
-            _validate_torch_compile_available()
 
         self.device: torch.device = device or init_from_env()
         self.precision: Optional[torch.dtype] = (
             convert_precision_str_to_dtype(precision)
             if isinstance(precision, str)
             else precision
         )
@@ -392,34 +402,40 @@
     To benefit from the AutoUnit, the user must subclass it and implement the ``compute_loss`` and ``configure_optimizers_and_lr_scheduler`` methods.
     Additionally, the AutoUnit offers these optional hooks:
 
     - ``on_train_step_end``
     - ``on_eval_step_end``
     - ``on_predict_step_end``
 
+    The user can also override the LR step method, ``step_lr_scheduler``, in case they want to have custom logic.
+
     Then use with the :py:func:`~torchtnt.framework.train`, :py:func:`~torchtnt.framework.evaluate`, :py:func:`~torchtnt.framework.fit`, or
     :py:func:`~torchtnt.framework.predict` entry point as normal.
 
     For more advanced customization, directly use the :class:`~torchtnt.framework.unit.TrainUnit`, :class:`~torchtnt.framework.unit.EvalUnit`,
     and :class:`~torchtnt.framework.unit.PredictUnit` interfaces.
 
     Args:
         module: module to be used during training/evaluation.
         device: the device to be used.
         strategy: the data parallelization strategy to be used. if a string, must be one of ``ddp`` or ``fsdp``.
         step_lr_interval: whether to step lr_scheduler every step or every epoch. Defaults to every epoch.
-        precision: the precision to use in training/evaluation, as either a string or a torch.dtype.
+        precision: the precision to use in training/evaluation (using automatic mixed precision), as either a string or a torch.dtype. Acceptable strings are ``'fp32'``, ``'fp16'``, and ``'bf16'``.
         gradient_accumulation_steps: how many batches to accumulate gradients over.
         detect_anomaly: whether to enable anomaly detection for the autograd engine https://pytorch.org/docs/stable/autograd.html#anomaly-detection
         clip_grad_norm: max norm of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_norm_.html
         clip_grad_value: max value of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_value_.html
         swa_params: params for stochastic weight averaging https://pytorch.org/docs/stable/optim.html#stochastic-weight-averaging
         torch_compile_params: params for Torch compile https://pytorch.org/docs/stable/generated/torch.compile.html
         activation_checkpoint_params: params for enabling activation checkpointing
         training: if True, the optimizer and optionally LR scheduler will be created after the class is initialized.
+        enable_compiled_autograd: if True, `compiled_autograd` will be used to compile the backward, this is an experimental flag.
+
+    Note:
+        Certain strategies, like :class:`~torchtnt.utils.prepare_module.FSDPStrategy` also support mixed precision as an argument, so can be configured through that class as well.
 
     Note:
         If :class:`~torchtnt.utils.prepare_module.FSDPStrategy` and SWAParams are passed in, the swa model will be sharded with the same FSDP parameters.
 
     Note:
         Torch compile support is only available in PyTorch 2.0 or higher.
 
@@ -437,14 +453,15 @@
         detect_anomaly: Optional[bool] = None,
         clip_grad_norm: Optional[float] = None,
         clip_grad_value: Optional[float] = None,
         swa_params: Optional[SWAParams] = None,
         torch_compile_params: Optional[TorchCompileParams] = None,
         activation_checkpoint_params: Optional[ActivationCheckpointParams] = None,
         training: bool = True,
+        enable_compiled_autograd: bool = False,
     ) -> None:
         super().__init__(
             module=module,
             device=device,
             precision=precision,
             detect_anomaly=detect_anomaly,
             torch_compile_params=torch_compile_params,
@@ -479,32 +496,34 @@
 
         self.module: torch.nn.Module = prepare_module(
             module,
             self.device,
             strategy=strategy,
             torch_compile_params=torch_compile_params,
             activation_checkpoint_params=activation_checkpoint_params,
+            enable_compiled_autograd=enable_compiled_autograd,
         )
 
-        self.grad_scaler: Optional[torch.amp.GradScaler] = None
+        self.grad_scaler: Optional[GradScaler] = None
         if self.precision:
             self.grad_scaler = get_grad_scaler_from_precision(
                 self.precision,
-                self.module,
+                is_fsdp_module=_is_fsdp_module(self.module),
             )
 
         self.step_lr_interval = step_lr_interval
 
         self.gradient_accumulation_steps = gradient_accumulation_steps
 
         self.clip_grad_norm = clip_grad_norm
         self.clip_grad_value = clip_grad_value
 
         # create autocast context based on precision and device type
 
+        self.enable_compiled_autograd = enable_compiled_autograd
         self.training = training
 
         self.optimizer: Optional[torch.optim.Optimizer] = None
         self.lr_scheduler: Optional[TLRScheduler] = None
         self.swa_scheduler: Optional[SWALR] = None
 
     @abstractmethod
@@ -577,21 +596,35 @@
                 ):
                     # Run the forward pass and compute the loss
                     loss, outputs = self.compute_loss(state, data)
 
             # normalize loss to account for gradient accumulation
             loss = loss / self.gradient_accumulation_steps
 
-            if grad_scaler:
-                scaled_loss = grad_scaler.scale(loss)
-                with get_timing_context(state, f"{self.__class__.__name__}.backward"):
-                    scaled_loss.backward()
-            else:
-                with get_timing_context(state, f"{self.__class__.__name__}.backward"):
-                    loss.backward()
+            try:
+                from torch._dynamo.utils import maybe_enable_compiled_autograd
+            except ImportError:
+
+                def maybe_enable_compiled_autograd(
+                    val: bool,
+                ) -> ContextManager:
+                    return contextlib.nullcontext()
+
+            with maybe_enable_compiled_autograd(self.enable_compiled_autograd):
+                if grad_scaler:
+                    scaled_loss = grad_scaler.scale(loss)
+                    with get_timing_context(
+                        state, f"{self.__class__.__name__}.backward"
+                    ):
+                        scaled_loss.backward()
+                else:
+                    with get_timing_context(
+                        state, f"{self.__class__.__name__}.backward"
+                    ):
+                        loss.backward()
 
         total_grad_norm = None
         if should_update_weights:
             total_grad_norm = self._update_weights(state)
 
         step = self.train_progress.num_steps_completed
         results = TrainStepResults(loss, total_grad_norm, outputs)
@@ -694,14 +727,20 @@
             state: a State object which is passed from the ``predict_step``
             data: a batch of data which is passed from the ``predict_step``
             step: how many ``predict_step``s have been completed
             outputs: the outputs of the model forward pass
         """
         pass
 
+    def step_lr_scheduler(self) -> None:
+        """
+        LR step method extracted to a method in case the user wants to override
+        """
+        none_throws(self.lr_scheduler).step()
+
     def _update_weights(self, state: State) -> Optional[torch.Tensor]:
         """
         Updates weights of the module, handles clip gradient norm, etc.
 
         Returns total norm of the parameter gradients, if gradient norm clipping is enabled.
         """
         module = self.module
@@ -828,21 +867,12 @@
         ):
             with get_timing_context(
                 state, f"{self.__class__.__name__}.swa_lr_scheduler_step"
             ):
                 none_throws(self.swa_scheduler).step()
         else:
             # optionally step lr scheduler if SWA not in use
-            lr_scheduler = self.lr_scheduler
-            if lr_scheduler:
+            if self.lr_scheduler:
                 with get_timing_context(
                     state, f"{self.__class__.__name__}.lr_scheduler_step"
                 ):
-                    lr_scheduler.step()
-
-
-def _validate_torch_compile_available() -> None:
-    if not is_torch_version_ge_1_13_1():
-        raise RuntimeError(
-            "Torch compile support is available only in PyTorch 2.0 or higher. "
-            "Please install PyTorch 2.0 or higher to continue: https://pytorch.org/get-started/locally/"
-        )
+                    self.step_lr_scheduler()
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callback.py` & `torchtnt-0.2.4/torchtnt/framework/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Union
 
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
 
 
 class Callback:
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/__init__.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,55 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from .base_csv_writer import BaseCSVWriter
+from .dcp_saver import DistributedCheckpointSaver
+from .early_stopping import EarlyStopping
 from .empty_cuda_cache import EmptyCudaCache
 from .garbage_collector import GarbageCollector
 from .iteration_time_logger import IterationTimeLogger
 from .lambda_callback import Lambda
 from .learning_rate_monitor import LearningRateMonitor
 from .memory_snapshot import MemorySnapshot
 from .module_summary import ModuleSummary
+from .progress_reporter import ProgressReporter
 from .pytorch_profiler import PyTorchProfiler
+from .slow_rank_detector import SlowRankDetector
 from .system_resources_monitor import SystemResourcesMonitor
 from .tensorboard_parameter_monitor import TensorBoardParameterMonitor
+from .throughput_logger import ThroughputLogger
+from .time_limit_interrupter import TimeLimitInterrupter
+from .time_wait_for_batch_logger import TimeWaitForBatchLogger
+from .torch_compile import TorchCompile
 from .torchsnapshot_saver import TorchSnapshotSaver
 from .tqdm_progress_bar import TQDMProgressBar
 from .train_progress_monitor import TrainProgressMonitor
 
 __all__ = [
     "BaseCSVWriter",
+    "EarlyStopping",
     "EmptyCudaCache",
     "GarbageCollector",
     "IterationTimeLogger",
     "Lambda",
     "LearningRateMonitor",
     "MemorySnapshot",
     "ModuleSummary",
+    "ProgressReporter",
     "PyTorchProfiler",
+    "SlowRankDetector",
     "SystemResourcesMonitor",
     "TensorBoardParameterMonitor",
+    "ThroughputLogger",
+    "TimeLimitInterrupter",
+    "TimeWaitForBatchLogger",
+    "TorchCompile",
     "TorchSnapshotSaver",
     "TQDMProgressBar",
     "TrainProgressMonitor",
+    "DistributedCheckpointSaver",
 ]
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/base_checkpointer.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/base_checkpointer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import abc
-import bisect
 import logging
-import os
 from datetime import timedelta
-from typing import Any, cast, Iterable, List, Literal, Optional, Union
+from typing import Any, cast, Iterable, Literal, Optional, Union
 
 import torch.distributed as dist
-
+from pyre_extensions import none_throws
 from torchtnt.framework.callback import Callback
-from torchtnt.framework.callbacks._checkpoint_utils import (
-    _delete_checkpoint,
-    _metadata_exists,
-    _sort_by_metric_value,
-    _sort_by_recency,
+from torchtnt.framework.callbacks._checkpoint_utils import _get_step_phase_mapping
+from torchtnt.framework.callbacks.checkpointer_types import RestoreOptions
+from torchtnt.framework.state import State
+from torchtnt.framework.unit import AppStateMixin, TEvalUnit, TTrainData, TTrainUnit
+from torchtnt.utils.checkpoint import (
+    BestCheckpointConfig,
+    CheckpointManager,
+    CheckpointPath,
     get_best_checkpoint_path,
-    get_checkpoint_dirpaths,
     get_latest_checkpoint_path,
-    rank_zero_read_and_broadcast,
-)
-from torchtnt.framework.callbacks.checkpointer_types import (
-    BestCheckpointConfig,
-    RestoreOptions,
+    MetricData,
 )
-from torchtnt.framework.state import EntryPoint, State
-from torchtnt.framework.unit import AppStateMixin, TEvalUnit, TTrainData, TTrainUnit
-from torchtnt.framework.utils import get_timing_context
 from torchtnt.utils.distributed import PGWrapper
-from torchtnt.utils.fsspec import get_filesystem
 from torchtnt.utils.rank_zero_log import rank_zero_info, rank_zero_warn
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class BaseCheckpointer(Callback, metaclass=abc.ABCMeta):
     """
@@ -105,42 +99,25 @@
             )
 
         self._save_every_n_train_steps = save_every_n_train_steps
         self._save_every_n_epochs = save_every_n_epochs
         self._save_every_n_eval_epochs = save_every_n_eval_epochs
         self._keep_last_n_checkpoints = keep_last_n_checkpoints
 
-        self._ckpt_dirpaths: List[str] = []
-        if self._keep_last_n_checkpoints:
-            metric_name = (
-                None
-                if not best_checkpoint_config
-                else best_checkpoint_config.monitored_metric
-            )
-            ckpt_dirpaths = get_checkpoint_dirpaths(
-                dirpath=dirpath,
-                metadata_fname=self.metadata_fname,
-                metric_name=metric_name,
-                process_group=process_group,
-            )
-
-            # sort by metric value if doing best checkpoint, else by recency
-            if best_checkpoint_config:
-                self._ckpt_dirpaths = _sort_by_metric_value(
-                    ckpt_dirpaths, mode=best_checkpoint_config.mode
-                )
-            else:
-                self._ckpt_dirpaths = _sort_by_recency(ckpt_dirpaths)
-
         self._process_group: Optional[dist.ProcessGroup] = None
         self._setup_gloo_pg(process_group)
         self._pg_wrapper = PGWrapper(process_group)
 
-        # sync dirpaths from rank 0
-        self._sync_dirpath_to_all_ranks(dirpath)
+        self._checkpoint_manager = CheckpointManager(
+            dirpath,
+            best_checkpoint_config,
+            keep_last_n_checkpoints,
+            metadata_fname=self.metadata_fname,
+            process_group=self._process_group,
+        )
 
     def _setup_gloo_pg(self, process_group: Optional[dist.ProcessGroup]) -> None:
         """
         Setups gloo process group to be used for any collectives called during
         checkpointing. If global process group is already gloo, no action is required.
         Gloo is used over nccl for better compatibility.
         """
@@ -157,32 +134,18 @@
             rank_zero_info("Creating new gloo process group for checkpointing.")
             self._process_group = dist.new_group(
                 timeout=timedelta(seconds=3600), backend=dist.Backend.GLOO
             )
         else:
             self._process_group = process_group
 
-    def _sync_dirpath_to_all_ranks(self, dirpath: str) -> None:
-        if not (dist.is_available() and dist.is_initialized()):
-            self._dirpath: str = dirpath
-            return
-
-        dirpath_container = [dirpath] if self._pg_wrapper.get_rank() == 0 else [""]
-        # broadcast directory from global rank 0
-        dist.broadcast_object_list(dirpath_container, src=0, group=self._process_group)
-        updated_dirpath = dirpath_container[0]
-        if updated_dirpath != dirpath:
-            logger.warning(f"Updating dirpath to match rank 0: {updated_dirpath}")
-
-        self._dirpath: str = updated_dirpath
-
     @property
     def dirpath(self) -> str:
         """Returns parent directory to save to."""
-        return self._dirpath
+        return self._checkpoint_manager.dirpath
 
     def _generate_checkpoint_and_upkeep(
         self, state: State, unit: Union[TTrainUnit, TEvalUnit], hook: str
     ) -> bool:
         """
         Implementation for saving checkpoint while taking care of checkpoint
         name generation and cleanup of oldest checkpoints.
@@ -191,112 +154,101 @@
             state: Current state of the trainer.
             unit: Current training unit.
             hook: Hook at which checkpoint is being saved.
 
         Returns:
             True if checkpoint was successfully saved. False otherwise.
         """
-        unit = cast(TTrainUnit, unit)
-
         # 1) generate checkpoint name
-        num_steps_completed = unit.train_progress.num_steps_completed
-        if state.entry_point == EntryPoint.FIT:
-            num_steps_completed += cast(
-                TEvalUnit, unit
-            ).eval_progress.num_steps_completed
-        epoch = unit.train_progress.num_epochs_completed
-        checkpoint_path = _get_save_path(self._dirpath, epoch, num_steps_completed)
+        epoch = cast(TTrainUnit, unit).train_progress.num_epochs_completed
+        step_mapping = _get_step_phase_mapping(state, unit)
 
-        # 1.5) Ensure the need to checkpoint again at the end of training
+        metric_data: Optional[MetricData] = None
+        if metric_value := self._get_tracked_metric_value(unit):
+            metric_data = MetricData(
+                name=none_throws(self._best_checkpoint_config).monitored_metric,
+                value=metric_value,
+            )
+
+        checkpoint_path = self._checkpoint_manager.generate_checkpoint_path(
+            epoch, step_mapping, metric_data
+        )
+
+        # 2) Determine if we should save checkpoint
+        if not self._checkpoint_manager.should_save_checkpoint(checkpoint_path):
+            return False
+
+        # 2.1) Make sure that last checkpoint does not already exist
         if hook == "on_train_end" and self._does_checkpoint_exist(
             checkpoint_path, self._process_group
         ):
             rank_zero_warn("Final checkpoint already exists, skipping.", logger=logger)
             return False
 
-        # 2) handle best checkpoint config on all hooks except `on_train_end`
-        # TODO: isolate this logic into its own function
-        metric_value_f: Optional[float] = None
-        best_checkpoint_config = self._best_checkpoint_config
-        if best_checkpoint_config and hook != "on_train_end":
-            if not hasattr(unit, best_checkpoint_config.monitored_metric):
-                raise RuntimeError(
-                    f"Unit does not have attribute {best_checkpoint_config.monitored_metric}, unable to retrieve metric to checkpoint."
-                )
+        # 3) try to save checkpoint
+        if not self._checkpoint_impl(
+            state, unit, checkpoint_path=checkpoint_path.path, hook=hook
+        ):
+            return False
 
-            metric_value = getattr(unit, best_checkpoint_config.monitored_metric)
-            if metric_value is not None:
-                try:
-                    metric_value_f = float(metric_value)
-                except Exception as e:
-                    raise RuntimeError(
-                        f"Unable to convert monitored metric {best_checkpoint_config.monitored_metric} to a float. Please ensure the value can be converted to float and is not a multi-element tensor value."
-                    ) from e
-
-                # update checkpoint path to include the metric value info
-                checkpoint_path += (
-                    f"_{best_checkpoint_config.monitored_metric}={metric_value_f}"
-                )
+        # 4) track checkpoint and clean up surplus if needed
+        self._checkpoint_manager.append_checkpoint(checkpoint_path)
 
-        should_checkpoint = self._should_save_checkpoint(metric_value_f)
-        if not should_checkpoint:
-            return False
+        return True
 
-        # 3) try to save checkpoint
-        success = self._checkpoint_impl(
-            state,
-            unit,
-            checkpoint_path=checkpoint_path,
-            hook=hook,
+    def _does_checkpoint_exist(
+        self,
+        checkpoint_path: CheckpointPath,
+        process_group: Optional[dist.ProcessGroup] = None,
+    ) -> bool:
+        # Only keep this function as a hook for downstream checkpointer
+        return self._checkpoint_manager.does_checkpoint_exist(
+            checkpoint_path, process_group
         )
 
-        if success:
-            # remove the checkpoint if applicable
-            # and update the tracked list of checkpoint paths
-
-            if self._should_remove_checkpoint():
-                self._remove_checkpoint(state)
-
-            if best_checkpoint_config:
-                if metric_value_f:
-                    # insert the checkpoint path at the right index to preserve ordering
-                    keys = [
-                        float(os.path.basename(x).split("=")[-1])
-                        for x in self._ckpt_dirpaths
-                    ]
-                    if best_checkpoint_config.mode == "min":
-                        keys.reverse()
-                    # Use bisect.bisect() to find the insertion point
-                    idx = bisect.bisect(keys, metric_value_f)
-                    if best_checkpoint_config.mode == "min":
-                        idx = len(self._ckpt_dirpaths) - idx
-                    self._ckpt_dirpaths.insert(idx, checkpoint_path)
-            else:
-                self._ckpt_dirpaths.append(checkpoint_path)
+    def _get_tracked_metric_value(
+        self, unit: Union[TTrainUnit, TEvalUnit]
+    ) -> Optional[float]:
+        """
+        If the checkpointer has a tracked metric, look the value in the unit using reflection, and cast to float.
+
+        Args:
+            unit: The training unit to look for the tracked metric in.
+
+        Returns:
+            The value of the tracked metric, or None if there is no best_checkpoint config defined.
+
+        Raises:
+            RuntimeError: If the unit does not have the attribute specified in the best_checkpoint config,
+                or if the value cannot be cast to a float.
+        """
+        if not self._best_checkpoint_config:
+            return None
+
+        monitored_metric_name = self._best_checkpoint_config.monitored_metric
+        if not hasattr(unit, monitored_metric_name):
+            raise RuntimeError(
+                f"Unit does not have attribute {monitored_metric_name}, unable to retrieve metric to checkpoint."
+            )
+
+        metric_value_f = None
+        if (metric_value := getattr(unit, monitored_metric_name)) is not None:
+            try:
+                metric_value_f = float(metric_value)
+            except ValueError as e:
+                raise RuntimeError(
+                    f"Unable to convert monitored metric {monitored_metric_name} to a float. Please ensure the value "
+                    "can be converted to float and is not a multi-element tensor value."
+                ) from e
 
-        return success
+        return metric_value_f
 
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
         # clean up the difference if surplus of checkpoints exist
-        keep_last_n_checkpoints = self._keep_last_n_checkpoints
-        if (
-            keep_last_n_checkpoints
-            and len(self._ckpt_dirpaths) > keep_last_n_checkpoints
-        ):
-            logger.warning(
-                " ".join(
-                    [
-                        f"{len(self._ckpt_dirpaths)} checkpoints found in {self._dirpath}.",
-                        f"Deleting {len(self._ckpt_dirpaths) - keep_last_n_checkpoints} oldest",
-                        "checkpoints to enforce ``keep_last_n_checkpoints`` argument.",
-                    ]
-                )
-            )
-            for _ in range(len(self._ckpt_dirpaths) - keep_last_n_checkpoints):
-                self._remove_checkpoint(state)
+        self._checkpoint_manager.prune_surplus_checkpoints()
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
         num_steps_completed = unit.train_progress.num_steps_completed
         save_every_n_train_steps = self._save_every_n_train_steps
         if (
             save_every_n_train_steps is None
             or num_steps_completed % save_every_n_train_steps != 0
@@ -343,68 +295,14 @@
             hook: name of callback hook that triggered this function call
 
         Returns:
             Whether a new checkpoint was created.
         """
         ...
 
-    def _should_save_checkpoint(self, metric_value: Optional[float] = None) -> bool:
-        """
-        Whether a new checkpoint should be saved.
-        """
-
-        keep_last_n_checkpoints = self._keep_last_n_checkpoints
-        if not keep_last_n_checkpoints:
-            # always save candidate checkpoint if no limit of checkpoints is specified
-            return True
-
-        if len(self._ckpt_dirpaths) < keep_last_n_checkpoints:
-            # limit of checkpoints has not been reached
-            return True
-
-        best_checkpoint_config = self._best_checkpoint_config
-        if not best_checkpoint_config:
-            # we always save the latest checkpoint
-            return True
-
-        # otherwise, we need to determine if we should overwrite the worst checkpoint
-        assert metric_value
-        ckpt_value = float(self._ckpt_dirpaths[0].split("=")[-1])
-
-        # do not checkpoint if candidate is worse than the existing one
-        if best_checkpoint_config.mode == "min" and metric_value > ckpt_value:
-            return False
-        elif best_checkpoint_config.mode == "max" and metric_value < ckpt_value:
-            return False
-        # the candidate checkpoint is better than the existing one, so we must overwrite it
-        return True
-
-    def _should_remove_checkpoint(self) -> bool:
-        """
-        Whether the oldest / worst checkpoint should be removed.
-
-        This is called after the candidate checkpoint is saved, so it is already evaluated that the
-        candidate checkpoint was worth saving.
-        """
-
-        keep_last_n_checkpoints = self._keep_last_n_checkpoints
-        return (
-            keep_last_n_checkpoints is not None
-            and len(self._ckpt_dirpaths) >= keep_last_n_checkpoints
-        )
-
-    def _remove_checkpoint(self, state: State) -> None:
-        # remove oldest checkpoint directory
-        oldest_ckpt_path = self._ckpt_dirpaths.pop(0)
-        with get_timing_context(state, f"{self.__class__.__name__}.delete_checkpoint"):
-            if self._pg_wrapper.get_rank() == 0:
-                # only delete on rank 0
-                _delete_checkpoint(oldest_ckpt_path)
-            self._pg_wrapper.barrier()
-
     @staticmethod
     @abc.abstractmethod
     def restore(
         path: str,
         unit: AppStateMixin,
         *,
         train_dataloader: Optional[Iterable[TTrainData]] = None,
@@ -433,15 +331,15 @@
         *,
         train_dataloader: Optional[Iterable[TTrainData]] = None,
         process_group: Optional[dist.ProcessGroup] = None,
         restore_options: Optional[RestoreOptions] = None,
         **kwargs: Any,
     ) -> bool:
         """
-        Given a parent directory where checkpoints are saved, restore the checkppoint state from the latest checkpoint in the directory.
+        Given a parent directory where checkpoints are saved, restore the checkpoint state from the latest checkpoint in the directory.
 
         There are additional flags offered should the user want to skip loading the train and eval progress.
         By default, the train and eval progress are restored, if applicable.
 
         Args:
             dirpath: Parent directory from which to get the latest checkpoint.
             unit: An instance of :class:`~torchtnt.framework.unit.TrainUnit`, :class:`~torchtnt.framework.unit.EvalUnit`, or :class:`~torchtnt.framework.unit.PredictUnit` containing states to restore.
@@ -452,14 +350,17 @@
         Returns:
             True if the latest checkpoint directory was found and successfully restored, otherwise False.
         """
         path = get_latest_checkpoint_path(
             dirpath, metadata_fname=cls.metadata_fname, process_group=process_group
         )
         if path is None:
+            logger.info(
+                f"Attempted to restore from the following path but no checkpoint was found: {dirpath=}, {cls.metadata_fname}"
+            )
             return False
         logger.info(f"Restoring from path: {path}")
         cls.restore(
             path,
             unit,
             train_dataloader=train_dataloader,
             process_group=process_group,
@@ -522,27 +423,7 @@
             train_dataloader=train_dataloader,
             process_group=process_group,
             restore_options=restore_options,
             **kwargs,
         )
 
         return True
-
-    @rank_zero_read_and_broadcast
-    def _does_checkpoint_exist(
-        self, checkpoint_path: str, process_group: Optional[dist.ProcessGroup] = None
-    ) -> bool:
-        """
-        Checking whether a checkpoint already exists by verifying whether the optional metadata file is present in the directory.
-        If the checkpointer doesn't have a metadata file, this function will always return False.
-        """
-        metadata_fname = self.metadata_fname
-        if not metadata_fname:
-            return False
-
-        fs = get_filesystem(checkpoint_path)
-        return _metadata_exists(fs, checkpoint_path, metadata_fname)
-
-
-def _get_save_path(dirpath: str, epoch: int, step: int) -> str:
-    # TODO: discuss whether this path should be customized
-    return os.path.join(dirpath, f"epoch_{epoch}_step_{step}")
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import csv
 import os
 from abc import ABC, abstractmethod
 from typing import Any, List, TextIO, Union
 
 from pyre_extensions import none_throws
 
@@ -57,16 +59,15 @@
     @abstractmethod
     def get_step_output_rows(
         self,
         state: State,
         unit: TPredictUnit,
         # pyre-fixme: Missing parameter annotation [2]
         step_output: Any,
-    ) -> Union[List[str], List[List[str]]]:
-        ...
+    ) -> Union[List[str], List[List[str]]]: ...
 
     def on_predict_start(self, state: State, unit: TPredictUnit) -> None:
         if get_global_rank() == 0:
             self._writer.writerow(self.header_row)
 
     def on_predict_step_end(self, state: State, unit: TPredictUnit) -> None:
         predict_state = none_throws(state.predict_state)
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/checkpointer_types.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/checkpointer_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from dataclasses import dataclass
-from typing import Literal, Optional
+from typing import Optional
+
 
 # TODO: eventually support overriding all knobs
 @dataclass
 class KnobOptions:
     """
-    Controls the knobs in TorchSnapshot.
+    Controls the knobs for Checkpoints.
 
     Args:
-        max_per_rank_io_concurrency: Maximum number of concurrent IO operations per rank. Defaults to 16.
+        max_per_rank_io_concurrency: Maximum number of concurrent IO operations per rank in checkpointing.
+                                     Defaults to 16.
+        enable_storage_optimization: Enable storage efficiency optimizations for Distributed Checkpointing.
     """
 
+    # use a more conservative number of concurrent IO operations per rank in Checkpointing
+    # the default value of 16 is too bandwidth hungry for most users
     max_per_rank_io_concurrency: Optional[int] = None
+    # This is a no-op and for future use. This would enable storage efficiency optimizations:
+    # e.g. Compression, Batching, Quantization etc.
+    enable_storage_optimization: bool = False
 
 
 @dataclass
 class RestoreOptions:
     """
     Options when restoring a snapshot.
 
     Args:
         restore_train_progress: Whether to restore the training progress state.
         restore_eval_progress: Whether to restore the evaluation progress state.
         restore_optimizers: Whether to restore the optimizer states.
         restore_lr_schedulers: Whether to restore the lr scheduler states.
+        strict: Whether to strictly restore app state and the module state dict.
     """
 
     restore_train_progress: bool = True
     restore_eval_progress: bool = True
     restore_optimizers: bool = True
     restore_lr_schedulers: bool = True
-
-
-@dataclass
-class BestCheckpointConfig:
-    """
-    Config for saving the best checkpoints.
-
-    Args:
-        monitored_metric: Metric to monitor for saving best checkpoints. Must be an numerical or tensor attribute on the unit.
-        mode: One of `min` or `max`. The save file is overwritten based the max or min of the monitored metric.
-    """
-
-    monitored_metric: str
-    mode: Literal["min", "max"] = "min"
+    strict: bool = True
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/empty_cuda_cache.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/empty_cuda_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import cast
 
 import torch
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import gc
 from typing import cast
 
 from pyre_extensions import none_throws
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/iteration_time_logger.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/time_wait_for_batch_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,100 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 
-from typing import Optional, Union
+from typing import cast, Union
 
 from pyre_extensions import none_throws
 from torch.utils.tensorboard import SummaryWriter
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
-from torchtnt.utils.distributed import get_global_rank
-from torchtnt.utils.loggers.tensorboard import TensorBoardLogger
+from torchtnt.utils.distributed import rank_zero_fn
+from torchtnt.utils.loggers.logger import MetricLogger
 from torchtnt.utils.timer import TimerProtocol
 
 
-class IterationTimeLogger(Callback):
+class TimeWaitForBatchLogger(Callback):
     """
-    A callback which logs iteration times as scalars to TensorBoard.
+    A callback which logs time wait for batch as scalars to a MetricLogger.
 
     Args:
-        logger: Either a :class:`torchtnt.loggers.tensorboard.TensorBoardLogger`
+        logger: Either a subclass of :class:`torchtnt.utils.loggers.logger.MetricLogger`
             or a :class:`torch.utils.tensorboard.SummaryWriter` instance.
-        moving_avg_window: an optional int to control the moving average window
-        log_every_n_steps: an optional int to control the log frequency
+        log_every_n_steps: an int to control the log frequency. Default is 1.
+        warmup_steps: an int to control the number of warmup steps. We will start logging only after the amount of warmup steps were completed. Default is 0.
     """
 
-    _writer: Optional[SummaryWriter] = None
-
     def __init__(
         self,
-        logger: Union[TensorBoardLogger, SummaryWriter],
-        moving_avg_window: int = 1,
+        logger: Union[MetricLogger, SummaryWriter],
+        *,
         log_every_n_steps: int = 1,
+        warmup_steps: int = 0,
     ) -> None:
-        if isinstance(logger, TensorBoardLogger):
-            logger = logger.writer
-
-        if get_global_rank() == 0:  # only write from the main rank
-            self._writer = none_throws(
-                logger, "TensorBoardLogger.writer should not be None"
+        self._logger = logger
+        if log_every_n_steps < 1:
+            raise ValueError(
+                f"log_every_n_steps must be at least 1, got {log_every_n_steps}"
             )
-        self.moving_avg_window = moving_avg_window
-        self.log_every_n_steps = log_every_n_steps
+        self._log_every_n_steps = log_every_n_steps
 
+        if warmup_steps < 0:
+            raise ValueError(f"warmup_steps must be at least 0, got {warmup_steps}")
+        self._warmup_steps = warmup_steps
+
+    @rank_zero_fn
     def _log_step_metrics(
         self,
-        writer: SummaryWriter,
-        metric_label: str,
-        iteration_timer: TimerProtocol,
-        step_logging_for: int,
+        *,
+        timer: TimerProtocol,
+        label: str,
+        step: int,
     ) -> None:
-        """
-        Helper function to write a timing log message to writer based on how the class
-        was configured.
-
-        """
-        if step_logging_for % self.log_every_n_steps != 0:
+        if step <= self._warmup_steps:
             return
 
-        human_metric_names = {
-            "train_iteration_time": "Train Iteration Time (seconds)",
-            "eval_iteration_time": "Eval Iteration Time (seconds)",
-            "predict_iteration_time": "Prediction Iteration Time (seconds)",
-        }
+        if step % self._log_every_n_steps != 0:
+            return
 
-        time_list = iteration_timer.recorded_durations.get(metric_label, [])
-        if not time_list:
+        data_wait_time_list = timer.recorded_durations.get("data_wait_time")
+        if not data_wait_time_list:
             return
 
-        last_n_values = time_list[-self.moving_avg_window :]
-        writer.add_scalar(
-            human_metric_names[metric_label],
-            sum(last_n_values) / len(last_n_values),
-            step_logging_for,
-        )
+        if isinstance(self._logger, SummaryWriter):
+            self._logger.add_scalar(
+                label,
+                data_wait_time_list[-1],
+                step,
+            )
+        else:
+            cast(MetricLogger, self._logger).log(
+                label,
+                data_wait_time_list[-1],
+                step,
+            )
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
-        timer = none_throws(state.train_state).iteration_timer
-        if writer := self._writer:
-            self._log_step_metrics(
-                writer,
-                "train_iteration_time",
-                timer,
-                unit.train_progress.num_steps_completed,
-            )
+        self._log_step_metrics(
+            timer=none_throws(state.train_state).iteration_timer,
+            label="Time Wait For Batch (Train)",
+            step=unit.train_progress.num_steps_completed,
+        )
 
     def on_eval_step_end(self, state: State, unit: TEvalUnit) -> None:
-        timer = none_throws(state.eval_state).iteration_timer
-        if writer := self._writer:
-            self._log_step_metrics(
-                writer,
-                "eval_iteration_time",
-                timer,
-                unit.eval_progress.num_steps_completed,
-            )
+        self._log_step_metrics(
+            timer=none_throws(state.eval_state).iteration_timer,
+            label="Time Wait For Batch (Eval)",
+            step=unit.eval_progress.num_steps_completed,
+        )
 
     def on_predict_step_end(self, state: State, unit: TPredictUnit) -> None:
-        timer = none_throws(state.predict_state).iteration_timer
-        if writer := self._writer:
-            self._log_step_metrics(
-                writer,
-                "predict_iteration_time",
-                timer,
-                unit.predict_progress.num_steps_completed,
-            )
+        self._log_step_metrics(
+            timer=none_throws(state.predict_state).iteration_timer,
+            label="Time Wait For Batch (Predict)",
+            step=unit.predict_progress.num_steps_completed,
+        )
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Callable, Optional, Union
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Dict, List, Union
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TTrainUnit
 from torchtnt.utils.loggers.logger import MetricLogger
 from torchtnt.utils.optimizer import extract_lr_from_optimizer
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/memory_snapshot.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/memory_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
 from torchtnt.utils.memory_snapshot_profiler import MemorySnapshotProfilerBase
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class MemorySnapshot(Callback):
-
     """
     A callback for memory snapshot collection during training, saving pickle files to the user-specified directory.
     Uses `Memory Snapshots <https://zdevito.github.io/2022/08/16/memory-snapshots.html>`.
 
     Args:
         memory_snapshot_profiler: Instance of MemorySnapshotProfilerBase, controls when and where to save the memory snapshots.
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/module_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Any, Callable, Dict, List, MutableMapping, Optional, Tuple
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
 from torchtnt.framework.unit import AppStateMixin, TEvalUnit, TPredictUnit, TTrainUnit
 from torchtnt.utils.module_summary import (
     get_module_summary,
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import torch
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
 
 
 class PyTorchProfiler(Callback):
     """
-    A callback which profiles user code using `PyTorch Profiler <https://pytorch.org/docs/stable/profiler.html/>`_.
+    A callback which profiles user code using `PyTorch Profiler <https://pytorch.org/docs/stable/profiler.html>`_.
 
     Args:
         profiler: a torch.profiler.profile context manager which will be used
 
     """
 
     def __init__(
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Dict, List, Optional, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Dict, Optional, Union
 
 import torch
 
 from torch.utils.tensorboard import SummaryWriter
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from __future__ import annotations
 
 import logging
 from contextlib import contextmanager, ExitStack
 from typing import Any, Dict, Generator, Iterable, List, Optional, Set, Union
 
 import torch.distributed as dist
@@ -16,28 +18,25 @@
     _prepare_app_state,
     _prepare_app_state_for_checkpoint,
     _prepare_app_state_for_restore,
     _TRAIN_DL_STATE_KEY,
 )
 
 from torchtnt.framework.callbacks.base_checkpointer import BaseCheckpointer
-from torchtnt.framework.callbacks.checkpointer_types import (
-    BestCheckpointConfig,
-    KnobOptions,
-    RestoreOptions,
-)
+from torchtnt.framework.callbacks.checkpointer_types import KnobOptions, RestoreOptions
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import (
     AppStateMixin,
     TEvalUnit,
     TPredictUnit,
     TTrainData,
     TTrainUnit,
 )
 from torchtnt.framework.utils import get_timing_context
+from torchtnt.utils.checkpoint import BestCheckpointConfig
 from torchtnt.utils.optimizer import init_optim_state
 from torchtnt.utils.rank_zero_log import rank_zero_info, rank_zero_warn
 from torchtnt.utils.stateful import Stateful
 
 try:
     import torchsnapshot
     from torchsnapshot.knobs import override_max_per_rank_io_concurrency
@@ -154,15 +153,20 @@
         *,
         checkpoint_path: str,
         hook: str,
     ) -> bool:
         """
         Checkpoint the current state of the application.
         """
-        if hook not in ["on_train_step_end", "on_train_epoch_end", "on_train_end"]:
+        if hook not in [
+            "on_train_step_end",
+            "on_train_epoch_end",
+            "on_train_end",
+            "on_eval_epoch_end",
+        ]:
             raise RuntimeError(f"Unexpected hook encountered '{hook}'")
 
         intra_epoch = False
         curr_snapshot_wait = False
 
         if hook == "on_train_step_end":
             intra_epoch = True
@@ -261,28 +265,30 @@
         unit: AppStateMixin,
         *,
         train_dataloader: Optional[Iterable[TTrainData]] = None,
         process_group: Optional[dist.ProcessGroup] = None,
         restore_options: Optional[RestoreOptions] = None,
         storage_options: Optional[Dict[str, Any]] = None,
         knob_options: Optional[KnobOptions] = None,
+        strict: bool = True,
     ) -> None:
         """Utility method to restore snapshot state from a path.
 
         There are additional flags offered should the user want to skip loading the train and eval progress.
         By default, the train and eval progress are restored, if applicable.
 
         Args:
             path: Path of the snapshot to restore.
             unit: An instance of :class:`~torchtnt.framework.unit.TrainUnit`, :class:`~torchtnt.framework.unit.EvalUnit`, or :class:`~torchtnt.framework.unit.PredictUnit` containing states to restore.
             train_dataloader: An optional train dataloader to restore.
             process_group: The process group on which the ranks will communicate on. default: ``None`` (the entire world)
             restore_options: Controls what to  filter when restoring the state.
             storage_options: Additional keyword options for the storage plugin to use, to be passed to `torchsnapshot.Snapshot <https://pytorch.org/torchsnapshot/stable/api_reference.html#torchsnapshot.Snapshot>`_. See each storage plugin's documentation for customizations.
             knob_options: Additional keyword options for the snapshot knobs
+            strict: If ``False``, allows loading a snapshot even if not all keys exist in the unit's app_state.
         """
 
         _validate_snapshot_available()
 
         # initialize optimizer state skeletons for in-place loading of optimizer state with torchsnapshot
         for optimizer in unit.tracked_optimizers().values():
             init_optim_state(optimizer)
@@ -313,17 +319,34 @@
                         break
 
                 if _TRAIN_DL_STATE_KEY not in app_state:
                     rank_zero_warn(
                         "train_dataloader was passed to `restore` but no train dataloader exists in the Snapshot"
                     )
 
+        if not strict:
+            # if app_state keys not in torchsnapshot checkpoint,
+            # remove them from app_state prior to checkpoint load
+            missing_stateful_keys = []
+            manifest = snapshot.get_manifest()
+            for stateful_key in app_state:
+                found = any((f"/{stateful_key}/" in key for key in manifest.keys()))
+                if not found:
+                    missing_stateful_keys.append(stateful_key)
+
+            for key in missing_stateful_keys:
+                rank_zero_warn(
+                    f"{key} was passed to `restore` but does not exists in the snapshot"
+                )
+                app_state.pop(key)
+
         knob_options = knob_options or KnobOptions()
         with _override_knobs(knob_options):
-            snapshot.restore(app_state)
+            strict = strict or restore_options.strict
+            snapshot.restore(app_state, strict=restore_options.strict)
         rank_zero_info(f"Restored snapshot from path: {path}", logger=logger)
 
 
 def _exclude_progress_from_replicated(app_state: Dict[str, _TStateful]) -> Set[str]:
     """
     Excludes progress state from being replicated. Called if replicated=["**"] is passed in.
     Works by populating replicated with all possible keys from app_state, except for
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import io
 from typing import Optional, TextIO, Union
 
 from pyre_extensions import none_throws
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-0.2.4/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import List, Union
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TTrainUnit
 from torchtnt.utils.loggers.logger import MetricLogger
 from torchtnt.utils.progress import Progress
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/evaluate.py` & `torchtnt-0.2.4/torchtnt/framework/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
 from torchtnt.framework._callback_handler import CallbackHandler
 from torchtnt.framework._loop_utils import (
@@ -89,15 +91,17 @@
     try:
         _evaluate_impl(state, eval_unit, callback_handler)
         logger.info("Finished evaluation")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
-        logger.info(e)
+        logger.info(
+            f"Exception during evaluate after the following progress: {eval_unit.eval_progress.get_progress_string()}:\n{e}"
+        )
         eval_unit.on_exception(state, e)
         callback_handler.on_exception(state, eval_unit, e)
         raise e
 
 
 @torch.no_grad()
 def _evaluate_impl(
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/fit.py` & `torchtnt-0.2.4/torchtnt/framework/fit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Iterable, List, Optional
 
 from torchtnt.framework._callback_handler import CallbackHandler
 from torchtnt.framework._loop_utils import _log_api_usage
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, PhaseState, State
@@ -130,11 +132,13 @@
     try:
         _train_impl(state, unit, callback_handler)
         logger.info("Finished fit")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
-        logger.info(f"Exception during fit:\n{e}")
+        logger.info(
+            f"Exception during fit after the following progress: train progress: {unit.train_progress.get_progress_string()} eval progress: {unit.eval_progress.get_progress_string()}:\n{e}"
+        )
         unit.on_exception(state, e)
         callback_handler.on_exception(state, unit, e)
         raise e
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/predict.py` & `torchtnt-0.2.4/torchtnt/framework/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
 
 from torchtnt.framework._callback_handler import CallbackHandler
@@ -89,15 +91,17 @@
     try:
         _predict_impl(state, predict_unit, callback_handler)
         logger.info("Finished predict")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
-        logger.info(f"Exception during predict:\n{e}")
+        logger.info(
+            f"Exception during predict after the following progress: {predict_unit.predict_progress.get_progress_string()}:\n{e}"
+        )
         predict_unit.on_exception(state, e)
         callback_handler.on_exception(state, predict_unit, e)
         raise e
 
 
 @torch.inference_mode()
 def _predict_impl(
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/state.py` & `torchtnt-0.2.4/torchtnt/framework/state.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # ignore errors due to `Any` type
 
 import logging
 from enum import auto, Enum
-from typing import Any, Iterable, Optional
+from typing import Generic, Iterable, Optional, TypeVar
+
+from pyre_extensions import none_throws
 
 from torchtnt.utils.timer import BoundedTimer, TimerProtocol
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
+TStepOutput = TypeVar("TStepOutput")
+TData = TypeVar("TData")
+
 
 def _check_loop_condition(name: str, val: Optional[int]) -> None:
     if val is not None and val < 0:
         raise ValueError(
             f"Invalid value provided for {name}. Expected a non-negative integer or None, but received {val}."
         )
 
@@ -52,53 +59,49 @@
     """
 
     TRAIN = auto()
     EVALUATE = auto()
     PREDICT = auto()
 
 
-class PhaseState:
+class PhaseState(Generic[TData, TStepOutput]):
     """State for each phase (train, eval, predict).
     Modified by the framework, read-only for the user.
     """
 
     def __init__(
         self,
         *,
-        # pyre-fixme[2]: Parameter annotation cannot contain `Any`.
-        dataloader: Iterable[Any],
+        dataloader: Iterable[TData],
         max_epochs: Optional[int] = None,  # used only for train
         max_steps: Optional[int] = None,  # used only for train
         max_steps_per_epoch: Optional[int] = None,
         evaluate_every_n_steps: Optional[int] = None,  # used only for evaluate
         evaluate_every_n_epochs: Optional[int] = None,  # used only for evaluate
     ) -> None:
         _check_loop_condition("max_epochs", max_epochs)
         _check_loop_condition("max_steps", max_steps)
         _check_loop_condition("max_steps_per_epoch", max_steps_per_epoch)
         _check_loop_condition("evaluate_every_n_steps", evaluate_every_n_steps)
         _check_loop_condition("evaluate_every_n_epochs", evaluate_every_n_epochs)
 
-        # pyre-fixme[4]: Attribute annotation cannot contain `Any`.
-        self._dataloader: Iterable[Any] = dataloader
+        self._dataloader: Iterable[TData] = dataloader
         self._max_epochs = max_epochs
         self._max_steps = max_steps
         self._max_steps_per_epoch = max_steps_per_epoch
         self._evaluate_every_n_steps = evaluate_every_n_steps
         self._evaluate_every_n_epochs = evaluate_every_n_epochs
 
-        # pyre-fixme[4]: Attribute annotation cannot be `Any`.
-        self._step_output: Any = None
+        self._step_output: Optional[TStepOutput] = None
         self._iteration_timer = BoundedTimer(
             cuda_sync=False, lower_bound=1_000, upper_bound=5_000
         )
 
     @property
-    # pyre-fixme[3]: Return annotation cannot contain `Any`.
-    def dataloader(self) -> Iterable[Any]:
+    def dataloader(self) -> Iterable[TData]:
         """Dataloader defined by the user."""
         return self._dataloader
 
     @property
     def max_epochs(self) -> Optional[int]:
         """Maximum number of epochs to train, defined by the user."""
         return self._max_epochs
@@ -120,38 +123,40 @@
 
     @property
     def evaluate_every_n_epochs(self) -> Optional[int]:
         """Frequency with which to evaluate in terms of training epochs, when running :func:`~torchtnt.framework.fit`. Defined by the user."""
         return self._evaluate_every_n_epochs
 
     @property
-    # pyre-fixme[3]: Return annotation cannot be `Any`.
-    def step_output(self) -> Any:
+    def step_output(self) -> Optional[TStepOutput]:
         """Output of the last step."""
         return self._step_output
 
     @property
     def iteration_timer(self) -> TimerProtocol:
         """An always-on :class:`~torchtnt.utils.TimerProtocol` object which contains CPU timings (without synchronisation) of the iterations."""
         return self._iteration_timer
 
 
+TPhaseState = PhaseState[TData, TStepOutput]
+
+
 class State:
     """Parent State class which can contain up to 3 instances of PhaseState, for the 3 phases.
     Modified by the framework, read-only for the user.
     """
 
     def __init__(
         self,
         *,
         entry_point: EntryPoint,
         timer: Optional[TimerProtocol] = None,
-        train_state: Optional[PhaseState] = None,
-        eval_state: Optional[PhaseState] = None,
-        predict_state: Optional[PhaseState] = None,
+        train_state: Optional[TPhaseState] = None,
+        eval_state: Optional[TPhaseState] = None,
+        predict_state: Optional[TPhaseState] = None,
     ) -> None:
         self._entry_point = entry_point
         self._timer = timer
         self._train_state = train_state
         self._eval_state = eval_state
         self._predict_state = predict_state
         self._should_stop: bool = False
@@ -169,30 +174,41 @@
 
     @property
     def timer(self) -> Optional[TimerProtocol]:
         """A :class:`~torchtnt.utils.TimerProtocol` object which can be used for debugging to record latencies of key events during loop execution."""
         return self._timer
 
     @property
-    def train_state(self) -> Optional[PhaseState]:
+    def train_state(self) -> Optional[TPhaseState]:
         """A :class:`~torchtnt.framework.state.PhaseState` object which contains meta information about the train phase."""
         return self._train_state
 
     @property
-    def eval_state(self) -> Optional[PhaseState]:
+    def eval_state(self) -> Optional[TPhaseState]:
         """A :class:`~torchtnt.framework.state.PhaseState` object which contains meta information about the eval phase."""
         return self._eval_state
 
     @property
-    def predict_state(self) -> Optional[PhaseState]:
+    def predict_state(self) -> Optional[TPhaseState]:
         """A :class:`~torchtnt.framework.state.PhaseState` object which contains meta information about the predict phase."""
         return self._predict_state
 
     @property
     def should_stop(self) -> bool:
         """Read-only property for whether to terminate the loop after the current step completes."""
         return self._should_stop
 
     def stop(self) -> None:
         """Signal to the loop to end after the current step completes."""
         _logger.warning("Received signal to stop")
         self._should_stop = True
+
+    def active_phase_state(self) -> TPhaseState:
+        """Returns the current active phase state."""
+        if self._active_phase == ActivePhase.TRAIN:
+            return none_throws(self._train_state)
+        elif self._active_phase == ActivePhase.EVALUATE:
+            return none_throws(self._eval_state)
+        elif self._active_phase == ActivePhase.PREDICT:
+            return none_throws(self._predict_state)
+        else:
+            raise ValueError(f"Invalid active phase: {self._active_phase}")
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/train.py` & `torchtnt-0.2.4/torchtnt/framework/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
 from torchtnt.framework._callback_handler import CallbackHandler
 from torchtnt.framework._loop_utils import (
@@ -99,15 +101,17 @@
     try:
         _train_impl(state, train_unit, callback_handler)
         logger.info("Finished train")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
-        logger.info(f"Exception during train:\n{e}")
+        logger.info(
+            f"Exception during train after the following progress: {train_unit.train_progress.get_progress_string()}:\n{e}"
+        )
         train_unit.on_exception(state, e)
         callback_handler.on_exception(state, train_unit, e)
         raise e
 
 
 # Enabling grad in case this function is called directly from elsewhere in the framework.
 @torch.enable_grad()
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/unit.py` & `torchtnt-0.2.4/torchtnt/framework/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
 
+
+import inspect
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, cast, Dict, Generic, Iterator, TypeVar, Union
 
 import torch
-from torchtnt.framework._loop_utils import _step_requires_iterator
-from torchtnt.framework._unit_utils import _find_optimizers_for_module
+from torchtnt.framework._unit_utils import (
+    _find_optimizers_for_module,
+    _step_requires_iterator,
+)
 
 from torchtnt.framework.state import State
 from torchtnt.utils.lr_scheduler import TLRScheduler
 from torchtnt.utils.prepare_module import _is_fsdp_module, FSDPOptimizerWrapper
 from torchtnt.utils.progress import Progress
 from torchtnt.utils.stateful import Stateful
 
@@ -140,15 +145,15 @@
             )
         elif isinstance(value, Progress):
             self._update_attr(
                 name,
                 value,
                 self.__dict__.get("_progress"),
             )
-        elif isinstance(value, Stateful):
+        elif isinstance(value, Stateful) and not inspect.isclass(value):
             self._update_attr(
                 name,
                 value,
                 self.__dict__.get("_misc_statefuls"),
             )
         else:
             if value is None:
```

### Comparing `torchtnt-0.2.3/torchtnt/framework/utils.py` & `torchtnt-0.2.4/torchtnt/framework/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from contextlib import contextmanager, nullcontext
 from typing import ContextManager, Generator, Tuple, TypeVar
 
 from torch.profiler import record_function
 from torchtnt.framework.state import State
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/__init__.py` & `torchtnt-0.2.4/torchtnt/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
+from .checkpoint import (
+    BestCheckpointConfig,
+    CheckpointManager,
+    CheckpointPath,
+    get_best_checkpoint_path,
+    get_checkpoint_dirpaths,
+    get_latest_checkpoint_path,
+    MetricData,
+)
 from .device import (
     copy_data_to_device,
     CPUStats,
     get_device_from_env,
     get_nvidia_smi_gpu_stats,
     get_psutil_cpu_stats,
     GPUStats,
@@ -68,27 +79,26 @@
 from .swa import AveragedModel
 from .test_utils import get_pet_launch_config
 from .timer import FullSyncPeriodicTimer, get_timer_summary, log_elapsed_time, Timer
 from .tqdm import close_progress_bar, create_progress_bar, update_progress_bar
 from .version import (
     get_python_version,
     get_torch_version,
-    is_torch_version_ge_1_13_1,
-    is_torch_version_geq_1_10,
-    is_torch_version_geq_1_11,
-    is_torch_version_geq_1_12,
-    is_torch_version_geq_1_13,
-    is_torch_version_geq_1_14,
-    is_torch_version_geq_1_8,
-    is_torch_version_geq_1_9,
-    is_torch_version_geq_2_0,
+    is_torch_version_geq,
     is_windows,
 )
 
 __all__ = [
+    "CheckpointPath",
+    "MetricData",
+    "get_best_checkpoint_path",
+    "get_checkpoint_dirpaths",
+    "get_latest_checkpoint_path",
+    "BestCheckpointConfig",
+    "CheckpointManager",
     "copy_data_to_device",
     "CPUStats",
     "get_device_from_env",
     "get_nvidia_smi_gpu_stats",
     "get_psutil_cpu_stats",
     "GPUStats",
     "set_float32_precision",
@@ -146,20 +156,12 @@
     "Timer",
     "create_progress_bar",
     "close_progress_bar",
     "update_progress_bar",
     "TLRScheduler",
     "get_python_version",
     "get_torch_version",
-    "is_torch_version_ge_1_13_1",
-    "is_torch_version_geq_1_10",
-    "is_torch_version_geq_1_11",
-    "is_torch_version_geq_1_12",
-    "is_torch_version_geq_1_13",
-    "is_torch_version_geq_1_14",
-    "is_torch_version_geq_1_8",
-    "is_torch_version_geq_1_9",
-    "is_torch_version_geq_2_0",
+    "is_torch_version_geq",
     "is_windows",
     "get_pet_launch_config",
     "spawn_multi_process",
 ]
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/data/__init__.py` & `torchtnt-0.2.4/torchtnt/utils/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from .data_prefetcher import CudaDataPrefetcher
 from .iterators import (
     AllDatasetBatchesIterator,
     DataIterationStrategy,
     DataIterationStrategyRegistry,
     InOrderIterator,
     MultiIterator,
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-0.2.4/torchtnt/utils/data/data_prefetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Iterable, Iterator, List, TypeVar
 
 import torch
 from torchtnt.utils.device import copy_data_to_device
 
 Batch = TypeVar("Batch")
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/data/iterators.py` & `torchtnt-0.2.4/torchtnt/utils/data/iterators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from __future__ import annotations
 
+import logging
+
 import random
 from abc import abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from itertools import cycle
 from typing import (
     Any,
+    cast,
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
     MutableMapping,
     Optional,
@@ -25,19 +30,21 @@
     TYPE_CHECKING,
     Union,
 )
 
 import torch
 import torch.distributed as dist
 
-
 if TYPE_CHECKING:
     from torch.utils.data import DataLoader
 
 
+logger: logging.Logger = logging.getLogger(__name__)
+
+
 @dataclass
 class DataIterationStrategy:
     pass
 
 
 class MultiIterator(Iterator[Dict[str, Any]]):
     """MultiIterator defines the iteration logic to get a batch, given
@@ -55,28 +62,33 @@
             sources reading support to achieve the same functionality provided by MultiIterator.
         For example, `mux`, `mux_longest`, `cycle`, `zip` etc. Please refer to the documentation for more details.
 
     """
 
     def __init__(
         self,
-        # pyre-fixme[24]: Generic type `Iterable` expects 1 type parameter
-        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable]],
+        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable[object]]],
         iteration_strategy: DataIterationStrategy,
     ) -> None:
         self.individual_dataloaders = individual_dataloaders
         self.iteration_strategy = iteration_strategy
 
     def __str__(self) -> str:
         return str(self.iteration_strategy)
 
     @abstractmethod
     def __next__(self) -> Dict[str, Any]:
         pass
 
+    def state_dict(self) -> Dict[str, Any]:
+        return {}
+
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+        pass
+
 
 class StoppingMechanism(Enum):
     ALL_DATASETS_EXHAUSTED = "ALL_DATASETS_EXHAUSTED"
     SMALLEST_DATASET_EXHAUSTED = "SMALLEST_DATASET_EXHAUSTED"
     RESTART_UNTIL_ALL_DATASETS_EXHAUSTED = "RESTART_UNTIL_ALL_DATASETS_EXHAUSTED"
 
     # used with RandomizedBatchSampler
@@ -120,31 +132,30 @@
         {'b': tensor([5, 6, 7, 8, 9])}
         {'b': tensor([10, 11, 12, 13, 14])}
 
     """
 
     def __init__(
         self,
-        # pyre-fixme[24]: Generic type `Iterable` expects 1 type parameter
-        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable]],
+        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable[object]]],
         iteration_strategy: RoundRobin,
     ) -> None:
         super().__init__(individual_dataloaders, iteration_strategy)
         self.iteration_strategy = iteration_strategy
 
         if (
             self.iteration_strategy.stopping_mechanism
             == StoppingMechanism.WRAP_AROUND_UNTIL_KILLED
         ):
             raise NotImplementedError(
                 "WRAP_AROUND_UNTIL_KILLED is not implemented for RoundRobin"
             )
-        self.individual_iterators: Mapping[str, Iterator[DataLoader]] = {
-            name: iter(dl) for name, dl in individual_dataloaders.items()
-        }
+        self.individual_iterators: Mapping[
+            str, Union[Iterator[DataLoader], Iterator[object]]
+        ] = {name: iter(dl) for name, dl in individual_dataloaders.items()}
         round_robin_order = iteration_strategy.iteration_order or list(
             self.individual_iterators.keys()
         )
         self.dataloader_cycle: Iterator[str] = cycle(round_robin_order)
         self.cur_dataloader: str = round_robin_order[0]
         self.finished_dataloaders: List[str] = []
 
@@ -171,14 +182,34 @@
             self.finished_dataloaders.append(self.cur_dataloader)
 
             if len(self.finished_dataloaders) == len(self.individual_iterators):
                 raise StopIteration
 
             return self.__next__()
 
+    def state_dict(self) -> Dict[str, Any]:
+        return {
+            "finished_dataloaders": self.finished_dataloaders,
+            "cur_dataloader": self.cur_dataloader,
+        }
+
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+        logger.info(
+            f"Loading RoundRobinIterator state. Finished dataloaders: {state_dict['finished_dataloaders']} and trying to set cur_dataloader to {self.cur_dataloader}"
+        )
+        self.finished_dataloaders = state_dict["finished_dataloaders"]
+        cur_dataloader = state_dict["cur_dataloader"]
+        if cur_dataloader not in self.dataloader_cycle:
+            logger.warning(
+                f"Did not find {cur_dataloader} in {list(self.dataloader_cycle)}. Skipping setting cur_dataloader"
+            )
+            return
+        while self.cur_dataloader != cur_dataloader:
+            self.cur_dataloader = next(self.dataloader_cycle)
+
 
 @dataclass
 class AllDatasetBatches(DataIterationStrategy):
     stopping_mechanism: StoppingMechanism = StoppingMechanism.ALL_DATASETS_EXHAUSTED
 
 
 class AllDatasetBatchesIterator(MultiIterator):
@@ -218,30 +249,29 @@
         {'b': tensor([5, 6, 7, 8, 9])}
         {'b': tensor([10, 11, 12, 13, 14])}
 
     """
 
     def __init__(
         self,
-        # pyre-fixme[24]: Generic type `Iterable` expects 1 type parameter
-        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable]],
+        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable[object]]],
         iteration_strategy: AllDatasetBatches,
     ) -> None:
         super().__init__(individual_dataloaders, iteration_strategy)
         self.iteration_strategy = iteration_strategy
         if (
             self.iteration_strategy.stopping_mechanism
             == StoppingMechanism.WRAP_AROUND_UNTIL_KILLED
         ):
             raise NotImplementedError(
                 "WRAP_AROUND_UNTIL_KILLED is not implemented for AllDatasetBatches"
             )
-        self.individual_iterators: Dict[str, Iterator[DataLoader]] = {
-            name: iter(dl) for name, dl in individual_dataloaders.items()
-        }
+        self.individual_iterators: Dict[
+            str, Union[Iterator[DataLoader], Iterator[object]]
+        ] = {name: iter(dl) for name, dl in individual_dataloaders.items()}
         self.iterators_finished: List[str] = []
 
     def __next__(self) -> Dict[str, Any]:
         batch_dict = {}
         for iterator in self.individual_iterators:
             try:
                 batch_dict[iterator] = next(self.individual_iterators[iterator])
@@ -306,49 +336,49 @@
         {'a': tensor([0, 1, 2, 3])}
         {'b': tensor([10, 11, 12, 13, 14])}
 
     """
 
     def __init__(
         self,
-        # pyre-fixme[24]: Generic type `Iterable` expects 1 type parameter
-        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable]],
+        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable[object]]],
         iteration_strategy: RandomizedBatchSampler,
     ) -> None:
         super().__init__(individual_dataloaders, iteration_strategy)
         self._iteration_strategy = iteration_strategy
         self._individual_dataloaders = individual_dataloaders
-        self._individual_iterators: MutableMapping[str, Iterator[DataLoader]] = {
-            name: iter(dl) for name, dl in self._individual_dataloaders.items()
-        }
+        self._individual_iterators: MutableMapping[
+            str, Union[Iterator[DataLoader], Iterator[object]]
+        ] = {name: iter(dl) for name, dl in self._individual_dataloaders.items()}
         self._iterator_names: List[str] = sorted(self._individual_dataloaders.keys())
         weights = iteration_strategy.weights
         if weights is None:
             self._iterator_weights: Optional[List[float]] = None
         else:
             assert set(self._iterator_names).issubset(
                 weights.keys()
             ), "Weight keys must match dataloader keys"
             self._iterator_weights = [
                 float(weights[name]) for name in self._iterator_names
             ]
         self._iterator_is_exhausted: List[bool] = [False] * len(self._iterator_names)
-        self.stopping_mechanism: Optional[
-            StoppingMechanism
-        ] = iteration_strategy.stopping_mechanism
+        self.stopping_mechanism: Optional[StoppingMechanism] = (
+            iteration_strategy.stopping_mechanism
+        )
         self.enforce_same_loader_across_ranks: bool = (
             iteration_strategy.enforce_same_loader_across_ranks
         )
         if self.enforce_same_loader_across_ranks:
             self._iterator_names_dict: Dict[str, torch.IntTensor] = {
                 name: torch.IntTensor([idx])
                 for idx, name in enumerate(self._iterator_names)
             }
-            # pyre-fixme[4]: missing attribute annotation
-            self._process_group = dist.new_group(backend="gloo", ranks=None)
+            self._process_group: dist.ProcessGroup = dist.new_group(
+                backend="gloo", ranks=None
+            )
 
         self._iterators_finished: List[str] = []
 
     def __next__(self) -> Dict[str, Any]:
         if (
             self.stopping_mechanism == StoppingMechanism.SMALLEST_DATASET_EXHAUSTED
             and any(self._iterator_is_exhausted)
@@ -391,17 +421,15 @@
         if (
             self.enforce_same_loader_across_ranks
             and dist.is_available()
             and dist.is_initialized()
         ):
             key_idx = self._iterator_names_dict[selected_key]
             dist.broadcast(key_idx, 0, group=self._process_group)
-            # pyre-fixme[6]: For 1st param expected `SupportsIndex` but got
-            #  `Union[bool, float, int]`.
-            selected_key = self._iterator_names[key_idx.item()]
+            selected_key = self._iterator_names[cast(int, key_idx.item())]
 
         try:
             batch = next(self._individual_iterators[selected_key])
         except StopIteration:
             if (
                 self.stopping_mechanism
                 == StoppingMechanism.RESTART_UNTIL_ALL_DATASETS_EXHAUSTED
@@ -460,23 +488,22 @@
         {'b': tensor([5, 6, 7, 8, 9])}
         {'b': tensor([10, 11, 12, 13, 14])}
 
     """
 
     def __init__(
         self,
-        # pyre-fixme[24]: Generic type `Iterable` expects 1 type parameter
-        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable]],
+        individual_dataloaders: Mapping[str, Union[DataLoader, Iterable[object]]],
         iteration_strategy: InOrder,
     ) -> None:
         super().__init__(individual_dataloaders, iteration_strategy)
         self.iteration_order: List[str] = iteration_strategy.iteration_order or list(
             self.individual_dataloaders.keys()
         )
-        self.cur_iter: Iterator[DataLoader] = iter(
+        self.cur_iter: Union[Iterator[DataLoader], Iterator[object]] = iter(
             self.individual_dataloaders[self.iteration_order[0]]
         )
         self.cur_iterator: str = self.iteration_order[0]
         self.num_iterators: int = len(self.iteration_order)
         self.iterators_finished: int = 0
 
     def __next__(self) -> Dict[str, Any]:
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-0.2.4/torchtnt/utils/data/multi_dataloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, Iterable, Iterator, Optional, Type, TYPE_CHECKING, Union
 
+from pyre_extensions import none_throws
+
 from torchtnt.utils.data.iterators import (
     DataIterationStrategy,
     DataIterationStrategyRegistry,
     MultiIterator,
 )
 from torchtnt.utils.stateful import Stateful
 
+
 if TYPE_CHECKING:
     from torch.utils.data import DataLoader
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class MultiDataLoader:
@@ -39,66 +44,79 @@
         provided by MultiIterator.
         For example, `mux`, `mux_longest`, `cycle`, `zip` etc. Please refer
         to the documentation for more details.
     """
 
     def __init__(
         self,
-        # pyre-fixme[24]: Generic type `Iterable` expects 1 type parameter
-        individual_dataloaders: Dict[str, Union[DataLoader, Iterable]],
+        individual_dataloaders: Dict[str, Union[DataLoader, Iterable[object]]],
         iteration_strategy: DataIterationStrategy,
         iterator_cls: Optional[Type[MultiIterator]] = None,
         ignore_empty_data: bool = False,
     ) -> None:
         self.individual_dataloaders = individual_dataloaders
         self.iteration_strategy = iteration_strategy
         self.iterator_cls = iterator_cls
+        self.current_iterator: Optional[MultiIterator] = None
         for name in list(individual_dataloaders.keys()):
             try:
                 next(iter(self.individual_dataloaders[name]))
             except StopIteration:
                 if not ignore_empty_data:
                     raise ValueError(f"Dataloader '{name}' contains no data.")
                 else:
                     logger.warning(
                         f"Dataloader '{name}' which contains no data. "
                         "You might have empty dataloaders in the input dict."
                     )
+        self.iterator_state: Optional[Dict[str, Any]] = None
 
     def __iter__(self) -> Iterator[Dict[str, Any]]:
         """Iterator functions for the collection of dataloaders.
 
         Returns:
             a newly created iterator based on DataIterationStrategy
 
         """
         iterator_cls = self.iterator_cls
         if iterator_cls is None:
             iterator_cls = DataIterationStrategyRegistry.get(self.iteration_strategy)
-        # pyre-fixme[16]: `MultiDataLoader` has no attribute `iterator`.
-        # pyre-fixme[45]: Cannot instantiate abstract class `MultiIterator`.
-        self.iterator = iterator_cls(
+        # in practice, DataIterationStrategyRegistry.get() returns just concrete classes
+        # pyre-ignore[45]: Cannot instantiate abstract class `MultiIterator`.
+        self.current_iterator = iterator_cls(
             individual_dataloaders=self.individual_dataloaders,
             iteration_strategy=self.iteration_strategy,
         )
-        return self.iterator
+        if self.iterator_state is not None:
+            self.current_iterator.load_state_dict(self.iterator_state)
+
+        self.iterator_state = None
+        return none_throws(self.current_iterator)
 
     def state_dict(self) -> Dict[str, Any]:
         """Return an aggregated state dict based on individual dataloaders.
 
         The state dict is keyed off the names provided by ``individual_dataloaders``.
 
         Note:
             Only states from dataloaders that implement the :class:`~torchtnt.utils.stateful.Stateful` protocol are included in the returned state dict.
         """
         state_dict = {}
         for name, dl in self.individual_dataloaders.items():
             if isinstance(dl, Stateful):
                 state_dict[name] = dl.state_dict()
 
+        if (current_iterator := self.current_iterator) is not None:
+            iterator_state = current_iterator.state_dict()
+            if iterator_state:
+                logger.info("Storing iterator state in MultiDataLoader state_dict")
+                # we make an implicit assumption here that none of the dataloaders have the "iterator_state" key in order to be backwards compatible
+                # with already saved checkpoints (we don't want to modify the dataloaders stateful names)
+                state_dict["iterator_state"] = iterator_state
+
         return state_dict
 
     def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
         """Loads aggregated state dict based on individual dataloaders.
 
         The provided state dict should be keyed off the names provided by ``individual_dataloaders``.
 
@@ -110,7 +128,11 @@
                 contents = state_dict.get(name, None)
                 if contents is None:
                     logger.warning(
                         f"Skipping loading state dict for dataloader {name} as there is no corresponding entry in the state dict"
                     )
                     continue
                 dl.load_state_dict(contents)
+
+        if "iterator_state" in state_dict:
+            # this will be used during the next __iter__ call
+            self.iterator_state = state_dict["iterator_state"]
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-0.2.4/torchtnt/utils/data/profile_dataloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Iterable, Optional
 
 import torch
 from torch.profiler import record_function
 from torchtnt.utils.device import copy_data_to_device
 from torchtnt.utils.timer import Timer, TimerProtocol
@@ -37,26 +39,23 @@
     timer = timer if timer is not None else Timer(cuda_sync=False)
     with timer.time("iter(dataloader)"), record_function("iter(dataloader)"):
         data_iter = iter(dataloader)
 
     # If max_steps is not set, run until the dataloader is exhausted
     steps_completed = 0
 
-    should_move_data_to_device = device is not None
-
     while max_steps is None or (steps_completed < max_steps):
         try:
             with timer.time("next(iter)"), record_function("next(iter)"):
                 data = next(data_iter)
 
-            if should_move_data_to_device:
+            if device is not None:
                 with timer.time("copy_data_to_device"), record_function(
                     "copy_data_to_device"
                 ):
-                    # pyre-fixme [6]: device is checked as not None before calling this
                     data = copy_data_to_device(data, device)
 
             steps_completed += 1
             if profiler:
                 profiler.step()
         except StopIteration:
             break
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/data/synthetic_data.py` & `torchtnt-0.2.4/torchtnt/utils/data/synthetic_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from __future__ import annotations
 
 import abc
 import logging
 from dataclasses import dataclass, field
 from typing import Generic, TypeVar
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/device.py` & `torchtnt-0.2.4/torchtnt/utils/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 import os
 import shutil
 import subprocess
 from collections import defaultdict
 from dataclasses import fields, is_dataclass
 from typing import Any, Dict, Mapping, TypeVar
 
 import torch
-from torchtnt.utils.version import is_torch_version_geq_1_12
 from typing_extensions import Protocol, runtime_checkable, TypedDict
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def get_device_from_env() -> torch.device:
     """Function that gets the torch.device based on the current environment.
@@ -36,19 +37,15 @@
         local_rank = int(os.environ.get("LOCAL_RANK", "0"))
         if local_rank >= torch.cuda.device_count():
             raise RuntimeError(
                 "The local rank is larger than the number of available GPUs."
             )
         device = torch.device(f"cuda:{local_rank}")
         torch.cuda.set_device(device)
-    elif (
-        is_torch_version_geq_1_12()
-        and torch.backends.mps.is_built()
-        and torch.backends.mps.is_available()
-    ):
+    elif torch.backends.mps.is_built() and torch.backends.mps.is_available():
         device = torch.device("mps")
     else:
         device = torch.device("cpu")
     return device
 
 
 T = TypeVar("T")
@@ -282,14 +279,17 @@
         Dict[str, float]: a dict that maps cpu stats to their values.
 
         Keys:
 
             - 'cpu_vm_percent'
             - 'cpu_percent'
             - 'cpu_swap_percent'
+            - 'worker_cpu_time_user'
+            - 'worker_cpu_time_system'
+            - 'worker_rss'
     """
     try:
         import psutil
     except ModuleNotFoundError:
         raise ModuleNotFoundError(
             "`get_cpu_process_metrics` requires `psutil` to be installed."
             " Install it by running `pip install -U psutil`."
@@ -308,24 +308,20 @@
     }
     return stats
 
 
 def collect_system_stats(device: torch.device) -> Dict[str, Any]:
     system_stats: Dict[str, Any] = {}
     cpu_stats = get_psutil_cpu_stats()
-
-    # pyre-fixme
-    system_stats.update(cpu_stats)
+    system_stats.update(**cpu_stats)
 
     if torch.cuda.is_available():
         try:
             gpu_stats = get_nvidia_smi_gpu_stats(device)
-
-            # pyre-fixme
-            system_stats.update(gpu_stats)
+            system_stats.update(**gpu_stats)
             system_stats.update(torch.cuda.memory_stats())
         except FileNotFoundError:
             logger.warning("Unable to find nvidia-smi. Skipping GPU stats collection.")
 
     return system_stats
 
 
@@ -335,18 +331,15 @@
     For more information, see the PyTorch docs:
     - https://pytorch.org/docs/stable/generated/torch.set_float32_matmul_precision.html
     - https://pytorch.org/docs/stable/backends.html#torch.backends.cudnn.allow_tf32
 
     Args:
         precision: The setting to determine which datatypes to use for matrix multiplication and convolution operations.
     """
-    if not (
-        torch.cuda.is_available()  # Not relevant for non-CUDA devices
-        and is_torch_version_geq_1_12()  # API exposed from PyTorch 1.12 onward
-    ):
+    if not (torch.cuda.is_available()):  # Not relevant for non-CUDA devices
         return
     # set precision for matrix multiplications
     torch.set_float32_matmul_precision(precision)
     # set precision for convolution operations
     if precision == "highest":
         torch.backends.cudnn.allow_tf32 = False
     else:
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/distributed.py` & `torchtnt-0.2.4/torchtnt/utils/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 
 import os
 import tempfile
 from dataclasses import dataclass
 from datetime import timedelta
 from functools import wraps
 from typing import Any, Callable, cast, Dict, List, Optional, TypeVar, Union
@@ -517,73 +519,112 @@
     port: str
     world_size: int
 
 
 def spawn_multi_process(
     world_size: int,
     backend: str,
-    test_method: Callable[TParams, TReturn],
-    *test_method_args: Any,
-    **test_method_kwargs: Any,
+    method: Callable[TParams, TReturn],
+    *method_args: Any,
+    **method_kwargs: Any,
 ) -> List[TReturn]:
     """
     Spawn single node, multi-rank function.
     Uses localhost and free port to communicate.
 
     Args:
         world_size: number of processes
         backend: backend to use. for example, "nccl", "gloo", etc
-        test_method: callable to spawn. first 3 arguments are rank, world_size and mp output dict
-        test_method_args: args for the test method
-        test_method_kwargs: kwargs for the test method
+        method: callable to spawn.
+        method_args: args for the method
+        method_kwargs: kwargs for the method
 
     Returns:
-        A list, l, where l[i] is the return value of test_method on rank i
+        A list, l, where l[i] is the return value of method(*method_args, **methods_kwargs) on rank i
     """
     manager = multiprocessing.Manager()
     mp_output_dict = manager.dict()
 
     port = str(get_free_port())
     torch.multiprocessing.spawn(
         # torch.multiprocessing.spawn sends rank as the first param
         # https://pytorch.org/docs/stable/multiprocessing.html#torch.multiprocessing.spawn
-        _init_pg_and_rank_and_launch_test,
+        _init_pg_and_rank_and_launch_method,
         args=(
             ProcessGroupSetupParams(backend=backend, port=port, world_size=world_size),
             mp_output_dict,
-            test_method,
-            test_method_args,
-            test_method_kwargs,
+            method,
+            method_args,
+            method_kwargs,
         ),
         nprocs=world_size,
     )
 
     output_list = []
     for i in range(world_size):
         output_list.append(mp_output_dict[i])
 
     return output_list
 
 
-def _init_pg_and_rank_and_launch_test(
+def _init_pg_and_rank_and_launch_method(
     rank: int,
     pg_setup_params: ProcessGroupSetupParams,
     mp_output_dict: Dict[int, object],
-    test_method: Callable[TParams, TReturn],
+    method: Callable[TParams, TReturn],
     args: List[object],
     kwargs: Dict[str, object],
 ) -> None:
     os.environ["MASTER_ADDR"] = "localhost"
     os.environ["MASTER_PORT"] = pg_setup_params.port
     os.environ["WORLD_SIZE"] = str(pg_setup_params.world_size)
     os.environ["LOCAL_RANK"] = str(rank)
     dist.init_process_group(
         rank=rank,
         world_size=pg_setup_params.world_size,
         backend=pg_setup_params.backend,
-        timeout=timedelta(seconds=10),  # setting up timeout for distributed collectives
+        timeout=timedelta(seconds=60),  # setting up timeout for distributed collectives
     )
     try:
-        mp_output_dict[rank] = test_method(*args, **kwargs)  # pyre-fixme
+        # pyre-ignore: spawn_multi_process uses unsafe types to begin with
+        mp_output_dict[rank] = method(*args, **kwargs)
 
     finally:
         destroy_process_group()
+
+
+def rank_zero_read_and_broadcast(
+    func: Callable[..., T],
+) -> Callable[..., T]:
+    """
+    Decorator that ensures a function is only executed by rank 0 and returns the result to all ranks.
+
+    Note:
+        By default will use the global process group. To use a custom process group, `process_group` must be an arg to the function and passed as a keyword argument.
+    """
+
+    def wrapper(*args: Any, **kwargs: Any) -> T:
+        ret = None
+        rank = get_global_rank()
+        process_group = kwargs.pop("process_group", None)
+
+        # Do all filesystem reads from rank 0 only
+        if rank == 0:
+            ret = func(*args, **kwargs)
+
+        # If not running in a distributed setting, return as is
+        if not (dist.is_available() and dist.is_initialized()):
+            # we cast here to avoid type errors, since it is
+            # guaranteed the return value is of type T
+            return cast(T, ret)
+
+        # Otherwise, broadcast result from rank 0 to all ranks
+        pg = PGWrapper(process_group)
+        path_container = [ret]
+        pg.broadcast_object_list(path_container, 0)
+        val = path_container[0]
+
+        # we cast here to avoid type errors, since it is
+        # guaranteed the return value is of type T
+        return cast(T, val)
+
+    return wrapper
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/early_stop_checker.py` & `torchtnt-0.2.4/torchtnt/utils/early_stop_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Any, Callable, Dict, Optional, Union
 
 import torch
 from typing_extensions import final, Literal
 
 _log: logging.Logger = logging.getLogger(__name__)
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/env.py` & `torchtnt-0.2.4/torchtnt/utils/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 import os
 import random
 from datetime import timedelta
 from typing import Optional, Union
 
 import numpy as np
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/flops.py` & `torchtnt-0.2.4/torchtnt/utils/flops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # Flop count implementation based on
 # https://dev-discuss.pytorch.org/t/the-ideal-pytorch-flop-counter-with-torch-dispatch/505
 
 import logging
 import operator
 from collections import defaultdict
 from functools import reduce
 from numbers import Number
-from typing import Any, Callable, DefaultDict, Dict, List, Tuple
+from typing import Any, Callable, cast, DefaultDict, Dict, List, Tuple, TypeVar, Union
 
 import torch
 from torch.utils._python_dispatch import TorchDispatchMode
 from torch.utils._pytree import PyTree, tree_map
 
 aten: torch._ops._OpNamespace = torch.ops.aten
+T = TypeVar("T")
+InputType = Union[torch.Tensor, bool, Tuple[bool]]
 
 
-# pyre-fixme [2] we don't care the type in outputs
-def _matmul_flop_jit(inputs: Tuple[torch.Tensor], outputs: Tuple[Any]) -> Number:
+def _matmul_flop_jit(inputs: Tuple[torch.Tensor], _outputs: Tuple[Any]) -> Number:
     """
     Count flops for matmul.
     """
     # Inputs should be a list of length 2.
     # Inputs contains the shapes of two matrices.
     input_shapes = [v.shape for v in inputs]
     assert len(input_shapes) == 2, input_shapes
     assert input_shapes[0][-1] == input_shapes[1][-2], input_shapes
     flop = inputs[0].numel() * input_shapes[-1][-1]
     return flop
 
 
-# pyre-fixme [2] we don't care the type in outputs
-def _addmm_flop_jit(inputs: Tuple[torch.Tensor], outputs: Tuple[Any]) -> Number:
+def _addmm_flop_jit(inputs: Tuple[torch.Tensor], _outputs: Tuple[Any]) -> Number:
     """
     Count flops for fully connected layers.
     """
     # Count flop for nn.Linear
     # inputs is a list of length 3.
     input_shapes = [v.shape for v in inputs[1:3]]
     # input_shapes[0]: [batch size, input feature dimension]
@@ -49,33 +51,32 @@
     assert len(input_shapes[1]) == 2, input_shapes[1]
     batch_size, input_dim = input_shapes[0]
     output_dim = input_shapes[1][1]
     flops = batch_size * input_dim * output_dim
     return flops
 
 
-# pyre-fixme [2] we don't care the type in outputs
-def _bmm_flop_jit(inputs: Tuple[torch.Tensor], outputs: Tuple[Any]) -> Number:
+def _bmm_flop_jit(inputs: Tuple[torch.Tensor], _outputs: Tuple[Any]) -> Number:
     """
     Count flops for the bmm operation.
     """
     # Inputs should be a list of length 2.
     # Inputs contains the shapes of two tensor.
     assert len(inputs) == 2, len(inputs)
     input_shapes = [v.shape for v in inputs]
     n, c, t = input_shapes[0]
     d = input_shapes[-1][-1]
     flop = n * c * t * d
     return flop
 
 
 def _conv_flop_count(
-    x_shape: List[int],
-    w_shape: List[int],
-    out_shape: List[int],
+    x_shape: Union[torch.Size, List[int]],
+    w_shape: Union[torch.Size, List[int]],
+    out_shape: Union[torch.Size, List[int]],
     transposed: bool = False,
 ) -> Number:
     """
     Count flops for convolution. Note only multiplication is
     counted. Computation for addition and bias is ignored.
     Flops for a transposed convolution are calculated as
     flops = (x_shape[2:] * prod(w_shape) * batch_size).
@@ -94,54 +95,56 @@
         * reduce(operator.mul, w_shape, 1)
         * reduce(operator.mul, conv_shape, 1)
     )
     return flop
 
 
 def _conv_flop_jit(
-    inputs: Tuple[Any],  # pyre-fixme [2] the inputs can be union of Tensor/bool/Tuple
+    inputs: List[Union[torch.Tensor, bool, Tuple[bool]]],
     outputs: Tuple[torch.Tensor],
 ) -> Number:
     """
     Count flops for convolution.
     """
-    x: torch.Tensor = inputs[0]
-    w: torch.Tensor = inputs[1]
+    x: torch.Tensor = cast(torch.Tensor, inputs[0])
+    w: torch.Tensor = cast(torch.Tensor, inputs[1])
     x_shape, w_shape, out_shape = (x.shape, w.shape, outputs[0].shape)
-    transposed: bool = inputs[6]
+    transposed: bool = cast(bool, inputs[6])
 
     return _conv_flop_count(
         list(x_shape), list(w_shape), list(out_shape), transposed=transposed
     )
 
 
 def _transpose_shape(shape: torch.Size) -> List[int]:
     return [shape[1], shape[0]] + list(shape[2:])
 
 
-# pyre-fixme [2] the inputs can be union of Tensor/bool/Tuple & we don't care about outputs
-def _conv_backward_flop_jit(inputs: Tuple[Any], outputs: Tuple[Any]) -> Number:
-    grad_out_shape, x_shape, w_shape = [i.shape for i in inputs[:3]]
+def _conv_backward_flop_jit(
+    inputs: Tuple[Union[torch.Tensor, bool, Tuple[bool]]], outputs: Tuple[torch.Tensor]
+) -> Number:
+
+    grad_out_shape, x_shape, w_shape = [cast(torch.Tensor, i).shape for i in inputs[:3]]
     output_mask = inputs[-1]
     fwd_transposed = inputs[7]
     flop_count: Number = 0
 
-    if output_mask[0]:
+    if cast(Tuple[bool], output_mask)[0]:
         grad_input_shape = outputs[0].shape
         # pyre-fixme [58] this is actually sum of Number and Number
         flop_count = flop_count + _conv_flop_count(
             grad_out_shape, w_shape, grad_input_shape, not fwd_transposed
         )
-    if output_mask[1]:
+    if cast(Tuple[bool], output_mask)[1]:
         grad_weight_shape = outputs[1].shape
         flop_count += _conv_flop_count(
             list(_transpose_shape(x_shape)),
             list(grad_out_shape),
             list(grad_weight_shape),
-            fwd_transposed,
+            cast(bool, fwd_transposed),
         )
 
     return flop_count
 
 
 # pyre-fixme [5]
 flop_mapping: Dict[Callable[..., Any], Callable[[Tuple[Any], Tuple[Any]], Number]] = {
@@ -159,16 +162,15 @@
     aten.bmm.default: _bmm_flop_jit,
     aten.convolution.default: _conv_flop_jit,
     aten._convolution.default: _conv_flop_jit,
     aten.convolution_backward.default: _conv_backward_flop_jit,
 }
 
 
-# pyre-fixme [2, 3] it can be Tuple of anything.
-def _normalize_tuple(x: Any) -> Tuple[Any]:
+def _normalize_tuple(x: T) -> Tuple[T]:
     if not isinstance(x, tuple):
         return (x,)
     return x
 
 
 class FlopTensorDispatchMode(TorchDispatchMode):
     """
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/fsspec.py` & `torchtnt-0.2.4/torchtnt/utils/fsspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Any
 
 import fsspec
 from fsspec.core import url_to_fs
 
 
 def get_filesystem(path: str, **kwargs: Any) -> fsspec.AbstractFileSystem:
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/__init__.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from .csv import CSVLogger
 from .file import FileLogger
 from .in_memory import InMemoryLogger
 from .json import JSONLogger
 from .logger import MetricLogger, Scalar
 from .stdout import StdoutLogger
 from .tensorboard import TensorBoardLogger
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/csv.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import csv
 import logging
 from threading import Thread
 from typing import Dict, List, Optional
 
 from fsspec import open as fs_open
 from torchtnt.utils.loggers.file import FileLogger
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/file.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import atexit
 import logging
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from time import monotonic
 from typing import Dict, Mapping
 
@@ -85,13 +87,11 @@
             len(self._log_buffer) - self._len_before_flush
             >= self._steps_before_flushing
         ):
             self.flush()
             self._len_before_flush = len(self._log_buffer)
 
     @abstractmethod
-    def flush(self) -> None:
-        ...
+    def flush(self) -> None: ...
 
     @abstractmethod
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/in_memory.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/in_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import atexit
 import logging
 from collections import OrderedDict
 from time import monotonic
 from typing import Dict, Mapping
 
 from torchtnt.utils.loggers.logger import MetricLogger, Scalar
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/json.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/json.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import json
 import logging
 
 from fsspec import open as fs_open
 from torchtnt.utils.loggers.file import FileLogger
 from torchtnt.utils.loggers.logger import MetricLogger
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/logger.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Mapping, Union
 
 from numpy import ndarray
 from torch import Tensor
 from typing_extensions import Protocol
 
 Scalar = Union[Tensor, ndarray, int, float]
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/stdout.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/stdout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import atexit
 import logging
 import sys
 from typing import Mapping, Optional
 
 from torchtnt.utils.distributed import rank_zero_fn
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/tensorboard.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from __future__ import annotations
 
 import atexit
 import logging
-from typing import Any, Dict, List, Mapping, Optional, Union
-
-import torch.distributed as dist
+from typing import Any, Dict, Mapping, Optional, Union
 
 from torch.utils.tensorboard import SummaryWriter
-from torchtnt.utils.distributed import get_global_rank, PGWrapper
+from torchtnt.utils.distributed import get_global_rank
 from torchtnt.utils.loggers.logger import MetricLogger, Scalar
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TensorBoardLogger(MetricLogger):
     """
@@ -47,46 +47,29 @@
         logger = TensorBoardLogger(path="tmp/tb_logs")
         logger.log("accuracy", 23.56, 10)
         logger.close()
     """
 
     def __init__(self: TensorBoardLogger, path: str, *args: Any, **kwargs: Any) -> None:
         self._writer: Optional[SummaryWriter] = None
-
+        self._path: str = path
         self._rank: int = get_global_rank()
-        self._sync_path_to_workers(path)
 
         if self._rank == 0:
             logger.info(
                 f"TensorBoard SummaryWriter instantiated. Files will be stored in: {path}"
             )
             self._writer = SummaryWriter(log_dir=path, *args, **kwargs)
         else:
             logger.debug(
                 f"Not logging metrics on this host because env RANK: {self._rank} != 0"
             )
 
         atexit.register(self.close)
 
-    def _sync_path_to_workers(self: TensorBoardLogger, path: str) -> None:
-        if not (dist.is_available() and dist.is_initialized()):
-            self._path: str = path
-            return
-
-        pg = PGWrapper(dist.group.WORLD)
-        path_container: List[str] = [path] if self._rank == 0 else [""]
-        pg.broadcast_object_list(path_container, 0)
-        updated_path = path_container[0]
-        if updated_path != path:
-            # because the logger only logs on rank 0, if users pass in a different path
-            # the logger will output the wrong `path` property, so we update it to match
-            # the correct path.
-            logger.info(f"Updating TensorBoard path to match rank 0: {updated_path}")
-        self._path: str = updated_path
-
     @property
     def writer(self: TensorBoardLogger) -> Optional[SummaryWriter]:
         return self._writer
 
     @property
     def path(self: TensorBoardLogger) -> str:
         return self._path
@@ -161,14 +144,25 @@
             *args (Any): Positional arguments passed to SummaryWriter.add_images
             **kwargs(Any): Keyword arguments passed to SummaryWriter.add_images
         """
         writer = self._writer
         if writer:
             writer.add_images(*args, **kwargs)
 
+    def log_figure(self: TensorBoardLogger, *args: Any, **kwargs: Any) -> None:
+        """Add matplotlib figure to TensorBoard.
+
+        Args:
+            *args (Any): Positional arguments passed to SummaryWriter.add_figure
+            **kwargs(Any): Keyword arguments passed to SummaryWriter.add_figure
+        """
+        writer = self._writer
+        if writer:
+            writer.add_figure(*args, **kwargs)
+
     def log_audio(self: TensorBoardLogger, *args: Any, **kwargs: Any) -> None:
         """Add audio data to TensorBoard.
 
         Args:
             *args (Any): Positional arguments passed to SummaryWriter.add_audio
             **kwargs (Any): Keyword arguments passed to SummaryWriter.add_audio
         """
@@ -196,14 +190,24 @@
             self._writer.add_scalars(
                 main_tag=main_tag,
                 tag_scalar_dict=tag_scalar_dict,
                 global_step=global_step,
                 walltime=walltime,
             )
 
+    def log_histogram(self: TensorBoardLogger, *args: Any, **kwargs: Any) -> None:
+        """Add histogram to TensorBoard.
+
+        Args:
+            *args (Any): Positional arguments passed to SummaryWriter.add_histogram
+            **kwargs(Any): Keyword arguments passed to SummaryWriter.add_histogram
+        """
+        if self._writer:
+            self._writer.add_histogram(*args, **kwargs)
+
     def flush(self: TensorBoardLogger) -> None:
         """Writes pending logs to disk."""
 
         if self._writer:
             self._writer.flush()
 
     def close(self: TensorBoardLogger) -> None:
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/loggers/utils.py` & `torchtnt-0.2.4/torchtnt/utils/loggers/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from numpy import ndarray
 from torch import Tensor
 from torchtnt.utils.loggers.logger import Scalar
 
 
 def scalar_to_float(scalar: Scalar) -> float:
     if isinstance(scalar, Tensor):
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/memory.py` & `torchtnt-0.2.4/torchtnt/utils/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import time
 from collections import deque
 from contextlib import contextmanager
 from datetime import timedelta
 from enum import Enum
 from threading import Event, Thread
-from typing import Any, Dict, Generator, List, Mapping, Sequence, Tuple
+from typing import Dict, Generator, List, Mapping, Sequence, Tuple
 
 import psutil
 import torch
 
 _DEFAULT_MEASURE_INTERVAL = timedelta(milliseconds=100)
 
 
 def _is_named_tuple(
-    # pyre-fixme: Missing parameter annotation [2]: Parameter `x` must have a type other than `Any`.
-    x: Any,
+    x: object,
 ) -> bool:
     return isinstance(x, tuple) and hasattr(x, "_asdict") and hasattr(x, "_fields")
 
 
 def get_tensor_size_bytes_map(
-    # pyre-fixme: Missing parameter annotation [2]: Parameter `obj` must have a type other than `Any`.
-    obj: Any,
+    obj: object,
 ) -> Dict[torch.Tensor, int]:
     tensor_map = {}
     attributes_q = deque()
     attributes_q.append(obj)
     while attributes_q:
         attribute = attributes_q.popleft()
         if isinstance(attribute, torch.Tensor):
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/memory_snapshot_profiler.py` & `torchtnt-0.2.4/torchtnt/utils/memory_snapshot_profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from types import TracebackType
 from typing import Optional, Type
 
 import torch
 from torchtnt.utils.oom import attach_oom_observer, log_memory_snapshot
-from torchtnt.utils.version import is_torch_version_geq_2_0
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
 class MemorySnapshotParams:
     """
@@ -53,24 +54,21 @@
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         tb: Optional[TracebackType],
     ) -> Optional[bool]:
         self.stop()
 
     @abstractmethod
-    def start(self) -> None:
-        ...
+    def start(self) -> None: ...
 
     @abstractmethod
-    def stop(self) -> None:
-        ...
+    def stop(self) -> None: ...
 
     @abstractmethod
-    def step(self) -> None:
-        ...
+    def step(self) -> None: ...
 
 
 class MemorySnapshotProfiler(MemorySnapshotProfilerBase):
     """
     Records a history of memory allocation and free events, and dumps to a
     file which can be visualized offline. It by default keeps track of
     100000 events, and dumps at user specified step as well as on OOM.
@@ -128,49 +126,57 @@
             and not self.params.enable_oom_observer
         ):
             raise ValueError(
                 "At least one of start_step/stop_step or enable_oom_observer must be set."
             )
 
         self.step_num: int = 0
+        self.is_started: bool = False
 
-        if not is_torch_version_geq_2_0():
-            raise RuntimeError("CUDA memory snapshot requires torch>=2.0")
         if self.params.enable_oom_observer:
             attach_oom_observer(
                 output_dir=output_dir, trace_max_entries=self.params.max_entries
             )
         if start_step is not None and start_step == 0:
             self.start()
 
         logger.info(
             f"Created MemorySnapshotProfiler with MemorySnapshotParams={self.params}."
         )
 
     def start(self) -> None:
+        if self.is_started:
+            return
         if not torch.cuda.is_available():
             logger.warn("CUDA unavailable. Not recording memory history.")
             return
 
         logger.info("Starting to record memory history.")
         torch.cuda.memory._record_memory_history(max_entries=self.params.max_entries)
+        self.is_started = True
 
     def stop(self) -> None:
+        if not self.is_started:
+            return
         if not torch.cuda.is_available():
             logger.warn("CUDA unavailable. Not recording memory history.")
             return
 
         logger.info("Stopping recording memory history.")
         torch.cuda.memory._record_memory_history(enabled=None)
+        self.is_started = False
 
     def step(self) -> None:
         self.step_num += 1
         if (
             self.params.start_step is not None
             and self.step_num == self.params.start_step
         ):
             self.start()
         if self.params.stop_step is not None and self.step_num == self.params.stop_step:
-            log_memory_snapshot(
-                output_dir=self.output_dir, file_prefix=f"step_{self.step_num}"
-            )
+            self.log_memory_snapshot()
             self.stop()
+
+    def log_memory_snapshot(self) -> None:
+        log_memory_snapshot(
+            output_dir=self.output_dir, file_prefix=f"step_{self.step_num}"
+        )
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/misc.py` & `torchtnt-0.2.4/torchtnt/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Optional
 
 import torch
 
 _SEC_IN_DAY: int = 60 * 60 * 24
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/module_summary.py` & `torchtnt-0.2.4/torchtnt/utils/module_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import copy
 import math
 import warnings
 from collections import defaultdict, deque
 from dataclasses import dataclass, field
 from enum import Enum
 from time import perf_counter
@@ -24,16 +26,16 @@
     Union,
 )
 
 import torch
 from torch.nn.parameter import UninitializedParameter
 from torch.utils._pytree import PyTree, tree_flatten
 from torch.utils.hooks import RemovableHandle
+from torchtnt.utils.flops import FlopTensorDispatchMode
 
-from torchtnt.utils.version import is_torch_version_geq_1_13
 from typing_extensions import Literal
 
 _ATTRIB_TO_COL_HEADER = {
     "module_name": "Name",
     "module_type": "Type",
     "num_parameters": "# Parameters",
     "num_trainable_parameters": "# Trainable Parameters",
@@ -238,43 +240,33 @@
 
     module.zero_grad()
 
     module_args = module_args or ()
     module_kwargs = module_kwargs or {}
     flops_forward = None
     flops_backward = None
-    if not is_torch_version_geq_1_13():
-        warnings.warn(
-            "Please install PyTorch 1.13 or higher to compute FLOPs: https://pytorch.org/get-started/locally/"
-        )
-        module(*module_args, **module_kwargs)
+
+    with FlopTensorDispatchMode(module) as ftdm:
+        # Count for forward flops (+ compute activation sizes)
+        res = module(*module_args, **module_kwargs)
+
         # detach activation size hook handles
         for hook_handle in activation_size_handles:
             hook_handle.remove()
-    else:
-        from torchtnt.utils.flops import FlopTensorDispatchMode
 
-        with FlopTensorDispatchMode(module) as ftdm:
-            # Count for forward flops (+ compute activation sizes)
-            res = module(*module_args, **module_kwargs)
-
-            # detach activation size hook handles
-            for hook_handle in activation_size_handles:
-                hook_handle.remove()
-
-            flops_forward = copy.deepcopy(ftdm.flop_counts)
-            if isinstance(res, torch.Tensor):
-                # Count for backward flops
-                ftdm.reset()
-                res.mean().backward()
-                flops_backward = copy.deepcopy(ftdm.flop_counts)
-            else:
-                warnings.warn(
-                    "Backward FLOPs are only computed if module foward returns a tensor."
-                )
+        flops_forward = copy.deepcopy(ftdm.flop_counts)
+        if isinstance(res, torch.Tensor):
+            # Count for backward flops
+            ftdm.reset()
+            res.mean().backward()
+            flops_backward = copy.deepcopy(ftdm.flop_counts)
+        else:
+            warnings.warn(
+                "Backward FLOPs are only computed if module foward returns a tensor."
+            )
 
     # remove forward time elapsed handles
     for hook_handle in forward_elapsed_time_handles:
         hook_handle.remove()
 
     # convert module timings to ms
     forward_time_elapsed_ms = {}
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/oom.py` & `torchtnt-0.2.4/torchtnt/utils/oom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 import os
 import pickle
 from typing import Any, Callable, Dict, Optional, Union
 
 import torch
 from torchtnt.utils.distributed import get_global_rank
 from torchtnt.utils.fsspec import get_filesystem
-from torchtnt.utils.version import is_torch_version_geq_2_0
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def is_out_of_cpu_memory(exception: BaseException) -> bool:
     """Returns True if the exception is related to CPU OOM"""
     return (
@@ -84,19 +85,14 @@
 
     Note:
         Outputs are only saved if running on a host with CUDA devices available.
     """
     if not torch.cuda.is_available():
         logger.info("CUDA unavailable. Not logging snapshot")
         return
-    if not is_torch_version_geq_2_0():
-        logger.warning(
-            "CUDA memory snapshot utilities are unavailable. Not logging snapshot"
-        )
-        return
 
     rank = get_global_rank()
     if file_prefix is None:
         file_prefix = "memory_snapshot"
     save_dir = os.path.join(output_dir, f"{file_prefix}_rank{rank}")
     try:
         snapshot = torch.cuda.memory._snapshot()
@@ -128,19 +124,14 @@
 
     Note:
         Outputs are only saved if running on a host with CUDA devices available.
     """
     if not torch.cuda.is_available():
         logger.info("CUDA unavailable. Not attaching OOM observer.")
         return
-    if not is_torch_version_geq_2_0():
-        logger.warning(
-            "CUDA memory snapshot utilities are unavailable. Not attaching OOM observer."
-        )
-        return
 
     torch.cuda.memory._record_memory_history(
         enabled="all", max_entries=trace_max_entries
     )
-    # pyre-fixme[16]: Module `_C` has no attribute
+    # pyre-ignore[16]: Module `_C` has no attribute
     #  `_cuda_attach_out_of_memory_observer`.
     torch._C._cuda_attach_out_of_memory_observer(_oom_observer(output_dir))
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/optimizer.py` & `torchtnt-0.2.4/torchtnt/utils/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Dict
 
 import torch
 
 
 def init_optim_state(optimizer: torch.optim.Optimizer) -> None:
     """
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/precision.py` & `torchtnt-0.2.4/torchtnt/utils/precision.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Mapping, Optional
 
 import torch
-from torch.cuda.amp.grad_scaler import GradScaler
-from torchtnt.utils.prepare_module import _is_fsdp_module
+from torch.cuda.amp.grad_scaler import GradScaler as CudaGradScaler
+
+try:
+    from torch.amp.grad_scaler import GradScaler
+except Exception:
+    GradScaler = CudaGradScaler
 
 _DTYPE_STRING_TO_DTYPE_MAPPING: Mapping[str, Optional[torch.dtype]] = {
     "fp16": torch.float16,
     "bf16": torch.bfloat16,
     "fp32": None,
 }
 
@@ -33,29 +39,29 @@
         raise ValueError(
             f"Precision {precision} not supported. Please use one of {list(_DTYPE_STRING_TO_DTYPE_MAPPING.keys())}"
         )
     return _DTYPE_STRING_TO_DTYPE_MAPPING[precision]
 
 
 def get_grad_scaler_from_precision(
-    precision: torch.dtype, module: torch.nn.Module
-) -> Optional[torch.amp.GradScaler]:
+    precision: torch.dtype, *, is_fsdp_module: Optional[bool] = False
+) -> Optional[GradScaler]:
     """
     Returns the correct grad scaler to use based on the precision and whether
     or not the model is FSDP.
 
     Args:
         precision: the precision being used
-        module: the module being trained
+        is_fsdp_module: whether the grad scaler is for an FSDP module
 
     Returns:
         The appropriate grad scaler to use, ``None`` if no grad scaler should be used.
     """
 
     if precision == torch.float16:
-        if _is_fsdp_module(module):
+        if is_fsdp_module:
             from torch.distributed.fsdp.sharded_grad_scaler import ShardedGradScaler
 
             return ShardedGradScaler()
         else:
-            return GradScaler()
+            return CudaGradScaler()
     return None
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/prepare_module.py` & `torchtnt-0.2.4/torchtnt/utils/prepare_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from dataclasses import asdict, dataclass
 from functools import partial
-from typing import Any, Callable, Dict, Iterable, Optional, Union
+from typing import Any, Callable, cast, Dict, Iterable, Optional, Union
 
 import torch
 import torch.distributed as dist
 from torch.distributed import ProcessGroup
-from torch.distributed.fsdp import FullyShardedDataParallel as FSDP, StateDictType
+
+from torch.distributed._composable_state import _get_module_state
+from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
+    apply_activation_checkpointing,
+    checkpoint_wrapper,
+    CheckpointImpl,
+)
+from torch.distributed.fsdp import (
+    FullyShardedDataParallel as FSDP,
+    StateDictType as _StateDictType,
+)
+from torch.distributed.fsdp._common_utils import _FSDPState
 from torch.distributed.fsdp.api import OptimStateDictConfig, StateDictConfig
 from torch.distributed.fsdp.fully_sharded_data_parallel import (
-    BackwardPrefetch,
+    BackwardPrefetch as _BackwardPrefetch,
     CPUOffload,
+    MixedPrecision as _MixedPrecision,
+    ShardingStrategy as _ShardingStrategy,
+)
+from torch.nn.parallel import DistributedDataParallel as DDP
+from torchtnt.utils.fsdp_utils import (
+    BackwardPrefetch,
     MixedPrecision,
     ShardingStrategy,
+    StateDictType,
 )
-from torch.nn.parallel import DistributedDataParallel as DDP
-from torchtnt.utils.rank_zero_log import rank_zero_warn
-from torchtnt.utils.version import is_torch_version_geq_1_12, is_torch_version_geq_2_0
 
-if is_torch_version_geq_2_0():
-    from torch.distributed._composable_state import _get_module_state
-    from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
-        apply_activation_checkpointing,
-        checkpoint_wrapper,
-        CheckpointImpl,
-    )
-    from torch.distributed.fsdp._common_utils import _FSDPState
+from torchtnt.utils.rank_zero_log import rank_zero_warn
+from torchtnt.utils.version import is_torch_version_geq
 
 
 @dataclass
 class Strategy:
     """Dataclass representing a parallelization strategy"""
 
     pass
@@ -81,42 +92,63 @@
 
 
 @dataclass
 class FSDPStrategy(Strategy):
     """Dataclass representing the `FullyShardedDataParallel <https://pytorch.org/docs/stable/fsdp.html>`_ strategy"""
 
     process_group: Optional[ProcessGroup] = None
-    sharding_strategy: Optional[ShardingStrategy] = None
+    sharding_strategy: Optional[Union[str, _ShardingStrategy]] = None
     cpu_offload: Optional[CPUOffload] = None
     auto_wrap_policy: Optional[Callable[[torch.nn.Module, bool, int], bool]] = None
-    backward_prefetch: Optional[BackwardPrefetch] = BackwardPrefetch.BACKWARD_PRE
-    mixed_precision: Optional[MixedPrecision] = None
+    backward_prefetch: Optional[Union[str, _BackwardPrefetch]] = (
+        _BackwardPrefetch.BACKWARD_PRE
+    )
+    mixed_precision: Optional[Union[_MixedPrecision, MixedPrecision]] = None
     ignored_modules: Optional[Iterable[torch.nn.Module]] = None
     param_init_fn: Optional[Callable[[torch.nn.Module], None]] = None
     sync_module_states: bool = False
     forward_prefetch: bool = False
     limit_all_gathers: bool = True
     use_orig_params: bool = False
 
     # FSDP set_state_dict_type params: https://pytorch.org/docs/stable/fsdp.html#torch.distributed.fsdp.FullyShardedDataParallel.set_state_dict_type
     # for setting type of state dict for checkpointing
-    state_dict_type: Optional[StateDictType] = None
+    state_dict_type: Optional[Union[str, _StateDictType]] = None
     state_dict_config: Optional[StateDictConfig] = None
     optim_state_dict_config: Optional[OptimStateDictConfig] = None
 
+    def __post_init__(self) -> None:
+        if isinstance(self.sharding_strategy, str):
+            self.sharding_strategy = ShardingStrategy.to_native_sharding_strategy(
+                self.sharding_strategy
+            )
+
+        if isinstance(self.backward_prefetch, str):
+            self.backward_prefetch = BackwardPrefetch.to_native_backward_prefetch(
+                self.backward_prefetch
+            )
+
+        if isinstance(self.state_dict_type, str):
+            self.state_dict_type = StateDictType.to_native_state_dict_type(
+                self.state_dict_type
+            )
+
+        if isinstance(self.mixed_precision, MixedPrecision):
+            self.mixed_precision = self.mixed_precision.to_native_mixed_precision()
+
 
 @dataclass
 class TorchCompileParams:
     """
     Dataclass to store parameters for torch compile. See https://pytorch.org/docs/stable/generated/torch.compile.html for details.
     """
 
     fullgraph: bool = False
     dynamic: bool = False
-    # pyre-fixme: Invalid type parameters [24]
+    # pyre-ignore: Invalid type parameters. Uses PyTorch types.
     backend: Union[str, Callable] = "inductor"
     mode: Union[str, None] = None
     options: Optional[Dict[str, Union[str, int, bool]]] = None
     disable: bool = False
 
 
 @dataclass
@@ -196,18 +228,14 @@
 
     Examples::
         strategy = FSDPStrategy(limit_all_gathers=True)
         module = nn.Linear(1, 1)
         device = torch.device("cuda")
         fsdp_module = prepare_fsdp(module, device, strategy)
     """
-    if not is_torch_version_geq_1_12():
-        raise RuntimeError(
-            "Please install PyTorch 1.12 or higher to use FSDP: https://pytorch.org/get-started/locally/"
-        )
     strategy = strategy if strategy is not None else FSDPStrategy()
 
     # we use __dict__ and not asdict() here because asdict() is recursively applied on nested objects
     params_dict = strategy.__dict__.copy()
 
     # extract params to set state dict type
     state_dict_type = params_dict.pop("state_dict_type")
@@ -250,65 +278,81 @@
         self.optimizer.load_state_dict(optim_state_dict)
 
 
 def _is_fsdp_module(module: torch.nn.Module) -> bool:
     if isinstance(module, FSDP):
         return True
 
-    if is_torch_version_geq_2_0():
-        # Also check for composable FSDP API
-        maybe_composable_state = _get_module_state(module)
-        if maybe_composable_state is not None:
-            return isinstance(maybe_composable_state, _FSDPState)
+    # Also check for composable FSDP API
+    maybe_composable_state = _get_module_state(module)
+    if maybe_composable_state is not None:
+        return isinstance(maybe_composable_state, _FSDPState)
 
     return False
 
 
 def prepare_module(
     module: torch.nn.Module,
     device: torch.device,
     *,
     strategy: Optional[Union[Strategy, str]] = None,
     torch_compile_params: Optional[TorchCompileParams] = None,
     activation_checkpoint_params: Optional[ActivationCheckpointParams] = None,
+    enable_compiled_autograd: bool = False,
 ) -> torch.nn.Module:
     """
     Utility to move a module to device, set up parallelism, activation checkpointing and compile.
 
     Args:
         module: module to be used.
         device: device to which module will be moved.
         strategy: the data parallelization strategy to be used. if a string, must be one of ``ddp``, ``fsdp``, or ``noop``.
         torch_compile_params: params for Torch compile https://pytorch.org/docs/stable/generated/torch.compile.html.
         activation_checkpoint_params: params for enabling activation checkpointing.
+        enable_compiled_autograd: if True, `compiled_autograd` will be used to compile the backward, this is an experimental flag.
     """
 
     if strategy:
         if isinstance(strategy, str):
             strategy = convert_str_to_strategy(strategy)
         if isinstance(strategy, DDPStrategy):
-            if torch_compile_params and strategy.static_graph is True:
-                # https://dev-discuss.pytorch.org/t/torchdynamo-update-9-making-ddp-work-with-torchdynamo/860
+            if (
+                torch_compile_params
+                and strategy.static_graph is True
+                and not is_torch_version_geq("2.1.0")
+            ):
                 raise RuntimeError(
-                    "Torch compile requires DDPStrategy's static_graph to be False"
+                    "Torch version >= 2.1.0 required for Torch compile + DDP with static graph"
                 )
+
+            if enable_compiled_autograd:
+                if not torch_compile_params:
+                    raise RuntimeError(
+                        "Compiled autograd should only be used when the module is compiled."
+                    )
+                try:
+                    from torch._dynamo.trace_rules import LEGACY_MOD_INLINELIST
+
+                    LEGACY_MOD_INLINELIST.add("torch.nn.parallel.distributed")
+                except ImportError:
+                    pass
+                # This has to be set before DDP wrapping
+                torch._dynamo.config.optimize_ddp = "python_reducer"
             module = prepare_ddp(module, device, strategy)
         elif isinstance(strategy, FSDPStrategy):
             if torch_compile_params and strategy.use_orig_params is False:
                 # as stated here https://pytorch.org/get-started/pytorch-2.0/
                 raise RuntimeError(
                     "Torch compile requires FSDPStrategy's use_orig_params to be True, since AOTAutograd needs to be aware of the original parameters"
                 )
             module = prepare_fsdp(module, device, strategy)
     else:
         module = module.to(device)
 
     if activation_checkpoint_params:
-        if not is_torch_version_geq_2_0():
-            raise RuntimeError("Activation checkpointing requires torch>=2.0")
         checkpoint_impl = activation_checkpoint_params.checkpoint_impl
         check_fn = activation_checkpoint_params.check_fn
         auto_wrap_policy = activation_checkpoint_params.auto_wrap_policy
         custom_checkpoint_wrapper = partial(
             checkpoint_wrapper,
             checkpoint_impl=checkpoint_impl,
         )
@@ -323,15 +367,17 @@
         try:
             # use in-place compile to avoid altering the state_dict keys
             module.compile(**asdict(torch_compile_params))
         except AttributeError:
             rank_zero_warn(
                 "Please install PyTorch nightlies to use in-place compile to avoid altering the state_dict keys when checkpointing."
             )
-            torch.compile(module, **asdict(torch_compile_params))
+            return cast(
+                torch.nn.Module, torch.compile(module, **asdict(torch_compile_params))
+            )
 
     return module
 
 
 def convert_str_to_strategy(
     strategy: str,
 ) -> Union[DDPStrategy, FSDPStrategy, NOOPStrategy]:
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/progress.py` & `torchtnt-0.2.4/torchtnt/utils/progress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from collections.abc import Sized
 from typing import Any, Dict, Iterable, Optional
 
 
 class Progress:
     """Class to track progress during the loop. Includes state_dict/load_state_dict for convenience for checkpointing."""
 
@@ -56,14 +58,17 @@
 
     def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
         """Restores a Progress instance from a state_dict in accordance with Stateful protocol."""
         self._num_epochs_completed = state_dict["num_epochs_completed"]
         self._num_steps_completed = state_dict["num_steps_completed"]
         self._num_steps_completed_in_epoch = state_dict["num_steps_completed_in_epoch"]
 
+    def get_progress_string(self) -> str:
+        return f"completed epochs: {self.num_epochs_completed}, completed steps: {self.num_steps_completed}, completed steps in current epoch: {self.num_steps_completed_in_epoch}."
+
 
 def estimated_steps_in_epoch(
     dataloader: Iterable[object],
     *,
     num_steps_completed: int,
     max_steps: Optional[int],
     max_steps_per_epoch: Optional[int],
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/rank_zero_log.py` & `torchtnt-0.2.4/torchtnt/utils/rank_zero_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 from typing import Any, Optional
 
 from packaging.version import Version
 
 from torchtnt.utils.distributed import get_global_rank
 from torchtnt.utils.version import get_python_version
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/stateful.py` & `torchtnt-0.2.4/torchtnt/utils/stateful.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Any, Dict, Union
 
 import torch
 from torchtnt.utils.lr_scheduler import TLRScheduler
 from torchtnt.utils.prepare_module import FSDPOptimizerWrapper
 from torchtnt.utils.progress import Progress
 
 from typing_extensions import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class Stateful(Protocol):
     """Defines the interface for checkpoint saving and loading."""
 
-    def state_dict(self) -> Dict[str, Any]:
-        ...
+    def state_dict(self) -> Dict[str, Any]: ...
 
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        ...
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None: ...
 
 
 StatefulDict = Dict[str, Stateful]
 ModuleDict = Dict[str, torch.nn.Module]
 OptimizerAndLRSchedulerDict = Dict[
     str, Union[TLRScheduler, torch.optim.Optimizer, FSDPOptimizerWrapper]
 ]
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/swa.py` & `torchtnt-0.2.4/torchtnt/utils/swa.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Callable, List, Literal, Optional
 
 import torch
 
-# TODO: torch/optim/swa_utils.pyi needs to be updated
-# pyre-fixme Undefined import [21]: Could not find a name `get_ema_multi_avg_fn` defined in module `torch.optim.swa_utils`.
-from torch.optim.swa_utils import (
-    AveragedModel as PyTorchAveragedModel,
-    get_ema_multi_avg_fn,
-    get_swa_multi_avg_fn,
-)
+_AVERAGED_MODEL_AVAIL: bool = True
+
+try:
+    from torch.optim.swa_utils import (
+        AveragedModel as PyTorchAveragedModel,
+        get_ema_multi_avg_fn,
+        get_swa_multi_avg_fn,
+    )
+except ImportError:
+    _AVERAGED_MODEL_AVAIL = False
+
 
 TSWA_avg_fn = Callable[[torch.Tensor, torch.Tensor, int], torch.Tensor]
 TSWA_multi_avg_fn = Callable[[List[torch.Tensor], List[torch.Tensor], int], None]
 
 
 class AveragedModel(PyTorchAveragedModel):
     def __init__(
@@ -45,25 +51,27 @@
                 is only needed for EMA, and is ignored otherwise (for SWA).
             skip_deepcopy: If True, will skip the deepcopy step. The user must ensure
                 that the module passed in is already copied in someway
             use_lit: If True, will use Lit EMA style by adjusting weight decay based on the
                 number of updates. The EMA decay will start small and will approach the
                 specified ema_decay as more updates occur.
         """
+        if not _AVERAGED_MODEL_AVAIL:
+            raise ImportError(
+                "AveragedModel is not available in this version of PyTorch. \
+                Please install the latest version of PyTorch."
+            )
+
         # setup averaging method
         if averaging_method == "ema":
             if ema_decay < 0.0 or ema_decay > 1.0:
                 raise ValueError(f"Decay must be between 0 and 1, got {ema_decay}")
 
-            # TODO: torch/optim/swa_utils.pyi needs to be updated
-            # pyre-fixme Undefined attribute [16]: Module `torch.optim.swa_utils` has no attribute `get_ema_multi_avg_fn`.
             multi_avg_fn = get_ema_multi_avg_fn(ema_decay)
         elif averaging_method == "swa":
-            # TODO: torch/optim/swa_utils.pyi needs to be updated
-            # pyre-fixme Undefined attribute [16]: Module `torch.optim.swa_utils` has no attribute `get_swa_multi_avg_fn`.
             multi_avg_fn = get_swa_multi_avg_fn()
 
             if use_lit:
                 raise ValueError("LitEMA is only supported for EMA.")
         else:
             raise ValueError(
                 f"Unknown averaging method: {averaging_method}. Only ema and swa are supported."
@@ -83,27 +91,23 @@
             )
             self.avg_fn: Optional[TSWA_avg_fn] = None
             self.multi_avg_fn: Optional[TSWA_multi_avg_fn] = multi_avg_fn
             self.use_buffers: bool = use_buffers
         else:
             # use default init implementation
 
-            # TODO: torch/optim/swa_utils.pyi needs to be updated
-            # pyre-fixme Unexpected keyword [28]
             super().__init__(
                 model,
                 device=device,
                 multi_avg_fn=multi_avg_fn,
                 use_buffers=use_buffers,
             )
 
     def update_parameters(self, model: torch.nn.Module) -> None:
         self._num_updates += 1
         if self._use_lit:
             decay = min(
                 self._ema_decay, (1 + self._num_updates) / (10 + self._num_updates)
             )
 
-            # TODO: torch/optim/swa_utils.pyi needs to be updated
-            # pyre-fixme Undefined attribute [16]: Module `torch.optim.swa_utils` has no attribute `get_ema_multi_avg_fn`.
             self.multi_avg_fn = get_ema_multi_avg_fn(decay)
         super().update_parameters(model)
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/test_utils.py` & `torchtnt-0.2.4/torchtnt/utils/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import ctypes
 import sys
 import unittest
 import uuid
 from contextlib import contextmanager
 from functools import wraps
 from io import StringIO
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/timer.py` & `torchtnt-0.2.4/torchtnt/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import datetime
 import logging
 import os
 from collections import defaultdict
 from contextlib import contextmanager
 from time import perf_counter
 from typing import (
@@ -101,17 +103,14 @@
     ) -> None:
         """
         A Timer class which implements TimerProtocol and stores timings in a dictionary `recorded_durations`.
 
         Args:
             cuda_sync: whether to call torch.cuda.synchronize() before and after timing. Defaults to True if CUDA is available.
             verbose: whether to enable verbose logging.
-            size_bounds: defines the range of samples that should be kept in the timer. The lower bound should be smaller than
-                the upper bound. When the number of samples reaches the upper bound, the oldest (upper-lower) bound samples will
-                be removed. This range is applied per action.
 
         Note:
             Enabling cuda_sync will incur a performance hit, but will ensure accurate timings on GPUs.
 
         Raises:
             ValueError: If cuda_sync is set to True but CUDA is not available.
 
@@ -360,15 +359,16 @@
 
     pg_wrapper = PGWrapper(pg)
     world_size = pg_wrapper.get_world_size()
     outputs = [None] * world_size
     pg_wrapper.all_gather_object(outputs, recorded_durations)
     ret = defaultdict(list)
     for output in outputs:
-        # pyre-fixme [16]: `Optional` has no attribute `__getitem__`.
+        if not output:
+            continue
         for k, v in output.items():
             if k not in ret:
                 ret[k] = []
             ret[k].extend(v)
     return ret
```

### Comparing `torchtnt-0.2.3/torchtnt/utils/tqdm.py` & `torchtnt-0.2.4/torchtnt/utils/tqdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import io
 import logging
 from typing import Iterable, Optional, TextIO, Union
 
 from torchtnt.utils.progress import estimated_steps_in_epoch
 from tqdm.auto import tqdm
```

### Comparing `torchtnt-0.2.3/torchtnt.egg-info/PKG-INFO` & `torchtnt-0.2.4/torchtnt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt
-Version: 0.2.3
+Version: 0.2.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,15 +30,15 @@
 Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: parameterized; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: torchsnapshot-nightly; extra == "dev"
 Requires-Dist: pyre-check; extra == "dev"
-Requires-Dist: torchvision==0.16.2; extra == "dev"
+Requires-Dist: torchvision==0.15.2; extra == "dev"
 
 TNT
 ==========
 
 **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and utilities.
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt Version: 0.2.3 Summary: A lightweight
+Metadata-Version: 2.1 Name: torchtnt Version: 0.2.4 Summary: A lightweight
 library for PyTorch training tools and utilities Home-page: https://github.com/
 pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com License: BSD-
 3 Keywords: pytorch,torch,training,tools,utilities Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
@@ -10,15 +10,15 @@
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch
 Requires-Dist: numpy Requires-Dist: fsspec Requires-Dist: tensorboard Requires-
 Dist: packaging Requires-Dist: psutil Requires-Dist: pyre_extensions Requires-
 Dist: typing_extensions Requires-Dist: setuptools Requires-Dist: tqdm Requires-
 Dist: tabulate Provides-Extra: dev Requires-Dist: parameterized; extra == "dev"
 Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: torchsnapshot-nightly; extra == "dev" Requires-Dist: pyre-check;
-extra == "dev" Requires-Dist: torchvision==0.16.2; extra == "dev" TNT
+extra == "dev" Requires-Dist: torchvision==0.15.2; extra == "dev" TNT
 ========== **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and
 utilities.
  _[_b_u_i_l_d_ _s_t_a_t_u_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_p_y_p_i_ _n_i_g_h_t_l_y_ _v_e_r_s_i_o_n_]_[_c_o_d_e_c_o_v_]_[_b_s_d
                         _l_i_c_e_n_s_e_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_ _s_t_a_t_u_s_]
 ## Installation TNT can be installed with pip: ```buildoutcfg pip install
 torchtnt ``` Or, alternatively, via conda: ```buildoutcfg conda install -
 c conda-forge torchtnt ``` If you run into issues, make sure that Pytorch is
```

### Comparing `torchtnt-0.2.3/torchtnt.egg-info/SOURCES.txt` & `torchtnt-0.2.4/torchtnt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,33 +26,42 @@
 torchtnt/framework/utils.py
 torchtnt/framework/callbacks/__init__.py
 torchtnt/framework/callbacks/_checkpoint_utils.py
 torchtnt/framework/callbacks/base_checkpointer.py
 torchtnt/framework/callbacks/base_csv_writer.py
 torchtnt/framework/callbacks/checkpointer_types.py
 torchtnt/framework/callbacks/dcp_saver.py
+torchtnt/framework/callbacks/early_stopping.py
 torchtnt/framework/callbacks/empty_cuda_cache.py
 torchtnt/framework/callbacks/garbage_collector.py
 torchtnt/framework/callbacks/iteration_time_logger.py
 torchtnt/framework/callbacks/lambda_callback.py
 torchtnt/framework/callbacks/learning_rate_monitor.py
 torchtnt/framework/callbacks/memory_snapshot.py
 torchtnt/framework/callbacks/module_summary.py
+torchtnt/framework/callbacks/progress_reporter.py
 torchtnt/framework/callbacks/pytorch_profiler.py
+torchtnt/framework/callbacks/slow_rank_detector.py
 torchtnt/framework/callbacks/system_resources_monitor.py
 torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+torchtnt/framework/callbacks/throughput_logger.py
+torchtnt/framework/callbacks/time_limit_interrupter.py
+torchtnt/framework/callbacks/time_wait_for_batch_logger.py
+torchtnt/framework/callbacks/torch_compile.py
 torchtnt/framework/callbacks/torchsnapshot_saver.py
 torchtnt/framework/callbacks/tqdm_progress_bar.py
 torchtnt/framework/callbacks/train_progress_monitor.py
 torchtnt/utils/__init__.py
+torchtnt/utils/checkpoint.py
 torchtnt/utils/device.py
 torchtnt/utils/distributed.py
 torchtnt/utils/early_stop_checker.py
 torchtnt/utils/env.py
 torchtnt/utils/flops.py
+torchtnt/utils/fsdp_utils.py
 torchtnt/utils/fsspec.py
 torchtnt/utils/lr_scheduler.py
 torchtnt/utils/memory.py
 torchtnt/utils/memory_snapshot_profiler.py
 torchtnt/utils/misc.py
 torchtnt/utils/module_summary.py
 torchtnt/utils/oom.py
```

