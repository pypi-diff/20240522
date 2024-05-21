# Comparing `tmp/storey-1.7.8.tar.gz` & `tmp/storey-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storey-1.7.8.tar", last modified: Wed Apr 17 05:51:24 2024, max compression
+gzip compressed data, was "storey-1.7.9.tar", last modified: Sun Apr 21 10:10:37 2024, max compression
```

## Comparing `storey-1.7.8.tar` & `storey-1.7.9.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.720724 storey-1.7.8/
--rw-r--r--   0 root         (0) root         (0)        5 2024-01-08 04:33:02.000000 storey-1.7.8/.dockerignore
--rw-r--r--   0 root         (0) root         (0)    11357 2024-01-08 04:33:02.000000 storey-1.7.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2024-01-08 04:33:02.000000 storey-1.7.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:51:24.720724 storey-1.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-17 05:48:42.000000 storey-1.7.8/README.md
--rw-r--r--   0 root         (0) root         (0)      292 2024-04-17 05:48:42.000000 storey-1.7.8/dev-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.710724 storey-1.7.8/integration/
--rw-r--r--   0 root         (0) root         (0)      571 2024-01-08 04:33:02.000000 storey-1.7.8/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5863 2024-01-08 04:33:02.000000 storey-1.7.8/integration/conftest.py
--rw-r--r--   0 root         (0) root         (0)     9748 2024-01-08 04:33:02.000000 storey-1.7.8/integration/integration_test_utils.py
--rw-r--r--   0 root         (0) root         (0)   170276 2024-01-08 04:33:02.000000 storey-1.7.8/integration/test_aggregation_integration.py
--rw-r--r--   0 root         (0) root         (0)    10034 2024-02-21 07:45:19.000000 storey-1.7.8/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 root         (0) root         (0)    21267 2024-01-08 04:33:02.000000 storey-1.7.8/integration/test_filesystems_integration.py
--rw-r--r--   0 root         (0) root         (0)    45491 2024-02-21 07:45:19.000000 storey-1.7.8/integration/test_flow_integration.py
--rw-r--r--   0 root         (0) root         (0)     4316 2024-04-11 08:38:21.000000 storey-1.7.8/integration/test_kafka_integration.py
--rw-r--r--   0 root         (0) root         (0)     3179 2024-01-08 04:33:02.000000 storey-1.7.8/integration/test_redis_specific.py
--rw-r--r--   0 root         (0) root         (0)    10355 2024-02-21 07:45:19.000000 storey-1.7.8/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-11 08:38:21.000000 storey-1.7.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-17 05:51:24.720724 storey-1.7.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2524 2024-01-08 04:33:02.000000 storey-1.7.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.713724 storey-1.7.8/storey/
--rw-r--r--   0 root         (0) root         (0)     3118 2024-04-17 05:51:18.000000 storey-1.7.8/storey/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2024-01-08 04:33:02.000000 storey-1.7.8/storey/aggregation_utils.py
--rw-r--r--   0 root         (0) root         (0)    17706 2024-01-08 04:33:02.000000 storey-1.7.8/storey/aggregations.py
--rw-r--r--   0 root         (0) root         (0)     4692 2024-01-08 04:33:02.000000 storey-1.7.8/storey/dataframe.py
--rw-r--r--   0 root         (0) root         (0)    28287 2024-04-17 05:48:42.000000 storey-1.7.8/storey/drivers.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-01-08 04:33:02.000000 storey-1.7.8/storey/dtypes.py
--rw-r--r--   0 root         (0) root         (0)    51707 2024-04-17 05:48:42.000000 storey-1.7.8/storey/flow.py
--rw-r--r--   0 root         (0) root         (0)     3204 2024-04-11 08:38:21.000000 storey-1.7.8/storey/queue.py
--rw-r--r--   0 root         (0) root         (0)    27946 2024-01-08 04:33:02.000000 storey-1.7.8/storey/redis_driver.py
--rw-r--r--   0 root         (0) root         (0)    46536 2024-04-11 08:38:21.000000 storey-1.7.8/storey/sources.py
--rw-r--r--   0 root         (0) root         (0)     4928 2024-01-08 04:33:02.000000 storey-1.7.8/storey/sql_driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.716724 storey-1.7.8/storey/steps/
--rw-r--r--   0 root         (0) root         (0)      807 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5418 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/assertion.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/flatten.py
--rw-r--r--   0 root         (0) root         (0)      903 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/foreach.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/partition.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-01-08 04:33:02.000000 storey-1.7.8/storey/steps/sample.py
--rw-r--r--   0 root         (0) root         (0)    81360 2024-04-17 05:48:42.000000 storey-1.7.8/storey/table.py
--rw-r--r--   0 root         (0) root         (0)    52569 2024-04-11 08:38:21.000000 storey-1.7.8/storey/targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.716724 storey-1.7.8/storey/transformations/
--rw-r--r--   0 root         (0) root         (0)     1564 2024-01-08 04:33:02.000000 storey-1.7.8/storey/transformations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11281 2024-01-08 04:33:02.000000 storey-1.7.8/storey/utils.py
--rw-r--r--   0 root         (0) root         (0)     8226 2024-01-08 04:33:02.000000 storey-1.7.8/storey/windowed_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.719724 storey-1.7.8/storey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1330 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 05:51:24.000000 storey-1.7.8/storey.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:51:24.718724 storey-1.7.8/tests/
--rw-r--r--   0 root         (0) root         (0)      571 2024-01-08 04:33:02.000000 storey-1.7.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)   144410 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_aggregate_by_key.py
--rw-r--r--   0 root         (0) root         (0)     4853 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_aggregate_store.py
--rw-r--r--   0 root         (0) root         (0)   135406 2024-04-11 08:38:21.000000 storey-1.7.8/tests/test_flow.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 08:38:21.000000 storey-1.7.8/tests/test_queue.py
--rw-r--r--   0 root         (0) root         (0)    11002 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_steps.py
--rw-r--r--   0 root         (0) root         (0)     2506 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_types.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     1459 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_v3io.py
--rw-r--r--   0 root         (0) root         (0)     2622 2024-01-08 04:33:02.000000 storey-1.7.8/tests/test_windowed_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.456885 storey-1.7.9/
+-rw-r--r--   0 root         (0) root         (0)        5 2024-01-08 04:33:02.000000 storey-1.7.9/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-01-08 04:33:02.000000 storey-1.7.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2024-01-08 04:33:02.000000 storey-1.7.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-21 10:10:37.456885 storey-1.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-17 05:48:42.000000 storey-1.7.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-17 05:48:42.000000 storey-1.7.9/dev-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.446885 storey-1.7.9/integration/
+-rw-r--r--   0 root         (0) root         (0)      571 2024-01-08 04:33:02.000000 storey-1.7.9/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2024-01-08 04:33:02.000000 storey-1.7.9/integration/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     9748 2024-01-08 04:33:02.000000 storey-1.7.9/integration/integration_test_utils.py
+-rw-r--r--   0 root         (0) root         (0)   170276 2024-01-08 04:33:02.000000 storey-1.7.9/integration/test_aggregation_integration.py
+-rw-r--r--   0 root         (0) root         (0)    10034 2024-02-21 07:45:19.000000 storey-1.7.9/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 root         (0) root         (0)    21267 2024-01-08 04:33:02.000000 storey-1.7.9/integration/test_filesystems_integration.py
+-rw-r--r--   0 root         (0) root         (0)    45491 2024-02-21 07:45:19.000000 storey-1.7.9/integration/test_flow_integration.py
+-rw-r--r--   0 root         (0) root         (0)     4316 2024-04-11 08:38:21.000000 storey-1.7.9/integration/test_kafka_integration.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2024-01-08 04:33:02.000000 storey-1.7.9/integration/test_redis_specific.py
+-rw-r--r--   0 root         (0) root         (0)    10355 2024-02-21 07:45:19.000000 storey-1.7.9/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-11 08:38:21.000000 storey-1.7.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-21 10:10:37.457885 storey-1.7.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-01-08 04:33:02.000000 storey-1.7.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.450885 storey-1.7.9/storey/
+-rw-r--r--   0 root         (0) root         (0)     3170 2024-04-21 10:10:31.000000 storey-1.7.9/storey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2024-01-08 04:33:02.000000 storey-1.7.9/storey/aggregation_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17706 2024-01-08 04:33:02.000000 storey-1.7.9/storey/aggregations.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2024-01-08 04:33:02.000000 storey-1.7.9/storey/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)    28287 2024-04-17 05:48:42.000000 storey-1.7.9/storey/drivers.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-01-08 04:33:02.000000 storey-1.7.9/storey/dtypes.py
+-rw-r--r--   0 root         (0) root         (0)    54530 2024-04-21 10:05:07.000000 storey-1.7.9/storey/flow.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2024-04-11 08:38:21.000000 storey-1.7.9/storey/queue.py
+-rw-r--r--   0 root         (0) root         (0)    27946 2024-01-08 04:33:02.000000 storey-1.7.9/storey/redis_driver.py
+-rw-r--r--   0 root         (0) root         (0)    46536 2024-04-11 08:38:21.000000 storey-1.7.9/storey/sources.py
+-rw-r--r--   0 root         (0) root         (0)     4928 2024-01-08 04:33:02.000000 storey-1.7.9/storey/sql_driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.452885 storey-1.7.9/storey/steps/
+-rw-r--r--   0 root         (0) root         (0)      807 2024-01-08 04:33:02.000000 storey-1.7.9/storey/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2024-01-08 04:33:02.000000 storey-1.7.9/storey/steps/assertion.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-01-08 04:33:02.000000 storey-1.7.9/storey/steps/flatten.py
+-rw-r--r--   0 root         (0) root         (0)      903 2024-01-08 04:33:02.000000 storey-1.7.9/storey/steps/foreach.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-01-08 04:33:02.000000 storey-1.7.9/storey/steps/partition.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-01-08 04:33:02.000000 storey-1.7.9/storey/steps/sample.py
+-rw-r--r--   0 root         (0) root         (0)    81360 2024-04-17 05:48:42.000000 storey-1.7.9/storey/table.py
+-rw-r--r--   0 root         (0) root         (0)    52569 2024-04-11 08:38:21.000000 storey-1.7.9/storey/targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.452885 storey-1.7.9/storey/transformations/
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-01-08 04:33:02.000000 storey-1.7.9/storey/transformations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11281 2024-01-08 04:33:02.000000 storey-1.7.9/storey/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2024-01-08 04:33:02.000000 storey-1.7.9/storey/windowed_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.455885 storey-1.7.9/storey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-21 10:10:37.000000 storey-1.7.9/storey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1365 2024-04-21 10:10:37.000000 storey-1.7.9/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 10:10:37.000000 storey-1.7.9/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2024-04-21 10:10:37.000000 storey-1.7.9/storey.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-21 10:10:37.000000 storey-1.7.9/storey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:10:37.455885 storey-1.7.9/tests/
+-rw-r--r--   0 root         (0) root         (0)      571 2024-01-08 04:33:02.000000 storey-1.7.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144410 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_aggregate_by_key.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_aggregate_store.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-21 10:05:07.000000 storey-1.7.9/tests/test_concurrent_execution.py
+-rw-r--r--   0 root         (0) root         (0)   135406 2024-04-11 08:38:21.000000 storey-1.7.9/tests/test_flow.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 08:38:21.000000 storey-1.7.9/tests/test_queue.py
+-rw-r--r--   0 root         (0) root         (0)    11002 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_steps.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_types.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_v3io.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2024-01-08 04:33:02.000000 storey-1.7.9/tests/test_windowed_store.py
```

### Comparing `storey-1.7.8/LICENSE` & `storey-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/PKG-INFO` & `storey-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.7.8
+Version: 1.7.9
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.7.8/integration/__init__.py` & `storey-1.7.9/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/conftest.py` & `storey-1.7.9/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/integration_test_utils.py` & `storey-1.7.9/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_aggregation_integration.py` & `storey-1.7.9/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_azure_filesystem_integration.py` & `storey-1.7.9/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_filesystems_integration.py` & `storey-1.7.9/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_flow_integration.py` & `storey-1.7.9/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_kafka_integration.py` & `storey-1.7.9/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_redis_specific.py` & `storey-1.7.9/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/integration/test_s3_filesystem_integration.py` & `storey-1.7.9/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/setup.py` & `storey-1.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/__init__.py` & `storey-1.7.9/storey/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.7.8"
+__version__ = "1.7.9"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
@@ -32,14 +32,15 @@
 from .dtypes import FixedWindows  # noqa: F401
 from .dtypes import FixedWindowType  # noqa: F401
 from .dtypes import LateDataHandling  # noqa: F401
 from .dtypes import SlidingWindows  # noqa: F401
 from .flow import Batch  # noqa: F401
 from .flow import Choice  # noqa: F401
 from .flow import Complete  # noqa: F401
