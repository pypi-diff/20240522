# Comparing `tmp/datapools-1.0.58.tar.gz` & `tmp/datapools-1.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.58.tar", last modified: Tue May 21 06:04:22 2024, max compression
+gzip compressed data, was "datapools-1.0.59.tar", last modified: Tue May 21 09:59:56 2024, max compression
```

## Comparing `datapools-1.0.58.tar` & `datapools-1.0.59.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 06:04:14.000000 datapools-1.0.58/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-05-21 06:04:14.000000 datapools-1.0.58/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-21 06:04:14.000000 datapools-1.0.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 06:04:14.000000 datapools-1.0.58/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 06:04:22.659753 datapools-1.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-21 06:04:14.000000 datapools-1.0.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.647753 datapools-1.0.58/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17785 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:04:22.663753 datapools-1.0.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-21 06:04:14.000000 datapools-1.0.58/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/test_session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.052801 datapools-1.0.59/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 09:59:45.000000 datapools-1.0.59/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    19856 2024-05-21 09:59:45.000000 datapools-1.0.59/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-21 09:59:45.000000 datapools-1.0.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 09:59:45.000000 datapools-1.0.59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 09:59:56.052801 datapools-1.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-21 09:59:45.000000 datapools-1.0.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.040801 datapools-1.0.59/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.044801 datapools-1.0.59/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.048801 datapools-1.0.59/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.052801 datapools-1.0.59/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.052801 datapools-1.0.59/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-21 09:59:45.000000 datapools-1.0.59/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.052801 datapools-1.0.59/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 09:59:55.000000 datapools-1.0.59/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-21 09:59:56.000000 datapools-1.0.59/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:59:55.000000 datapools-1.0.59/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 09:59:55.000000 datapools-1.0.59/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-21 09:59:55.000000 datapools-1.0.59/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:59:55.000000 datapools-1.0.59/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:56.052801 datapools-1.0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-21 09:59:45.000000 datapools-1.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:56.052801 datapools-1.0.59/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:45.000000 datapools-1.0.59/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 09:59:45.000000 datapools-1.0.59/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 09:59:45.000000 datapools-1.0.59/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 09:59:45.000000 datapools-1.0.59/tests/test_session_manager.py
```

### Comparing `datapools-1.0.58/HISTORY.md` & `datapools-1.0.59/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Session tag stats. [sergpsu]
+
+
+1.0.58 (2024-05-21)
+-------------------
+- Release: version 1.0.58 🚀 [sergpsu]
 - Merge pull request #76 from torrentsai/sergpsu-async-redis. [S]
 
   Async redis and thinner plugins
 - . [sergpsu]
 - . [sergpsu]
 - Async redis, thinner plugins. [sergpsu]
```

### Comparing `datapools-1.0.58/LICENSE` & `datapools-1.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/PKG-INFO` & `datapools-1.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.58
+Version: 1.0.59
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.58/README.md` & `datapools-1.0.59/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/api.py` & `datapools-1.0.59/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/cli.py` & `datapools-1.0.59/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/backend_api.py` & `datapools-1.0.59/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/queues/__init__.py` & `datapools-1.0.59/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/queues/rabbitmq.py` & `datapools-1.0.59/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/queues/types.py` & `datapools-1.0.59/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/session_manager.py` & `datapools-1.0.59/datapools/common/session_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,35 +9,38 @@
 from .types import CrawlerHintURLStatus
 
 # from ..logger import logger
 
 SESSION_METADATA_KEY_PREFIX = "crawler_session_meta_"  # hash
 SESSION_URLS_KEY_PREFIX = "crawler_session_urls_"  # set
 SESSION_CONTENT_KEY_PREFIX = "crawler_session_content_"  # set
+SESSION_TAGS_USAGE_KEY_PREFIX = "crawler_session_tags_usage_key_"  # hash: tag_id => count
 
 
 class SessionStatus(Enum):
     NORMAL = 0
     STOPPED = 1
 
 
 class Session:
     id: str
     r: Redis
     meta_key: str
     urls_key: str
     content_key: str
+    tags_usage_key: str
     stats_channel: str
 
     def __init__(self, session_id, redis_inst: Redis):
         self.id = session_id
         self.r = redis_inst
         self.meta_key = SessionManager.get_meta_key(self.id)
         self.urls_key = SessionManager.get_urls_key(self.id)
         self.content_key = SessionManager.get_content_key(self.id)
