# Comparing `tmp/Aruna-Python-API-2.0.0b8.tar.gz` & `tmp/Aruna-Python-API-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-2.0.0b8.tar", last modified: Tue Nov 14 20:32:31 2023, max compression
+gzip compressed data, was "Aruna-Python-API-2.0.0b9.tar", last modified: Wed Nov 22 13:24:13 2023, max compression
```

## Comparing `Aruna-Python-API-2.0.0b8.tar` & `Aruna-Python-API-2.0.0b9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.398836 Aruna-Python-API-2.0.0b8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.386836 Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-11-14 20:32:31.000000 Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2023-11-14 20:32:31.000000 Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 20:32:31.000000 Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-14 20:32:31.000000 Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-14 20:32:31.000000 Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-14 20:32:13.000000 Aruna-Python-API-2.0.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-11-14 20:32:31.398836 Aruna-Python-API-2.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-11-14 20:32:13.000000 Aruna-Python-API-2.0.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.386836 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/bundler_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/bundler_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/bundler_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35250 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/dataproxy_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/hooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.386836 Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/hooks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/hooks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/hooks_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/notification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/notification/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.386836 Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12703 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/storage/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.390836 Aruna-Python-API-2.0.0b8/aruna/api/storage/models/v2/
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/models/v2/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27496 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/models/v2/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/models/v2/models_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.382836 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:32:31.394836 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/authorization_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/authorization_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/authorization_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13107 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22532 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/data_replication_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/data_replication_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/data_replication_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/dataset_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/dataset_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21805 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/dataset_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/license_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/license_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/license_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20093 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/relations_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/relations_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/relations_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/search_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/search_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/search_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24443 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21612 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    41903 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/workspace_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/workspace_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/workspace_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-14 20:32:31.398836 Aruna-Python-API-2.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-11-14 20:32:23.000000 Aruna-Python-API-2.0.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.431083 Aruna-Python-API-2.0.0b9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.431083 Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-11-22 13:24:13.000000 Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2023-11-22 13:24:13.000000 Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 13:24:13.000000 Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-22 13:24:13.000000 Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-22 13:24:13.000000 Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-22 13:23:50.000000 Aruna-Python-API-2.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-11-22 13:24:13.431083 Aruna-Python-API-2.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-11-22 13:23:50.000000 Aruna-Python-API-2.0.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.415083 Aruna-Python-API-2.0.0b9/aruna/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.415083 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.415083 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/bundler_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/bundler_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/bundler_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35369 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/dataproxy_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/hooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.423083 Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/hooks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/hooks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/hooks_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/notification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/notification/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.423083 Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/storage/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.423083 Aruna-Python-API-2.0.0b9/aruna/api/storage/models/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18699 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/models/v2/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27629 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/models/v2/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/models/v2/models_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.419083 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:24:13.431083 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/authorization_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/authorization_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/authorization_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13107 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22586 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/data_replication_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/data_replication_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/data_replication_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/dataset_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/dataset_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21805 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/dataset_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/license_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/license_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/license_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20240 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/relations_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/relations_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/relations_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/search_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/search_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/search_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24291 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21615 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    41948 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/workspace_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/workspace_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2023-11-22 13:24:03.000000 Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/workspace_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-22 13:24:13.431083 Aruna-Python-API-2.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-11-22 13:24:04.000000 Aruna-Python-API-2.0.0b9/setup.py
```

### Comparing `Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Sebastian Beyvers, Jannis Hochmuth, Lukas Brehm
 Author-email: sebastian.beyvers@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de, lukas.brehm@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-2.0.0b8/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-2.0.0b9/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/LICENSE` & `Aruna-Python-API-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/PKG-INFO` & `Aruna-Python-API-2.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Sebastian Beyvers, Jannis Hochmuth, Lukas Brehm
 Author-email: sebastian.beyvers@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de, lukas.brehm@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-2.0.0b8/README.md` & `Aruna-Python-API-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/bundler_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/bundler_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/dataproxy/services/v2/bundler_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/bundler_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/bundler_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/bundler_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/bundler_service_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from aruna.api.dataproxy.services.v2 import bundler_service_pb2 as aruna_dot_api_dot_dataproxy_dot_services_dot_v2_dot_bundler__service__pb2
 
 
 class BundlerServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
+    """BundlerService
+
+    Status: ALPHA
+
+    Dataproxy specific service for creating and deleting bundles.
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
@@ -23,24 +28,39 @@
                 '/aruna.api.dataproxy.services.v2.BundlerService/DeleteBundle',
                 request_serializer=aruna_dot_api_dot_dataproxy_dot_services_dot_v2_dot_bundler__service__pb2.DeleteBundleRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_dataproxy_dot_services_dot_v2_dot_bundler__service__pb2.DeleteBundleResponse.FromString,
                 )
 
 
 class BundlerServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
+    """BundlerService
+
+    Status: ALPHA
+
+    Dataproxy specific service for creating and deleting bundles.
+    """
 
     def CreateBundle(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """CreateBundle
+
+        Status: ALPHA
+
+        Creates a bundle with multiple resources, dataproxy only.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteBundle(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """DeleteBundle
+
+        Status: ALPHA
+
+        Delete an existing bundle, dataproxy only.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_BundlerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -58,15 +78,20 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.dataproxy.services.v2.BundlerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class BundlerService(object):
-    """Missing associated documentation comment in .proto file."""
+    """BundlerService
+
+    Status: ALPHA
+
+    Dataproxy specific service for creating and deleting bundles.
+    """
 
     @staticmethod
     def CreateBundle(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/dataproxy/services/v2/dataproxy_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/dataproxy_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/dataproxy/services/v2/dataproxy_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/dataproxy/services/v2/dataproxy_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from aruna.api.dataproxy.services.v2 import dataproxy_service_pb2 as aruna_dot_api_dot_dataproxy_dot_services_dot_v2_dot_dataproxy__service__pb2
 
 
 class DataproxyServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
+    """DataproxyService
+
+    Status: ALPHA
+
+    Service for data replication between data-proxies
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
@@ -23,31 +28,36 @@
                 '/aruna.api.dataproxy.services.v2.DataproxyService/InitReplication',
                 request_serializer=aruna_dot_api_dot_dataproxy_dot_services_dot_v2_dot_dataproxy__service__pb2.InitReplicationRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_dataproxy_dot_services_dot_v2_dot_dataproxy__service__pb2.InitReplicationResponse.FromString,
                 )
 
 
 class DataproxyServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
+    """DataproxyService
+
+    Status: ALPHA
+
+    Service for data replication between data-proxies
+    """
 
     def RequestReplication(self, request, context):
         """RequestReplication
 
-        Status: BETA
+        Status: ALPHA
 
         Creates a replication request
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def InitReplication(self, request, context):
         """InitReplication
 
