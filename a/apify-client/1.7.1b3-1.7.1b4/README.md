# Comparing `tmp/apify_client-1.7.1b3.tar.gz` & `tmp/apify_client-1.7.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.7.1b3.tar", last modified: Wed May 22 12:55:35 2024, max compression
+gzip compressed data, was "apify_client-1.7.1b4.tar", last modified: Wed May 22 13:34:00 2024, max compression
```

## Comparing `apify_client-1.7.1b3.tar` & `apify_client-1.7.1b4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.176345 apify_client-1.7.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-22 12:55:35.176345 apify_client-1.7.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-22 12:55:32.000000 apify_client-1.7.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:55:35.176345 apify_client-1.7.1b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.164345 apify_client-1.7.1b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.164345 apify_client-1.7.1b3/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.168345 apify_client-1.7.1b3/src/apify_client/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.168345 apify_client-1.7.1b3/src/apify_client/clients/base/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/base/actor_job_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/base/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/base/resource_collection_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.172345 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34982 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_env_var_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_version_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    46556 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    21378 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/schedule_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25355 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/task_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:04.000000 apify_client-1.7.1b3/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:35.172345 apify_client-1.7.1b3/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-22 12:55:35.000000 apify_client-1.7.1b3/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 12:55:35.000000 apify_client-1.7.1b3/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:55:35.000000 apify_client-1.7.1b3/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 12:55:35.000000 apify_client-1.7.1b3/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 12:55:35.000000 apify_client-1.7.1b3/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.031250 apify_client-1.7.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-22 13:34:00.031250 apify_client-1.7.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-22 13:33:57.000000 apify_client-1.7.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:34:00.031250 apify_client-1.7.1b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.015250 apify_client-1.7.1b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.019250 apify_client-1.7.1b4/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.019250 apify_client-1.7.1b4/src/apify_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.023250 apify_client-1.7.1b4/src/apify_client/clients/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/base/actor_job_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/base/resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/base/resource_collection_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.027250 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34982 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_env_var_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_version_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46556 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21378 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/schedule_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25355 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/task_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:33:33.000000 apify_client-1.7.1b4/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:00.027250 apify_client-1.7.1b4/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-22 13:34:00.000000 apify_client-1.7.1b4/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 13:34:00.000000 apify_client-1.7.1b4/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:34:00.000000 apify_client-1.7.1b4/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 13:34:00.000000 apify_client-1.7.1b4/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 13:34:00.000000 apify_client-1.7.1b4/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.7.1b3/LICENSE` & `apify_client-1.7.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/PKG-INFO` & `apify_client-1.7.1b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.7.1b3
+Version: 1.7.1b4
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
@@ -23,27 +23,27 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apify-shared~=1.1.1
 Requires-Dist: httpx>=0.25.1
 Provides-Extra: dev