+        self.tags_usage_key = SessionManager.get_tags_usage_key(self.id)
         self.stats_channel = Session.get_stats_channel(self.id)
 
     @staticmethod
     def get_stats_channel(session_id_or_mask):
         return f"stats_channel_{session_id_or_mask}"
 
     @staticmethod
@@ -105,14 +108,28 @@
         await self.r.hincrby(self.meta_key, "crawled_content", 1)
         await self.r.publish(self.stats_channel, "crawled_content")
 
     async def inc_evaluated_content(self):
         await self.r.hincrby(self.meta_key, "evaluated_content", 1)
         await self.r.publish(self.stats_channel, "evaluated_content")
 
+    async def inc_tag_usage(self, tag_id: str, keepout: bool):
+        if keepout is False:
+            await self.r.hincrby(self.tags_usage_key, f"n/{tag_id}", 1)
+        else:
+            await self.r.hincrby(self.tags_usage_key, tag_id, 1)
+
+    async def get_tag_usage(self, tag_id: str):
+        tag_id = str(tag_id)
+        bres = await self.r.hget(self.tags_usage_key, tag_id)
+        usage = int(bres.decode()) if bres is not None else 0
+        bres = await self.r.hget(self.tags_usage_key, f"n/{tag_id}")
+        keepout = int(bres.decode()) if bres is not None else 0
+        return (usage, keepout)
+
     async def exists(self):
         res = await self.r.exists(self.meta_key)
         return res
 
     async def set_last_reported_status(self, status: CrawlerHintURLStatus):
         await self.r.hset(self.meta_key, "last_reported_status", status.value)
 
@@ -183,13 +200,17 @@
     def get_urls_key(session_id):
         return f"{SESSION_URLS_KEY_PREFIX}{session_id}"
 
     @staticmethod
     def get_content_key(session_id):
         return f"{SESSION_CONTENT_KEY_PREFIX}{session_id}"
 
+    @staticmethod
+    def get_tags_usage_key(session_id):
+        return f"{SESSION_TAGS_USAGE_KEY_PREFIX}{session_id}"
+
     async def get_ids(self, limit) -> List[str]:
         keys = await self.r.keys(f"{SESSION_METADATA_KEY_PREFIX}*")
         if len(keys) > limit:
             keys = keys[0:limit]
         n = len(SESSION_METADATA_KEY_PREFIX)
         return [k[n:] for k in keys]
```

### Comparing `datapools-1.0.58/datapools/common/stoppable.py` & `datapools-1.0.59/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/storage/base_storage.py` & `datapools-1.0.59/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/storage/file_storage.py` & `datapools-1.0.59/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.59/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.59/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/common/types.py` & `datapools-1.0.59/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/producer/base_producer.py` & `datapools-1.0.59/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/scheduler/scheduler.py` & `datapools-1.0.59/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.59/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.59/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/default/default.py` & `datapools-1.0.59/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.59/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.59/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.59/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.59/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.59/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.59/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.59/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.59/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.59/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/datapools/worker/worker.py` & `datapools-1.0.59/datapools/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,20 @@
 
                 storage_id = self.storage.gen_id(cc.url)
                 logger.info(f"putting to {storage_id=}")
                 await self.storage.put(storage_id, cc.content)
 
                 await session.add_content(cc.url)
                 await session.inc_crawled_content()
+                if cc.tag_id is not None:
+                    await session.inc_tag_usage(cc.tag_id, cc.tag_keepout)
+                if cc.copyright_tag_id is not None:
+                    await session.inc_tag_usage(cc.copyright_tag_id, cc.copyright_tag_keepout)
+                if cc.platform_tag_id is not None:
+                    await session.inc_tag_usage(cc.platform_tag_id, cc.platform_tag_keepout)
 
                 # notifying producer about new crawled data
                 await self.producer_queue.push(
                     QueueMessage(
                         session.id,
                         QueueMessageType.Task,
                         {
```

### Comparing `datapools-1.0.58/datapools.egg-info/PKG-INFO` & `datapools-1.0.59/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.58
+Version: 1.0.59
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.58/datapools.egg-info/SOURCES.txt` & `datapools-1.0.59/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/setup.py` & `datapools-1.0.59/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/tests/test_base.py` & `datapools-1.0.59/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.58/tests/test_session_manager.py` & `datapools-1.0.59/tests/test_session_manager.py`

 * *Files identical despite different names*