-        Status: BETA
+        Status: ALPHA
 
         Provides the necessary url to init replication
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -68,15 +78,20 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.dataproxy.services.v2.DataproxyService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class DataproxyService(object):
-    """Missing associated documentation comment in .proto file."""
+    """DataproxyService
+
+    Status: ALPHA
+
+    Service for data replication between data-proxies
+    """
 
     @staticmethod
     def RequestReplication(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/hooks_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/hooks_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/hooks/services/v2/hooks_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/hooks_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/hooks_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/hooks/services/v2/hooks_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/hooks/services/v2/hooks_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,46 +56,77 @@
 
     Status: ALPHA
 
     A service that enables automatic Hook scheduling
     """
 
     def CreateHook(self, request, context):
-        """Created Hooks are always associated with the owner that creates the hook
+        """CreateHook
+
+        Status: ALPHA
+
+        Creates a replication request
+        Hooks are always associated with the owner that created the hook
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def AddProjectsToHook(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """AddProjectsToHook
+
+        Status: ALPHA
+
+        Assigns a hook to a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListProjectHooks(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """ListProjectHooks
+
+        Status: ALPHA
+
+        List all hooks assigned to a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListOwnedHooks(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """ListOwnedHooks
+
+        Status: ALPHA
+
+        List all hooks created by a user
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteHook(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """DeleteHook
+
+        Status: ALPHA
+
+        Delete a hook by id
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def HookCallback(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Callback API
+
+        Status: ALPHA
+
+        Externally triggered hooks should respond to this endpoint to
+        signal completion or failure and to provide additional flags for the object
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_HooksServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/notification_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/notification_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/notification/services/v2/notification_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/notification_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/notification/services/v2/notification_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/notification/services/v2/notification_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from aruna.api.notification.services.v2 import notification_service_pb2 as aruna_dot_api_dot_notification_dot_services_dot_v2_dot_notification__service__pb2
 
 
 class EventNotificationServiceStub(object):
     """EventNotificationService
 
-    A service to receive events in the AOS storage
+    Status: BETA
+
+    A service to receive events for CRUD operations on resources (users, resources etc.)
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -43,61 +45,73 @@
                 response_deserializer=aruna_dot_api_dot_notification_dot_services_dot_v2_dot_notification__service__pb2.DeleteStreamConsumerResponse.FromString,
                 )
 
 
 class EventNotificationServiceServicer(object):
     """EventNotificationService
 
-    A service to receive events in the AOS storage
+    Status: BETA
+
+    A service to receive events for CRUD operations on resources (users, resources etc.)
     """
 
     def CreateStreamConsumer(self, request, context):
         """CreateStreamConsumer
 
+        Status: BETA
+
         Creates a new event stream consumer.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetEventMessageBatch(self, request, context):
         """GetEventMessageBatch
 
+        Status: BETA
+
         Reads a set of messages from a given stream group 
         Each message contains a separate acknowledgement message thatis protected by a salt and an hmac for verification.
         The message can be send directly through the AcknowledgeMessageBatch call to acknowledge the message.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetEventMessageStream(self, request, context):
         """GetEventMessageBatch
 
+        Status: BETA
+
         Opens a stream which pushes each received notification individual and just-in-time.
         Each message contains a separate acknowledgement message that is protected by a salt and an hmac for verification.
         The message can be send directly through the AcknowledgeMessageBatch call to acknowledge the message.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def AcknowledgeMessageBatch(self, request, context):
         """AcknowledgeMessageBatch
 
+        Status: BETA
+
         List of messages to acknowledge
         Each reply is protected by a salt and and hmac that verifies the message
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteStreamConsumer(self, request, context):
         """DeleteEventStreamingGroup
 
+        Status: BETA
+
         Deletes an existing event stream consumer by ID.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -134,15 +148,17 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class EventNotificationService(object):
     """EventNotificationService
 
-    A service to receive events in the AOS storage
+    Status: BETA
+
+    A service to receive events for CRUD operations on resources (users, resources etc.)
     """
 
     @staticmethod
     def CreateStreamConsumer(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/models/v2/models_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/models/v2/models_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/models/v2/models.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/storage/models/v2/models.proto\x12\x1b\x61runa.api.storage.models.v2\x1a\x1fgoogle/protobuf/timestamp.proto\"\xba\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x14\n\x05\x65mail\x18\x05 \x01(\tR\x05\x65mail\x12K\n\nattributes\x18\x06 \x01(\x0b\x32+.aruna.api.storage.models.v2.UserAttributesR\nattributesJ\x04\x08\x02\x10\x03\"\xfc\x01\n\nPermission\x12\x1f\n\nproject_id\x18\x01 \x01(\tH\x00R\tprojectId\x12%\n\rcollection_id\x18\x02 \x01(\tH\x00R\x0c\x63ollectionId\x12\x1f\n\ndataset_id\x18\x03 \x01(\tH\x00R\tdatasetId\x12\x1d\n\tobject_id\x18\x04 \x01(\tH\x00R\x08objectId\x12W\n\x10permission_level\x18\x06 \x01(\x0e\x32,.aruna.api.storage.models.v2.PermissionLevelR\x0fpermissionLevelB\r\n\x0bresource_id\"\xea\x01\n\x05Token\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x39\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12G\n\npermission\x18\x05 \x01(\x0b\x32\'.aruna.api.storage.models.v2.PermissionR\npermission\"F\n\x06Pubkey\x12\x0e\n\x02id\x18\x01 \x01(\x05R\x02id\x12\x10\n\x03key\x18\x02 \x01(\tR\x03key\x12\x1a\n\x08location\x18\x03 \x01(\tR\x08location\"b\n\x10\x43ustomAttributes\x12%\n\x0e\x61ttribute_name\x18\x01 \x01(\tR\rattributeName\x12\'\n\x0f\x61ttribute_value\x18\x02 \x01(\tR\x0e\x61ttributeValue\"I\n\x0bOidcMapping\x12\x1f\n\x0b\x65xternal_id\x18\x01 \x01(\tR\nexternalId\x12\x19\n\x08oidc_url\x18\x02 \x01(\tR\x07oidcUrl\"\xca\x03\n\x0eUserAttributes\x12!\n\x0cglobal_admin\x18\x01 \x01(\x08R\x0bglobalAdmin\x12\'\n\x0fservice_account\x18\x02 \x01(\x08R\x0eserviceAccount\x12:\n\x06tokens\x18\x03 \x03(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x06tokens\x12+\n\x11trusted_endpoints\x18\x04 \x03(\tR\x10trustedEndpoints\x12Z\n\x11\x63ustom_attributes\x18\x05 \x03(\x0b\x32-.aruna.api.storage.models.v2.CustomAttributesR\x10\x63ustomAttributes\x12Z\n\x14personal_permissions\x18\x06 \x03(\x0b\x32\'.aruna.api.storage.models.v2.PermissionR\x13personalPermissions\x12K\n\x0c\x65xternal_ids\x18\x07 \x03(\x0b\x32(.aruna.api.storage.models.v2.OidcMappingR\x0b\x65xternalIds\"z\n\x08KeyValue\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x12\x46\n\x07variant\x18\x03 \x01(\x0e\x32,.aruna.api.storage.models.v2.KeyValueVariantR\x07variant\"\xb0\x01\n\x08Relation\x12K\n\x08\x65xternal\x18\x01 \x01(\x0b\x32-.aruna.api.storage.models.v2.ExternalRelationH\x00R\x08\x65xternal\x12K\n\x08internal\x18\x02 \x01(\x0b\x32-.aruna.api.storage.models.v2.InternalRelationH\x00R\x08internalB\n\n\x08relation\"\xd0\x01\n\x10\x45xternalRelation\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12]\n\x0f\x64\x65\x66ined_variant\x18\x02 \x01(\x0e\x32\x34.aruna.api.storage.models.v2.ExternalRelationVariantR\x0e\x64\x65\x66inedVariant\x12*\n\x0e\x63ustom_variant\x18\x03 \x01(\tH\x00R\rcustomVariant\x88\x01\x01\x42\x11\n\x0f_custom_variant\"\xf8\x02\n\x10InternalRelation\x12\x1f\n\x0bresource_id\x18\x01 \x01(\tR\nresourceId\x12W\n\x10resource_variant\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.ResourceVariantR\x0fresourceVariant\x12]\n\x0f\x64\x65\x66ined_variant\x18\x03 \x01(\x0e\x32\x34.aruna.api.storage.models.v2.InternalRelationVariantR\x0e\x64\x65\x66inedVariant\x12*\n\x0e\x63ustom_variant\x18\x04 \x01(\tH\x00R\rcustomVariant\x88\x01\x01\x12L\n\tdirection\x18\x05 \x01(\x0e\x32..aruna.api.storage.models.v2.RelationDirectionR\tdirectionB\x11\n\x0f_custom_variant\"K\n\x0bPageRequest\x12\x1f\n\x0bstart_after\x18\x01 \x01(\tR\nstartAfter\x12\x1b\n\tpage_size\x18\x02 \x01(\x03R\x08pageSize\"p\n\x05Stats\x12\x14\n\x05\x63ount\x18\x01 \x01(\x03R\x05\x63ount\x12\x12\n\x04size\x18\x02 \x01(\x03R\x04size\x12=\n\x0clast_updated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"X\n\x04Hash\x12<\n\x03\x61lg\x18\x01 \x01(\x0e\x32*.aruna.api.storage.models.v2.HashalgorithmR\x03\x61lg\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\"\xc4\x01\n\x12\x45ndpointHostConfig\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\x12\x1d\n\nis_primary\x18\x02 \x01(\x08R\tisPrimary\x12\x10\n\x03ssl\x18\x03 \x01(\x08R\x03ssl\x12\x16\n\x06public\x18\x04 \x01(\x08R\x06public\x12S\n\x0chost_variant\x18\x05 \x01(\x0e\x32\x30.aruna.api.storage.models.v2.EndpointHostVariantR\x0bhostVariant\"\xb2\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12K\n\nep_variant\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.EndpointVariantR\tepVariant\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12\x44\n\x06status\x18\x05 \x01(\x0e\x32,.aruna.api.storage.models.v2.ComponentStatusR\x06status\x12R\n\x0chost_configs\x18\x06 \x03(\x0b\x32/.aruna.api.storage.models.v2.EndpointHostConfigR\x0bhostConfigs\"?\n\x0c\x44\x61taEndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x66ull_synced\x18\x02 \x01(\x08R\nfullSynced\"_\n\x04\x43opy\x12\x1a\n\x08resource\x18\x01 \x01(\tR\x08resource\x12\'\n\x0ftarget_endpoint\x18\x02 \x01(\tR\x0etargetEndpoint\x12\x12\n\x04push\x18\x03 \x01(\x08R\x04push\"v\n\x07\x43ontext\x12\'\n\x0es3_credentials\x18\x01 \x01(\x08H\x00R\rs3Credentials\x12\x37\n\x04\x63opy\x18\x02 \x01(\x0b\x32!.aruna.api.storage.models.v2.CopyH\x00R\x04\x63opyB\t\n\x07\x63ontext\"U\n\x07License\x12\x10\n\x03tag\x18\x01 \x01(\tR\x03tag\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x12\n\x04text\x18\x03 \x01(\tR\x04text\x12\x10\n\x03url\x18\x04 \x01(\tR\x03url\"\xab\x02\n\x0fGenericResource\x12@\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectH\x00R\x07project\x12I\n\ncollection\x18\x02 \x01(\x0b\x32\'.aruna.api.storage.models.v2.CollectionH\x00R\ncollection\x12@\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32$.aruna.api.storage.models.v2.DatasetH\x00R\x07\x64\x61taset\x12=\n\x06object\x18\x04 \x01(\x0b\x32#.aruna.api.storage.models.v2.ObjectH\x00R\x06objectB\n\n\x08resource\"\xc0\x05\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x38\n\x05stats\x18\x06 \x01(\x0b\x32\".aruna.api.storage.models.v2.StatsR\x05stats\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x30\n\x14metadata_license_tag\x18\r \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x0e \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"\xc3\x05\n\nCollection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x38\n\x05stats\x18\x06 \x01(\x0b\x32\".aruna.api.storage.models.v2.StatsR\x05stats\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x30\n\x14metadata_license_tag\x18\r \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x0e \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"\xc0\x05\n\x07\x44\x61taset\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x38\n\x05stats\x18\x06 \x01(\x0b\x32\".aruna.api.storage.models.v2.StatsR\x05stats\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x30\n\x14metadata_license_tag\x18\r \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x0e \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"\xd2\x05\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x1f\n\x0b\x63ontent_len\x18\x06 \x01(\x03R\ncontentLen\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x39\n\x06hashes\x18\r \x03(\x0b\x32!.aruna.api.storage.models.v2.HashR\x06hashes\x12\x30\n\x14metadata_license_tag\x18\x0e \x01(\tR\x12metadataLicenseTag\x12(\n\x10\x64\x61ta_license_tag\x18\x0f \x01(\tR\x0e\x64\x61taLicenseTag*\x8d\x01\n\tDataClass\x12\x1a\n\x16\x44\x41TA_CLASS_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44\x41TA_CLASS_PUBLIC\x10\x01\x12\x16\n\x12\x44\x41TA_CLASS_PRIVATE\x10\x02\x12\x18\n\x14\x44\x41TA_CLASS_WORKSPACE\x10\x04\x12\x1b\n\x17\x44\x41TA_CLASS_CONFIDENTIAL\x10\x05*s\n\x0f\x45ndpointVariant\x12 \n\x1c\x45NDPOINT_VARIANT_UNSPECIFIED\x10\x00\x12\x1f\n\x1b\x45NDPOINT_VARIANT_PERSISTENT\x10\x01\x12\x1d\n\x19\x45NDPOINT_VARIANT_VOLATILE\x10\x02*z\n\x13\x45ndpointHostVariant\x12%\n!ENDPOINT_HOST_VARIANT_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45NDPOINT_HOST_VARIANT_GRPC\x10\x01\x12\x1c\n\x18\x45NDPOINT_HOST_VARIANT_S3\x10\x02*\xbe\x01\n\x0fPermissionLevel\x12 \n\x1cPERMISSION_LEVEL_UNSPECIFIED\x10\x00\x12\x19\n\x15PERMISSION_LEVEL_NONE\x10\x02\x12\x19\n\x15PERMISSION_LEVEL_READ\x10\x03\x12\x1b\n\x17PERMISSION_LEVEL_APPEND\x10\x04\x12\x1a\n\x16PERMISSION_LEVEL_WRITE\x10\x05\x12\x1a\n\x16PERMISSION_LEVEL_ADMIN\x10\x06*\xb4\x01\n\x0fKeyValueVariant\x12!\n\x1dKEY_VALUE_VARIANT_UNSPECIFIED\x10\x00\x12\x1b\n\x17KEY_VALUE_VARIANT_LABEL\x10\x01\x12\"\n\x1eKEY_VALUE_VARIANT_STATIC_LABEL\x10\x02\x12\x1a\n\x16KEY_VALUE_VARIANT_HOOK\x10\x03\x12!\n\x1dKEY_VALUE_VARIANT_HOOK_STATUS\x10\x04*\xb7\x01\n\x17\x45xternalRelationVariant\x12)\n%EXTERNAL_RELATION_VARIANT_UNSPECIFIED\x10\x00\x12!\n\x1d\x45XTERNAL_RELATION_VARIANT_URL\x10\x01\x12(\n$EXTERNAL_RELATION_VARIANT_IDENTIFIER\x10\x02\x12$\n EXTERNAL_RELATION_VARIANT_CUSTOM\x10\x03*\xaf\x02\n\x17InternalRelationVariant\x12)\n%INTERNAL_RELATION_VARIANT_UNSPECIFIED\x10\x00\x12(\n$INTERNAL_RELATION_VARIANT_BELONGS_TO\x10\x01\x12$\n INTERNAL_RELATION_VARIANT_ORIGIN\x10\x02\x12%\n!INTERNAL_RELATION_VARIANT_VERSION\x10\x03\x12&\n\"INTERNAL_RELATION_VARIANT_METADATA\x10\x04\x12$\n INTERNAL_RELATION_VARIANT_POLICY\x10\x05\x12$\n INTERNAL_RELATION_VARIANT_CUSTOM\x10\x06*x\n\x11RelationDirection\x12\"\n\x1eRELATION_DIRECTION_UNSPECIFIED\x10\x00\x12\x1e\n\x1aRELATION_DIRECTION_INBOUND\x10\x01\x12\x1f\n\x1bRELATION_DIRECTION_OUTBOUND\x10\x02*\xbb\x01\n\x0eResourceAction\x12\x1f\n\x1bRESOURCE_ACTION_UNSPECIFIED\x10\x00\x12\x1a\n\x16RESOURCE_ACTION_CREATE\x10\x01\x12\x1a\n\x16RESOURCE_ACTION_APPEND\x10\x02\x12\x1a\n\x16RESOURCE_ACTION_UPDATE\x10\x03\x12\x18\n\x14RESOURCE_ACTION_READ\x10\x04\x12\x1a\n\x16RESOURCE_ACTION_DELETE\x10\x05*\xa4\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13STATUS_INITIALIZING\x10\x01\x12\x15\n\x11STATUS_VALIDATING\x10\x02\x12\x14\n\x10STATUS_AVAILABLE\x10\x03\x12\x16\n\x12STATUS_UNAVAILABLE\x10\x04\x12\x10\n\x0cSTATUS_ERROR\x10\x05\x12\x12\n\x0eSTATUS_DELETED\x10\x06*\xd9\x01\n\x0f\x43omponentStatus\x12 \n\x1c\x43OMPONENT_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1d\x43OMPONENT_STATUS_INITIALIZING\x10\x01\x12\x1e\n\x1a\x43OMPONENT_STATUS_AVAILABLE\x10\x02\x12\x1d\n\x19\x43OMPONENT_STATUS_DEGRADED\x10\x03\x12 \n\x1c\x43OMPONENT_STATUS_UNAVAILABLE\x10\x04\x12 \n\x1c\x43OMPONENT_STATUS_MAINTENANCE\x10\x05*_\n\rHashalgorithm\x12\x1d\n\x19HASHALGORITHM_UNSPECIFIED\x10\x00\x12\x15\n\x11HASHALGORITHM_MD5\x10\x01\x12\x18\n\x14HASHALGORITHM_SHA256\x10\x02*\xad\x01\n\x0fResourceVariant\x12 \n\x1cRESOURCE_VARIANT_UNSPECIFIED\x10\x00\x12\x1c\n\x18RESOURCE_VARIANT_PROJECT\x10\x01\x12\x1f\n\x1bRESOURCE_VARIANT_COLLECTION\x10\x02\x12\x1c\n\x18RESOURCE_VARIANT_DATASET\x10\x03\x12\x1b\n\x17RESOURCE_VARIANT_OBJECT\x10\x04\x42?Z=github.com/ArunaStorage/go-api/v2/aruna/api/storage/models/v2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/storage/models/v2/models.proto\x12\x1b\x61runa.api.storage.models.v2\x1a\x1fgoogle/protobuf/timestamp.proto\"\xba\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x14\n\x05\x65mail\x18\x05 \x01(\tR\x05\x65mail\x12K\n\nattributes\x18\x06 \x01(\x0b\x32+.aruna.api.storage.models.v2.UserAttributesR\nattributesJ\x04\x08\x02\x10\x03\"\xfc\x01\n\nPermission\x12\x1f\n\nproject_id\x18\x01 \x01(\tH\x00R\tprojectId\x12%\n\rcollection_id\x18\x02 \x01(\tH\x00R\x0c\x63ollectionId\x12\x1f\n\ndataset_id\x18\x03 \x01(\tH\x00R\tdatasetId\x12\x1d\n\tobject_id\x18\x04 \x01(\tH\x00R\x08objectId\x12W\n\x10permission_level\x18\x06 \x01(\x0e\x32,.aruna.api.storage.models.v2.PermissionLevelR\x0fpermissionLevelB\r\n\x0bresource_id\"\xea\x01\n\x05Token\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x39\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12G\n\npermission\x18\x05 \x01(\x0b\x32\'.aruna.api.storage.models.v2.PermissionR\npermission\"F\n\x06Pubkey\x12\x0e\n\x02id\x18\x01 \x01(\x05R\x02id\x12\x10\n\x03key\x18\x02 \x01(\tR\x03key\x12\x1a\n\x08location\x18\x03 \x01(\tR\x08location\"b\n\x10\x43ustomAttributes\x12%\n\x0e\x61ttribute_name\x18\x01 \x01(\tR\rattributeName\x12\'\n\x0f\x61ttribute_value\x18\x02 \x01(\tR\x0e\x61ttributeValue\"I\n\x0bOidcMapping\x12\x1f\n\x0b\x65xternal_id\x18\x01 \x01(\tR\nexternalId\x12\x19\n\x08oidc_url\x18\x02 \x01(\tR\x07oidcUrl\"\xca\x03\n\x0eUserAttributes\x12!\n\x0cglobal_admin\x18\x01 \x01(\x08R\x0bglobalAdmin\x12\'\n\x0fservice_account\x18\x02 \x01(\x08R\x0eserviceAccount\x12:\n\x06tokens\x18\x03 \x03(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x06tokens\x12+\n\x11trusted_endpoints\x18\x04 \x03(\tR\x10trustedEndpoints\x12Z\n\x11\x63ustom_attributes\x18\x05 \x03(\x0b\x32-.aruna.api.storage.models.v2.CustomAttributesR\x10\x63ustomAttributes\x12Z\n\x14personal_permissions\x18\x06 \x03(\x0b\x32\'.aruna.api.storage.models.v2.PermissionR\x13personalPermissions\x12K\n\x0c\x65xternal_ids\x18\x07 \x03(\x0b\x32(.aruna.api.storage.models.v2.OidcMappingR\x0b\x65xternalIds\"z\n\x08KeyValue\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x12\x46\n\x07variant\x18\x03 \x01(\x0e\x32,.aruna.api.storage.models.v2.KeyValueVariantR\x07variant\"\xb0\x01\n\x08Relation\x12K\n\x08\x65xternal\x18\x01 \x01(\x0b\x32-.aruna.api.storage.models.v2.ExternalRelationH\x00R\x08\x65xternal\x12K\n\x08internal\x18\x02 \x01(\x0b\x32-.aruna.api.storage.models.v2.InternalRelationH\x00R\x08internalB\n\n\x08relation\"\xd0\x01\n\x10\x45xternalRelation\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12]\n\x0f\x64\x65\x66ined_variant\x18\x02 \x01(\x0e\x32\x34.aruna.api.storage.models.v2.ExternalRelationVariantR\x0e\x64\x65\x66inedVariant\x12*\n\x0e\x63ustom_variant\x18\x03 \x01(\tH\x00R\rcustomVariant\x88\x01\x01\x42\x11\n\x0f_custom_variant\"\xf8\x02\n\x10InternalRelation\x12\x1f\n\x0bresource_id\x18\x01 \x01(\tR\nresourceId\x12W\n\x10resource_variant\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.ResourceVariantR\x0fresourceVariant\x12]\n\x0f\x64\x65\x66ined_variant\x18\x03 \x01(\x0e\x32\x34.aruna.api.storage.models.v2.InternalRelationVariantR\x0e\x64\x65\x66inedVariant\x12*\n\x0e\x63ustom_variant\x18\x04 \x01(\tH\x00R\rcustomVariant\x88\x01\x01\x12L\n\tdirection\x18\x05 \x01(\x0e\x32..aruna.api.storage.models.v2.RelationDirectionR\tdirectionB\x11\n\x0f_custom_variant\"K\n\x0bPageRequest\x12\x1f\n\x0bstart_after\x18\x01 \x01(\tR\nstartAfter\x12\x1b\n\tpage_size\x18\x02 \x01(\x03R\x08pageSize\"p\n\x05Stats\x12\x14\n\x05\x63ount\x18\x01 \x01(\x03R\x05\x63ount\x12\x12\n\x04size\x18\x02 \x01(\x03R\x04size\x12=\n\x0clast_updated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"X\n\x04Hash\x12<\n\x03\x61lg\x18\x01 \x01(\x0e\x32*.aruna.api.storage.models.v2.HashalgorithmR\x03\x61lg\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\"\xc4\x01\n\x12\x45ndpointHostConfig\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\x12\x1d\n\nis_primary\x18\x02 \x01(\x08R\tisPrimary\x12\x10\n\x03ssl\x18\x03 \x01(\x08R\x03ssl\x12\x16\n\x06public\x18\x04 \x01(\x08R\x06public\x12S\n\x0chost_variant\x18\x05 \x01(\x0e\x32\x30.aruna.api.storage.models.v2.EndpointHostVariantR\x0bhostVariant\"\xb2\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12K\n\nep_variant\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.EndpointVariantR\tepVariant\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12\x44\n\x06status\x18\x05 \x01(\x0e\x32,.aruna.api.storage.models.v2.ComponentStatusR\x06status\x12R\n\x0chost_configs\x18\x06 \x03(\x0b\x32/.aruna.api.storage.models.v2.EndpointHostConfigR\x0bhostConfigs\"?\n\x0c\x44\x61taEndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x66ull_synced\x18\x02 \x01(\x08R\nfullSynced\"_\n\x04\x43opy\x12\x1a\n\x08resource\x18\x01 \x01(\tR\x08resource\x12\'\n\x0ftarget_endpoint\x18\x02 \x01(\tR\x0etargetEndpoint\x12\x12\n\x04push\x18\x03 \x01(\x08R\x04push\"v\n\x07\x43ontext\x12\'\n\x0es3_credentials\x18\x01 \x01(\x08H\x00R\rs3Credentials\x12\x37\n\x04\x63opy\x18\x02 \x01(\x0b\x32!.aruna.api.storage.models.v2.CopyH\x00R\x04\x63opyB\t\n\x07\x63ontext\"U\n\x07License\x12\x10\n\x03tag\x18\x01 \x01(\tR\x03tag\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x12\n\x04text\x18\x03 \x01(\tR\x04text\x12\x10\n\x03url\x18\x04 \x01(\tR\x03url\"\xab\x02\n\x0fGenericResource\x12@\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectH\x00R\x07project\x12I\n\ncollection\x18\x02 \x01(\x0b\x32\'.aruna.api.storage.models.v2.CollectionH\x00R\ncollection\x12@\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32$.aruna.api.storage.models.v2.DatasetH\x00R\x07\x64\x61taset\x12=\n\x06object\x18\x04 \x01(\x0b\x32#.aruna.api.storage.models.v2.ObjectH\x00R\x06objectB\n\n\x08resource\"\xc0\x05\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x38\n\x05stats\x18\x06 \x01(\x0b\x32\".aruna.api.storage.models.v2.StatsR\x05stats\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x30\n\x14metadata_license_tag\x18\r \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x0e \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"\xc3\x05\n\nCollection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x38\n\x05stats\x18\x06 \x01(\x0b\x32\".aruna.api.storage.models.v2.StatsR\x05stats\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x30\n\x14metadata_license_tag\x18\r \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x0e \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"\xc0\x05\n\x07\x44\x61taset\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x38\n\x05stats\x18\x06 \x01(\x0b\x32\".aruna.api.storage.models.v2.StatsR\x05stats\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x30\n\x14metadata_license_tag\x18\r \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x0e \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"\xd2\x05\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x1f\n\x0b\x63ontent_len\x18\x06 \x01(\x03R\ncontentLen\x12\x45\n\ndata_class\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12\x39\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x1d\n\ncreated_by\x18\t \x01(\tR\tcreatedBy\x12;\n\x06status\x18\n \x01(\x0e\x32#.aruna.api.storage.models.v2.StatusR\x06status\x12\x18\n\x07\x64ynamic\x18\x0b \x01(\x08R\x07\x64ynamic\x12G\n\tendpoints\x18\x0c \x03(\x0b\x32).aruna.api.storage.models.v2.DataEndpointR\tendpoints\x12\x39\n\x06hashes\x18\r \x03(\x0b\x32!.aruna.api.storage.models.v2.HashR\x06hashes\x12\x30\n\x14metadata_license_tag\x18\x0e \x01(\tR\x12metadataLicenseTag\x12(\n\x10\x64\x61ta_license_tag\x18\x0f \x01(\tR\x0e\x64\x61taLicenseTag*\x8d\x01\n\tDataClass\x12\x1a\n\x16\x44\x41TA_CLASS_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44\x41TA_CLASS_PUBLIC\x10\x01\x12\x16\n\x12\x44\x41TA_CLASS_PRIVATE\x10\x02\x12\x18\n\x14\x44\x41TA_CLASS_WORKSPACE\x10\x04\x12\x1b\n\x17\x44\x41TA_CLASS_CONFIDENTIAL\x10\x05*s\n\x0f\x45ndpointVariant\x12 \n\x1c\x45NDPOINT_VARIANT_UNSPECIFIED\x10\x00\x12\x1f\n\x1b\x45NDPOINT_VARIANT_PERSISTENT\x10\x01\x12\x1d\n\x19\x45NDPOINT_VARIANT_VOLATILE\x10\x02*z\n\x13\x45ndpointHostVariant\x12%\n!ENDPOINT_HOST_VARIANT_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45NDPOINT_HOST_VARIANT_GRPC\x10\x01\x12\x1c\n\x18\x45NDPOINT_HOST_VARIANT_S3\x10\x02*\xbe\x01\n\x0fPermissionLevel\x12 \n\x1cPERMISSION_LEVEL_UNSPECIFIED\x10\x00\x12\x19\n\x15PERMISSION_LEVEL_NONE\x10\x02\x12\x19\n\x15PERMISSION_LEVEL_READ\x10\x03\x12\x1b\n\x17PERMISSION_LEVEL_APPEND\x10\x04\x12\x1a\n\x16PERMISSION_LEVEL_WRITE\x10\x05\x12\x1a\n\x16PERMISSION_LEVEL_ADMIN\x10\x06*\xb4\x01\n\x0fKeyValueVariant\x12!\n\x1dKEY_VALUE_VARIANT_UNSPECIFIED\x10\x00\x12\x1b\n\x17KEY_VALUE_VARIANT_LABEL\x10\x01\x12\"\n\x1eKEY_VALUE_VARIANT_STATIC_LABEL\x10\x02\x12\x1a\n\x16KEY_VALUE_VARIANT_HOOK\x10\x03\x12!\n\x1dKEY_VALUE_VARIANT_HOOK_STATUS\x10\x04*\xb7\x01\n\x17\x45xternalRelationVariant\x12)\n%EXTERNAL_RELATION_VARIANT_UNSPECIFIED\x10\x00\x12!\n\x1d\x45XTERNAL_RELATION_VARIANT_URL\x10\x01\x12(\n$EXTERNAL_RELATION_VARIANT_IDENTIFIER\x10\x02\x12$\n EXTERNAL_RELATION_VARIANT_CUSTOM\x10\x03*\xd6\x02\n\x17InternalRelationVariant\x12)\n%INTERNAL_RELATION_VARIANT_UNSPECIFIED\x10\x00\x12(\n$INTERNAL_RELATION_VARIANT_BELONGS_TO\x10\x01\x12$\n INTERNAL_RELATION_VARIANT_ORIGIN\x10\x02\x12%\n!INTERNAL_RELATION_VARIANT_VERSION\x10\x03\x12&\n\"INTERNAL_RELATION_VARIANT_METADATA\x10\x04\x12$\n INTERNAL_RELATION_VARIANT_POLICY\x10\x05\x12%\n!INTERNAL_RELATION_VARIANT_DELETED\x10\x06\x12$\n INTERNAL_RELATION_VARIANT_CUSTOM\x10\x07*x\n\x11RelationDirection\x12\"\n\x1eRELATION_DIRECTION_UNSPECIFIED\x10\x00\x12\x1e\n\x1aRELATION_DIRECTION_INBOUND\x10\x01\x12\x1f\n\x1bRELATION_DIRECTION_OUTBOUND\x10\x02*\xbb\x01\n\x0eResourceAction\x12\x1f\n\x1bRESOURCE_ACTION_UNSPECIFIED\x10\x00\x12\x1a\n\x16RESOURCE_ACTION_CREATE\x10\x01\x12\x1a\n\x16RESOURCE_ACTION_APPEND\x10\x02\x12\x1a\n\x16RESOURCE_ACTION_UPDATE\x10\x03\x12\x18\n\x14RESOURCE_ACTION_READ\x10\x04\x12\x1a\n\x16RESOURCE_ACTION_DELETE\x10\x05*\xa4\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13STATUS_INITIALIZING\x10\x01\x12\x15\n\x11STATUS_VALIDATING\x10\x02\x12\x14\n\x10STATUS_AVAILABLE\x10\x03\x12\x16\n\x12STATUS_UNAVAILABLE\x10\x04\x12\x10\n\x0cSTATUS_ERROR\x10\x05\x12\x12\n\x0eSTATUS_DELETED\x10\x06*\xd9\x01\n\x0f\x43omponentStatus\x12 \n\x1c\x43OMPONENT_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1d\x43OMPONENT_STATUS_INITIALIZING\x10\x01\x12\x1e\n\x1a\x43OMPONENT_STATUS_AVAILABLE\x10\x02\x12\x1d\n\x19\x43OMPONENT_STATUS_DEGRADED\x10\x03\x12 \n\x1c\x43OMPONENT_STATUS_UNAVAILABLE\x10\x04\x12 \n\x1c\x43OMPONENT_STATUS_MAINTENANCE\x10\x05*_\n\rHashalgorithm\x12\x1d\n\x19HASHALGORITHM_UNSPECIFIED\x10\x00\x12\x15\n\x11HASHALGORITHM_MD5\x10\x01\x12\x18\n\x14HASHALGORITHM_SHA256\x10\x02*\xad\x01\n\x0fResourceVariant\x12 \n\x1cRESOURCE_VARIANT_UNSPECIFIED\x10\x00\x12\x1c\n\x18RESOURCE_VARIANT_PROJECT\x10\x01\x12\x1f\n\x1bRESOURCE_VARIANT_COLLECTION\x10\x02\x12\x1c\n\x18RESOURCE_VARIANT_DATASET\x10\x03\x12\x1b\n\x17RESOURCE_VARIANT_OBJECT\x10\x04\x42?Z=github.com/ArunaStorage/go-api/v2/aruna/api/storage/models/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.models.v2.models_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z=github.com/ArunaStorage/go-api/v2/aruna/api/storage/models/v2'
@@ -32,27 +32,27 @@
   _globals['_PERMISSIONLEVEL']._serialized_start=7083
   _globals['_PERMISSIONLEVEL']._serialized_end=7273
   _globals['_KEYVALUEVARIANT']._serialized_start=7276
   _globals['_KEYVALUEVARIANT']._serialized_end=7456
   _globals['_EXTERNALRELATIONVARIANT']._serialized_start=7459
   _globals['_EXTERNALRELATIONVARIANT']._serialized_end=7642
   _globals['_INTERNALRELATIONVARIANT']._serialized_start=7645
-  _globals['_INTERNALRELATIONVARIANT']._serialized_end=7948
-  _globals['_RELATIONDIRECTION']._serialized_start=7950
-  _globals['_RELATIONDIRECTION']._serialized_end=8070
-  _globals['_RESOURCEACTION']._serialized_start=8073
-  _globals['_RESOURCEACTION']._serialized_end=8260
-  _globals['_STATUS']._serialized_start=8263
-  _globals['_STATUS']._serialized_end=8427
-  _globals['_COMPONENTSTATUS']._serialized_start=8430
-  _globals['_COMPONENTSTATUS']._serialized_end=8647
-  _globals['_HASHALGORITHM']._serialized_start=8649
-  _globals['_HASHALGORITHM']._serialized_end=8744
-  _globals['_RESOURCEVARIANT']._serialized_start=8747
-  _globals['_RESOURCEVARIANT']._serialized_end=8920
+  _globals['_INTERNALRELATIONVARIANT']._serialized_end=7987
+  _globals['_RELATIONDIRECTION']._serialized_start=7989
+  _globals['_RELATIONDIRECTION']._serialized_end=8109
+  _globals['_RESOURCEACTION']._serialized_start=8112
+  _globals['_RESOURCEACTION']._serialized_end=8299
+  _globals['_STATUS']._serialized_start=8302
+  _globals['_STATUS']._serialized_end=8466
+  _globals['_COMPONENTSTATUS']._serialized_start=8469
+  _globals['_COMPONENTSTATUS']._serialized_end=8686
+  _globals['_HASHALGORITHM']._serialized_start=8688
+  _globals['_HASHALGORITHM']._serialized_end=8783
+  _globals['_RESOURCEVARIANT']._serialized_start=8786
+  _globals['_RESOURCEVARIANT']._serialized_end=8959
   _globals['_USER']._serialized_start=107
   _globals['_USER']._serialized_end=293
   _globals['_PERMISSION']._serialized_start=296
   _globals['_PERMISSION']._serialized_end=548
   _globals['_TOKEN']._serialized_start=551
   _globals['_TOKEN']._serialized_end=785
   _globals['_PUBKEY']._serialized_start=787
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/models/v2/models_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/models/v2/models_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     __slots__ = ()
     INTERNAL_RELATION_VARIANT_UNSPECIFIED: _ClassVar[InternalRelationVariant]
     INTERNAL_RELATION_VARIANT_BELONGS_TO: _ClassVar[InternalRelationVariant]
     INTERNAL_RELATION_VARIANT_ORIGIN: _ClassVar[InternalRelationVariant]
     INTERNAL_RELATION_VARIANT_VERSION: _ClassVar[InternalRelationVariant]
     INTERNAL_RELATION_VARIANT_METADATA: _ClassVar[InternalRelationVariant]
     INTERNAL_RELATION_VARIANT_POLICY: _ClassVar[InternalRelationVariant]
+    INTERNAL_RELATION_VARIANT_DELETED: _ClassVar[InternalRelationVariant]
     INTERNAL_RELATION_VARIANT_CUSTOM: _ClassVar[InternalRelationVariant]
 
 class RelationDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     RELATION_DIRECTION_UNSPECIFIED: _ClassVar[RelationDirection]
     RELATION_DIRECTION_INBOUND: _ClassVar[RelationDirection]
     RELATION_DIRECTION_OUTBOUND: _ClassVar[RelationDirection]
@@ -136,14 +137,15 @@
 EXTERNAL_RELATION_VARIANT_CUSTOM: ExternalRelationVariant
 INTERNAL_RELATION_VARIANT_UNSPECIFIED: InternalRelationVariant
 INTERNAL_RELATION_VARIANT_BELONGS_TO: InternalRelationVariant
 INTERNAL_RELATION_VARIANT_ORIGIN: InternalRelationVariant
 INTERNAL_RELATION_VARIANT_VERSION: InternalRelationVariant
 INTERNAL_RELATION_VARIANT_METADATA: InternalRelationVariant
 INTERNAL_RELATION_VARIANT_POLICY: InternalRelationVariant
+INTERNAL_RELATION_VARIANT_DELETED: InternalRelationVariant
 INTERNAL_RELATION_VARIANT_CUSTOM: InternalRelationVariant
 RELATION_DIRECTION_UNSPECIFIED: RelationDirection
 RELATION_DIRECTION_INBOUND: RelationDirection
 RELATION_DIRECTION_OUTBOUND: RelationDirection
 RESOURCE_ACTION_UNSPECIFIED: ResourceAction
 RESOURCE_ACTION_CREATE: ResourceAction
 RESOURCE_ACTION_APPEND: ResourceAction
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/authorization_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/authorization_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/authorization_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/authorization_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/authorization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/authorization_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/authorization_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from aruna.api.storage.services.v2 import authorization_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_authorization__service__pb2
 
 
 class AuthorizationServiceStub(object):
     """AuthorizationService
 
+    Status: BETA
+
     Contains all methods to edit and change user authorization
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
@@ -38,14 +40,16 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_authorization__service__pb2.UpdateAuthorizationResponse.FromString,
                 )
 
 
 class AuthorizationServiceServicer(object):
     """AuthorizationService
 
+    Status: BETA
+
     Contains all methods to edit and change user authorization
     """
 
     def CreateAuthorization(self, request, context):
         """CreateAuthorization
 
         Status: BETA
@@ -121,14 +125,16 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class AuthorizationService(object):
     """AuthorizationService
 
+    Status: BETA
+
     Contains all methods to edit and change user authorization
     """
 
     @staticmethod
     def CreateAuthorization(request,
             target,
             options=(),
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/collection_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/collection_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/collection_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/collection_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/collection_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/collection_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from aruna.api.storage.services.v2 import collection_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_collection__service__pb2
 
 
 class CollectionServiceStub(object):
     """CollectionService
 
+    Status: BETA
+
     Contains all methods that get/create or update Collection and associated resources
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
@@ -68,14 +70,16 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_collection__service__pb2.UpdateCollectionLicensesResponse.FromString,
                 )
 
 
 class CollectionServiceServicer(object):
     """CollectionService
 
+    Status: BETA
+
     Contains all methods that get/create or update Collection and associated resources
     """
 
     def CreateCollection(self, request, context):
         """CreateNewCollection
 
         Status: BETA
@@ -244,14 +248,16 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class CollectionService(object):
     """CollectionService
 