-Requires-Dist: build~=1.0.3; extra == "dev"
-Requires-Dist: mypy~=1.7.0; extra == "dev"
-Requires-Dist: pre-commit~=3.4.0; extra == "dev"
-Requires-Dist: pydoc-markdown~=4.8.2; extra == "dev"
-Requires-Dist: pytest~=7.4.2; extra == "dev"
-Requires-Dist: pytest-asyncio~=0.21.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
-Requires-Dist: pytest-only~=2.0.0; extra == "dev"
-Requires-Dist: pytest-timeout~=2.2.0; extra == "dev"
-Requires-Dist: pytest-xdist~=3.3.1; extra == "dev"
-Requires-Dist: redbaron~=0.9.2; extra == "dev"
-Requires-Dist: ruff~=0.1.13; extra == "dev"
-Requires-Dist: twine~=4.0.2; extra == "dev"
+Requires-Dist: build~=1.2.0; extra == "dev"
+Requires-Dist: mypy~=1.10.0; extra == "dev"
+Requires-Dist: pre-commit~=3.5.0; extra == "dev"
+Requires-Dist: pydoc-markdown~=4.8.0; extra == "dev"
+Requires-Dist: pytest~=8.0.0; extra == "dev"
+Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
+Requires-Dist: pytest-only~=2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout~=2.3.0; extra == "dev"
+Requires-Dist: pytest-xdist~=3.6.0; extra == "dev"
+Requires-Dist: redbaron~=0.9.0; extra == "dev"
+Requires-Dist: ruff~=0.4.0; extra == "dev"
+Requires-Dist: twine~=5.0.0; extra == "dev"
 
 # Apify API client for Python
 
 The Apify API Client for Python is the official library to access the [Apify API](https://docs.apify.com/api/v2) from your Python applications.
 It provides useful features like automatic retries and convenience functions to improve your experience with the Apify API.
 
 If you want to develop Apify Actors in Python,
```

### Comparing `apify_client-1.7.1b3/README.md` & `apify_client-1.7.1b4/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/pyproject.toml` & `apify_client-1.7.1b4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apify_client"
-version = "1.7.1b3"
+version = "1.7.1b4"
 description = "Apify API client for Python"
 readme = "README.md"
 license = { text = "Apache Software License" }
 authors = [{ name = "Apify Technologies s.r.o.", email = "support@apify.com" }]
 keywords = ["apify", "api", "client", "scraping", "automation"]
 
 classifiers = [
@@ -28,27 +28,27 @@
 dependencies = [
     "apify-shared ~= 1.1.1",
     "httpx >= 0.25.1",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "build ~= 1.0.3",
-    "mypy ~= 1.7.0",
-    "pre-commit ~= 3.4.0",
-    "pydoc-markdown ~= 4.8.2",
-    "pytest ~= 7.4.2",
-    "pytest-asyncio ~= 0.21.0",
-    "pytest-cov ~= 4.1.0",
-    "pytest-only ~= 2.0.0",
-    "pytest-timeout ~= 2.2.0",
-    "pytest-xdist ~= 3.3.1",
-    "redbaron ~= 0.9.2",
-    "ruff ~= 0.1.13",
-    "twine ~= 4.0.2",
+    "build ~= 1.2.0",
+    "mypy ~= 1.10.0",
+    "pre-commit ~= 3.5.0",
+    "pydoc-markdown ~= 4.8.0",
+    "pytest ~= 8.0.0",
+    "pytest-asyncio ~= 0.23.0",
+    "pytest-cov ~= 5.0.0",
+    "pytest-only ~= 2.1.0",
+    "pytest-timeout ~= 2.3.0",
+    "pytest-xdist ~= 3.6.0",
+    "redbaron ~= 0.9.0",
+    "ruff ~= 0.4.0",
+    "twine ~= 5.0.0",
 ]
 
 [project.urls]
 "Homepage" = "https://docs.apify.com/api/client/python/"
 "Documentation" = "https://docs.apify.com/api/client/python/"
 "Source" = "https://github.com/apify/apify-client-python"
 "Issue tracker" = "https://github.com/apify/apify-client-python/issues"
```

### Comparing `apify_client-1.7.1b3/src/apify_client/_errors.py` & `apify_client-1.7.1b4/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/_http_client.py` & `apify_client-1.7.1b4/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/_logging.py` & `apify_client-1.7.1b4/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/_utils.py` & `apify_client-1.7.1b4/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/client.py` & `apify_client-1.7.1b4/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/__init__.py` & `apify_client-1.7.1b4/src/apify_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/base/__init__.py` & `apify_client-1.7.1b4/src/apify_client/clients/base/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/base/actor_job_base_client.py` & `apify_client-1.7.1b4/src/apify_client/clients/base/actor_job_base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/base/base_client.py` & `apify_client-1.7.1b4/src/apify_client/clients/base/base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/base/resource_client.py` & `apify_client-1.7.1b4/src/apify_client/clients/base/resource_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/base/resource_collection_client.py` & `apify_client-1.7.1b4/src/apify_client/clients/base/resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/__init__.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_env_var.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_env_var.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_env_var_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_env_var_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_version.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_version.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/actor_version_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/actor_version_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/build.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/build.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/build_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/build_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/dataset.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/dataset_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/key_value_store.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/key_value_store_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/log.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/log.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/request_queue.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/request_queue_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/run.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/run.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/run_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/run_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/schedule.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/schedule.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/schedule_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/schedule_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/store_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/store_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/task.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/task.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/task_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/task_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/user.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/user.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook_dispatch.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook_dispatch.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py` & `apify_client-1.7.1b4/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client/consts.py` & `apify_client-1.7.1b4/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.7.1b3/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.7.1b4/src/apify_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.7.1b3
+Version: 1.7.1b4
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
@@ -23,27 +23,27 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apify-shared~=1.1.1
 Requires-Dist: httpx>=0.25.1
 Provides-Extra: dev
-Requires-Dist: build~=1.0.3; extra == "dev"
-Requires-Dist: mypy~=1.7.0; extra == "dev"
-Requires-Dist: pre-commit~=3.4.0; extra == "dev"
-Requires-Dist: pydoc-markdown~=4.8.2; extra == "dev"
-Requires-Dist: pytest~=7.4.2; extra == "dev"
-Requires-Dist: pytest-asyncio~=0.21.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
-Requires-Dist: pytest-only~=2.0.0; extra == "dev"
-Requires-Dist: pytest-timeout~=2.2.0; extra == "dev"
-Requires-Dist: pytest-xdist~=3.3.1; extra == "dev"
-Requires-Dist: redbaron~=0.9.2; extra == "dev"
-Requires-Dist: ruff~=0.1.13; extra == "dev"
-Requires-Dist: twine~=4.0.2; extra == "dev"
+Requires-Dist: build~=1.2.0; extra == "dev"
+Requires-Dist: mypy~=1.10.0; extra == "dev"
+Requires-Dist: pre-commit~=3.5.0; extra == "dev"
+Requires-Dist: pydoc-markdown~=4.8.0; extra == "dev"
+Requires-Dist: pytest~=8.0.0; extra == "dev"
+Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
+Requires-Dist: pytest-only~=2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout~=2.3.0; extra == "dev"
+Requires-Dist: pytest-xdist~=3.6.0; extra == "dev"
+Requires-Dist: redbaron~=0.9.0; extra == "dev"
+Requires-Dist: ruff~=0.4.0; extra == "dev"
+Requires-Dist: twine~=5.0.0; extra == "dev"
 
 # Apify API client for Python
 
 The Apify API Client for Python is the official library to access the [Apify API](https://docs.apify.com/api/v2) from your Python applications.
 It provides useful features like automatic retries and convenience functions to improve your experience with the Apify API.
 
 If you want to develop Apify Actors in Python,
```

### Comparing `apify_client-1.7.1b3/src/apify_client.egg-info/SOURCES.txt` & `apify_client-1.7.1b4/src/apify_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