+from .flow import ConcurrentExecution  # noqa: F401
 from .flow import Context  # noqa: F401
 from .flow import Extend  # noqa: F401
 from .flow import Filter  # noqa: F401
 from .flow import FlatMap  # noqa: F401
 from .flow import Flow  # noqa: F401
 from .flow import FlowError  # noqa: F401
 from .flow import HttpRequest  # noqa: F401
```

### Comparing `storey-1.7.8/storey/aggregation_utils.py` & `storey-1.7.9/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/aggregations.py` & `storey-1.7.9/storey/aggregations.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/dataframe.py` & `storey-1.7.9/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/drivers.py` & `storey-1.7.9/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/dtypes.py` & `storey-1.7.9/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/flow.py` & `storey-1.7.9/storey/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import asyncio
 import copy
 import datetime
 import inspect
+import pickle
 import time
 import traceback
 from asyncio import Task
 from collections import defaultdict
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Union
 
 import aiohttp
 
 from .dtypes import Event, FlowError, V3ioError, _termination_obj, known_driver_schemes
 from .queue import AsyncQueue
 from .table import Table
@@ -796,19 +798,19 @@
 class _ConcurrentJobExecution(Flow):
     _BACKOFF_MAX = 120
 
     def __init__(self, max_in_flight=None, retries=None, backoff_factor=None, **kwargs):
         Flow.__init__(self, **kwargs)
         if max_in_flight is not None and max_in_flight < 1:
             raise ValueError(f"max_in_flight may not be less than 1 (got {max_in_flight})")