+    Status: BETA
+
     Contains all methods that get/create or update Collection and associated resources
     """
 
     @staticmethod
     def CreateCollection(request,
             target,
             options=(),
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/data_replication_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/data_replication_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/data_replication_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/data_replication_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/data_replication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/data_replication_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/data_replication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/dataset_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/dataset_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/dataset_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/dataset_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/dataset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/dataset_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/dataset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/endpoint_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/endpoint_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/endpoint_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from aruna.api.storage.models.v2 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v2_dot_models__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4aruna/api/storage/services/v2/endpoint_service.proto\x12\x1d\x61runa.api.storage.services.v2\x1a(aruna/api/storage/models/v2/models.proto\x1a\x1cgoogle/api/annotations.proto\"\x81\x02\n\x15\x43reateEndpointRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12K\n\nep_variant\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.EndpointVariantR\tepVariant\x12\x1b\n\tis_public\x18\x03 \x01(\x08R\x08isPublic\x12\x16\n\x06pubkey\x18\x04 \x01(\tR\x06pubkey\x12R\n\x0chost_configs\x18\x05 \x03(\x0b\x32/.aruna.api.storage.models.v2.EndpointHostConfigR\x0bhostConfigs\"[\n\x16\x43reateEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint\"\x19\n\x17\x46ullSyncEndpointRequest\"\xf7\x01\n\x18\x46ullSyncEndpointResponse\x12Y\n\x10generic_resource\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v2.GenericResourceH\x00R\x0fgenericResource\x12\x37\n\x04user\x18\x02 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserH\x00R\x04user\x12=\n\x06pubkey\x18\x03 \x01(\x0b\x32#.aruna.api.storage.models.v2.PubkeyH\x00R\x06pubkeyB\x08\n\x06target\"j\n\x12GetEndpointRequest\x12%\n\rendpoint_name\x18\x01 \x01(\tH\x00R\x0c\x65ndpointName\x12!\n\x0b\x65ndpoint_id\x18\x02 \x01(\tH\x00R\nendpointIdB\n\n\x08\x65ndpoint\"X\n\x13GetEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint\"\x15\n\x13GetEndpointsRequest\"[\n\x14GetEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\tendpoints\"8\n\x15\x44\x65leteEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"\x18\n\x16\x44\x65leteEndpointResponse\"\x1b\n\x19GetDefaultEndpointRequest\"_\n\x1aGetDefaultEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint2\xcc\x07\n\x0f\x45ndpointService\x12\x97\x01\n\x0e\x43reateEndpoint\x12\x34.aruna.api.storage.services.v2.CreateEndpointRequest\x1a\x35.aruna.api.storage.services.v2.CreateEndpointResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v2/endpoints:\x01*\x12\xa1\x01\n\x10\x46ullSyncEndpoint\x12\x36.aruna.api.storage.services.v2.FullSyncEndpointRequest\x1a\x37.aruna.api.storage.services.v2.FullSyncEndpointResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/v2/endpoints/sync0\x01\x12\x99\x01\n\x0bGetEndpoint\x12\x31.aruna.api.storage.services.v2.GetEndpointRequest\x1a\x32.aruna.api.storage.services.v2.GetEndpointResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2/endpoints/{endpoint_id}\x12\x8e\x01\n\x0cGetEndpoints\x12\x32.aruna.api.storage.services.v2.GetEndpointsRequest\x1a\x33.aruna.api.storage.services.v2.GetEndpointsResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v2/endpoints\x12\xa2\x01\n\x0e\x44\x65leteEndpoint\x12\x34.aruna.api.storage.services.v2.DeleteEndpointRequest\x1a\x35.aruna.api.storage.services.v2.DeleteEndpointResponse\"#\x82\xd3\xe4\x93\x02\x1d*\x1b/v2/endpoints/{endpoint_id}\x12\xa8\x01\n\x12GetDefaultEndpoint\x12\x38.aruna.api.storage.services.v2.GetDefaultEndpointRequest\x1a\x39.aruna.api.storage.services.v2.GetDefaultEndpointResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v2/endpoints/defaultB\x94\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\x0f\x45ndpointServiceP\x01Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4aruna/api/storage/services/v2/endpoint_service.proto\x12\x1d\x61runa.api.storage.services.v2\x1a(aruna/api/storage/models/v2/models.proto\x1a\x1cgoogle/api/annotations.proto\"\x81\x02\n\x15\x43reateEndpointRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12K\n\nep_variant\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.EndpointVariantR\tepVariant\x12\x1b\n\tis_public\x18\x03 \x01(\x08R\x08isPublic\x12\x16\n\x06pubkey\x18\x04 \x01(\tR\x06pubkey\x12R\n\x0chost_configs\x18\x05 \x03(\x0b\x32/.aruna.api.storage.models.v2.EndpointHostConfigR\x0bhostConfigs\"[\n\x16\x43reateEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint\"\x19\n\x17\x46ullSyncEndpointRequest\"\xf7\x01\n\x18\x46ullSyncEndpointResponse\x12Y\n\x10generic_resource\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v2.GenericResourceH\x00R\x0fgenericResource\x12\x37\n\x04user\x18\x02 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserH\x00R\x04user\x12=\n\x06pubkey\x18\x03 \x01(\x0b\x32#.aruna.api.storage.models.v2.PubkeyH\x00R\x06pubkeyB\x08\n\x06target\"j\n\x12GetEndpointRequest\x12%\n\rendpoint_name\x18\x01 \x01(\tH\x00R\x0c\x65ndpointName\x12!\n\x0b\x65ndpoint_id\x18\x02 \x01(\tH\x00R\nendpointIdB\n\n\x08\x65ndpoint\"X\n\x13GetEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint\"\x15\n\x13GetEndpointsRequest\"[\n\x14GetEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\tendpoints\"8\n\x15\x44\x65leteEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"\x18\n\x16\x44\x65leteEndpointResponse\"\x1b\n\x19GetDefaultEndpointRequest\"_\n\x1aGetDefaultEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint\"\x81\x01\n\x18SetEndpointStatusRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\x12\x44\n\x06status\x18\x02 \x01(\x0e\x32,.aruna.api.storage.models.v2.ComponentStatusR\x06status\"^\n\x19SetEndpointStatusResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v2.EndpointR\x08\x65ndpoint2\x81\t\n\x0f\x45ndpointService\x12\x97\x01\n\x0e\x43reateEndpoint\x12\x34.aruna.api.storage.services.v2.CreateEndpointRequest\x1a\x35.aruna.api.storage.services.v2.CreateEndpointResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v2/endpoints:\x01*\x12\xa1\x01\n\x10\x46ullSyncEndpoint\x12\x36.aruna.api.storage.services.v2.FullSyncEndpointRequest\x1a\x37.aruna.api.storage.services.v2.FullSyncEndpointResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/v2/endpoints/sync0\x01\x12\xb2\x01\n\x11SetEndpointStatus\x12\x37.aruna.api.storage.services.v2.SetEndpointStatusRequest\x1a\x38.aruna.api.storage.services.v2.SetEndpointStatusResponse\"*\x82\xd3\xe4\x93\x02$2\"/v2/endpoints/{endpoint_id}/status\x12\x99\x01\n\x0bGetEndpoint\x12\x31.aruna.api.storage.services.v2.GetEndpointRequest\x1a\x32.aruna.api.storage.services.v2.GetEndpointResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2/endpoints/{endpoint_id}\x12\x8e\x01\n\x0cGetEndpoints\x12\x32.aruna.api.storage.services.v2.GetEndpointsRequest\x1a\x33.aruna.api.storage.services.v2.GetEndpointsResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v2/endpoints\x12\xa2\x01\n\x0e\x44\x65leteEndpoint\x12\x34.aruna.api.storage.services.v2.DeleteEndpointRequest\x1a\x35.aruna.api.storage.services.v2.DeleteEndpointResponse\"#\x82\xd3\xe4\x93\x02\x1d*\x1b/v2/endpoints/{endpoint_id}\x12\xa8\x01\n\x12GetDefaultEndpoint\x12\x38.aruna.api.storage.services.v2.GetDefaultEndpointRequest\x1a\x39.aruna.api.storage.services.v2.GetDefaultEndpointResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v2/endpoints/defaultB\x94\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\x0f\x45ndpointServiceP\x01Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v2.endpoint_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\017EndpointServiceP\001Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2'
   _globals['_ENDPOINTSERVICE'].methods_by_name['CreateEndpoint']._options = None
   _globals['_ENDPOINTSERVICE'].methods_by_name['CreateEndpoint']._serialized_options = b'\202\323\344\223\002\022\"\r/v2/endpoints:\001*'
   _globals['_ENDPOINTSERVICE'].methods_by_name['FullSyncEndpoint']._options = None
   _globals['_ENDPOINTSERVICE'].methods_by_name['FullSyncEndpoint']._serialized_options = b'\202\323\344\223\002\024\022\022/v2/endpoints/sync'
+  _globals['_ENDPOINTSERVICE'].methods_by_name['SetEndpointStatus']._options = None
+  _globals['_ENDPOINTSERVICE'].methods_by_name['SetEndpointStatus']._serialized_options = b'\202\323\344\223\002$2\"/v2/endpoints/{endpoint_id}/status'
   _globals['_ENDPOINTSERVICE'].methods_by_name['GetEndpoint']._options = None
   _globals['_ENDPOINTSERVICE'].methods_by_name['GetEndpoint']._serialized_options = b'\202\323\344\223\002\035\022\033/v2/endpoints/{endpoint_id}'
   _globals['_ENDPOINTSERVICE'].methods_by_name['GetEndpoints']._options = None
   _globals['_ENDPOINTSERVICE'].methods_by_name['GetEndpoints']._serialized_options = b'\202\323\344\223\002\017\022\r/v2/endpoints'
   _globals['_ENDPOINTSERVICE'].methods_by_name['DeleteEndpoint']._options = None
   _globals['_ENDPOINTSERVICE'].methods_by_name['DeleteEndpoint']._serialized_options = b'\202\323\344\223\002\035*\033/v2/endpoints/{endpoint_id}'
   _globals['_ENDPOINTSERVICE'].methods_by_name['GetDefaultEndpoint']._options = None
@@ -56,10 +58,14 @@
   _globals['_DELETEENDPOINTREQUEST']._serialized_end=1159
   _globals['_DELETEENDPOINTRESPONSE']._serialized_start=1161
   _globals['_DELETEENDPOINTRESPONSE']._serialized_end=1185
   _globals['_GETDEFAULTENDPOINTREQUEST']._serialized_start=1187
   _globals['_GETDEFAULTENDPOINTREQUEST']._serialized_end=1214
   _globals['_GETDEFAULTENDPOINTRESPONSE']._serialized_start=1216
   _globals['_GETDEFAULTENDPOINTRESPONSE']._serialized_end=1311
-  _globals['_ENDPOINTSERVICE']._serialized_start=1314
-  _globals['_ENDPOINTSERVICE']._serialized_end=2286
+  _globals['_SETENDPOINTSTATUSREQUEST']._serialized_start=1314
+  _globals['_SETENDPOINTSTATUSREQUEST']._serialized_end=1443
+  _globals['_SETENDPOINTSTATUSRESPONSE']._serialized_start=1445
+  _globals['_SETENDPOINTSTATUSRESPONSE']._serialized_end=1539
+  _globals['_ENDPOINTSERVICE']._serialized_start=1542
+  _globals['_ENDPOINTSERVICE']._serialized_end=2695
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/endpoint_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/endpoint_service_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -80,7 +80,21 @@
     def __init__(self) -> None: ...
 
 class GetDefaultEndpointResponse(_message.Message):
     __slots__ = ("endpoint",)
     ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     endpoint: _models_pb2.Endpoint
     def __init__(self, endpoint: _Optional[_Union[_models_pb2.Endpoint, _Mapping]] = ...) -> None: ...
+
+class SetEndpointStatusRequest(_message.Message):
+    __slots__ = ("endpoint_id", "status")
+    ENDPOINT_ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    endpoint_id: str
+    status: _models_pb2.ComponentStatus
+    def __init__(self, endpoint_id: _Optional[str] = ..., status: _Optional[_Union[_models_pb2.ComponentStatus, str]] = ...) -> None: ...
+
+class SetEndpointStatusResponse(_message.Message):
+    __slots__ = ("endpoint",)
+    ENDPOINT_FIELD_NUMBER: _ClassVar[int]
+    endpoint: _models_pb2.Endpoint
+    def __init__(self, endpoint: _Optional[_Union[_models_pb2.Endpoint, _Mapping]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/endpoint_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from aruna.api.storage.services.v2 import endpoint_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2
 
 
 class EndpointServiceStub(object):
     """EndpointService
 
