# Comparing `tmp/telicent_lib-2.0.1.tar.gz` & `tmp/telicent_lib-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telicent_lib-2.0.1.tar", last modified: Thu May  9 13:18:46 2024, max compression
+gzip compressed data, was "telicent_lib-2.0.2.tar", last modified: Wed May 22 14:36:34 2024, max compression
```

## Comparing `telicent_lib-2.0.1.tar` & `telicent_lib-2.0.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.580571 telicent_lib-2.0.1/telicent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/access/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/edhv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/edhv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/security_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/access/ukihm/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/ukihm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/ukihm/edh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/config/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/config/configSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/config/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/middleware/decode_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/projector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/dataSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/dictSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/kafkaSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/listSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.588571 telicent_lib-2.0.1/telicent_lib/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/dataSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/dictSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/kafkaSource.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/listSource.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/telicent_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_decode_token_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_edh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_generate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_protocol_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_security_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_security_labels_edhv1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_serdes.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:34.002628 telicent_lib-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-22 14:36:34.002628 telicent_lib-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:36:34.002628 telicent_lib-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/access/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/edhv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/edhv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/security_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/access/ukihm/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/ukihm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/ukihm/edh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/config/configSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/config/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/middleware/decode_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-05-22 14:36:30.000000 telicent_lib-2.0.2/telicent_lib/sbom.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/telicent_lib/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/dataSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/dictSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/kafkaSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/listSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/telicent_lib/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/dataSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/dictSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/kafkaSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/listSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/telicent_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_decode_token_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_edh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_generate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_protocol_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_security_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_security_labels_edhv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_serdes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_sources.py
```

### Comparing `telicent_lib-2.0.1/LICENSE` & `telicent_lib-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/PKG-INFO` & `telicent_lib-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-lib
-Version: 2.0.1
+Version: 2.0.2
 Summary: A helper package for building Adapters, Mappers and Projectors for Telicent Core
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,40 +218,41 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: colored==1.4.4
 Requires-Dist: rdflib==6.3.2
-Requires-Dist: Werkzeug==3.0.1
+Requires-Dist: Werkzeug==3.0.3
 Requires-Dist: PyJWT==2.8.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: pytz==2022.6
 Requires-Dist: confluent-kafka==2.3.0
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: pydantic==2.5.2
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: ruff==0.1.5; extra == "dev"
 Requires-Dist: types-pytz==2023.3.1.1; extra == "dev"
 Requires-Dist: types-requests==2.31.0.10; extra == "dev"
 Requires-Dist: mypy==1.7.0; extra == "dev"
 Requires-Dist: mkdocs==1.5.3; extra == "dev"
+Requires-Dist: cyclonedx-bom==4.4.3; extra == "dev"
 
 # telicent-lib
 
 telicent-lib provides useful helper libraries for building Adaptors, Mappers and Projectors for the Telicent Core Platform.
 
 ## Dependencies
 
 - Python \>=3.10
 - Kafka*
 