-        self.max_in_flight = max_in_flight
         self.retries = retries
         self.backoff_factor = backoff_factor
 
-        self._queue_size = max_in_flight - 1 if max_in_flight else 8
+        self._max_in_flight = max_in_flight or 8
+        self._queue_size = self._max_in_flight - 1
 
     def _init(self):
         super()._init()
         self._q = None
         self._lazy_init_complete = False
 
     async def _worker(self):
@@ -912,14 +914,81 @@
             else:
                 task = asyncio.get_running_loop().create_task(coroutine)
                 await self._q.put((event, task))
                 if self._worker_awaitable.done():
                     await self._worker_awaitable
 
 
+class ConcurrentExecution(_ConcurrentJobExecution):
+    """
+    Inherit this class and override `process_event()` to process events concurrently.
+
+    :param process_event: Function that will be run on each event
+
+    :param concurrency_mechanism: One of:
+      * "asyncio" (default) – for I/O implemented using asyncio
+      * "threading" – for blocking I/O
+      * "multiprocessing" – for processing-intensive tasks
+
+    :param max_in_flight: Maximum number of events to be processed at a time (default 8)
+    :param retries: Maximum number of retries per event (default 0)
+    :param backoff_factor: Wait time in seconds between retries (default 1)
+    :param pass_context: If False, the process_event function will be called with just one parameter (event). If True,
+      the process_event function will be called with two parameters (event, context). Defaults to False.
+    """
+
+    _supported_concurrency_mechanisms = ["asyncio", "threading", "multiprocessing"]
+
+    def __init__(
+        self,
+        event_processor: Union[Callable[[Event], Any], Callable[[Event, Any], Any]],
+        concurrency_mechanism=None,
+        pass_context=None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+
+        self._event_processor = event_processor
+
+        if concurrency_mechanism and concurrency_mechanism not in self._supported_concurrency_mechanisms:
+            raise ValueError(f"Concurrency mechanism '{concurrency_mechanism}' is not supported")
+
+        if concurrency_mechanism == "multiprocessing" and pass_context:
+            try:
+                pickle.dumps(self.context)
+            except Exception as ex:
+                raise ValueError(
+                    'When concurrency_mechanism="multiprocessing" is used in conjunction with '
+                    "pass_context=True, context must be serializable"
+                ) from ex
+
+        self._executor = None
+        if concurrency_mechanism == "threading":
+            self._executor = ThreadPoolExecutor(max_workers=self._max_in_flight)
+        elif concurrency_mechanism == "multiprocessing":
+            self._executor = ProcessPoolExecutor(max_workers=self._max_in_flight)
+
+        self._pass_context = pass_context
+
+    async def _process_event(self, event):
+        args = [event]
+        if self._pass_context:
+            args.append(self.context)
+        if self._executor:
+            result = await asyncio.get_running_loop().run_in_executor(self._executor, self._event_processor, *args)
+        else:
+            result = self._event_processor(*args)
+        if asyncio.iscoroutine(result):
+            result = await result
+        return result
+
+    async def _handle_completed(self, event, response):
+        await self._do_downstream(response)
+
+
 class SendToHttp(_ConcurrentJobExecution):
     """Joins each event with data from any HTTP source. Used for event augmentation.
 
     :param request_builder: Creates an HTTP request from the event. This request is then sent to its destination.
     :type request_builder: Function (Event=>HttpRequest)
     :param join_from_response: Joins the original event with the HTTP response into a new event.
     :type join_from_response: Function ((Event, HttpResponse)=>Event)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `storey-1.7.8/storey/queue.py` & `storey-1.7.9/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/redis_driver.py` & `storey-1.7.9/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/sources.py` & `storey-1.7.9/storey/sources.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/sql_driver.py` & `storey-1.7.9/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/steps/__init__.py` & `storey-1.7.9/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/steps/assertion.py` & `storey-1.7.9/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/steps/flatten.py` & `storey-1.7.9/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/steps/foreach.py` & `storey-1.7.9/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/steps/partition.py` & `storey-1.7.9/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/steps/sample.py` & `storey-1.7.9/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/table.py` & `storey-1.7.9/storey/table.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/targets.py` & `storey-1.7.9/storey/targets.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/transformations/__init__.py` & `storey-1.7.9/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/utils.py` & `storey-1.7.9/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey/windowed_store.py` & `storey-1.7.9/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/storey.egg-info/PKG-INFO` & `storey-1.7.9/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.7.8
+Version: 1.7.9
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.7.8/storey.egg-info/SOURCES.txt` & `storey-1.7.9/storey.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 storey/steps/foreach.py
 storey/steps/partition.py
 storey/steps/sample.py
 storey/transformations/__init__.py
 tests/__init__.py
 tests/test_aggregate_by_key.py
 tests/test_aggregate_store.py
+tests/test_concurrent_execution.py
 tests/test_flow.py
 tests/test_queue.py
 tests/test_steps.py
 tests/test_types.py
 tests/test_utils.py
 tests/test_v3io.py
 tests/test_windowed_store.py
```

### Comparing `storey-1.7.8/tests/__init__.py` & `storey-1.7.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_aggregate_by_key.py` & `storey-1.7.9/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_aggregate_store.py` & `storey-1.7.9/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_flow.py` & `storey-1.7.9/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_queue.py` & `storey-1.7.9/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_steps.py` & `storey-1.7.9/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_types.py` & `storey-1.7.9/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_utils.py` & `storey-1.7.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_v3io.py` & `storey-1.7.9/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.8/tests/test_windowed_store.py` & `storey-1.7.9/tests/test_windowed_store.py`

 * *Files identical despite different names*