-    Contains all methods that get/create or update Endpoint and associated resources
+    Status: BETA
+
+    Contains all methods that get/create or update Endpoint (Dataproxies) and associated resources
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -23,14 +25,19 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.CreateEndpointResponse.FromString,
                 )
         self.FullSyncEndpoint = channel.unary_stream(
                 '/aruna.api.storage.services.v2.EndpointService/FullSyncEndpoint',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.FullSyncEndpointRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.FullSyncEndpointResponse.FromString,
                 )
+        self.SetEndpointStatus = channel.unary_unary(
+                '/aruna.api.storage.services.v2.EndpointService/SetEndpointStatus',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.SetEndpointStatusRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.SetEndpointStatusResponse.FromString,
+                )
         self.GetEndpoint = channel.unary_unary(
                 '/aruna.api.storage.services.v2.EndpointService/GetEndpoint',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.GetEndpointRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.GetEndpointResponse.FromString,
                 )
         self.GetEndpoints = channel.unary_unary(
                 '/aruna.api.storage.services.v2.EndpointService/GetEndpoints',
@@ -48,24 +55,26 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.GetDefaultEndpointResponse.FromString,
                 )
 
 
 class EndpointServiceServicer(object):
     """EndpointService
 
-    Contains all methods that get/create or update Endpoint and associated resources
+    Status: BETA
+
+    Contains all methods that get/create or update Endpoint (Dataproxies) and associated resources
     """
 
     def CreateEndpoint(self, request, context):
         """CreateEndpoint
 
         Status: BETA
 
         Registers a new Endpoint (Aruna DataProxy) to the server
-        Needs admin permissions
+        requires admin permissions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def FullSyncEndpoint(self, request, context):
         """FullSyncEndpoint