-maplib uses `confluent-kafka` to manage connections to Kafka. 
+telicent-lib uses `confluent-kafka` to manage connections to Kafka. 
 Please see [confluent-kafka's compatability documentation](https://docs.confluent.io/platform/current/installation/versions-interoperability.html) to ensure you have a compatible Kafka instance.
 
 
 ## Installation
 
 ```shell
 pip install telicent-lib
```

### Comparing `telicent_lib-2.0.1/README.md` & `telicent_lib-2.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 telicent-lib provides useful helper libraries for building Adaptors, Mappers and Projectors for the Telicent Core Platform.
 
 ## Dependencies
 
 - Python \>=3.10
 - Kafka*
 
-maplib uses `confluent-kafka` to manage connections to Kafka. 
+telicent-lib uses `confluent-kafka` to manage connections to Kafka. 
 Please see [confluent-kafka's compatability documentation](https://docs.confluent.io/platform/current/installation/versions-interoperability.html) to ensure you have a compatible Kafka instance.
 
 
 ## Installation
 
 ```shell
 pip install telicent-lib
```

### Comparing `telicent_lib-2.0.1/pyproject.toml` & `telicent_lib-2.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.2.0", "wheel==0.41.3", "pip-tools==7.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "telicent-lib"
-version = "2.0.1"
+version = "2.0.2"
 authors = [{name = "Telicent Ltd", email = "admin@telicent.io"}]
 description = "A helper package for building Adapters, Mappers and Projectors for Telicent Core"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
     "colored==1.4.4",
     "rdflib==6.3.2",
-    "Werkzeug==3.0.1",
+    "Werkzeug==3.0.3",
     "PyJWT==2.8.0",
     "requests==2.31.0",
     "pytz==2022.6",
     "confluent-kafka==2.3.0",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
-    "pydantic==2.5.2"
+    "pydantic==2.5.2",
 ]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
@@ -39,14 +39,15 @@
 dev = [
     "pre-commit==3.5.0",
     "ruff==0.1.5",
     "types-pytz==2023.3.1.1",
     "types-requests==2.31.0.10",
     "mypy==1.7.0",
     "mkdocs==1.5.3",
+    "cyclonedx-bom==4.4.3"
 ]
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"]}
 
 [tool.ruff]
 target-version = "py38"
@@ -96,11 +97,14 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["telicent_lib*"]
 namespaces = true
 
+[tool.setuptools.package-data]
+"telicent_lib" = ["sbom.json"]
+
 [tool.mypy]
 no_implicit_optional = false
 ignore_missing_imports = true
 modules = ["telicent_lib", "tests", "debug"]
```

### Comparing `telicent_lib-2.0.1/telicent_lib/__init__.py` & `telicent_lib-2.0.2/telicent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/access/__init__.py` & `telicent_lib-2.0.2/telicent_lib/access/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/access/edhv1.py` & `telicent_lib-2.0.2/telicent_lib/access/edhv1.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/access/edhv2.py` & `telicent_lib-2.0.2/telicent_lib/access/edhv2.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/access/security_labels.py` & `telicent_lib-2.0.2/telicent_lib/access/security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/access/ukihm/__init__.py` & `telicent_lib-2.0.2/telicent_lib/access/ukihm/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/access/ukihm/edh_model.py` & `telicent_lib-2.0.2/telicent_lib/access/ukihm/edh_model.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/action.py` & `telicent_lib-2.0.2/telicent_lib/action.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/adapter.py` & `telicent_lib-2.0.2/telicent_lib/adapter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/config/__init__.py` & `telicent_lib-2.0.2/telicent_lib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/config/configSource.py` & `telicent_lib-2.0.2/telicent_lib/config/configSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/config/configurator.py` & `telicent_lib-2.0.2/telicent_lib/config/configurator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import sys
 from enum import Enum
 from typing import Any, Callable
 
 from telicent_lib.config.configSource import ConfigSource, EnvironmentSource
 
 __license__ = """
@@ -16,14 +17,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+logger = logging.getLogger(__name__)
 
 class OnError(Enum):
     """
     Possible on error behaviours.
 
     There is `RAISE_EXCEPTION` to raise en exception and `EXIT` to exit the program.
     """
@@ -52,15 +54,15 @@
         if not isinstance(config_source, ConfigSource):
             raise TypeError('Not provided with a valid ConfigSource')
 
         self.exit_code = exit_code
         self.debug = debug
         self.source = config_source
         if self.debug:
-            print(f"Configuration Source is {str(self.source)}")
+            logger.debug(f"Configuration Source is {str(self.source)}")
 
     @staticmethod
     def string_to_bool(value):
         if value.lower() == 'true':
             return True
         elif value.lower() == 'false':
             return False
@@ -101,28 +103,28 @@
         :return: Configuration value
         :raises ValueError:
             Raised if a suitable configuration value is not provided and `on_error` was `OnError.RAISE_EXCEPTION`
         """
         value: Any = None
         raw_value = self.source.get(config_key)
         if self.debug:
-            print(f"Raw Value for Configuration Key {config_key} is {raw_value}")
+            logger.debug(f"Raw Value for Configuration Key {config_key} is {raw_value}")
 
         if raw_value is None:
             raw_value = default
             if self.debug and default is not None:
-                print(f"Using default value {default}")
+                logger.debug(f"Using default value {default}")
             if raw_value is None and required:
                 self.__handle_errors__(f"Required Configuration Key {config_key} is not set.  {description}", on_error)
 
         if converter is not None:
             try:
                 value = converter(raw_value)
                 if self.debug:
-                    print(f"Converted raw value {raw_value} into typed value {value} with type {type(value)}")
+                    logger.debug(f"Converted raw value {raw_value} into typed value {value} with type {type(value)}")
             except Exception as e:
                 self.__handle_errors__(
                     f"Configuration Key {config_key} has raw value {raw_value} that failed value conversion: {e}",
                     on_error)
         else:
             value = raw_value
 
@@ -139,11 +141,12 @@
         """
         Handles configuration errors
 
         :param message: Error message
         :param on_error: On Error behaviour
         """
         if on_error is OnError.EXIT:
-            print(message)
+            logger.critical(message)
             sys.exit(self.exit_code)
         else:
             raise ValueError(message)
+
```

### Comparing `telicent_lib-2.0.1/telicent_lib/errors.py` & `telicent_lib-2.0.2/telicent_lib/errors.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/exceptions.py` & `telicent_lib-2.0.2/telicent_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/logging.py` & `telicent_lib-2.0.2/telicent_lib/logging.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/mapper.py` & `telicent_lib-2.0.2/telicent_lib/mapper.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/middleware/__init__.py` & `telicent_lib-2.0.2/telicent_lib/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/middleware/decode_token.py` & `telicent_lib-2.0.2/telicent_lib/middleware/decode_token.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/projector.py` & `telicent_lib-2.0.2/telicent_lib/projector.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/records.py` & `telicent_lib-2.0.2/telicent_lib/records.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/reporter.py` & `telicent_lib-2.0.2/telicent_lib/reporter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sinks/__init__.py` & `telicent_lib-2.0.2/telicent_lib/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sinks/dataSink.py` & `telicent_lib-2.0.2/telicent_lib/sinks/dataSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sinks/dictSink.py` & `telicent_lib-2.0.2/telicent_lib/sinks/dictSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sinks/kafkaSink.py` & `telicent_lib-2.0.2/telicent_lib/sinks/kafkaSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sinks/listSink.py` & `telicent_lib-2.0.2/telicent_lib/sinks/listSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sinks/serializers.py` & `telicent_lib-2.0.2/telicent_lib/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sources/dataSource.py` & `telicent_lib-2.0.2/telicent_lib/sources/dataSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sources/deserializers.py` & `telicent_lib-2.0.2/telicent_lib/sources/deserializers.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sources/dictSource.py` & `telicent_lib-2.0.2/telicent_lib/sources/dictSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sources/kafkaSource.py` & `telicent_lib-2.0.2/telicent_lib/sources/kafkaSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/sources/listSource.py` & `telicent_lib-2.0.2/telicent_lib/sources/listSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/status.py` & `telicent_lib-2.0.2/telicent_lib/status.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib/utils.py` & `telicent_lib-2.0.2/telicent_lib/utils.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/telicent_lib.egg-info/PKG-INFO` & `telicent_lib-2.0.2/telicent_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-lib
-Version: 2.0.1
+Version: 2.0.2
 Summary: A helper package for building Adapters, Mappers and Projectors for Telicent Core
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,40 +218,41 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: colored==1.4.4
 Requires-Dist: rdflib==6.3.2
-Requires-Dist: Werkzeug==3.0.1
+Requires-Dist: Werkzeug==3.0.3
 Requires-Dist: PyJWT==2.8.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: pytz==2022.6
 Requires-Dist: confluent-kafka==2.3.0
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: pydantic==2.5.2
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: ruff==0.1.5; extra == "dev"
 Requires-Dist: types-pytz==2023.3.1.1; extra == "dev"
 Requires-Dist: types-requests==2.31.0.10; extra == "dev"
 Requires-Dist: mypy==1.7.0; extra == "dev"
 Requires-Dist: mkdocs==1.5.3; extra == "dev"
+Requires-Dist: cyclonedx-bom==4.4.3; extra == "dev"
 
 # telicent-lib
 
 telicent-lib provides useful helper libraries for building Adaptors, Mappers and Projectors for the Telicent Core Platform.
 
 ## Dependencies
 
 - Python \>=3.10
 - Kafka*
 
-maplib uses `confluent-kafka` to manage connections to Kafka. 
+telicent-lib uses `confluent-kafka` to manage connections to Kafka. 
 Please see [confluent-kafka's compatability documentation](https://docs.confluent.io/platform/current/installation/versions-interoperability.html) to ensure you have a compatible Kafka instance.
 
 
 ## Installation
 
 ```shell
 pip install telicent-lib
```

### Comparing `telicent_lib-2.0.1/telicent_lib.egg-info/SOURCES.txt` & `telicent_lib-2.0.2/telicent_lib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 telicent_lib/errors.py
 telicent_lib/exceptions.py
 telicent_lib/logging.py
 telicent_lib/mapper.py
 telicent_lib/projector.py
 telicent_lib/records.py
 telicent_lib/reporter.py
+telicent_lib/sbom.json
 telicent_lib/status.py
 telicent_lib/utils.py
 telicent_lib.egg-info/PKG-INFO
 telicent_lib.egg-info/SOURCES.txt
 telicent_lib.egg-info/dependency_links.txt
 telicent_lib.egg-info/requires.txt
 telicent_lib.egg-info/top_level.txt
```

### Comparing `telicent_lib-2.0.1/tests/test_adapter.py` & `telicent_lib-2.0.2/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_decode_token_middleware.py` & `telicent_lib-2.0.2/tests/test_decode_token_middleware.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_edh_model.py` & `telicent_lib-2.0.2/tests/test_edh_model.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_error_handler.py` & `telicent_lib-2.0.2/tests/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_generate_ids.py` & `telicent_lib-2.0.2/tests/test_generate_ids.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_mapper.py` & `telicent_lib-2.0.2/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_projector.py` & `telicent_lib-2.0.2/tests/test_projector.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_protocol_validation.py` & `telicent_lib-2.0.2/tests/test_protocol_validation.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_records.py` & `telicent_lib-2.0.2/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_reporter.py` & `telicent_lib-2.0.2/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_security_labels.py` & `telicent_lib-2.0.2/tests/test_security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_security_labels_edhv1.py` & `telicent_lib-2.0.2/tests/test_security_labels_edhv1.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_serdes.py` & `telicent_lib-2.0.2/tests/test_serdes.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_sinks.py` & `telicent_lib-2.0.2/tests/test_sinks.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.1/tests/test_sources.py` & `telicent_lib-2.0.2/tests/test_sources.py`

 * *Files identical despite different names*