@@ -74,14 +83,25 @@
 
         Requests a full sync of all endpoint related data
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SetEndpointStatus(self, request, context):
+        """SetEndpointStatus
+
+        Status: BETA
+
+        This request sets the status of a specific Endpoint
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetEndpoint(self, request, context):
         """GetEndpoint
 
         Status: BETA
 
         Gets an specific endpoint by ID or Name
         """
@@ -133,14 +153,19 @@
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.CreateEndpointResponse.SerializeToString,
             ),
             'FullSyncEndpoint': grpc.unary_stream_rpc_method_handler(
                     servicer.FullSyncEndpoint,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.FullSyncEndpointRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.FullSyncEndpointResponse.SerializeToString,
             ),
+            'SetEndpointStatus': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetEndpointStatus,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.SetEndpointStatusRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.SetEndpointStatusResponse.SerializeToString,
+            ),
             'GetEndpoint': grpc.unary_unary_rpc_method_handler(
                     servicer.GetEndpoint,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.GetEndpointRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.GetEndpointResponse.SerializeToString,
             ),
             'GetEndpoints': grpc.unary_unary_rpc_method_handler(
                     servicer.GetEndpoints,
@@ -163,15 +188,17 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class EndpointService(object):
     """EndpointService
 
-    Contains all methods that get/create or update Endpoint and associated resources
+    Status: BETA
+
+    Contains all methods that get/create or update Endpoint (Dataproxies) and associated resources
     """
 
     @staticmethod
     def CreateEndpoint(request,
             target,
             options=(),
             channel_credentials=None,
@@ -201,14 +228,31 @@
         return grpc.experimental.unary_stream(request, target, '/aruna.api.storage.services.v2.EndpointService/FullSyncEndpoint',
             aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.FullSyncEndpointRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.FullSyncEndpointResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SetEndpointStatus(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v2.EndpointService/SetEndpointStatus',
+            aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.SetEndpointStatusRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v2_dot_endpoint__service__pb2.SetEndpointStatusResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetEndpoint(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/info_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/info_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/info_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/info_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/info_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/info_service_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 from aruna.api.storage.services.v2 import info_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_info__service__pb2
 
 
 class StorageStatusServiceStub(object):
     """StorageStatusService
 
+    Status: BETA
+
     This is a generic service that contains utility functions 
     these functions are used to query additional meta-information
-    about the status of the overall storage architecture
+    about the status of storage components
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -45,17 +47,19 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_info__service__pb2.SetAnnouncementsResponse.FromString,
                 )
 
 
 class StorageStatusServiceServicer(object):
     """StorageStatusService
 
+    Status: BETA
+
     This is a generic service that contains utility functions 
     these functions are used to query additional meta-information
-    about the status of the overall storage architecture
+    about the status of storage components
     """
 
     def GetStorageVersion(self, request, context):
         """GetStorageVersion
 
         Status: BETA
 
@@ -74,27 +78,42 @@
         A request to get the current status of the storage components by location(s)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetPubkeys(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """GetPubkeys
+
+        Status: BETA
+
+        Get all public keys of all storage components
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetAnnouncements(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """GetAnnouncements
+
+        Status: BETA
+
+        Query global announcements
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetAnnouncements(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """SetAnnouncements
+
+        Status: BETA
+
+        Update / add global announcements
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_StorageStatusServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -129,17 +148,19 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class StorageStatusService(object):
     """StorageStatusService
 
+    Status: BETA
+
     This is a generic service that contains utility functions 
     these functions are used to query additional meta-information
-    about the status of the overall storage architecture
+    about the status of storage components
     """
 
     @staticmethod
     def GetStorageVersion(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/license_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/license_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/license_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/license_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/license_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/license_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/license_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from aruna.api.storage.services.v2 import license_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_license__service__pb2
 
 
 class LicenseServiceStub(object):
     """LicenseService
 
-    Contains all methods to add, get or list licenses
+    Status: BETA
+
+    Contains all methods to add, get or list (custom) licenses
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -33,15 +35,17 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_license__service__pb2.ListLicensesResponse.FromString,
                 )
 
 
 class LicenseServiceServicer(object):
     """LicenseService
 
-    Contains all methods to add, get or list licenses
+    Status: BETA
+
+    Contains all methods to add, get or list (custom) licenses
     """
 
     def CreateLicense(self, request, context):
         """CreateLicense
 
         Status: BETA
 
@@ -97,15 +101,17 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class LicenseService(object):
     """LicenseService
 
-    Contains all methods to add, get or list licenses
+    Status: BETA
+
+    Contains all methods to add, get or list (custom) licenses
     """
 
     @staticmethod
     def CreateLicense(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/object_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/object_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/object_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/object_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/object_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/object_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/object_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from aruna.api.storage.services.v2 import object_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_object__service__pb2
 
 
 class ObjectServiceStub(object):
     """ObjectService
 
-    Contains all methods that get/create or update Objects and associated resources
+    Status: BETA
+
+    Contains all methods that get/create or update objects and associated resources
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -63,24 +65,27 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_object__service__pb2.GetObjectsResponse.FromString,
                 )
 
 
 class ObjectServiceServicer(object):
     """ObjectService
 
-    Contains all methods that get/create or update Objects and associated resources
+    Status: BETA
+
+    Contains all methods that get/create or update objects and associated resources
     """
 
     def CreateObject(self, request, context):
         """CreateObject
 
         Status: BETA
 
-        This creates a new object
-        Initializing an object will put it in a staging area.
+        This creates a new object and puts it in a staging area.
+        Staging objects have an "INITIALIZING" status
+        and need to be finished either manually or by uploading data.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetUploadURL(self, request, context):
         """GetUploadURL
@@ -237,15 +242,17 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ObjectService(object):
     """ObjectService
 
-    Contains all methods that get/create or update Objects and associated resources
+    Status: BETA
+
+    Contains all methods that get/create or update objects and associated resources
     """
 
     @staticmethod
     def CreateObject(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/project_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/project_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/project_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,22 +14,22 @@
 
 from aruna.api.storage.models.v2 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v2_dot_models__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v2/project_service.proto\x12\x1d\x61runa.api.storage.services.v2\x1a(aruna/api/storage/models/v2/models.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1bgoogle/api/visibility.proto\"\xb8\x03\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x45\n\ndata_class\x18\x05 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12-\n\x12preferred_endpoint\x18\x06 \x01(\tR\x11preferredEndpoint\x12\x30\n\x14metadata_license_tag\x18\x07 \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x08 \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"W\n\x15\x43reateProjectResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"T\n\x12GetProjectResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"5\n\x12GetProjectsRequest\x12\x1f\n\x0bproject_ids\x18\x01 \x03(\tR\nprojectIds\"W\n\x13GetProjectsResponse\x12@\n\x08projects\x18\x01 \x03(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x08projects\"5\n\x14\x44\x65leteProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x17\n\x15\x44\x65leteProjectResponse\"M\n\x18UpdateProjectNameRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"[\n\x19UpdateProjectNameResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"b\n\x1fUpdateProjectDescriptionRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"b\n UpdateProjectDescriptionResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"\xde\x01\n\x1dUpdateProjectKeyValuesRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12K\n\x0e\x61\x64\x64_key_values\x18\x02 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\x0c\x61\x64\x64KeyValues\x12Q\n\x11remove_key_values\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\x0fremoveKeyValues\"`\n\x1eUpdateProjectKeyValuesResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"\x85\x01\n\x1dUpdateProjectDataClassRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x45\n\ndata_class\x18\x02 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\"`\n\x1eUpdateProjectDataClassResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"6\n\x15\x41rchiveProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"X\n\x16\x41rchiveProjectResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"\xa8\x01\n\x1cUpdateProjectLicensesRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x30\n\x14metadata_license_tag\x18\x02 \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x03 \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"_\n\x1dUpdateProjectLicensesResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project2\x82\x0e\n\x0eProjectService\x12\x93\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v2.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v2.CreateProjectResponse\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v2/projects:\x01*\x12\x94\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v2.GetProjectRequest\x1a\x31.aruna.api.storage.services.v2.GetProjectResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v2/projects/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v2.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v2.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/projects\x12\x9d\x01\n\rDeleteProject\x12\x33.aruna.api.storage.services.v2.DeleteProjectRequest\x1a\x34.aruna.api.storage.services.v2.DeleteProjectResponse\"!\x82\xd3\xe4\x93\x02\x1b*\x19/v2/projects/{project_id}\x12\xb1\x01\n\x11UpdateProjectName\x12\x37.aruna.api.storage.services.v2.UpdateProjectNameRequest\x1a\x38.aruna.api.storage.services.v2.UpdateProjectNameResponse\")\x82\xd3\xe4\x93\x02#2\x1e/v2/projects/{project_id}/name:\x01*\x12\xcd\x01\n\x18UpdateProjectDescription\x12>.aruna.api.storage.services.v2.UpdateProjectDescriptionRequest\x1a?.aruna.api.storage.services.v2.UpdateProjectDescriptionResponse\"0\x82\xd3\xe4\x93\x02*2%/v2/projects/{project_id}/description:\x01*\x12\xc6\x01\n\x16UpdateProjectKeyValues\x12<.aruna.api.storage.services.v2.UpdateProjectKeyValuesRequest\x1a=.aruna.api.storage.services.v2.UpdateProjectKeyValuesResponse\"/\x82\xd3\xe4\x93\x02)2$/v2/projects/{project_id}/key_values:\x01*\x12\xc6\x01\n\x16UpdateProjectDataClass\x12<.aruna.api.storage.services.v2.UpdateProjectDataClassRequest\x1a=.aruna.api.storage.services.v2.UpdateProjectDataClassResponse\"/\x82\xd3\xe4\x93\x02)2$/v2/projects/{project_id}/data_class:\x01*\x12\xc1\x01\n\x15UpdateProjectLicenses\x12;.aruna.api.storage.services.v2.UpdateProjectLicensesRequest\x1a<.aruna.api.storage.services.v2.UpdateProjectLicensesResponse\"-\x82\xd3\xe4\x93\x02\'2\"/v2/projects/{project_id}/licenses:\x01*\x12\xab\x01\n\x0e\x41rchiveProject\x12\x34.aruna.api.storage.services.v2.ArchiveProjectRequest\x1a\x35.aruna.api.storage.services.v2.ArchiveProjectResponse\",\x82\xd3\xe4\x93\x02&\"!/v2/projects/{project_id}/archive:\x01*\x1a\x0e\xfa\xd2\xe4\x93\x02\x08\x12\x06SERVERB\xea\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\x0eProjectServiceP\x01Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2\x92\x41\xd3\x01\x12\x33\n#Aruna Object Storage (AOS) REST API2\x0c\x32.0.0-beta.8*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v2/project_service.proto\x12\x1d\x61runa.api.storage.services.v2\x1a(aruna/api/storage/models/v2/models.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1bgoogle/api/visibility.proto\"\xb8\x03\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x44\n\nkey_values\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\tkeyValues\x12\x43\n\trelations\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v2.RelationR\trelations\x12\x45\n\ndata_class\x18\x05 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\x12-\n\x12preferred_endpoint\x18\x06 \x01(\tR\x11preferredEndpoint\x12\x30\n\x14metadata_license_tag\x18\x07 \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x08 \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"W\n\x15\x43reateProjectResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"T\n\x12GetProjectResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"5\n\x12GetProjectsRequest\x12\x1f\n\x0bproject_ids\x18\x01 \x03(\tR\nprojectIds\"W\n\x13GetProjectsResponse\x12@\n\x08projects\x18\x01 \x03(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x08projects\"5\n\x14\x44\x65leteProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x17\n\x15\x44\x65leteProjectResponse\"M\n\x18UpdateProjectNameRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"[\n\x19UpdateProjectNameResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"b\n\x1fUpdateProjectDescriptionRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"b\n UpdateProjectDescriptionResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"\xde\x01\n\x1dUpdateProjectKeyValuesRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12K\n\x0e\x61\x64\x64_key_values\x18\x02 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\x0c\x61\x64\x64KeyValues\x12Q\n\x11remove_key_values\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v2.KeyValueR\x0fremoveKeyValues\"`\n\x1eUpdateProjectKeyValuesResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"\x85\x01\n\x1dUpdateProjectDataClassRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x45\n\ndata_class\x18\x02 \x01(\x0e\x32&.aruna.api.storage.models.v2.DataClassR\tdataClass\"`\n\x1eUpdateProjectDataClassResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"6\n\x15\x41rchiveProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"X\n\x16\x41rchiveProjectResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project\"\xa8\x01\n\x1cUpdateProjectLicensesRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x30\n\x14metadata_license_tag\x18\x02 \x01(\tR\x12metadataLicenseTag\x12\x37\n\x18\x64\x65\x66\x61ult_data_license_tag\x18\x03 \x01(\tR\x15\x64\x65\x66\x61ultDataLicenseTag\"_\n\x1dUpdateProjectLicensesResponse\x12>\n\x07project\x18\x01 \x01(\x0b\x32$.aruna.api.storage.models.v2.ProjectR\x07project2\x82\x0e\n\x0eProjectService\x12\x93\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v2.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v2.CreateProjectResponse\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v2/projects:\x01*\x12\x94\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v2.GetProjectRequest\x1a\x31.aruna.api.storage.services.v2.GetProjectResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v2/projects/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v2.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v2.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/projects\x12\x9d\x01\n\rDeleteProject\x12\x33.aruna.api.storage.services.v2.DeleteProjectRequest\x1a\x34.aruna.api.storage.services.v2.DeleteProjectResponse\"!\x82\xd3\xe4\x93\x02\x1b*\x19/v2/projects/{project_id}\x12\xb1\x01\n\x11UpdateProjectName\x12\x37.aruna.api.storage.services.v2.UpdateProjectNameRequest\x1a\x38.aruna.api.storage.services.v2.UpdateProjectNameResponse\")\x82\xd3\xe4\x93\x02#2\x1e/v2/projects/{project_id}/name:\x01*\x12\xcd\x01\n\x18UpdateProjectDescription\x12>.aruna.api.storage.services.v2.UpdateProjectDescriptionRequest\x1a?.aruna.api.storage.services.v2.UpdateProjectDescriptionResponse\"0\x82\xd3\xe4\x93\x02*2%/v2/projects/{project_id}/description:\x01*\x12\xc6\x01\n\x16UpdateProjectKeyValues\x12<.aruna.api.storage.services.v2.UpdateProjectKeyValuesRequest\x1a=.aruna.api.storage.services.v2.UpdateProjectKeyValuesResponse\"/\x82\xd3\xe4\x93\x02)2$/v2/projects/{project_id}/key_values:\x01*\x12\xc6\x01\n\x16UpdateProjectDataClass\x12<.aruna.api.storage.services.v2.UpdateProjectDataClassRequest\x1a=.aruna.api.storage.services.v2.UpdateProjectDataClassResponse\"/\x82\xd3\xe4\x93\x02)2$/v2/projects/{project_id}/data_class:\x01*\x12\xc1\x01\n\x15UpdateProjectLicenses\x12;.aruna.api.storage.services.v2.UpdateProjectLicensesRequest\x1a<.aruna.api.storage.services.v2.UpdateProjectLicensesResponse\"-\x82\xd3\xe4\x93\x02\'2\"/v2/projects/{project_id}/licenses:\x01*\x12\xab\x01\n\x0e\x41rchiveProject\x12\x34.aruna.api.storage.services.v2.ArchiveProjectRequest\x1a\x35.aruna.api.storage.services.v2.ArchiveProjectResponse\",\x82\xd3\xe4\x93\x02&\"!/v2/projects/{project_id}/archive:\x01*\x1a\x0e\xfa\xd2\xe4\x93\x02\x08\x12\x06SERVERB\xea\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\x0eProjectServiceP\x01Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2\x92\x41\xd3\x01\x12\x33\n#Aruna Object Storage (AOS) REST API2\x0c\x32.0.0-beta.9*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v2.project_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\016ProjectServiceP\001Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2\222A\323\001\0223\n#Aruna Object Storage (AOS) REST API2\0142.0.0-beta.8*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  _globals['DESCRIPTOR']._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\016ProjectServiceP\001Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2\222A\323\001\0223\n#Aruna Object Storage (AOS) REST API2\0142.0.0-beta.9*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _globals['_PROJECTSERVICE']._options = None
   _globals['_PROJECTSERVICE']._serialized_options = b'\372\322\344\223\002\010\022\006SERVER'
   _globals['_PROJECTSERVICE'].methods_by_name['CreateProject']._options = None
   _globals['_PROJECTSERVICE'].methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\021\"\014/v2/projects:\001*'
   _globals['_PROJECTSERVICE'].methods_by_name['GetProject']._options = None
   _globals['_PROJECTSERVICE'].methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\033\022\031/v2/projects/{project_id}'
   _globals['_PROJECTSERVICE'].methods_by_name['GetProjects']._options = None
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/project_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/project_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/project_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from aruna.api.storage.services.v2 import project_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_project__service__pb2
 
 
 class ProjectServiceStub(object):
     """ProjectService
 
+    Status: BETA
+
     Contains all methods that get/create or update Projects and associated resources
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
@@ -68,14 +70,16 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_project__service__pb2.ArchiveProjectResponse.FromString,
                 )
 
 
 class ProjectServiceServicer(object):
     """ProjectService
 
+    Status: BETA
+
     Contains all methods that get/create or update Projects and associated resources
     """
 
     def CreateProject(self, request, context):
         """CreateProject
 
         Status: BETA
@@ -244,14 +248,16 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ProjectService(object):
     """ProjectService
 
+    Status: BETA
+
     Contains all methods that get/create or update Projects and associated resources
     """
 
     @staticmethod
     def CreateProject(request,
             target,
             options=(),
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/relations_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/relations_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/relations_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/relations_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/relations_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/relations_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/relations_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from aruna.api.storage.services.v2 import relations_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_relations__service__pb2
 
 
 class RelationsServiceStub(object):
     """RelationsService
 
+    Status: BETA
+
     Contains all methods to edit and change resource relations
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
@@ -28,34 +30,38 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_relations__service__pb2.GetHierarchyResponse.FromString,
                 )
 
 
 class RelationsServiceServicer(object):
     """RelationsService
 
+    Status: BETA
+
     Contains all methods to edit and change resource relations
     """
 
     def ModifyRelations(self, request, context):
         """ModifyRelation
 
         Status: BETA
 
-        Modifys all relations to / from a resource
+        Add/Remove/Modifies all relation types to / from a resource
+        Works for internal and external relations
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetHierarchy(self, request, context):
         """GetHierachy
 
         Status: BETA
 
         Gets all downstream hierarchy relations from a resource
+        results in a tree structure
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_RelationsServiceServicer_to_server(servicer, server):
@@ -76,14 +82,16 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class RelationsService(object):
     """RelationsService
 
+    Status: BETA
+
     Contains all methods to edit and change resource relations
     """
 
     @staticmethod
     def ModifyRelations(request,
             target,
             options=(),
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/search_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/search_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/search_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/search_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/search_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/search_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/search_service_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from aruna.api.storage.services.v2 import search_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_search__service__pb2
 
 
 class SearchServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
+    """SearchService
+
+    Status: BETA
+
+    SearchService is used to query resources in the index and get a public view of them.
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
@@ -33,15 +38,20 @@
                 '/aruna.api.storage.services.v2.SearchService/RequestResourceAccess',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_search__service__pb2.RequestResourceAccessRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_search__service__pb2.RequestResourceAccessResponse.FromString,
                 )
 
 
 class SearchServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
+    """SearchService
+
+    Status: BETA
+
+    SearchService is used to query resources in the index and get a public view of them.
+    """
 
     def SearchResources(self, request, context):
         """SearchResources
 
         Status: BETA
 
         Searches the index for applicable resources (only public + private can be searched)
@@ -110,15 +120,20 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.storage.services.v2.SearchService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class SearchService(object):
-    """Missing associated documentation comment in .proto file."""
+    """SearchService
+
+    Status: BETA
+
+    SearchService is used to query resources in the index and get a public view of them.
+    """
 
     @staticmethod
     def SearchResources(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/service_account_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/service_account_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/service_account_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/service_account_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/service_account_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/service_account_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 from aruna.api.storage.services.v2 import service_account_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_service__account__service__pb2
 
 
 class ServiceAccountServiceStub(object):
     """ServiceAccountService
 
-    Service that contains all methods for service_accounts, these are Accounts that are
-    project specific (or global) and can be used for automation. 
-    Service account users will always contain (bot) behind their name
+    Status: BETA
+
+    Service that contains CRUD operations for service_accounts.
+    Service accounts are project specific accounts that can be used for automation. 
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -70,17 +71,18 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_service__account__service__pb2.CreateDataproxyTokenSvcAccountResponse.FromString,
                 )
 
 
 class ServiceAccountServiceServicer(object):
     """ServiceAccountService
 
-    Service that contains all methods for service_accounts, these are Accounts that are
-    project specific (or global) and can be used for automation. 
-    Service account users will always contain (bot) behind their name
+    Status: BETA
+
+    Service that contains CRUD operations for service_accounts.
+    Service accounts are project specific accounts that can be used for automation. 
     """
 
     def CreateServiceAccount(self, request, context):
         """CreateServiceAccount
 
         Status: BETA
 
@@ -95,15 +97,15 @@
     def CreateServiceAccountToken(self, request, context):
         """CreateServiceAccountToken
 
         Status: BETA
 
         Creates a token for a service account
         Each service account can only have one permission -> The token will have the same permission as the
-        service account
+        service account or a subset of it.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetServiceAccountPermission(self, request, context):
         """SetServiceAccountPermission
@@ -254,17 +256,18 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ServiceAccountService(object):
     """ServiceAccountService
 
-    Service that contains all methods for service_accounts, these are Accounts that are
-    project specific (or global) and can be used for automation. 
-    Service account users will always contain (bot) behind their name
+    Status: BETA
+
+    Service that contains CRUD operations for service_accounts.
+    Service accounts are project specific accounts that can be used for automation. 
     """
 
     @staticmethod
     def CreateServiceAccount(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/user_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/user_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/user_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,15 +14,15 @@
 
 from aruna.api.storage.models.v2 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v2_dot_models__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0aruna/api/storage/services/v2/user_service.proto\x12\x1d\x61runa.api.storage.services.v2\x1a(aruna/api/storage/models/v2/models.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/api/visibility.proto\"h\n\x13RegisterUserRequest\x12!\n\x0c\x64isplay_name\x18\x01 \x01(\tR\x0b\x64isplayName\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\"/\n\x14RegisterUserResponse\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\xaf\x01\n\x15\x43reateAPITokenRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12G\n\npermission\x18\x02 \x01(\x0b\x32\'.aruna.api.storage.models.v2.PermissionR\npermission\x12\x39\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"u\n\x16\x43reateAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x05token\x12!\n\x0ctoken_secret\x18\x02 \x01(\tR\x0btokenSecret\"/\n\x12GetAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"O\n\x13GetAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x05token\"\x15\n\x13GetAPITokensRequest\"R\n\x14GetAPITokensResponse\x12:\n\x06tokens\x18\x01 \x03(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x06tokens\"2\n\x15\x44\x65leteAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"\x18\n\x16\x44\x65leteAPITokenResponse\"1\n\x16\x44\x65leteAPITokensRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x19\n\x17\x44\x65leteAPITokensResponse\")\n\x0eGetUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"H\n\x0fGetUserResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"1\n\x16GetUserRedactedRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"P\n\x17GetUserRedactedResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"H\n\x1cUpdateUserDisplayNameRequest\x12(\n\x10new_display_name\x18\x01 \x01(\tR\x0enewDisplayName\"V\n\x1dUpdateUserDisplayNameResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\".\n\x13\x41\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x16\n\x14\x41\x63tivateUserResponse\"\x1d\n\x1bGetNotActivatedUsersRequest\"W\n\x1cGetNotActivatedUsersResponse\x12\x37\n\x05users\x18\x01 \x03(\x0b\x32!.aruna.api.storage.models.v2.UserR\x05users\"\x14\n\x12GetAllUsersRequest\"L\n\x13GetAllUsersResponse\x12\x35\n\x04user\x18\x01 \x03(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"0\n\x15\x44\x65\x61\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x18\n\x16\x44\x65\x61\x63tivateUserResponse\"N\n\x16UpdateUserEmailRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1b\n\tnew_email\x18\x02 \x01(\tR\x08newEmail\"P\n\x17UpdateUserEmailResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"W\n\x1bGetS3CredentialsUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1f\n\x0b\x65ndpoint_id\x18\x02 \x01(\tR\nendpointId\"\x8e\x01\n\x1cGetS3CredentialsUserResponse\x12\"\n\rs3_access_key\x18\x01 \x01(\tR\x0bs3AccessKey\x12\"\n\rs3_secret_key\x18\x02 \x01(\tR\x0bs3SecretKey\x12&\n\x0fs3_endpoint_url\x18\x03 \x01(\tR\rs3EndpointUrl\"\x98\x01\n\x1cGetDataproxyTokenUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1f\n\x0b\x65ndpoint_id\x18\x02 \x01(\tR\nendpointId\x12>\n\x07\x63ontext\x18\x03 \x01(\x0b\x32$.aruna.api.storage.models.v2.ContextR\x07\x63ontext\"5\n\x1dGetDataproxyTokenUserResponse\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\"!\n\x1fGetPersonalNotificationsRequest\"}\n GetPersonalNotificationsResponse\x12Y\n\rnotifications\x18\x01 \x03(\x0b\x32\x33.aruna.api.storage.services.v2.PersonalNotificationR\rnotifications\"T\n\'AcknowledgePersonalNotificationsRequest\x12)\n\x10notification_ids\x18\x01 \x03(\tR\x0fnotificationIds\"*\n(AcknowledgePersonalNotificationsResponse\"\x8c\x01\n\tReference\x12G\n\x08ref_type\x18\x01 \x01(\x0e\x32,.aruna.api.storage.services.v2.ReferenceTypeR\x07refType\x12\x19\n\x08ref_name\x18\x02 \x01(\tR\x07refName\x12\x1b\n\tref_value\x18\x03 \x01(\tR\x08refValue\"\xd4\x01\n\x14PersonalNotification\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12T\n\x07variant\x18\x02 \x01(\x0e\x32:.aruna.api.storage.services.v2.PersonalNotificationVariantR\x07variant\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12<\n\x04refs\x18\x04 \x03(\x0b\x32(.aruna.api.storage.services.v2.ReferenceR\x04refs\"B\n\x16\x41\x64\x64OidcProviderRequest\x12(\n\x10new_access_token\x18\x01 \x01(\tR\x0enewAccessToken\"P\n\x17\x41\x64\x64OidcProviderResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\">\n\x19RemoveOidcProviderRequest\x12!\n\x0cprovider_url\x18\x01 \x01(\tR\x0bproviderUrl\"S\n\x1aRemoveOidcProviderResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user*e\n\rReferenceType\x12\x1e\n\x1aREFERENCE_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13REFERENCE_TYPE_USER\x10\x01\x12\x1b\n\x17REFERENCE_TYPE_RESOURCE\x10\x02*\xd2\x02\n\x1bPersonalNotificationVariant\x12-\n)PERSONAL_NOTIFICATION_VARIANT_UNSPECIFIED\x10\x00\x12\x32\n.PERSONAL_NOTIFICATION_VARIANT_ACCESS_REQUESTED\x10\x01\x12\x34\n0PERSONAL_NOTIFICATION_VARIANT_PERMISSION_GRANTED\x10\x02\x12\x34\n0PERSONAL_NOTIFICATION_VARIANT_PERMISSION_REVOKED\x10\x03\x12\x34\n0PERSONAL_NOTIFICATION_VARIANT_PERMISSION_UPDATED\x10\x04\x12.\n*PERSONAL_NOTIFICATION_VARIANT_ANNOUNCEMENT\x10\x05\x32\xb0\x1a\n\x0bUserService\x12\x95\x01\n\x0cRegisterUser\x12\x32.aruna.api.storage.services.v2.RegisterUserRequest\x1a\x33.aruna.api.storage.services.v2.RegisterUserResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/v2/user/register:\x01*\x12\xa7\x01\n\x0e\x44\x65\x61\x63tivateUser\x12\x34.aruna.api.storage.services.v2.DeactivateUserRequest\x1a\x35.aruna.api.storage.services.v2.DeactivateUserResponse\"(\x82\xd3\xe4\x93\x02\"2\x1d/v2/user/{user_id}/deactivate:\x01*\x12\x9f\x01\n\x0c\x41\x63tivateUser\x12\x32.aruna.api.storage.services.v2.ActivateUserRequest\x1a\x33.aruna.api.storage.services.v2.ActivateUserResponse\"&\x82\xd3\xe4\x93\x02 2\x1b/v2/user/{user_id}/activate:\x01*\x12\x99\x01\n\x0e\x43reateAPIToken\x12\x34.aruna.api.storage.services.v2.CreateAPITokenRequest\x1a\x35.aruna.api.storage.services.v2.CreateAPITokenResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v2/user/tokens:\x01*\x12\x98\x01\n\x0bGetAPIToken\x12\x31.aruna.api.storage.services.v2.GetAPITokenRequest\x1a\x32.aruna.api.storage.services.v2.GetAPITokenResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/v2/user/tokens/{token_id}\x12\x90\x01\n\x0cGetAPITokens\x12\x32.aruna.api.storage.services.v2.GetAPITokensRequest\x1a\x33.aruna.api.storage.services.v2.GetAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/v2/user/tokens\x12\xa1\x01\n\x0e\x44\x65leteAPIToken\x12\x34.aruna.api.storage.services.v2.DeleteAPITokenRequest\x1a\x35.aruna.api.storage.services.v2.DeleteAPITokenResponse\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v2/user/tokens/{token_id}\x12\x99\x01\n\x0f\x44\x65leteAPITokens\x12\x35.aruna.api.storage.services.v2.DeleteAPITokensRequest\x1a\x36.aruna.api.storage.services.v2.DeleteAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11*\x0f/v2/user/tokens\x12z\n\x07GetUser\x12-.aruna.api.storage.services.v2.GetUserRequest\x1a..aruna.api.storage.services.v2.GetUserResponse\"\x10\x82\xd3\xe4\x93\x02\n\x12\x08/v2/user\x12\xa5\x01\n\x0fGetUserRedacted\x12\x35.aruna.api.storage.services.v2.GetUserRedactedRequest\x1a\x36.aruna.api.storage.services.v2.GetUserRedactedResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2/user/{user_id}/redacted\x12\xb4\x01\n\x15UpdateUserDisplayName\x12;.aruna.api.storage.services.v2.UpdateUserDisplayNameRequest\x1a<.aruna.api.storage.services.v2.UpdateUserDisplayNameResponse\" \x82\xd3\xe4\x93\x02\x1a\x32\x15/v2/user/display_name:\x01*\x12\x9b\x01\n\x0fUpdateUserEmail\x12\x35.aruna.api.storage.services.v2.UpdateUserEmailRequest\x1a\x36.aruna.api.storage.services.v2.UpdateUserEmailResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x32\x0e/v2/user/email:\x01*\x12\xb4\x01\n\x14GetNotActivatedUsers\x12:.aruna.api.storage.services.v2.GetNotActivatedUsersRequest\x1a;.aruna.api.storage.services.v2.GetNotActivatedUsersResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2/user/list/not_activated\x12\x8b\x01\n\x0bGetAllUsers\x12\x31.aruna.api.storage.services.v2.GetAllUsersRequest\x1a\x32.aruna.api.storage.services.v2.GetAllUsersResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v2/user/list\x12\xba\x01\n\x14GetS3CredentialsUser\x12:.aruna.api.storage.services.v2.GetS3CredentialsUserRequest\x1a;.aruna.api.storage.services.v2.GetS3CredentialsUserResponse\")\x82\xd3\xe4\x93\x02#\x12!/v2/user/{user_id}/s3_credentials\x12\xba\x01\n\x15GetDataproxyTokenUser\x12;.aruna.api.storage.services.v2.GetDataproxyTokenUserRequest\x1a<.aruna.api.storage.services.v2.GetDataproxyTokenUserResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v2/user/{user_id}/proxy_token\x12\xbb\x01\n\x18GetPersonalNotifications\x12>.aruna.api.storage.services.v2.GetPersonalNotificationsRequest\x1a?.aruna.api.storage.services.v2.GetPersonalNotificationsResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/v2/user/notifications\x12\xdf\x01\n AcknowledgePersonalNotifications\x12\x46.aruna.api.storage.services.v2.AcknowledgePersonalNotificationsRequest\x1aG.aruna.api.storage.services.v2.AcknowledgePersonalNotificationsResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v2/user/notifications/acknowledge\x12\x9d\x01\n\x0e\x41\x64\x64OidcProvier\x12\x35.aruna.api.storage.services.v2.AddOidcProviderRequest\x1a\x36.aruna.api.storage.services.v2.AddOidcProviderResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x32\x11/v2/user/add_oidc:\x01*\x12\xaa\x01\n\x12RemoveOidcProvider\x12\x38.aruna.api.storage.services.v2.RemoveOidcProviderRequest\x1a\x39.aruna.api.storage.services.v2.RemoveOidcProviderResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x32\x14/v2/user/remove_oidc:\x01*\x1a\x0e\xfa\xd2\xe4\x93\x02\x08\x12\x06SERVERB\x90\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\x0bUserServiceP\x01Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0aruna/api/storage/services/v2/user_service.proto\x12\x1d\x61runa.api.storage.services.v2\x1a(aruna/api/storage/models/v2/models.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/api/visibility.proto\"h\n\x13RegisterUserRequest\x12!\n\x0c\x64isplay_name\x18\x01 \x01(\tR\x0b\x64isplayName\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\"/\n\x14RegisterUserResponse\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\xaf\x01\n\x15\x43reateAPITokenRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12G\n\npermission\x18\x02 \x01(\x0b\x32\'.aruna.api.storage.models.v2.PermissionR\npermission\x12\x39\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"u\n\x16\x43reateAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x05token\x12!\n\x0ctoken_secret\x18\x02 \x01(\tR\x0btokenSecret\"/\n\x12GetAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"O\n\x13GetAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x05token\"\x15\n\x13GetAPITokensRequest\"R\n\x14GetAPITokensResponse\x12:\n\x06tokens\x18\x01 \x03(\x0b\x32\".aruna.api.storage.models.v2.TokenR\x06tokens\"2\n\x15\x44\x65leteAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"\x18\n\x16\x44\x65leteAPITokenResponse\"1\n\x16\x44\x65leteAPITokensRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x19\n\x17\x44\x65leteAPITokensResponse\")\n\x0eGetUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"H\n\x0fGetUserResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"1\n\x16GetUserRedactedRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"P\n\x17GetUserRedactedResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"H\n\x1cUpdateUserDisplayNameRequest\x12(\n\x10new_display_name\x18\x01 \x01(\tR\x0enewDisplayName\"V\n\x1dUpdateUserDisplayNameResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\".\n\x13\x41\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x16\n\x14\x41\x63tivateUserResponse\"\x1d\n\x1bGetNotActivatedUsersRequest\"W\n\x1cGetNotActivatedUsersResponse\x12\x37\n\x05users\x18\x01 \x03(\x0b\x32!.aruna.api.storage.models.v2.UserR\x05users\"\x14\n\x12GetAllUsersRequest\"L\n\x13GetAllUsersResponse\x12\x35\n\x04user\x18\x01 \x03(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"0\n\x15\x44\x65\x61\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x18\n\x16\x44\x65\x61\x63tivateUserResponse\"N\n\x16UpdateUserEmailRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1b\n\tnew_email\x18\x02 \x01(\tR\x08newEmail\"P\n\x17UpdateUserEmailResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\"W\n\x1bGetS3CredentialsUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1f\n\x0b\x65ndpoint_id\x18\x02 \x01(\tR\nendpointId\"\x8e\x01\n\x1cGetS3CredentialsUserResponse\x12\"\n\rs3_access_key\x18\x01 \x01(\tR\x0bs3AccessKey\x12\"\n\rs3_secret_key\x18\x02 \x01(\tR\x0bs3SecretKey\x12&\n\x0fs3_endpoint_url\x18\x03 \x01(\tR\rs3EndpointUrl\"\x98\x01\n\x1cGetDataproxyTokenUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1f\n\x0b\x65ndpoint_id\x18\x02 \x01(\tR\nendpointId\x12>\n\x07\x63ontext\x18\x03 \x01(\x0b\x32$.aruna.api.storage.models.v2.ContextR\x07\x63ontext\"5\n\x1dGetDataproxyTokenUserResponse\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\"!\n\x1fGetPersonalNotificationsRequest\"}\n GetPersonalNotificationsResponse\x12Y\n\rnotifications\x18\x01 \x03(\x0b\x32\x33.aruna.api.storage.services.v2.PersonalNotificationR\rnotifications\"T\n\'AcknowledgePersonalNotificationsRequest\x12)\n\x10notification_ids\x18\x01 \x03(\tR\x0fnotificationIds\"*\n(AcknowledgePersonalNotificationsResponse\"\x8c\x01\n\tReference\x12G\n\x08ref_type\x18\x01 \x01(\x0e\x32,.aruna.api.storage.services.v2.ReferenceTypeR\x07refType\x12\x19\n\x08ref_name\x18\x02 \x01(\tR\x07refName\x12\x1b\n\tref_value\x18\x03 \x01(\tR\x08refValue\"\xd4\x01\n\x14PersonalNotification\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12T\n\x07variant\x18\x02 \x01(\x0e\x32:.aruna.api.storage.services.v2.PersonalNotificationVariantR\x07variant\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12<\n\x04refs\x18\x04 \x03(\x0b\x32(.aruna.api.storage.services.v2.ReferenceR\x04refs\"B\n\x16\x41\x64\x64OidcProviderRequest\x12(\n\x10new_access_token\x18\x01 \x01(\tR\x0enewAccessToken\"P\n\x17\x41\x64\x64OidcProviderResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user\">\n\x19RemoveOidcProviderRequest\x12!\n\x0cprovider_url\x18\x01 \x01(\tR\x0bproviderUrl\"S\n\x1aRemoveOidcProviderResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v2.UserR\x04user*e\n\rReferenceType\x12\x1e\n\x1aREFERENCE_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13REFERENCE_TYPE_USER\x10\x01\x12\x1b\n\x17REFERENCE_TYPE_RESOURCE\x10\x02*\xd2\x02\n\x1bPersonalNotificationVariant\x12-\n)PERSONAL_NOTIFICATION_VARIANT_UNSPECIFIED\x10\x00\x12\x32\n.PERSONAL_NOTIFICATION_VARIANT_ACCESS_REQUESTED\x10\x01\x12\x34\n0PERSONAL_NOTIFICATION_VARIANT_PERMISSION_GRANTED\x10\x02\x12\x34\n0PERSONAL_NOTIFICATION_VARIANT_PERMISSION_REVOKED\x10\x03\x12\x34\n0PERSONAL_NOTIFICATION_VARIANT_PERMISSION_UPDATED\x10\x04\x12.\n*PERSONAL_NOTIFICATION_VARIANT_ANNOUNCEMENT\x10\x05\x32\xb1\x1a\n\x0bUserService\x12\x95\x01\n\x0cRegisterUser\x12\x32.aruna.api.storage.services.v2.RegisterUserRequest\x1a\x33.aruna.api.storage.services.v2.RegisterUserResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/v2/user/register:\x01*\x12\xa7\x01\n\x0e\x44\x65\x61\x63tivateUser\x12\x34.aruna.api.storage.services.v2.DeactivateUserRequest\x1a\x35.aruna.api.storage.services.v2.DeactivateUserResponse\"(\x82\xd3\xe4\x93\x02\"2\x1d/v2/user/{user_id}/deactivate:\x01*\x12\x9f\x01\n\x0c\x41\x63tivateUser\x12\x32.aruna.api.storage.services.v2.ActivateUserRequest\x1a\x33.aruna.api.storage.services.v2.ActivateUserResponse\"&\x82\xd3\xe4\x93\x02 2\x1b/v2/user/{user_id}/activate:\x01*\x12\x99\x01\n\x0e\x43reateAPIToken\x12\x34.aruna.api.storage.services.v2.CreateAPITokenRequest\x1a\x35.aruna.api.storage.services.v2.CreateAPITokenResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v2/user/tokens:\x01*\x12\x98\x01\n\x0bGetAPIToken\x12\x31.aruna.api.storage.services.v2.GetAPITokenRequest\x1a\x32.aruna.api.storage.services.v2.GetAPITokenResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/v2/user/tokens/{token_id}\x12\x90\x01\n\x0cGetAPITokens\x12\x32.aruna.api.storage.services.v2.GetAPITokensRequest\x1a\x33.aruna.api.storage.services.v2.GetAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/v2/user/tokens\x12\xa1\x01\n\x0e\x44\x65leteAPIToken\x12\x34.aruna.api.storage.services.v2.DeleteAPITokenRequest\x1a\x35.aruna.api.storage.services.v2.DeleteAPITokenResponse\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v2/user/tokens/{token_id}\x12\x99\x01\n\x0f\x44\x65leteAPITokens\x12\x35.aruna.api.storage.services.v2.DeleteAPITokensRequest\x1a\x36.aruna.api.storage.services.v2.DeleteAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11*\x0f/v2/user/tokens\x12z\n\x07GetUser\x12-.aruna.api.storage.services.v2.GetUserRequest\x1a..aruna.api.storage.services.v2.GetUserResponse\"\x10\x82\xd3\xe4\x93\x02\n\x12\x08/v2/user\x12\xa5\x01\n\x0fGetUserRedacted\x12\x35.aruna.api.storage.services.v2.GetUserRedactedRequest\x1a\x36.aruna.api.storage.services.v2.GetUserRedactedResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2/user/{user_id}/redacted\x12\xb4\x01\n\x15UpdateUserDisplayName\x12;.aruna.api.storage.services.v2.UpdateUserDisplayNameRequest\x1a<.aruna.api.storage.services.v2.UpdateUserDisplayNameResponse\" \x82\xd3\xe4\x93\x02\x1a\x32\x15/v2/user/display_name:\x01*\x12\x9b\x01\n\x0fUpdateUserEmail\x12\x35.aruna.api.storage.services.v2.UpdateUserEmailRequest\x1a\x36.aruna.api.storage.services.v2.UpdateUserEmailResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x32\x0e/v2/user/email:\x01*\x12\xb4\x01\n\x14GetNotActivatedUsers\x12:.aruna.api.storage.services.v2.GetNotActivatedUsersRequest\x1a;.aruna.api.storage.services.v2.GetNotActivatedUsersResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2/user/list/not_activated\x12\x8b\x01\n\x0bGetAllUsers\x12\x31.aruna.api.storage.services.v2.GetAllUsersRequest\x1a\x32.aruna.api.storage.services.v2.GetAllUsersResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v2/user/list\x12\xba\x01\n\x14GetS3CredentialsUser\x12:.aruna.api.storage.services.v2.GetS3CredentialsUserRequest\x1a;.aruna.api.storage.services.v2.GetS3CredentialsUserResponse\")\x82\xd3\xe4\x93\x02#\x12!/v2/user/{user_id}/s3_credentials\x12\xba\x01\n\x15GetDataproxyTokenUser\x12;.aruna.api.storage.services.v2.GetDataproxyTokenUserRequest\x1a<.aruna.api.storage.services.v2.GetDataproxyTokenUserResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v2/user/{user_id}/proxy_token\x12\xbb\x01\n\x18GetPersonalNotifications\x12>.aruna.api.storage.services.v2.GetPersonalNotificationsRequest\x1a?.aruna.api.storage.services.v2.GetPersonalNotificationsResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/v2/user/notifications\x12\xdf\x01\n AcknowledgePersonalNotifications\x12\x46.aruna.api.storage.services.v2.AcknowledgePersonalNotificationsRequest\x1aG.aruna.api.storage.services.v2.AcknowledgePersonalNotificationsResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v2/user/notifications/acknowledge\x12\x9e\x01\n\x0f\x41\x64\x64OidcProvider\x12\x35.aruna.api.storage.services.v2.AddOidcProviderRequest\x1a\x36.aruna.api.storage.services.v2.AddOidcProviderResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x32\x11/v2/user/add_oidc:\x01*\x12\xaa\x01\n\x12RemoveOidcProvider\x12\x38.aruna.api.storage.services.v2.RemoveOidcProviderRequest\x1a\x39.aruna.api.storage.services.v2.RemoveOidcProviderResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x32\x14/v2/user/remove_oidc:\x01*\x1a\x0e\xfa\xd2\xe4\x93\x02\x08\x12\x06SERVERB\x90\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\x0bUserServiceP\x01Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v2.user_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v2B\013UserServiceP\001Z?github.com/ArunaStorage/go-api/v2/aruna/api/storage/services/v2'
@@ -60,16 +60,16 @@
   _globals['_USERSERVICE'].methods_by_name['GetS3CredentialsUser']._serialized_options = b'\202\323\344\223\002#\022!/v2/user/{user_id}/s3_credentials'
   _globals['_USERSERVICE'].methods_by_name['GetDataproxyTokenUser']._options = None
   _globals['_USERSERVICE'].methods_by_name['GetDataproxyTokenUser']._serialized_options = b'\202\323\344\223\002 \022\036/v2/user/{user_id}/proxy_token'
   _globals['_USERSERVICE'].methods_by_name['GetPersonalNotifications']._options = None
   _globals['_USERSERVICE'].methods_by_name['GetPersonalNotifications']._serialized_options = b'\202\323\344\223\002\030\022\026/v2/user/notifications'
   _globals['_USERSERVICE'].methods_by_name['AcknowledgePersonalNotifications']._options = None
   _globals['_USERSERVICE'].methods_by_name['AcknowledgePersonalNotifications']._serialized_options = b'\202\323\344\223\002$\022\"/v2/user/notifications/acknowledge'
-  _globals['_USERSERVICE'].methods_by_name['AddOidcProvier']._options = None
-  _globals['_USERSERVICE'].methods_by_name['AddOidcProvier']._serialized_options = b'\202\323\344\223\002\0262\021/v2/user/add_oidc:\001*'
+  _globals['_USERSERVICE'].methods_by_name['AddOidcProvider']._options = None
+  _globals['_USERSERVICE'].methods_by_name['AddOidcProvider']._serialized_options = b'\202\323\344\223\002\0262\021/v2/user/add_oidc:\001*'
   _globals['_USERSERVICE'].methods_by_name['RemoveOidcProvider']._options = None
   _globals['_USERSERVICE'].methods_by_name['RemoveOidcProvider']._serialized_options = b'\202\323\344\223\002\0312\024/v2/user/remove_oidc:\001*'
   _globals['_REFERENCETYPE']._serialized_start=3397
   _globals['_REFERENCETYPE']._serialized_end=3498
   _globals['_PERSONALNOTIFICATIONVARIANT']._serialized_start=3501
   _globals['_PERSONALNOTIFICATIONVARIANT']._serialized_end=3839
   _globals['_REGISTERUSERREQUEST']._serialized_start=217
@@ -153,9 +153,9 @@
   _globals['_ADDOIDCPROVIDERRESPONSE']._serialized_start=3166
   _globals['_ADDOIDCPROVIDERRESPONSE']._serialized_end=3246
   _globals['_REMOVEOIDCPROVIDERREQUEST']._serialized_start=3248
   _globals['_REMOVEOIDCPROVIDERREQUEST']._serialized_end=3310
   _globals['_REMOVEOIDCPROVIDERRESPONSE']._serialized_start=3312
   _globals['_REMOVEOIDCPROVIDERRESPONSE']._serialized_end=3395
   _globals['_USERSERVICE']._serialized_start=3842
-  _globals['_USERSERVICE']._serialized_end=7218
+  _globals['_USERSERVICE']._serialized_end=7219
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/user_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/user_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/user_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 from aruna.api.storage.services.v2 import user_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2
 
 
 class UserServiceStub(object):
     """UserService
 
-    Contains all methods that get/create or update Users and associated resource
-    including all autorization methods
+    Status: BETA
+
+    Contains all CRUD methods for users and associated resource
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -104,31 +105,32 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.GetPersonalNotificationsResponse.FromString,
                 )
         self.AcknowledgePersonalNotifications = channel.unary_unary(
                 '/aruna.api.storage.services.v2.UserService/AcknowledgePersonalNotifications',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AcknowledgePersonalNotificationsRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AcknowledgePersonalNotificationsResponse.FromString,
                 )
-        self.AddOidcProvier = channel.unary_unary(
-                '/aruna.api.storage.services.v2.UserService/AddOidcProvier',
+        self.AddOidcProvider = channel.unary_unary(
+                '/aruna.api.storage.services.v2.UserService/AddOidcProvider',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AddOidcProviderRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AddOidcProviderResponse.FromString,
                 )
         self.RemoveOidcProvider = channel.unary_unary(
                 '/aruna.api.storage.services.v2.UserService/RemoveOidcProvider',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.RemoveOidcProviderRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.RemoveOidcProviderResponse.FromString,
                 )
 
 
 class UserServiceServicer(object):
     """UserService
 
-    Contains all methods that get/create or update Users and associated resource
-    including all autorization methods
+    Status: BETA
+
+    Contains all CRUD methods for users and associated resource
     """
 
     def RegisterUser(self, request, context):
         """RegisterUser
 
         Status: BETA
 
@@ -324,22 +326,33 @@
 
         Acknowledges personal notifications
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AddOidcProvier(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def AddOidcProvider(self, request, context):
+        """AddOidcProvider
+
+        Status: BETA
+
+        Add alternative oidc login method for user
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def RemoveOidcProvider(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """RemoveOidcProvider
+
+        Status: BETA
+
+        Remove alternative oidc login method from user
+        (Only works if user has more than one oidc provider)
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_UserServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -429,16 +442,16 @@
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.GetPersonalNotificationsResponse.SerializeToString,
             ),
             'AcknowledgePersonalNotifications': grpc.unary_unary_rpc_method_handler(
                     servicer.AcknowledgePersonalNotifications,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AcknowledgePersonalNotificationsRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AcknowledgePersonalNotificationsResponse.SerializeToString,
             ),
-            'AddOidcProvier': grpc.unary_unary_rpc_method_handler(
-                    servicer.AddOidcProvier,
+            'AddOidcProvider': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddOidcProvider,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AddOidcProviderRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AddOidcProviderResponse.SerializeToString,
             ),
             'RemoveOidcProvider': grpc.unary_unary_rpc_method_handler(
                     servicer.RemoveOidcProvider,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.RemoveOidcProviderRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.RemoveOidcProviderResponse.SerializeToString,
@@ -449,16 +462,17 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class UserService(object):
     """UserService
 
-    Contains all methods that get/create or update Users and associated resource
-    including all autorization methods
+    Status: BETA
+
+    Contains all CRUD methods for users and associated resource
     """
 
     @staticmethod
     def RegisterUser(request,
             target,
             options=(),
             channel_credentials=None,
@@ -760,25 +774,25 @@
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v2.UserService/AcknowledgePersonalNotifications',
             aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AcknowledgePersonalNotificationsRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AcknowledgePersonalNotificationsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def AddOidcProvier(request,
+    def AddOidcProvider(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v2.UserService/AddOidcProvier',
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v2.UserService/AddOidcProvider',
             aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AddOidcProviderRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v2_dot_user__service__pb2.AddOidcProviderResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def RemoveOidcProvider(request,
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/workspace_service_pb2.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/workspace_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aruna/api/storage/services/v2/workspace_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/workspace_service_pb2.pyi` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/workspace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-2.0.0b8/aruna/api/storage/services/v2/workspace_service_pb2_grpc.py` & `Aruna-Python-API-2.0.0b9/aruna/api/storage/services/v2/workspace_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from aruna.api.storage.services.v2 import workspace_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v2_dot_workspace__service__pb2
 
 
 class WorkspaceServiceStub(object):
-    """Service to manage "special" anonymous collections / workspaces 
+    """WorkspaceService
+
+    Status: BETA
+
+    Service to manage anonymous "scratch" projects / workspaces 
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -49,15 +53,19 @@
                 '/aruna.api.storage.services.v2.WorkspaceService/ClaimWorkspace',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_workspace__service__pb2.ClaimWorkspaceRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v2_dot_workspace__service__pb2.ClaimWorkspaceResponse.FromString,
                 )
 
 
 class WorkspaceServiceServicer(object):
-    """Service to manage "special" anonymous collections / workspaces 
+    """WorkspaceService
+
+    Status: BETA
+
+    Service to manage anonymous "scratch" projects / workspaces 
     """
 
     def CreateWorkspaceTemplate(self, request, context):
         """CreatesNewWorkspaceTemplate
 
         Status: ALPHA
 
@@ -101,15 +109,15 @@
         raise NotImplementedError('Method not implemented!')
 
     def CreateWorkspace(self, request, context):
         """CreateWorkspace
 
         Status: ALPHA
 
-        A new request to create a personal anonymous workspace
+        Create a personal anonymous workspace
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteWorkspace(self, request, context):
         """DeleteWorkspace
@@ -175,15 +183,19 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.storage.services.v2.WorkspaceService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class WorkspaceService(object):
-    """Service to manage "special" anonymous collections / workspaces 
+    """WorkspaceService
+
+    Status: BETA
+
+    Service to manage anonymous "scratch" projects / workspaces 
     """
 
     @staticmethod
     def CreateWorkspaceTemplate(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `Aruna-Python-API-2.0.0b8/setup.py` & `Aruna-Python-API-2.0.0b9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="2.0.0-beta.8",
+    version="2.0.0-beta.9",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Sebastian Beyvers, Jannis Hochmuth, Lukas Brehm',
     author_email='sebastian.beyvers@computational.bio.uni-giessen.de, '
```

